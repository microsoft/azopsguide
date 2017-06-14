# カスタマイズしたログを監視したい

本ページでは Microsoft Azure OMS(Operational Management Suite)にあるLog Analyticsを使った特定ログの監視方法を紹介します。

## はじめに
システム監視にはサービス監視とリソース監視と大きく２つに分かれますが、ここではリソース監視の中で特定の  
アプリケーションが出力するログを監視対象にする、という条件に対してAzureのサービスをどのように利用する  
ことで本条件を満たすかを中心に有益なサイトをピックアップしています。  

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


