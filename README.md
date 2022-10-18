# WebViewTest
WebViewによるモデルの見方を体験いただけるDemoです。

## モデルのWebViewの作成
WebViewの作成はSimulink Report Generatorが持つ機能です。

下記リンクに示す通り、Simulink ライセンスがなくても、Web ビューの参照、移動、共有が可能です。
https://jp.mathworks.com/help/rptgenext/ug/tutorial-creating-web-views-of-simulink-models.html

下記２つのリンク先にはSimulinkより出力されたWebViewを閲覧できます。

## System Composer or Simulink編集画面からWebViewの作成

下記の通り”保存”→”モデルのエクスポート先”→”WebView”を選択いただくと

- WebView形式のHTMLファイル:webview.html
- スタイルシート:stylesheetsフルだ
- インタラクティブ表示をするスクリプト記述：supportフォルダ

![Snag_1ea6a34](https://user-images.githubusercontent.com/62166747/196384738-a16febba-e756-48c5-838b-6acc17a37693.png)
を生成できます。

![Snag_1d65d44](https://user-images.githubusercontent.com/62166747/196379420-ce912bc8-32e1-432e-b80e-f71bbdd21a87.png)

あとは任意のWebサーバーに上記すべてのファイルをアップロードするだけで共有が可能になります。
例としてGitHubに設定されたHTTPサーバーにアップロードを行った結果を下記リンク先で確認できます。

https://griffin921.github.io/WebViewTest/SystemComposer_Webview/webview.html


## Requirements ToolboxからWebViewの作成
WebViewはRequirements Toolbox側からも生成できます。
この場合前者の方法で生成されたものより、要件データがより見やすい形でWebView出力がされるのでおすすめでございます。

まずSimulinkおよびSystemComposerの上部ツールストリップから
アプリ→要件マネージャを選択して”要件”タブを表示していただきます。

次に下記図が示す通り、
共有→モデルをWebビューにエクスポートを選択してください。
![Snag_1e3da64](https://user-images.githubusercontent.com/62166747/196382879-f3a64c26-12ea-4a44-b494-b23bc947399d.png)

前者の操作と同様にWebViewファイルが生成されますが、下記リンク先に示す通り要件情報がより見やすくなります。

https://griffin921.github.io/WebViewTest/ReqTbx_Webview/webview.html

## SharepointでのWebViewの公開について

上記 GitHubでの例の通り、Webサーバに配置さえすれば問題なく閲覧は可能です。
一方でSharepointで共有する際にはhtmlファイルをそのまま配置しても閲覧はできず、
.master拡張子のファイルに変換が必要になります。

この変換においてはMicrosoft側の範疇になります。

Microsoftのサポートページを調べたところ、
Sharepointにはhtmlファイルをsharepointページに変換するような機能があるようですが、
おそらく、これはSharepoint管理者側に提供されている機能であって、閲覧ユーザにおいては
この機能が制限されている場合もあるかとおもいます。

https://learn.microsoft.com/ja-jp/sharepoint/dev/general-development/how-to-convert-an-html-file-into-a-master-page-in-sharepoint

Sharepointで下記機能が利用できるかどうかは、お客様の所属組織のセキュリティポリシーによって変わると思いますので、
IT担当部署等にお問い合わせください。


## ご注意　ローカルで生成されたファイルを閲覧する場合

下記リンク先に記述されている通りブラウザごとに設定が必要です。
https://jp.mathworks.com/help/rptgenext/ug/open-a-web-view.html#bt8ff54

これはブラウザに対して「ローカルファイルを開く際のセキュリティエラーを回避する旨を指定する設定になります。
例：Google chromeの対処法に対する解説：https://developer.chrome.com/blog/debugging-the-filesystem-api/


