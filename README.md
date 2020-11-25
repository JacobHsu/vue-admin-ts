# vue-admin-ts

vue-element-admin [guide](https://panjiachen.github.io/vue-element-admin-site/zh/guide/)
Typescript 版: [vue-typescript-admin-template](https://github.com/Armour/vue-typescript-admin-template)

## setting

mock-server.ts

```js
const app = express()
const port = 9528
```

vue.config.js

```js
const devServerPort = 9527 // TODO: get this variable from setting.ts
const mockServerPort = 9528 // TODO: get this variable from setting.ts
```

## mock

package.json

```js
  "scripts": {
    "mock": "cd mock && ts-node-dev mock-server.ts"
  },
```

yarn mock

http://localhost:9528/mock-api/v1/articles

## vue cli

```js
  "dependencies": {
    "core-js": "^2.6.5",
    "vue": "^2.6.10",
    "vue-class-component": "^7.0.2",
    "vue-property-decorator": "^8.1.0",
    "vue-router": "^3.0.3",
    "vuex": "^3.0.1"
  },
```

## typescript

`vue-class-component` 是一個 Class Decorator,也就是類的裝飾器
`vue-property-decorator` 是基於 vue 組織裡 vue-class-component 所做的拓展
`vuex-module-decorators`: 用 typescript 寫 vuex 很好用的一個庫

## vue.config.js

style-resources-loader