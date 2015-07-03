# 命令介绍

最方便的了解方式是看`gulpfile.js`里面的代码和注释

### gulp clean

清理dist目录

### gulp prefixer

使用`gulp-autoprefixer`插件来添加css3前缀

### gulp hint

使用`gulp-jshint`插件来检查js代码

### gulp template

把js/[项目名]/tpl/目录下.tpl后缀文件（内容是html代码片段）编译为seajs模块封装的js文件

### gulp jsx

把js/[项目名]/jsx/目录下.jsx后缀文件（reactjs文件）编译为js文件

### gulp connect

启动Node.js本地server，默认端口8000，livereload为true（自动刷新）

### gulp styles

使用`gulp-sass`插件编译scss文件为css文件

### gulp stableStyles

使用`gulp-sass`插件编译scss文件为css文件，后再使用`gulp-autoprefixer`插件来添加css3前缀

### gulp watch

监听文件变化.当html，css，scss，tpl，jsx文件发生变化时，会执行各自的编译task。当html和css变化时会通知浏览器自动刷新

### gulp compress

- 先执行`gulp template`和`gulp jsx`任
- 之后使用`gulp-uglify`压缩js（require作为关键字保留），js中使用seajs引入其他js的地址会被替换为.min.js





