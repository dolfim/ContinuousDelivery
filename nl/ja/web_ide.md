---

copyright:
  years: 2015, 2017
lastupdated: "2017-6-9"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}
{:pre: .pre}

# Eclipse Orion Web IDE での開発
{: #web_ide}

Eclipse Orion {{site.data.keyword.webide}} は、Web 開発を行うことのできるブラウザー・ベースの開発環境です。コンテンツ・アシスト、コード補完、エラー・チェックによる支援を利用して JavaScript、HTML、CSS での開発を行うことができます。{{site.data.keyword.webide}} は、ほとんどすべての言語に対応しており、大部分のファイル・タイプに対して構文の強調表示を提供します。ソース管理が組み込まれており、コードをローカルにデプロイしてアプリのテストとデバッグを行うことができます。
{:shortdesc}

何よりも良い点は、{{site.data.keyword.webide}} が Web ベースであるという点です。インストールが必要なものは何もなく、保守や拡大縮小が必要なものも何もありません。インターネット接続さえあれば、どこでも開発を行うことができます。

## IDE のセットアップ
{: #editorsetup}

{{site.data.keyword.webide}} はカスタマイズ可能であり、開発ニーズに合わせて、カラー・スキーム、テクニカル・ツール、および設定を選択することができます。これらの設定を表示したり変更したりするには、左側のメニューから**「設定」**アイコン<img class="inline" src="images/webide_settings_icon_light_small.png"  alt="設定アイコン">をクリックします。


編集中にしばしば設定を変更する必要がある場合は、**「ローカル・エディター設定」**アイコン <img class="inline" src="images/webide_local_settings_icon_light_small.png"  alt="「ローカル・エディター設定」アイコン">から簡単に設定にアクセスできます。

![ローカル・エディター設定](images/webide_local_editor_settings_light.png)

デフォルトでは、エディター・スタイルとフォント・サイズの設定が常に表示されます。他のエディター設定をメニューに含めるには、以下の手順を実行します。

1. **「ローカル・エディター設定」**アイコン<img class="inline" src="images/webide_local_settings_icon_light_small.png"  alt="「ローカル・エディター設定」アイコン">をクリックします。

2. **「エディター設定」**をクリックします。

3. **「ローカル・エディター設定」**メニューから設定を組み込んだり除外したりするには、各設定の星印をクリックします。

![「エディター設定」トグル](images/webide_editor_settings_toggle_light.png)


## コードの編集
{: #editcode}

{{site.data.keyword.webide}} には、2 つの主要セクションがあります。1 つ目のセクションはファイル・ナビゲーターであり、プロジェクト・ファイルがツリー構造で表示されます。ファイル・ナビゲーターから、ファイルとフォルダーの作成、名前変更、削除、管理を行うことができます。

**ヒント:** ファイルをファイル・ナビゲーターにアップロードするには、対象のファイルをコンピューターからファイル・ナビゲーターにドラッグします。

2 つ目のセクションはエディター・ペインです。このエディターは、コンテンツ・アシストや構文検査など、いくつかのコーディング機能を備えています。

![Web IDE](images/webide_light.png)

### 複数のファイルの処理
1. 2 つのファイルを同時に操作するには、**「分割エディター・モードを変更します」**アイコン<img class="inline" src="images/webide_split_editor_icon_light_small.png"  alt="「分割エディター」アイコン">をクリックします。
2. 開いたメニューから、1 つのビューを選択します。

 ビューを選択した後、既にエディターで開かれていたファイルがある場合、そのファイルは両方のエディター・ビューに表示されます。

 一方のエディター・ビューに表示されているファイルをオープンまたは変更するには、次のようにします。
 1. 変更するエディター・ビューにカーソルを移動します。
 2. ファイル・ナビゲーターで、いずれかのファイルをクリックします。

### キーボード・ショートカット
{{site.data.keyword.webide}} のコマンドの多くは、キーボード・ショートカットでもアクセス可能です。

エディターのキーボード・ショートカットのリストを表示するには、**「ツール (Tools)」** > **「キーの表示 (Show keys)」**をクリックします。または、Alt+Shift+? を押すか、MacOS の場合は Ctrl+Shift+? を押してリストを表示することもできます。キーの上に移動し、鉛筆をクリックして新しいキー・バインディングを入力することで、ショートカットをカスタマイズできます。

## ソース・コードの管理
{: #sourcecontrol}

{{site.data.keyword.webide}} は、ソース・コード管理ツールと統合されています。Git リポジトリーに関する作業を行うには、**「Git リポジトリー」**アイコン<img class="inline" src="images/webide_git_icon_light_small.png"  alt="「Git リポジトリー」アイコン">をクリックします。

 **ヒント**: {{site.data.keyword.webide}} をオープン・ツールチェーンと共に使用している場合、ワークスペースには GitHub、{{site.data.keyword.ghe_short}}、または Git Repos and Issue Tracking のリポジトリーが事前に取り込まれます。現行のツールチェーンと関連付けられているリポジトリーは強調表示されます。


## ワークスペースからのアプリのデプロイ
{: #deploy}

1. アプリをデプロイするには、実行バーから、起動構成を選択または作成します。![実行バー](images/webide_runbar_light.png)   
1. 「デプロイ」アイコン<img class="inline" src="images/webide_deploy_button_light_small.png"  alt="「デプロイ」アイコン">をクリックします。ワークスペースの現在の内容と、起動構成に定義された環境を使用して、アプリのインスタンスがデプロイされます。
2. アプリがデプロイされた後、実行バーを使用して、アプリの停止、再始動、デバッグ、ログの表示などを行うことができます。

<table>
<tr><td><img src="./images/stop_button.png"  alt="停止アイコン"></td><td>アプリを停止します</td></tr>
<tr><td> <img src="./images/open_app_url.png"  alt="アプリ URL を開くアイコン"></td><td> デプロイされたアプリを開きます</td></tr>
<tr><td><img src="./images/view_logs.png"  alt="ログ表示アイコン"></td><td>デプロイされたアプリのログを表示します</td></tr>
<tr><td><img src="./images/open_dashboard.png"  alt="ダッシュボードを開くアイコン"></td><td>アプリのダッシュボードを開きます</td></tr>
</table>

Node.js アプリを開発している場合は、ライブ編集モードを有効にします <img  src="./images/enable_live_edit.png"  alt="ライブ編集を有効にするスライダー">。

<table><tr><td><img src="./images/live_edit_restart.png"  alt="ライブ編集再開アイコン"></td><td>ライブ編集モードを有効にして、再デプロイメントなしでアプリを素早く再始動します</td></tr>
<tr><td> <img src="./images/debug_icon.png"  alt="デバッグ・アイコン"></td>
<td>ライブ編集モードを有効にして、デバッガーにアクセスします
</td></tr>
</table>

<!-- 3/6/2016: bl commands don't work with V2/CD
## Editing outside of the {{site.data.keyword.webide}}
{: #editlocal}

To use an editor besides the {{site.data.keyword.webide}}, set up {{site.data.keyword.Bluemix_live}} so that you can work directly with your project files in any tool. {{site.data.keyword.Bluemix_live_notm}} is a command-line application that synchronizes the changes in your local file system with your cloud workspace in {{site.data.keyword.jazzhub}}.

### Before you begin

Download and install the [{{site.data.keyword.Bluemix_live_notm}} command-line interface ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://livesyncdownload.ng.bluemix.net){: new_window}.

### Synchronizing your local environment with {{site.data.keyword.Bluemix_notm}}
{: #edit_local_download}

1. Open a command-line window.
2. Sign in to {{site.data.keyword.Bluemix_notm}}:

	```
	bl login
	```
	{: pre}

3. When you are prompted, enter your IBMid and password.
4. View a list of your {{site.data.keyword.Bluemix_notm}} projects:

	```
	bl projects
	```
	{: pre}

4. Synchronize your local environment with your project on {{site.data.keyword.Bluemix_notm}}:

	```
	bl sync projectName
	```
	{: pre}

where `projectName` is your {{site.data.keyword.Bluemix_notm}} app's name.

When you are finished editing, enter `q` to end synchronization.

### Enabling the Desktop Sync feature to edit code locally

The Desktop Sync feature is like Live Edit mode for the command line. You need the Desktop Sync feature to debug on the command line.
1. In another command-line window, enable the Desktop Sync feature:

	```
	cd localDirectory
	bl start
	```
	{: codeblock}

2. Use the launch configuration that you created in the {{site.data.keyword.webide}}. After you select the launch configuration, the Desktop Sync feature is enabled in your local environment. In the command-line window that you just opened, you can view the app's URL, the debug URL, the manage URL, and view the {{site.data.keyword.Bluemix_live_notm}} state.

3. Refresh the browser and verify that you can see the changes that you saved to static files in the local workspace.

### Disabling the Desktop Sync feature

1. In the second command-line window, enter `bl stop`.
2. In the first command-line window, enter `q`.

-->

## サポートされる言語
{: #supported_languages}

Eclipse Orion {{site.data.keyword.webide}} では、JavaScript、HTML、CSS、Markdown の各ファイルでコンテンツ・アシスト、ツールチップ、プレビュー、妥当性検査、構文強調表示を利用できます。構文強調表示は、以下のファイル・タイプでも使用できます。

<table>
<tr>
<td>
<ul><li>Arduino
</li><li>C</li>
<li>C#
</li><li>C++
</li><li>CoffeeScript
</li><li>CSHTML
</li><li>組み込み JavaScript (ejs)
</li><li>Erlang
</li><li>Go
</li><li>HTML 抽象化マークアップ言語 (Haml)
</li><li>Jade
</li><li>Java
</li><li>JSON
</li><li>Less  
</li><li>Lua  
</li><li>Objective-C
</li><li>PHP
</li><li>Python</li></ul>
</td>
<td>
<ul><li>Ruby
</li><li>Sass/SCSS
</li><li>SQL
</li><li>Swift
</li><li>TypeScript
</li><li>Visual Basic (vb)
</li><li>VMHTML
</li><li>XHTML
</li><li>XML
</li><li>XQuery
</li><li>YAML
</li><li>Launch ファイル 	
</li><li>Dockerfile
</li><li>gitignore
</li><li>git config
</li><li>cfignore
</li><li>properties
</li></ul>
</td>
</tr>
</table>

## チュートリアルを始める: Eclipse Orion Web IDE
{: #toolchain_tutorials}

[IBM&reg; Cloud Garage Method ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://www.ibm.com/cloud/garage){:new_window} の以下のチュートリアルのいずれかをチェックアウトします。
  * [Create and use your first toolchain (GitHub) ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://www.ibm.com/cloud/garage/tutorials/tutorial_toolchain_flow?task=1){:new_window}
  * [Create a toolchain that uses Git Repos and Issue Tracking ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://www.ibm.com/cloud/garage/tutorials/tutorial_toolchain_cfv2?task=1){:new_window}
  * [Create and use a microservices toolchain with DevOps Insights (v2) ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://www.ibm.com/cloud/garage/tutorials/tutorial_toolchain_microservices_cd?task=1){:new_window}
