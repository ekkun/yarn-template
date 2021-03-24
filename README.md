# Yarn Template

## npm パッケージをインストール

```terminal
#プロジェクトのディレクトリに移動して
// npm install
$ yarn
```

## yarn の監視

```
$ yarn start
// mode development
// $ yarn dev
```

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
│  │  ├─ fonts/
│  │  ├─ images/
│  │  ├─ css/
│  │  └─ js/
│  └─ index.html など
│
├─ src/（ビルド前のソース）
│  ├─ fonts/
│  ├─ html/ (直にHTMLを生成する場合)
│  ├─ images/
│  ├─ javascript/
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

## パッケージのバージョン管理

更新、アップデートの確認に npm-check-updates をインストールする

```
$ sudo npm install -g npm-check-updates
```

ncu コマンドでアップデート

```
$ ncu -u
```

## 参考・参照

- [frontend_develop_environment](https://github.com/macotok/frontend_develop_environment)

- [stylelint.config.js](https://gist.github.com/buchiya4th/f4ca1be2ab98ee5a8098fa68a93e752c)
