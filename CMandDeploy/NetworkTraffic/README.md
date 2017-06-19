# ネットワークトラフィック（利用帯域）を監視したい

本ページではGestOS側ネットワークの監視方法を紹介します。

## はじめに
システム監視にはサービス監視とリソース監視と大きく２つに分かれますが、ここではリソース監視の中でOSログ  
が出力する「特定のメッセージ」を監視対象にする、という条件に対してAzureのサービスをどのように利用する  
ことで本条件を満たすかを中心に有益なサイトをピックアップしています。  

## 参考となるサイト

### ネットワーク監視について
Log Analytics のネットワーク パフォーマンス モニター ソリューション  
https://docs.microsoft.com/ja-jp/azure/log-analytics/log-analytics-network-performance-monitor

Azure のネットワーク監視の概要  
https://docs.microsoft.com/ja-jp/azure/network-watcher/network-watcher-monitoring-overview

Log Analyticsとは  
https://docs.microsoft.com/ja-jp/azure/log-analytics/log-analytics-overview


### その他　ユースケース/ブログ記事等
Azure CentOS7.xの環境におけるrsyslogを使った特定ログの監視とアラートメールの発信について  
<http://akazure.hatenablog.com/entry/2017/06/05/155201>  


