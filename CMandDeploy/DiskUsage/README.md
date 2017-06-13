# Disk容量の監視をしたい

本ページでは Microsoft Azure OMS(Operational Management Suite)にあるLog Analyticsを使ったディスク容量の監視  
について記載します。  

## はじめに
OS内のディスク容量（ドライブ、マウントポイント） が100%になるとディスク領域への書き込みが不可となり、サービスへの  
影響やバックアップ処理の停止など、ディスク領域への破壊まではいかないまでも不都合なことが大量に発生します。回避する  
ためには十分なディスク容量を備えることはもちろんですが、それでもバースト的に発生するアンコントローラブルな大量書き  
込み処理や、想定外のソフトウェアバグによる多重書き込み等、ディスク容量の使用量・空き状態を定期的に監視する必要が  
あります。ここではMicrosoft Azureのサービスを使い、どのように監視するかの参考となる情報をまとめてあります。  

OMS Log Analyticsは、エージェント型ログ検索サービスです。監視対象となる仮想マシンにエージェントをインストールし、  
エージェントからazure storage(tables)にログを飛ばします。OMSポータル(Web-UI)では、既に用意されているソリュー  
ションサービスを利用することでログのvisualizationを行うことができます。また、該当の生ログを検索することもでき、  
検索キーワードを基に検知と一次処理のキック、アラートメールを飛ばすといったロジックを設定することができます。  
Disk容量監視について、WindowsOSの場合はagentから送られるログを基にソリューションサービスをOMSポータルで設定する  
ことで利用できます。Linuxの場合はshell scriptで容量をチェックするスクリプトを用意します。scriptはcrontabに登録  
しておき異常を検知した場合はsyslog/rsyslogへログを吐き出すことでLog Analyticsと連動させた監視を行うことができます。  


## 参考となるサイト

### OMS Log Analyticsについて
Log Analyticsとは  
https://docs.microsoft.com/ja-jp/azure/log-analytics/log-analytics-overview

容量とパフォーマンス ソリューション (プレビュー) を使って Hyper-V 仮想マシンの容量を計画する  
https://docs.microsoft.com/ja-jp/azure/log-analytics/log-analytics-capacity

Agentのインストール方法 for Windows  
https://docs.microsoft.com/ja-jp/azure/log-analytics/log-analytics-windows-agents

Agentのインストール方法 for Linux  
https://docs.microsoft.com/ja-jp/azure/log-analytics/log-analytics-agent-linux

Log Analytics 検索リファレンス  
https://docs.microsoft.com/ja-jp/azure/log-analytics/log-analytics-search-reference

Log Analytics アラートルールの操作  
https://docs.microsoft.com/ja-jp/azure/log-analytics/log-analytics-alerts-creating

### その他　ユースケース/ブログ記事等
Azure CentOS7.xの環境におけるrsyslogを使った特定ログの監視とアラートメールの発信について  
<http://akazure.hatenablog.com/entry/2017/06/05/155201>  


