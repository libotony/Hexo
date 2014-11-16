title: 使用Hexo在github搭建博客  
date: 2014-11-16 20:19:44  
categories: Hexo  
tags: [HEXO,github,blog,博客] 
toc: true 
---
&#160; &#160; &#160; &#160;作为程序员，总有写写博客的想法，总是想找个方便快捷的方式写写博客，偶然一个机会，发现了一个逼格极高而且非常适合程序猿的写博客的工具[Hexo](http://hexo.io/)，看了一眼就喜欢上了。本文就是介绍如何用Hexo简便快捷的创建属于自己的blog。  
<!--more--> 
&#160; &#160; &#160; &#160;在Hexo的官网你可以看到它的介绍:`Hexo —— 简单、快速、强大的Node.js静态博客框架`,它是一个基于Nodejs的静态博客程序，编译速度非常快，编译出来的静态网页可以直接放到GitHub Pages,这也是我选择他的原因之一，方便省事，不用费心去买空间。GitHub Pages有300MB的空间，对于一般的博主是够用了，后期也可以搬到自己的VPS上，绝对无痛。 
## 环境准备
1. 由于Hexo基于Nodejs，所以你需要先安装Nodejs，参考[Node官网](http://nodejs.org/)即可。
2. 博客要部署到GitHub，所以我们也需要Git客户端。
3. Markdown编辑器：Submlie Text（Win、Mac）、Mou（Mac）。
4. 操作系统不同，上述工具略有不同，各位根据实际情况自己安装。  

##GitHub  
&#160; &#160; &#160; &#160;作为码农，这都是最基本的哈，配置好即可，要使用GitHub Pages&#160; &#160; &#160; &#160;只需要在GitHub新建一个仓库，仓库的名字必须为[your_user_name.github.io]，添加你的SSH公钥到[Account settings -> SSH Keys -> Add SSH Key]。  
![github repo](http://libotony.qiniudn.com/QQ20141116-1.png)  
***  
好啦到这里，准备工作就完成了，接下来就要开工啦！  
##HEXO
###安装
``` bash
$ npm install -g hexo
```
###初始化工作空间
然后，执行初始化命令  
``` bash
$ hexo init <target folder>
```  
**也可以cd进目录直接 hexo init**  
###生成静态页面  
进入刚刚初始化的文件夹，执行如下命令，你可以直接执行生成命令。当出现错误时，清除一下再生成。  
``` bash
$ hexo clean  ##清除
$ hexo g      ##生成
```  
生成命令执行后，生成的静态页面文件会出现在public目录中，这就是你要上传到GitHub的文件。
###本地服务
你在写文章、配置hexo、修改主题等操作时，你可以在本地预览调试，只需要启动本地服务即可。执行一下命令启动本地服务。  
``` bash
$ hexo s  ##启动本地服务
```
根据提示，在浏览器输入[http://localhost:4000](http://localhost:4000),就可以看到效果啦。  
`未完待续`




