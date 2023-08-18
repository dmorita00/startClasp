# 既存のスプレッドシートを使用する場合

1. ログインする
    ```shell
    clasp login
    ```
2. スプレッドシートを作成する
3. cloneする
    ```shell
    clasp clone <スクリプトファイルのURL>
    ```
4. clasp.jsonを編集する
    ```json
    {
        "scriptId":"<スクリプトID>",
        "rootDir":"./dist"
    }
    ```
5. appsscript.jsonをdistへ移動する

参考：

https://www.ykicchan.dev/posts/2020-07-12
https://yuru-wota.hateblo.jp/entry/GAS/Create-Project-via-Clasp
