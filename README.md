
<h1 align="center">AdminLTE Theme for Ant Design</h1>

<div align="center">

基于Ant Design设计语言的 AdminLTE 主题样式

![](https://user-images.githubusercontent.com/8186664/44953195-581e3d80-aec4-11e8-8dcb-54b9db38ec11.png)

</div>

- 预览：http://preview.pro.ant.design
- 首页：http://pro.ant.design/index-cn
- 使用文档：http://pro.ant.design/docs/getting-started-cn
- 更新日志: http://pro.ant.design/docs/changelog-cn
- 常见问题：http://pro.ant.design/docs/faq-cn
- 国内镜像：http://ant-design-pro.gitee.io


## 特性

- 基于Ant Design，同一种设计价值观
- 保留了AdminLTE所有的特性和功能
- 提供LESS源文件，可进行二次开发
- 提供六种主题配色，拂晓蓝（默认）、极客蓝、酱紫、极光绿、火山、日暮
- 只修改框架样式，结构不受影响，可平滑升级使用


## 使用

### 1、框架源码
下载框架源码，修改LESS样式文件，启动Grunt脚手架编译，适用于LESS源代码的二次开发。

```bash
$ git clone https://github.com/ant-design/ant-design-pro.git --depth=1
$ cd ant-design-pro
$ npm install grunt --save-dev
```

### 2、样式文件
如果你的项目是基于AdminLTE的，若想直接使用这套主题样式，可以下载样式文件直接在你的项目中替换对样式文件即可。
使用这种方法的前提，需要AdminLTE的版本保持一致，并且项目中的AdminLTE样式文件没有做修改，以防样式文件丢失。

- 样式文件下载：http://preview.pro.ant.design

#### 样式替换目录

```
- dist
  - css
    - skins // 主题文件夹全部替换
    - AdminLTE.css // 框架样式文件替换 
    - AdminLTE.min.css	// 框架样式压缩文件替换
```

## 问题反馈

首先非常感谢Ant Design及AdminLTE(Bootstrap)这么优秀开源框架，可以提供我们学习及使用。
当然我也会力所能及的将优秀的代码及产品分享给大家，但是考虑到个人能力和精力有限，所以当你们在使用的过程中遇到问题：

	- 通过 [Issue](http://github.com/ant-design/ant-design-pro/issues) 报告 bug 或进行咨询。
	- 或者直接联系我的个人邮箱 [chyi722@163.com](mailto:chyi722@163.com)




## 更新日志

### 1.0.0





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



#### 系统布局及样式切换说明
1. 提供固定Header及侧边栏的开关
2. 提供主内容区域的固定模式的开关
3. 提供开启收缩侧边栏的开关
4. 提供6种主色调及深浅各两种风格主题的切换
5. 主色调：拂晓蓝（默认）、极客蓝、酱紫、极光绿、火山、日暮

#### 主题切换说明
系统主题的切换主要表现在以下几个方面：
1. 全局：a超链接的颜色会根据主题色进行变化
2. 侧边栏：分为亮色和暗色的风格，一套主题分别提供两套风格选择
3. 侧边栏：侧边栏的菜单选中背景会根据主题色变化
4. 侧边栏：当选择亮色系时，侧边栏LOGO的字体也根据主题色变化
5. 按钮： 主要按钮和默认按钮的颜色会根据主题色发生变化
6. 标签页： 标签页的边框和字体颜色会根据主题色发生变化
7. 表单：表单元素的focus边框颜色会根据主题色发生变化



