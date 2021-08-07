# demo

> An electron-vue project

#### Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:9080
npm run dev

# build electron application for production
npm run build

# run unit & end-to-end tests
npm test


# lint all JS/Vue component files in `src/`
npm run lint

```
### 项目结构
```
demo（项目名称）
├─ .electron-vue（webpack配置文件）
│  └─ build.js（生产环境构建代码） 
|  └─ dev-client.js（热加载相关）
│  └─ dev-runner.js（开发环境启动入口）
│  └─ webpack.main.config.js（主进程配置文件）
│  └─ webpack.renderer.config.js（渲染进程配置文件）
│  └─ webpack.web.config.js
├─ build（是文件打包使用的）
│  └─ win-unpacked/
│  │  ├─ locales（地区语言资源包）
│  │  ├─ resources（地区语言资源包）
│  │  ├─ *.dll（动态链接库）
├─ dist(打包后的文件资源)
│  ├─ electron
|  ├─ web
├─ node_modules/（依赖目录）
├─ src（源码）
│  ├─ main(主进程)
│  │  └─ index.dev.js（捆绑index.js）
│  │  └─ index.js(主进程的进程JS)
│  ├─ renderer（渲染进程）
│  │  ├─ assets/（放置静态资源，如图片，视频，静态配置）
│  │  ├─ components/（放置vue页面）
│  │  ├─ router/（放置页面路由）
│  │  ├─ store/（放置公共模块，如vuex）
│  │  ├─ App.vue
│  │  └─ main.js
│  └─ index.ejs
├─ static/（静态文件）
├─ test
│  ├─ e2e
│  │  ├─ specs/
│  │  ├─ index.js
│  │  └─ utils.js
│  ├─ unit
│  │  ├─ specs/
│  │  ├─ index.js
│  │  └─ karma.config.js
│  └─ .eslintrc#全局配置文件
├─ .babelrc
├─ .eslintignore
├─ .eslintrc.js
├─ .gitignore
├─ package.json
└─ README.md

---

This project was generated with [electron-vue](https://github.com/SimulatedGREG/electron-vue)@[8d4ed60](https://github.com/SimulatedGREG/electron-vue/tree/8d4ed607d65300381a8f47d97923eb07832b1a9a) using [vue-cli](https://github.com/vuejs/vue-cli). Documentation about the original structure can be found [here](https://simulatedgreg.gitbooks.io/electron-vue/content/index.html).
