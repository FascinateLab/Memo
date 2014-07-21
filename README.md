
勢いでアカウントを作成したけど使い道が無いので、  
今後の利用方法を考えて見るテスト。

現在（2014/07/01時点）でのMinecraftの【旧バージョン】のModding環境の構築方法を記載してみた。  
Minecraftの環境構築が上手く行かない場合はこれらを試して見ると  
運が良ければ環境構築に成功するかも知れません。

環境構築の方法は各txtファイルをご覧ください。

現在のMinecraftのModding環境の構築はMinecraftの環境変更のゴタゴタ続きで  
普通にinstall.bat(.sh)を実行してもModding環境が構築できないバージョンも存在しますので。

＜基本的な注意点＞  
旧MCPはJava6で操作する事を前提に作成されていますので、  
環境構築用にJava6を用意しておくと良いです。  
Java7でも構築は可能ですが、Java8は構築できない可能性があります。  
Java8に対応したのはv1.7.2の中期辺りです。  
Javaの切り替えはOSによって違うので適当に調べてください。


＜ubuntu 14.04 LTS環境の注意点＞  
ubuntu 14.04 LTS環境の場合、幾つか注意点があります。

１つは環境構築などの処理にwindowsプログラムを使用しているため、  
事前にwineをインストールしておく必要がある。  
（mcpのdocに書いてありますし、インストール中に注意が出ます）

もう１つはv1.5.2以下のMinecraftはmcpやForgeがダウンロードしてくる  
LWJGLライブラリ（v2.4.2）ではクライアントの起動時にエラーが発生します。

解決策はLWJGL（ http://lwjgl.org/ ）から新しいライブラリ（v2.9.0など）をダウンロードして導入します。

binフォルダの内部を把握している場合は.minecraft/librariesフォルダと  
.minecraft/versionsフォルダから必要なファイルを集めてくるだけで問題ありません。

by,flabs
