# wepy-tony-demo
https://tencent.github.io/wepy/document.html#/


### WePY项目构建
- 小程序官方程序的默认模板

```
全局安装或更新WePY命令行工具

npm install wepy-cli -g
在开发目录中生成Demo开发项目

wepy new myproject
切换至项目目录

cd myproject
开启实时编译

wepy build --watch
```


### 重要提醒
- 使用微信开发者工具-->添加项目，项目目录请选择dist目录。

- 微信开发者工具-->项目-->关闭ES6转ES5。 重要：漏掉此项会运行报错。

- 微信开发者工具-->项目-->关闭上传代码时样式自动补全。 重要：某些情况下漏掉此项也会运行报错。

- 微信开发者工具-->项目-->关闭代码压缩上传。 重要：开启后，会导致真机computed, props.sync 等等属性失效。（注：压缩功能可使用WePY提供的build指令代替，详见后文相关介绍以及Demo项目根目录中的wepy.config.js和package.json文件。）

- 本地项目根目录运行wepy build --watch，开启实时编译。（注：如果同时在微信开发者工具-->设置-->编辑器中勾选了文件保存时自动编译小程序，将可以实时预览，非常方便。）
