# 安装开发环境

首先你得安装Node.js，安装Node.js时会默认安装NPM

Git可以去官网下载安装包安装

拥有了NPM后，使用NPM安装Yo

```sh
npm install -g yo
```

安装项目脚手架 generator-tmfde

```sh
npm install -g generator-tmfde
```

进入你想创建项目的文件夹，使用以下命令创建项目

```sh
yo tmfde
```

按照提示输入项目名，项目描述， PHP项目branch分支路径地址
```sh
D:\tuniu\demo> yo tmfde

     _-----_
    |       |    .--------------------------.
    |--(o)--|    |  Welcome to tuniu mobile |
   `---------´   |     frontend develop     |
    ( _´U`_ )    |  environment generator!  |
    /___A___\    '--------------------------'
     |  ~  |
   __'.___.'__
 ´   `  |° ´ Y `

? 请输入你的英文项目名称,后续会创建以此命名的文件夹 drive
? 请输入项目描述 drive
? 请输入本地MTUNIU项目branch分支路径 (D://Source/Tuniu/MTUNIU/branch/)
```
> 注意项目名是否已存在，如已存在，请勿创建同名文件已免覆盖

yo会自动执行`npm install`安装项目的依赖，安装过程中请等待

安装完成后，执行`git init`，初始化git。如果不使用git，也可以跳过此步

进入项目会看到以下目录结构

```
project
  |- .git/
  |- dist/
  |- node_modules/
  |- src/
  |- package.json
  |- gulpfile.js
  |- README.md
  |- .gitignore
```

执行`gulp`命令，在浏览器中输入：http://localhost:8000/prototypes/[项目名]/html/index.html

看到Hello World即Ok





