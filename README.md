介绍
============

**AIFish Design** -- 是我们基于 AdminLTE（Bootstrap） 引入了企业级产品的设计体系，形成了一套完整的设计语言，并且重新给这套UI库取了一个新名称叫 AIFish Design。

**预览地址 [aifish.github.io](https://aifish.github.io)**

### 如何使用？
	1. 下载项目到本地
	2. 安装node及npm，版本v8.12.0
	3. 安装grunt `npm install -g grunt-cli`
	4. 命令行的当前目录转到项目的根目录下
	5. 安装Grunt最新版本到项目目录中 `npm install grunt --save-dev`
	6. 执行`grunt`命令


### LESS文件更新日志

#### Bootstrap variables文件（build/bootstrap-less/variables.less)
 * L360 `@navbar-height:50px;` 修改为 `@navbar-height:64px;`,设置顶部导航栏的高度，将高度调整为64px；


#### AdminLTE core.less 文件（build/less/core.less)
 * L14 `font-family: 'Source Sans Pro', 'Helvetica Neue', Helvetica, Arial, sans-serif;` 修改为 `font-family: @font-family-base;`  将字体设置统一用变量设置.
 * L148 `font-family: 'Source Sans Pro', sans-serif;', 'Helvetica Neue', Helvetica, Arial, sans-serif;` 修改为 `font-family: @font-family-base;`  将字体设置统一用变量设置.


#### AdminLTE variables.less 文件（build/less/variables.less)
 * L7 `@light-blue:#3c8dbc`  修改为  `@light-blue:#1890ff` ，此变量为主色调背景，运用于按钮颜色！
 * L9 `@red: #dd4b39;` 修改为 `@red: #F5222D;`  ，此变量危险色背景，运用于错误，失败，气泡背景！
 * L11 `@green: #00a65a;` 修改为 `@green: #52c41a;`，此变量成功色背景，运用于提交成功！
 * L32 `@sidebar-width: 230px;` 修改为 `@sidebar-width: 256px;`， 此变量是侧边栏宽度，宽度从230调整至256，更适合大屏幕比例显示。
 * L44 `@content-bg: #ecf0f5; ` 修改为 `@content-bg: #f0f2f5;`，设置主要背景色，（主内容区的背景色），将颜色调的更浅一些，更舒适。
 * L50 `@sidebar-dark-bg: #222d32;` 修改为 `@sidebar-dark-bg: #001529;` 设置深色侧边栏背景色，颜色调的更深一些。
 * L59 `@sidebar-light-bg: #f9fafc;` 修改为 `@sidebar-light-bg: #fff;` 设置亮色侧边栏背景色，颜色调整为白色。


#### AdminLTE header.less 文件（build/less/header.less)
 * L115 `line-height: 50px;` 修改为 `line-height: @navbar-height;` ，将行高值修改为变量，用于灵活设置进行垂直居中对齐。

#### AdminLTE sidebar.less 文件（build/less/sidebar.less)
 * L0 `padding-top: 50px;` 修改为 `padding-top: @navbar-height;` ，将行高值修改为变量，用于灵活设置侧边栏的上边距。


#### AdminLTE Skin文件（build/less/skin/skin-blue.less)
 * L39 `.logo-variant(darken(@light-blue, 5%));` 修改为 `.logo-variant(lighten(@sidebar-dark-bg, 4.5%));` ,设置logo处的背景色，是根据侧边栏的背景色高亮4.5%
