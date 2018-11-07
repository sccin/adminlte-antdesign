
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
$ git clone https://github.com/Alsiso/adminlte-antdesign.git --depth=1
$ cd adminlte-antdesign
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

首先非常感谢Ant Design及AdminLTE(Bootstrap)这么优秀开源框架，可以供我们学习及使用。<br/>
我也会力所能及的将优秀的代码及产品分享给大家，但是考虑到个人能力和精力有限，所以当你们在使用的过程中遇到问题：

- 通过 [Issue](http://github.com/ant-design/ant-design-pro/issues) 报告 bug 或进行咨询。
- 或者直接联系我的个人邮箱 [chyi722@163.com](mailto:chyi722@163.com)



## 更新日志

### 1.0.0

#### 全局
- 修改基础的字体家族
- 修改字体默认、链接样式
- 修改字体的粗细为400
- 增加MacOS下字体抗锯齿渲染

#### 侧边导航
- 修改侧边栏的宽度，包括mini时的宽度
- 修改侧边栏的背景色，包括深色及浅色
- 增加侧边栏的投影效果
- 修改字体默认、滑动，选中的样式
- 修改菜单子项的间距及边距
- 修改文字与图标的间距
- 支持主题切换时的样式切换

#### 顶部导航
- 调整顶部导航的高度
- 增加顶部导航的投影效果
- 调整收缩图标的大小
- 修改了气泡的样式，包括间距及字体大小
- 调整了导航栏子项的滑动效果
- 增加了导航栏中下拉菜单的投影效果

#### 组件

- 按钮 buttons
  - 修改默认按钮的样式
  - 修改主要按钮的样式
  - 修改禁用按钮的样式
  - 修改危险按钮的样式
  - 修改组合按钮的样式
  - 修改不同颜色按钮的色值
- boxes 盒子
  - 修改了边框颜色
  - 修改了盒子投影值
  - 修改了盒子内部的间距
  - 修改了盒子header的字体大小及颜色
  - 修改了不同颜色盒子的显示效果
- alert 警告
  - 修改了主体的圆角值
  - 修改了多种警告的背景颜色，边框颜色，文字颜色，图标间距
- callout 标注
  - 修改了主体的圆角值
  - 修改了多种标注的背景颜色，边框颜色，文字颜色，图标间距
- dropmenu 下拉菜单
  - 修改footer的字体大小
  - 增加一种常用的圆角背景图标
- form 表单
  - 增加表单元素的阴影效果
  - 增加表单元素的focus样式
- progress-bars 进度条
  - 修改横向进度条的高度
  - 修改纵向进度条的宽度
  - 修改进度的背景颜色
  - 修改进度条文字的粗细
- navs 导航
  - 修改导航页签的整体样式

#### 主题
系统主题的切换主要表现在以下几个方面：

1. 全局：a超链接的颜色会根据主题色进行变化
2. 侧边栏：分为亮色和暗色的风格，一套主题分别提供两套风格选择
3. 侧边栏：侧边栏的菜单选中背景会根据主题色变化
4. 侧边栏：当选择亮色系时，侧边栏LOGO的字体也根据主题色变化
5. 按钮： 主要按钮和默认按钮的颜色会根据主题色发生变化
6. 标签页： 标签页的边框和字体颜色会根据主题色发生变化
7. 表单：表单元素的focus边框颜色会根据主题色发生变化



