# 特定メッセージの監視について

本ページでは Microsoft Azure OMS(Operational Management Suite)にあるLog Analyticsを使った特定ログの監視方法を紹介します。

## はじめに
システム監視にはサービス監視とリソース監視と大きく２つに分かれますが、ここではリソース監視の中で特定の  
アプリケーションが出力する「特定のメッセージ」を監視対象にする、という条件に対してAzureのサービスをどの  
ように利用することで本条件を満たすかを中心に有益なサイトをピックアップしています。  
例：  
apacheのhttpdが落下したメッセージを定期的に監視対象とし、落下したメッセージを検知した場合は任意のメール  
アドレスへアラートメールを送る、または用意した一次対応スクリプトを走らせる。  

## 参考となるサイト

### OMS Log Analyticsについて
Log Analyticsとは  
https://docs.microsoft.com/ja-jp/azure/log-analytics/log-analytics-overview

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


