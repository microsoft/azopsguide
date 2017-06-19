# SQLインジェクションやクロスサイトスクリプティングの監視をしたい

本ページではSQLインジェクションやクロスサイトスクリプティングの監視方法を紹介します。  

## はじめに
個人情報やクレジットカード番号の漏洩など、今や１つの社会現象として企業のブランドイメージを大きく  
損なうリスクが存在します。安易なプログラムの実装や不必要なインターネットアクセス経路など、  
最低限守るべき情報と手立てについては企業によって様々ですが、本記事ではよく耳にするSQLインジェク  
ションやクロスサイトスクリプティングについての対策を中心に触れています。  
SQLインジェクションは受け付けたアプリケーションがDatabaseにSQLの命令処理を実行する時に発生  
するため、GetOS内でWeb/APサーバーを組み立てている場合はお客様にて対応するか、Azure MarketPlace  
にある3rd party製のWAFを導入することで検知や対策をとることができます。また、Azure SQL Database  
のようなPaaSサービスにおいても、機能をONにするといった対応を取ることができるようになっています。  

## 参考となるサイト

### SQLインジェクションの監視について
Azure SQL Database の脅威検出機能の一般提供を 2017 年 4 月に開始  
https://blogs.technet.microsoft.com/jpitpro/2017/02/16/azure-sql-database-threat-detection-general-availability-in-spring-2017/

Azure の高度な脅威の検出  
https://docs.microsoft.com/ja-jp/azure/security/azure-threat-detection

### その他　ユースケース/ブログ記事等


