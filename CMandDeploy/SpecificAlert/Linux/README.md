# OMS Log Analyticsの利用

本ページでは Microsoft Azure OMS(Operational Management Suite)にあるLog Analyticsを使った特定ログの監視方法を紹介します。

〇はじめに
    システム監視にはサービス監視とリソース監視と大きく２つに分かれますが、ここではリソース監視の中で特定のアプリケーションが
    syslog/rsyslog経由で出力する「特定のメッセージ」を監視対象にする、という条件に対して、Azureのサービスをどのように利用すること
    で本条件を満たすかを中心に有益なサイトをピックアップしています。
    例：apacheのhttpdが落下したメッセージを定期的に監視対象とし、落下したメッセージを検知した場合は任意のメールアドレスへアラート
    　　メールを送る、または用意した一次対応スクリプトを走らせる。

〇参考となるサイト
    【Azure CentOS7.xの環境におけるrsyslogを使った特定ログの監視とアラートメールの発信について】
        http://akazure.hatenablog.com/entry/2017/06/05/155201


