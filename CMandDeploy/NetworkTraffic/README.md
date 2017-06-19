# ネットワークトラフィック（利用帯域）を監視したい

本ページではGestOS側ネットワークの監視方法を紹介します。

## はじめに
GestOS側で突発的な負荷や想定外の事象が確認された時、ネットワーク経路や帯域の情報を必要とするケースが  
あります。本記事ではLog Analyticsを使ったネットワークパフォーマンスのモニタリングや、GestOSに  
設定するタイプのNetwork Watcherを使い、仮想マシンから見たネットワークの可視化について触れています。  
統計的な情報としてご利用いただくことも可能となっており、不特定多数のoutbound通信を制御する際に  
どの経路を残しどの経路が必要、といった判断する上でも役立つものがあります。  

## 参考となるサイト

### ネットワーク監視について
Log Analytics のネットワーク パフォーマンス モニター ソリューション  
https://docs.microsoft.com/ja-jp/azure/log-analytics/log-analytics-network-performance-monitor

Azure のネットワーク監視の概要  
https://docs.microsoft.com/ja-jp/azure/network-watcher/network-watcher-monitoring-overview

Log Analyticsとは  
https://docs.microsoft.com/ja-jp/azure/log-analytics/log-analytics-overview


### その他　ユースケース/ブログ記事等
ネットワーク調査ツール「Network Watcher」を見る！！   
http://www.cloudou.net/virtual-network/vnet013/

Azureネットワークウォッチャーでパケットキャプチャー  
http://ccnw-jun.hatenablog.com/entry/2017/03/12/151555


