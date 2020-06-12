## 1.构建入口
### 构建步骤：
1. 入口文件在build.js，通过config.js不同的配置，进行文件对应的编译
2. aliases和resolve，分别是追踪文件地址和获取文件地址头
3. 例如enter构建入口是web/entry-runtime.js，追踪获取到地址src/platforms/web/entry-runtime.js
4. entry-runtime.js经过rollup构建打包在dist生成