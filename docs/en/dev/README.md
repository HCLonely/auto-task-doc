---
title: Contribution
lang: en-US
---

> The content of this page is translated through Google translation. If the description is incorrect, please click 'Edit this page on GitHub' at the bottom of the page to help us improve the translation.

## How to participate in development

1. Fork this repo
2. Clone the repo
3. `npm install` to install dependencies
4. Add feature/fix bug
5. Run `npm test` without error
6. Submit PR

## Style

1. [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)
2. Try to use the new version of ES features for the source code.

## Directory tree

```shell
auto-task # Root directory
├── auto-task-helper.user.js # Auxiliary script to obtain Discord auth
├── auto-task-test.user.js # auto-task script pre version
├── auto-task.user.js # auto-task script official version
├── build.dev.js # Used to process pre version js files
├── build.js # Used to process official version js files
├── package.json
├── gulpfile.js # Used to build scripts and websites
├── docs # Pre-version setting page website directory (automatically generated)
|  └── ...
├── public # Official version setting page website directory (automatically generated)
|  └── ...
├── lib # gulp plugin directory
|  ├── doSomething.js # Process js files
|  ├── log.js # Pre-defined console log style
|  └── minCss.js # Process and compress css files
├── require # The static file directory the script depends on
|  ├── require.min.js # The dependent js files are packaged from the files in the /src/requirejs folder
|  ├── fuck-task.min.css # The dependent css files are packaged from the files in the /src/style folder
|  ├── fuck.cur
|  ├── iconfont.eot
|  ├── iconfont.svg
|  ├── iconfont.ttf
|  ├── iconfont.woff
|  └── iconfont.woff2
└── src # Source directory
   ├── helper # Auxiliary script source directory
   |  └── auto-task-helper.user.js # Helper script
   ├── page # Settings website source directory
   |  ├── img # Image directory
   |  |  └── ...
   |  ├── index.html
   |  ├── js
   |  |  ├── lang # Setting page i18n language directory
   |  |  |  ├── zh-CN.json # Chinese
   |  |  |  └── en-US.json # English
   |  |  ├── i18n.js
   |  |  └── main.js
   |  ├── setting.html # Settings page
   |  ├── time.html # Countdown page (Chinese)
   |  └── time_en.html # Countdown page (English)
   ├── requirejs # Dependent js folder
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
   ├── scripts # Script source directory
   |  ├── config.js # Configuration item handling
   |  ├── defaultConf.js # Default configuration
   |  ├── header.js # UserScript header information
   |  ├── i18n.js # i18n related
   |  ├── main.js # Function integration
   |  ├── lang # Script i18n language directory
   |  |  ├── zh-CN.json # Chinese
   |  |  ├── en-US.json # English
   |  ├── function # Function directory
   |  |  ├── getAuth.js # Obtain Discord auth
   |  |  ├── httpRequest.js # http request
   |  |  ├── log.js # Used to output task log
   |  |  ├── main.js # Load ui and functions
   |  |  ├── tool.js # Tool Library
   |  |  └── social # Social-related tasks
   |  |     ├── discord.js # Discord related tasks
   |  |     ├── instagram.js # Instagram related tasks
   |  |     ├── reddit.js # Reddit related tasks
   |  |     ├── steam.js # Steam related tasks
   |  |     ├── toggleActions.js # Social task integration distribution
   |  |     ├── twitch.js # Twitch related tasks
   |  |     ├── twitter.js # Twitter related tasks
   |  |     ├── vk.js # Vk related tasks
   |  |     └── youtube.js # Youtube related tasks
   |  └── website # List of functions related to each website
   |     ├── main.js # Automatically generated, please do not modify!
   |     ├── main.template # Template of main.js file, used to generate main.js
   |     └── [website].js # Functions related to each website
   └── style # Style sheet directory
      ├── bootstrap.min.css
      ├── iconfont.min.css
      ├── other.css # Please add new styles to this file, do not modify other files
      └── overhang.min.css
```
