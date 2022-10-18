# WebViewTest
WebViewによるモデルの見方を体験いただけるDemoです。

## モデルのWebViewの作成
WebViewの作成はSimulink Report Generatorが持つ機能です。

下記リンクに示す通り、Simulink ライセンスがなくても、Web ビューの参照、移動、共有が可能です。
https://jp.mathworks.com/help/rptgenext/ug/tutorial-creating-web-views-of-simulink-models.html

下記２つのリンク先にはSimulinkより出力されたWebViewを閲覧できます。

## System Composer or Simulink編集画面からWebViewの作成

下記の通り”保存”→”モデルのエクスポート先”→”WebView”を選択いただくと
- WebView形式のHTMLファイル
- スタイルシート
- Javascriptによるインタラクティブ表示をするスクリプト記述
を生成できます。
![Snag_1d65d44](https://user-images.githubusercontent.com/62166747/196379420-ce912bc8-32e1-432e-b80e-f71bbdd21a87.png)

あとは任意のWebサーバーにすべてをアップロードするだけで共有が可能になります。
例としてGitHubに設定されたHTTPサーバーにアップロードを行った結果を下記リンク先で確認できます。




## Requirements ToolboxからWebViewの作成


## ご注意　ローカルで生成されたファイルを閲覧する場合

下記リンク先に記述されている通りブラウザごとに設定が必要です。
https://jp.mathworks.com/help/rptgenext/ug/open-a-web-view.html#bt8ff54

これはブラウザに対して「ローカルファイルを開く際のセキュリティエラーを回避する旨を指定する設定になります。
例：Google chromeの対処法に対する解説：https://developer.chrome.com/blog/debugging-the-filesystem-api/
