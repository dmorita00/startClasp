## GASを有効化
https://script.google.com/home/usersettings

# 既存のスプレッドシートを使用する場合

1. ログインする（CLI）
    ```shell
    clasp login
    ```
2. envファイルを作る
    ```shell
    cp .env.template .env
    ```
3. スプレッドシートを作成する（ブラウザ）
4. GASを作成する（ブラウザ）
5. デプロイする（ブラウザ）
   1. Webappを選択する
   2. DeploymentIDをenvに貼り付ける
6. cloneする（CLI）
    ```shell
    clasp clone <スクリプトファイルのURL>
    ```
7. clasp.jsonを編集する
    ```json
    {
        "scriptId":"<スクリプトID>",
        "rootDir":"./dist"
    }
    ```
8. appsscript.jsonをdistへ移動する

参考：

https://www.ykicchan.dev/posts/2020-07-12
https://yuru-wota.hateblo.jp/entry/GAS/Create-Project-via-Clasp

# yarnを使う場合

- ライブラリをインストール

```shell
rm -rf .yarn*
yarn set version berry
yarn install
```

- .yarnrc.ymlを編集する

```shell
nodeLinker: node-modules # 追加
```

## GAS GCP連携
https://blog.gluegent.com/2022/04/gas-3-gasgcp.html
