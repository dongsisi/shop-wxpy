# WePY - 小程序的组件化开发框架

## wepy vs mpvue

- [腾讯 WePY](https://tencent.github.io/wepy/)
  - ![wepy](./imgs/wepy.png)
- [美团 mpvue](http://mpvue.com/)
  - ![mpvue](./imgs/mpvue.png)

## quick start

- [wepy 开发文档](https://tencent.github.io/wepy/document.html#/)
- 1 全局安装 cli：`npm i -g wepy-cli`
  - 查看版本：`wepy --version`
- 2 通过脚手架初始化项目结构：`wepy init empty my-project`
  - empty 空模板
- 3 进入项目根目录，安装项目所有依赖项：`npm i`
- 4 启动项目，并开启实时编译：`wepy build --watch` or `npm run dev`
- 5 使用 微信开发者工具 打开 `dist` 目录
- 6 在 微信开发者工具中 配置：
  - 关闭：ES6 转 ES5
  - 关闭：上传代码时样式自动补全
  - 关闭：代码压缩上传
  - 开启：不校验合法域名

```shell
# 初始化 standard（示例） 模板项目
wepy init standard my-project
```

## .wpy 文件语法高亮

- 1 安装 `vetur` 插件（Vue 插件）
- 2 打开任意 `.wpy` 文件
- 3 点击右下角的选择语言模式，默认为`纯文本`
- 4 在弹出的窗口中选择 `.wpy 的配置文件关联...`
- 5 在`选择要与 .wpy 关联的语言模式` 中选择 `Vue`

## 不校验 wepy 文件的 template

- 在 VSCode 中添加配置：`"vetur.validation.template": false`

## 功能实现

- 1 结构+样式
- 2 data 假数据
- 3 获取接口数据

## 开启 Promise 和 async

- [开启 async](https://github.com/Tencent/wepy/wiki/wepy%E9%A1%B9%E7%9B%AE%E4%B8%AD%E4%BD%BF%E7%94%A8async-await)

## 解析 HTML

- 说明：将 HTML 解析为 wxml
- 使用场景：服务器端返回的商品详情是 HTML 字符串，需要转化为 wxml 才能展示
- [wxParse](https://github.com/icindy/wxParse)
