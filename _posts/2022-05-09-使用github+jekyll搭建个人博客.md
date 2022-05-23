---
layout: post

title: "使用github+jekyll搭建个人博客"




---

*github pages 主页 [https://pages.github.com/][git-hub]

jekyll中文网站 主页 [https://www.jekyll.com.cn/][jek-yll]

我的博客主页 [https://restrungx.github.io/][my-bl]

[git-hub]: https://pages.github.com/
[jek-yll]: https://www.jekyll.com.cn/
[my-bl]: https://restrungx.github.io/

## 步骤一,创建GitHub博客

  注册一个github自行打开GitHub官网输入昵称邮箱密码注册




## 步骤二,前往jekyll的主题商店挑选主题

主题商店：[http://jekyllthemes.org/][sd],挑一个你喜欢的点击

[sd]:http://jekyllthemes.org/

## 步骤三，fork别人的github项目

fork到自己的项目之后，打开设置把项目名称改成*`GitHub用户名＋gitiub.io*`,比如我的 RestrungX.github.io

**如果没有意外，这个时候你就可以打开你的个人博客了，地址是： 你的github名字.github.io，如我的github名字是Hectoor，则我的个人博客是https://restrungx.github.io/，但是里面的信息还是别人的**

## **步骤四:在电脑上修改文件配置**

修改完之后，转到Code，此时需要借助一个软件，github 的桌面软件，方便你更好的上传代码。

*github for windows https://desktop.github.com/*

下载完成后打开你刚刚fork的项目，点击右上角的clone or download里面的Open in Desktop**系统会自动打开这个软件** 

小提示：`在GitHub desktop软件弹开时，下面的Local path地址就是你下载下来的本地的远程仓库地址`

打开路径，里面有一个_config.yml文件，打开，里面是一些基本配置，你的文章都在_posts里面编写，重要的一点是，md文件的命名必须都要严格按照格式来写，`xxxx-xx-xx-标题.md`