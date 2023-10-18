# VRC PosterSystem

## What is This

インターネット上の画像を収集して、GitHub Pages上に表示するツールです。

VRChatには、インターネット上の画像をワールドに表示するシステムがあります。
([Image Loading | VRChat Creation](https://creators.vrchat.com/worlds/udon/image-loading/))

画像DLの際に悪意のあるURLにアクセスしないために、whitelist方式でのドメイン制限があります。
whitelistに登録されているドメインにて、固定URLで画像を任意に変更できるドメインは`*.github.io`のみになります。

"Allow Untrusted URLs"という設定を有効化することで、whitelist外のURLも読み込むことができますが、そう言わずに、「面倒なことを相手に要求せずに、world上に示したい!!」という方向けのシステムになります。

## Usage

downloadlist.csvを編集します。

|設定項目名|説明|
|:--|:--|
|Output File Name|GitHub Pagesに設定するファイル名, ダウンロード先のファイル名と異なる名前でも可|
|URL|ダウンロード先|

GitHubのレポジトリから"Settings"->"Pages"に遷移、
"Build and deployment"から、Sourceを"GitHub Actions"に変更します

GitHub Actionsから、"Update Poster"を実行します。

## Lisense

ソースコードライセンス: MIT License
GitHub Pagesに表示される画像ライセンス: 各画像のオリジナルのライセンス
