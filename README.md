# Vertical BlogTheme

このテーマははてなブログのデザインテーマです。

## 開発するには？

このテーマははてなブログの Boilerplate テーマをベースにしています。

- <https://github.com/hatena/Hatena-Blog-Theme-Boilerplate>

SCSSで開発する場合は、下記の手順でリポジトリのcloneとモジュールのインストールを行います。

### 必要なもの

- [Node.js](http://nodejs.org/)
  - Windows 環境の場合は 8.x をご用意することをおすすめします。 (10.x 以降では node-sass の実行に失敗する可能性があります。)

### モジュールのインストール

```
$ git clone https://github.com/aokashi/vertical-blogtheme.git
$ cd vertical-blogtheme
$ npm install
```

### 通常のテーマ開発

下記のコマンドで、SCSSファイル変更の監視とコンパイルを行います。

```
$ npm start
```

また、コンパイル後 `build/boilerplate.css` が作られます。

つづいて、[はてなブログ](http://blog.hatena.ne.jp/)でテーマ検証に使うブログを1つ用意します。ブログの「設定」->「詳細設定」にアクセスし、「headに要素を追加」欄に下記を貼り付けて保存します。

```
<link rel="stylesheet" href="http://localhost:3000/boilerplate.css"/>
<script async src="http://localhost:3000/browser-sync/browser-sync-client.js"></script>
```

以降は、ブログを開いた状態でSCSSファイルを保存すると、変更したスタイルが自動的に反映されます。

## 構成

```
vertical-blogtheme/
|- scss/
|  |- lib/
|  `- boilerplate.scss
`- build/
   `- boilerplate.css
```

## ライセンス
このCSSおよびSCSSファイルはMITライセンスのもと自由に複製・再配布できます。 記事本文の書式やコメント欄のスタイルなど、必要な部分だけをコピーして使ってもかまいません。 このデザインテーマをもとにしたテーマの配布も自由です。
