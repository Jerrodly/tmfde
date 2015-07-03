# 日常开发

## gulp

**命令：**

```sh
gulp
```

**功能：**

启动本地server，并监听文件变化

当html，css，scss，tpl，jsx文件发生变化时，会执行编译task，并刷新浏览器


## gulp stable

**命令：**

```sh
gulp stable
```

**功能：**

- 编译scss样式文件
- 为编译好的css文件增加prefixer css3前缀
- tpl，jsx文件编译为js文件
- js文件进行jshint错误扫描
- 压缩js文件并添加.min.js
- 拷贝src下面的文件到dist目录


## gulp pullOrigin

**命令：**

```sh
gulp pullOrigin
```

**功能：**

切换到master分支，拷贝PHP项目中的文件到src中。执行前最好在PHP项目中SVN update一下


## gulp push

**命令：**

```sh
gulp push
```

**功能：**

把开发好的静态文件拷贝到PHP项目中，范围限定在项目内。不会将公用文件拷贝覆盖



