#mupdf使用
@(菜鸟教程笔记本)[Android|mupdf|pdf]

**mupdf**是PFD阅读器开源库，本文使用1.14.0-relase版本进行下载编译。


-------------------

##源码下载

>git下载源码 —— [官网地址](https://mupdf.com)

在主分支master上，拉去tag-1.14.0版本。

```shell
    git clone git://git.ghostscript.com/mupdf.git
    git checkout master
    git checkout -b 1.14.0-relase 1.14.0
    git branch
    git pull --rebase
```

##编译

首先介绍编译Android的so文件。

###主目录编译
终端在下载的mupdf根目录，使用make命令来编译下这些c代码，此时在MacOS环境下使用make generate命令。

```shell
    make generate
```
###更新thirdparty
编译so前，需要更新第三方依赖的文件源码。切换mupdf/thirdparty/文件下查看README文件。需要执行命令如下

```shell
    git submodule init
    git submodule update
```

###so文件编译
更新完thirdparty后，切换到/mupdf/platform/java文件夹下执行ndk编译。前提需要配置Android-ndk环境（自行百度）。
因为文件夹下文件结构不通，不能直接使用ndk-build。

```shell
    ndk-build NDK_PROJECT_PATH=. APP_BUILD_SCRIPT=./Android.mk
```









