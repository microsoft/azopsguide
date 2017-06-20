# Azureの構成変更を監視したい

本ページではAzure構成更の監視方法を紹介します。

## はじめに
Microsoft Azureの仮想マシンを作成する際、vNETやPublicIP、可用性セット、データディスクの追加、ロード  
バランサの導入などなど、１つのシステムを用意するために必要なシステムリソースが多数あります。  
このシステムが稼働しはじめると、どのシステムがいつどのように変更されたかの変更管理が大切な要素となって  
きます。以下は各リソースの操作や影響レベルに応じたアラート設定や、アクティビティログと呼ばれる操作ログ  
の取得方法などを記載しています。

## 参考となるサイト

### Azure構成変更の監視について
Azure Monitor の概要  
https://docs.microsoft.com/ja-jp/azure/monitoring-and-diagnostics/monitoring-overview-azure-monitor

Azure アクティビティ ログの概要
https://docs.microsoft.com/ja-jp/azure/monitoring-and-diagnostics/monitoring-overview-activity-logs

### その他　ユースケース/ブログ記事等


