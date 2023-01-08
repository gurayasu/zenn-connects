---
title: "Laravel Artisan【拡張機能】をDocker環境で使う"
emoji: "🐥"
type: "tech" # tech: 技術記事 / idea: アイデア
topics: [laravel]
published: true
---

# 1. 概要

- Laravel 向けの拡張機能`Laravel Artisan`を Docker 環境で使うための Tips です。
- コマンドパレットから Artisan コマンドを実行できる便利ツールですが、Docker 環境で使うには設定が必要でした。

https://marketplace.visualstudio.com/items?itemName=ryannaddy.laravel-artisan

https://habataki-blog.com/laravel-artisan-vscode-extensions/

# 2. Docker 環境で使うための設定

###### 2-1. まずは拡張機能をインストールして設定を開きます

![](https://storage.googleapis.com/zenn-user-upload/a54e3d6125d7-20230108.png)

###### 2-2. Docker で実行するのでチェック

![](https://storage.googleapis.com/zenn-user-upload/131b973d2fab-20230108.png)

###### 2-3. Artisan コマンドを実行するコンテナを起動するコマンドを書きます

`app`というサービス名のアプリケーションコンテナで、Artisan コマンドを実行するのでこのような書き方をしてます。`app`の部分は自分の環境に合わせて変えます。

![](https://storage.googleapis.com/zenn-user-upload/205f88834f22-20230108.png)

![](https://storage.googleapis.com/zenn-user-upload/57df8ed2d83a-20230108.png)

# 3. コマンドパレットから実行

コマンドパレットを開いて`Artisan`と入力すれば候補が出るのでクリックするだけです。
ターミナルを開かず実行できるので便利！

![](https://storage.googleapis.com/zenn-user-upload/6e9c99d4851a-20230108.png)
