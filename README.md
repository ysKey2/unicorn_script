# Unicorn Script

* 対象：AmazonEC2/CentOS6
* CapistranoにてDeployしている人向け

## 使い方

* ディレクトリやユーザーの環境変数を適宜変更
* unicornファイルをサーバー上の`/etc/init.d/`配下に配置
* `chmod 755`で実行権限付与
* rootユーザーで`chkconfig unicorn on`で自動起動設定完了
* 以下のようにも起動処理/停止可能に

```
service unicorn start
service unicorn stop
```

