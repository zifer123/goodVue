# goodvue

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

# 打包优化必看
``` bash
main.js判断了是否是开发环境，如果是快发环境，才引入必要的第三方css文件和Vue.use第三方库
config.js开启gzip压缩优化
如果以后还有需要引入的第三方库，第一步需要在webpack.prod.conf.js的externals配置项添加对应的键值对（值是第三方暴露的全局变量值）
参考这篇文章：https://juejin.im/post/5a291092518825293b50366d
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
