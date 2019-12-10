#GitBook文档
##1. 什么是GitBook
```
gitbook 是一款文档编辑工作，它可以用来写文档、建表格、插图片、生成pdf。
它可以用文档建立一个网站，支持Git,也就意味着，它是一个分布式的文档编辑工具。
在GitBook中，你可以使用markdown语法或者AsciiDoc语法。
```
##2. 安装和使用GitBook
###2.1 本地通过NPM安装GitBook命令行工具
运行下面的命令进行安装
```
$ npm install gitbook-cli -g
```
其中gitbook-cli是gitbook的一个命令行工机具，通过它可以在电脑上安装和管理gitbook的多个版本
###2.2 GitBook创建以及预览
####2.2.1 初始化
1.打开一个文件夹Mygitbook,使用gitbook init 初始化文件夹，会自动生成两个必要的文件README.md和SUMMARY.md。
```
gitbook init
```
* README.md：书的介绍文字，如前言、简介，在章节中也可作为章节的简介。
* SUMMARY.md：定制书籍的章节结构和顺序,SUMMARY.md中[]内的内容是标题，()内是文档的路径。

README.md和SUMMARY.md是GitBook制作电子书的必要文件，可用gitbook init命令自动生成。

2.在Mygitbook文件夹下面增加其他章节下的文件，文件目录如下：
![文件目录](https://upload-images.jianshu.io/upload_images/2423912-b5d71c6b3f56a937.png)
#GitBook文档
##1. 什么是GitBook
```
gitbook 是一款文档编辑工作，它可以用来写文档、建表格、插图片、生成pdf。
它可以用文档建立一个网站，支持Git,也就意味着，它是一个分布式的文档编辑工具。
在GitBook中，你可以使用markdown语法或者AsciiDoc语法。
```
##2. 安装和使用GitBook
###2.1 本地通过NPM安装GitBook命令行工具
运行下面的命令进行安装
```
$ npm install gitbook-cli -g
```
其中gitbook-cli是gitbook的一个命令行工机具，通过它可以在电脑上安装和管理gitbook的多个版本
###2.2 GitBook创建以及预览
####2.2.1 初始化
1.打开一个文件夹Mygitbook,使用gitbook init 初始化文件夹，会自动生成两个必要的文件README.md和SUMMARY.md。
```
gitbook init
```
* README.md：书的介绍文字，如前言、简介，在章节中也可作为章节的简介。
* SUMMARY.md：定制书籍的章节结构和顺序,SUMMARY.md中[]内的内容是标题，()内是文档的路径。

README.md和SUMMARY.md是GitBook制作电子书的必要文件，可用gitbook init命令自动生成。

2.在Mygitbook文件夹下面增加其他章节下的文件，文件目录如下：
![文件目录](https://upload-images.jianshu.io/upload_images/2423912-b5d71c6b3f56a937.png)

3.Gitbook使用SUMMARY.md文件作为书籍的目录结构，可以用来制作书籍目录。
```
// SUMMARY.md

# Summary
* [Introduction](README.md)
* Gitbook
    * [gitbook 介绍以及安装](Chapter1/1.md)
    * [Markdown语法](Chapter1/2.md)
```
####2.2.2 预览
1.执行命令gitbook serve , gitbook 会启动一个4000端口用于预览。
```
gitbook serve
```
你可以你的浏览器中打开这个网址： http://localhost:4000 预览电子书效果。

