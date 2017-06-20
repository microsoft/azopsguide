# Microsoft Azureに影響するメンテナンスを監視したい

本ページではMicrosoft Azure メンテナンスの監視方法を紹介します。  

## はじめに
Microsoft Azureの裏側では定期的なメンテナンスが実施されております。同一用途の仮想マシンは  
可用性セットを付けることで同一日時に再起動されない工夫ができますが、そもそも固有の仮想マシン  
に対するメンテナンスはどのタイミングで実施されるのか知る必要がでてきます。  
以下は、2016/6時点でプレビュー版となりますが、固有の仮想マシンのメンテナンススケジュールを  
確認することができます。  

## 参考となるサイト

### Azureメンテナンスの監視について
Azure Instance Metadata Service -- プレビュー  
https://docs.microsoft.com/ja-jp/azure/virtual-machines/virtual-machines-instancemetadataservice-overview

Azure Metadata Service: スケジュールされたイベント (プレビュー)  
https://docs.microsoft.com/ja-jp/azure/virtual-machines/virtual-machines-scheduled-events

Azure VM のメンテナンス FAQ  
https://blogs.technet.microsoft.com/jpaztech/2016/03/25/azure-vm-sinins-maintenance-faq/


### その他　ユースケース/ブログ記事等


