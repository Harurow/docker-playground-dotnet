# Docker Playgorund - dotnet

コンテナ上でdotnetの実行環境を構築しVisual Studio Codeから接続・実行できる環境を提供する

コンテナイメージのベースは
[mcr.microsoft.com/dotnet/sdk:6.0](https://mcr.microsoft.com/en-us/product/dotnet/sdk/about)
を利用。最新の最小限の環境としている。

追加で以下をインストールしている

* `git`
* `curl`

実行ユーザ:`vscode`  
ワークスペース:`/workspace`  

ホスト側の`workspace`フォルダをコンテナ側の`/workspace`としてマウントしている

以下のVisual Studio Code 拡張をインストール

* EditorConfig.EditorConfig
* ms-dotnettools.csharp
* Ionide.Ionide-fsharp

## 使い方

[Docker Desktop](https://www.docker.com/products/docker-desktop/)を立ち上げる

[Visual Studio Code](https://azure.microsoft.com/ja-jp/products/visual-studio-code/)に[Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)をインストール

後は Dev Containerで起動する
