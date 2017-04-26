# Unicorn Script

* 対象：CapistranoにてDeployしている人向け

## 使い方(CeontOS6/AmazonLinux)

* `unicorn`ファイルのディレクトリやユーザーの環境変数を適宜変更
* 上記unicornファイルをサーバー上の`/etc/init.d/`配下に配置
* `chmod 755`で実行権限付与
* rootユーザーで`chkconfig unicorn on`で自動起動設定完了
* 以下のようにも起動処理/停止可能に

```
service unicorn start
service unicorn stop
```

## 使い方(CeontOS7)

* `unicorn`ファイルのディレクトリやユーザーの環境変数を適宜変更
* 上記unicornファイルをサーバー上の`/etc/init.d/`配下に配置
* `chmod 755`で実行権限付与
* `/usr/lib/systemd/system`配下に`unicorn.service`のファイルを配置
* `systemctl daemon-reload`実行
* `systemctl enable unicorn.service`で自動起動設定

### memo

* ちゃんと試しきれてないのでご利用は自己責任でお願いします
* 使う際はご自身の環境に合ったように自由にカスタマイズしてみて下さい

