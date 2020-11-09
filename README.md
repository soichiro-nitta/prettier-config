# @soichiro_nitta/prettier-config

.prettierrc.jsに記述する設定をパッケージ化しました。

https://www.npmjs.com/package/@soichiro_nitta/prettier-config



## 使い方

`prettier`と`@soichiro_nitta/prettier-config`をインストール後、`.prettier.js`で呼び出してエクスポートします。

以下を実行します

```
yarn add -D prettier @soichiro_nitta/prettier-config
```

npmの場合

```
npm install --save-dev prettier @soichiro_nitta/prettier-config
```

`.prettierrc.js`


```
const { prettierConfig } = require('@soichiro_nitta/prettier-config')

module.exports = prettierConfig
```

ルールはお好みで上書きが可能です

```
const { prettierConfig } = require('@soichiro_nitta/prettier-config')

module.exports = {...prettierConfig, ...{
  semi: true,
}}
```
