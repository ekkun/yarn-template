# Yarn Template

## npm パッケージをインストール

```terminal
#プロジェクトのディレクトリに移動して
$ yarn
```

<!-- npm install -->

## yarn の監視

```
$ yarn start
```

<!--
 mode development
$ yarn dev
-->

## 納品ファイル生成

デプロイ用のファイル一式を生成

```
$ yarn build
```

## ディレクトリ構成

./src/ 内のファイルを編集

- pug -> html
- js -> babel -> js
- sass -> css

```
├─ node_modules/
│  └─ パッケージ各種
│
├─ dist/（ビルド後、納品ファイルがここに生成される）
│  ├─ assets/
│  │  ├─ css/
│  │  ├─ images/
│  │  ├─ js/
│  │  ├─ json/
│  │  ├─ media/
│  │  └─ webfonts/
│  └─ index.html など
│
├─ src/（ビルド前のソース）
│  ├─ assets/
│  │  ├─ images/
│  │  ├─ json/
│  │  ├─ media/
│  │  └─ webfonts/
│  ├─ js/
│  │  ├─ _app/
│  │  ├─ _core/
│  │  └─ functions.js など
│  ├─ pug/
│  │  ├─ _template/
│  │  └─ index.pug
│  └─ sass/
│      ├─ foundation/
│      ├─ layout/
│      ├─ object/
│      ├─ page/
│      │  └─ index/
│      ├─ style.scss
│      └─ index.scss
│
├─ .browserslistrc
├─ .eslintrc
├─ babel.config.js
├─ package.json
├─ stylelint.config.js
├─ tsconfig.json
├─ webpack.config.js
└─ README.md
```

## 参考・参照

- [frontend_develop_environment](https://github.com/macotok/frontend_develop_environment)

- [stylelint.config.js](https://gist.github.com/buchiya4th/f4ca1be2ab98ee5a8098fa68a93e752c)
