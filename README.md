# morihiromusic.com サイトコンテンツソース

## 概要

本リポジトリは、morihiromusic.com のコンテンツを生成するためのソースファイル一式です。

- hugo によるスタティックページ生成
- 音楽を配信するため、mp3ファイルがコンテンツに含まれている (2020/03/05 現在)
- デプロイ時に basic認証の追加が必要なコンテンツがある

## 必要リソース

### hugo

下記 URL より、最新版をDLして使用(?)

https://github.com/gohugoio/hugo/releases

### hugo テンプレート

以下のサイトで公開されているテンプレートを使用している。

https://rakuishi.com/archives/hugo-zen/

## コンテンツのビルド方法

ビルド時に hugo-zen テンプレートが必要。hugo-zen テンプレートの git リポジトリから clone して使用する
hugo コマンドの実行により、public/ ディレクトリにデプロイ用のコンテンツ一式がビルドされる

```
$ cd themes/
$ git clone https://github.com/rakuishi/hugo-zen.git
$ cd -
$ hugo
```

## コンテンツの更新方法

- TBD

## Todo

- コンテンツから mp3 ファイルを分離
- アクセス制限対象コンテンツ (basic認証配下)の提供方法を検討

