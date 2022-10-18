# WebViewTest
WebViewによるモデルの見方を体験いただけるDemoです。

## モデルのWebViewの作成
WebViewの作成はSimulink Report Generatorが持つ機能です。

下記リンクに示す通り、Simulink ライセンスがなくても、Web ビューの参照、移動、共有が可能です。
https://jp.mathworks.com/help/rptgenext/ug/tutorial-creating-web-views-of-simulink-models.html

下記２つのリンク先にはSimulinkより出力されたWebViewを閲覧できます。

## System Composer or Simulink編集画面からWebViewの作成

出力結果の例はこちらになります。
生成されたモデルファイルをローカル環境下で閲覧する場合は下記リンク先に記述されている通り
ブラウザごとに設定が必要です。
https://jp.mathworks.com/help/rptgenext/ug/open-a-web-view.html#bt8ff54

これはブラウザに対して「ローカルファイルを開く際のセキュリティエラーを回避する旨を指定する設定になります。
例：Google chromeの対処法に対する解説：https://developer.chrome.com/blog/debugging-the-filesystem-api/


ローカルファイルを開くのではなく
任意のWebサーバーにアップロードする場合は特に設定の必要はありません。
例としてGitHubに設定されたHTTPサーバーにWebViewによって生成されたファイルをそのまま配置した結果を下記から確認できます。




## Requirements ToolboxからWebViewの作成