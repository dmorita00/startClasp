## claspをインストール
https://github.com/google/clasp?tab=readme-ov-file

-  GASを有効化
https://script.google.com/home/usersettings

## 準備
1. ログインする（CLI）
    ```shell
    clasp login
    ```
2. clasprc.jsonをプロジェクトルートに移動させる
   ```
   cp /Users/username/.clasprc.json ./
   ```

## 既存のファイルを使用する場合
1. cloneする（CLI）
    ```shell
    clasp clone <スクリプトファイルのURL>
    ```
2. clasp.jsonを編集する
    ```json
    {
        "scriptId":"<スクリプトID>",
        "rootDir":"./dist"
    }
    ```
3.  appsscript.jsonをdistへ移動する

## デプロイする場合
1. envファイルを作る
    ```shell
    cp .env.template .env
    ```
2. スプレッドシートを作成する（ブラウザ）
3. GASを作成する（ブラウザ）
4. デプロイする（ブラウザ）
   1. Webappを選択する
   2. DeploymentIDをenvに貼り付ける

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
