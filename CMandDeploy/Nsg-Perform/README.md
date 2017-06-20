# NSGのトラフィックログを分析したい

本ページではNSG(Network Security Group)ログの監視方法を紹介します。

## はじめに
NSG(Network Security Group)はMicrosoft Azureが提供するFirewall的な機能ですが、どのルールに対して
何件該当してフィルタリングされたのか、といったNSGログを出力させることができます。  
本記事ではこのNSGログを分析するためにLog Analyticsを使った可視化やログそのものの確認方法などに触れて  
います。  

## 参考となるサイト

### NSGログ分析について
ネットワーク セキュリティ グループ (NSG) のためのログ分析  
https://docs.microsoft.com/ja-jp/azure/virtual-network/virtual-network-nsg-manage-log

### その他　ユースケース/ブログ記事等
Log Analytics で NSG のログ分析  
http://www.cloudou.net/log-analytics/loga002/

Network Security Group(NSG) のログを確認してみました   
http://75.live-style.jp/?p=1268

