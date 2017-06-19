# Microsoft Azureに影響するメンテナンスを監視したい

本ページではMicrosoft Azure メンテナンスの監視方法を紹介します。  

## はじめに
一昔前までMicrosoft Azureのホスト側で行うメンテナンスについてはGestOS側にも影響が出る状態  
でしたので、突然仮想マシンが再起動する事象も多く、お客様からfeedbackのご意見を多く頂戴して  
おりました。現在、このメンテナンス方式はGestOS側に影響（再起動）が発生しない方式に変わって  
おります。

## 参考となるサイト

### Azureメンテナンスの監視について
Azure Instance Metadata Service -- プレビュー  
https://docs.microsoft.com/ja-jp/azure/virtual-machines/virtual-machines-instancemetadataservice-overview

Azure Metadata Service: スケジュールされたイベント (プレビュー)  
https://docs.microsoft.com/ja-jp/azure/virtual-machines/virtual-machines-scheduled-events

Azure VM のメンテナンス FAQ  
https://blogs.technet.microsoft.com/jpaztech/2016/03/25/azure-vm-sinins-maintenance-faq/


### その他　ユースケース/ブログ記事等


