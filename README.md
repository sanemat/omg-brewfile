omg-brewfile
============

OMGで開発に必要なパッケージをインストールします

利用方法
============

1. Apple DeveloperサイトからCommand Line Toolをダウンロードしてインストールする
    * https://developer.apple.com/jp/
2. このリポジトリをForkして自分のインストールしたいソフト追加する
    * https://github.com/phinze/homebrew-cask/tree/master/Casks
    * https://github.com/Homebrew/homebrew/tree/master/Library/Formula
3. ``rake brew:setup``
4. ``rake brew:bundle``
5. ``rake nodebrew:setup``
6. ``rake nodebrew:install``

Q & A
============

A. AppStoreからインストールしたAlfredがbrew-caskでインストールしたアプリケーションを認識しません。

Q. brew-caskでalfredをインストールして以下のコマンドを実行してください

```shell
brew cask alfred link
```
