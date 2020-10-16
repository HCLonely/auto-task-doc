---
title: 参与开发
lang: zh-CN
---

## 如何参与开发

1. Fork 本仓库
2. 克隆仓库到本地
3. 运行`npm install`安装依赖
4. 添加功能/修复 BUG
5. 运行`npm test`无报错
6. 提交 PR

## 代码风格

1. [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)
2. 源码尽量使用新版 ES 特性

## 目录结构

```shell
auto-task # 根目录
├── auto-task-helper.user.js # 辅助脚本，用于获取Discord auth
├── auto-task-test.user.js # auto-task脚本预览版
├── auto-task.user.js # auto-task脚本正式版版
├── build.dev.js # 用于处理预览版js文件
├── build.js # 用于处理正式版js文件
├── package.json
├── gulpfile.js # 用于构建脚本及网站
├── docs # 预览版设置页面网站目录（自动生成）
|  └── ...
├── public # 正式版设置页面网站目录（自动生成）
|  └── ...
├── lib # gulp插件目录
|  ├── doSomething.js # js文件处理
|  ├── log.js # 预定义控制台日志样式
|  └── minCss.js # 处理并压缩css文件
├── require # 脚本依赖的静态文件目录
|  ├── require.min.js # 依赖js文件，由/src/requirejs文件夹内的文件打包而来
|  ├── fuck-task.min.css # 依赖css文件，由/src/style文件夹内的文件打包而来
|  ├── fuck.cur
|  ├── iconfont.eot
|  ├── iconfont.svg
|  ├── iconfont.ttf
|  ├── iconfont.woff
|  └── iconfont.woff2
└── src # 源码目录
   ├── helper # 辅助脚本源码目录
   |  └── auto-task-helper.user.js # 辅助脚本
   ├── page # 设置网站源码目录
   |  ├── img # 图片目录
   |  |  └── ...
   |  ├── index.html
   |  ├── js
   |  |  ├── lang # 设置页面i18n语言目录
   |  |  |  ├── zh-CN.json # 中文
   |  |  |  └── en-US.json # 英文
   |  |  ├── i18n.js
   |  |  └── main.js
   |  ├── setting.html # 设置页面
   |  ├── time.html # 倒计时页面(中文)
   |  └── time_en.html # 倒计时页面(英文)
   ├── requirejs # 依赖js文件夹
   |  ├── js.cookie.min.js
   |  ├── jquery.min.js
   |  ├── effect.min.js
   |  ├── popper.min.js
   |  ├── bootstrap.min.js
   |  ├── runtime.min.js
   |  ├── sweetalert2@9.min.js
   |  ├── polyfill.min.js
   |  ├── overhang.min.js
   |  └── sha1.min.js
   ├── scripts # 脚本源码目录
   |  ├── config.js # 配置项处理
   |  ├── defaultConf.js # 默认配置
   |  ├── header.js # UserScript头部信息
   |  ├── i18n.js # i18n相关
   |  ├── main.js # 功能函数整合
   |  ├── lang # 脚本i18n语言目录
   |  |  ├── zh-CN.json # 中文
   |  |  ├── en-US.json # 英文
   |  ├── function # 功能函数目录
   |  |  ├── getAuth.js # 获取Discord凭证
   |  |  ├── httpRequest.js # http请求函数
   |  |  ├── log.js # 输出任务日志
   |  |  ├── main.js # 加载ui及功能
   |  |  ├── tool.js # 工具库
   |  |  └── social # 社交相关任务
   |  |     ├── discord.js # discord相关任务
   |  |     ├── instagram.js # instagram相关任务
   |  |     ├── reddit.js # reddit相关任务
   |  |     ├── steam.js # steam相关任务
   |  |     ├── toggleActions.js # 社交任务整合分配
   |  |     ├── twitch.js # twitch相关任务
   |  |     ├── twitter.js # twitter相关任务
   |  |     ├── vk.js # vk相关任务
   |  |     └── youtube.js # youtube相关任务
   |  └── website # 各网站相关功能函数目录
   |     ├── main.js # 自动生成，修改无用！
   |     ├── main.template # main.js的模板，用于生成main.js
   |     └── [website].js # 各网站相关功能函数
   └── style # 样式表目录
      ├── bootstrap.min.css
      ├── iconfont.min.css
      ├── other.css # 新增样式请放到这个文件里，不要修改其他文件
      └── overhang.min.css
```
