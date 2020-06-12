## 1.构建入口
### 构建步骤：
1. 入口文件在build.js，通过config.js不同的配置，进行文件对应的编译
2. aliases和resolve，分别是追踪文件地址和获取文件地址头
3. 例如enter构建入口是web/entry-runtime.js，追踪获取到地址src/platforms/web/entry-runtime.js
4. entry-runtime.js经过rollup构建打包在dist生成

### Runtime Only VS Runtime + Compiler
1. Runtime Only： 使用 Runtime Only 版本的 Vue.js 的时候，通常需要借助如 webpack 的 vue-loader 工具把 .vue 文件编译成 JavaScript，因为是在编译阶段做的，所以它只包含运行时的 Vue.js 代码，因此代码体积也会更轻量。
2. Runtime + Compiler： 没有对代码做预编译，但又使用了 Vue 的 template 属性并传入一个字符串，则需要在客户端编译模板。