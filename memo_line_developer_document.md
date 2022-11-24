
# 修正したいところ
## [ライブラリをプロジェクトにインポートする](https://developers.line.biz/ja/docs/android-sdk/integrate-line-login/#import-library-into-your-project)でのライブラリインポート部分
- 気になったこと
    - 公式ドキュメントからコピペするとビルドが通らない
- どのように修正するか
    - 以下のように修正する
    ```
    implementation 'com.linecorp:linesdk:latest.release'
    ↓
    implementation 'com.linecorp.linesdk:linesdk:$linesdk_version'
    ```

## [LINE SDKに組み込まれているログインボタンを使う](https://developers.line.biz/ja/docs/android-sdk/integrate-line-login/#use-button)のサンプルコード
- 気になったこと
    - Kotlinのサンプルコードがない
- どのように修正するか
    - JavaとKotlin両方のソースコードを用意する