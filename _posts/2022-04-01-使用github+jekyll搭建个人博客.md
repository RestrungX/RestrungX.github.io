---
layout: post
toc: true
title: "使用github+jekyll搭建个人博客"
categories: junk
tags: [markdown, css, html]
author:
  - Xiao LijiA
  
---

github的优势
1、GitHub作为托管平台只支持git版本库托管而不像其他开源项目托管平台还对CVS、SVN、Hg 等格式的版本库进行托管。GitHub 的哲学很简单，既然 Git 是最好的版本控制系统之一（对于很多喜欢 Git 和 GitHub 的人没有之一），没有必要为兼顾其他版本控制系统而牺牲 Git 某些独有特性。因此没有支持其他版本控制系统的历史负担，是 GitHub 成功的要素之一。
2、GitHub 对 Git 版本库提供了完整的协议支持，支持 HTTP 智能协议、Git-daemon、SSH 协议。
3、GitHub 提供在线编辑文件的功能，不熟悉 Git 的用户也可以直接通过浏览器修改版本库里的文件。
4、将社交网络引入项目托管平台是 GitHub 的创举。用户可以关注项目、关注其他用户进而了解项目和开发者动态。
5、项目的 Fork 和 Pull Request 构成 GitHub 最独具一格的工作模式。对提交代码的逐行评注及 Pull Request 构成 GitHub 特色的代码审核。
6、GitHub 通过私有版本库托管、面向企业的版本库托管和项目管理平台、人员招聘等付费服务获得了商业上的成功，这种成功使得 GitHub 不必以页面中嵌入广告的方式维持运营，最大的受益者还是用户。
7、GitHub 网站采用 Ruby on Rails 架构，在 Web 设计中运用了大量的 JavaScript、AJAX、HTML5 等技术，支持对使用 Markdown 等标记语言的内容进行渲染和显示等。关注细节使得 GitHub 成为了项目托管领域的后起之秀。

说这么多，我们回到主题。我突然想建立一个属于自己的个人博客，通过搜索了很多资料，发现一个免费而又简单的搭建博客的方法。就是利用github下面的github pages+jekyll一个简单的免费的Blog生成工具。

*github pages 主页 [https://pages.github.com/][git-hub]

jekyll中文网站 主页 [https://www.jekyll.com.cn/][jek-yll]

我的博客主页 [https://restrungx.github.io/][my-bl]

[git-hub]: https://pages.github.com/
[jek-yll]: https://www.jekyll.com.cn/
[my-bl]: https://restrungx.github.io/
## 步骤一,创建GitHub博客
  注册一个github自行打开GitHub官网输入昵称邮箱密码注册

<img src="C:\Users\25301\Desktop\RestrungX.github.io\RestrungX.github.io\_posts\2022-04-01-使用github+jekyll搭建个人博客\image-20220401222441721.png" alt="image-20220401222441721" style="zoom:25%;" />


## 步骤二,前往jekyll的主题商店挑选主题

主题商店：[http://jekyllthemes.org/][sd],挑一个你喜欢的点击
[sd]:http://jekyllthemes.org/
### Some great subheading (h3)

Proin convallis mi ac felis pharetra aliquam. Curabitur dignissim accumsan rutrum. In arcu magna, aliquet vel pretium et, molestie et arcu. Mauris lobortis nulla et felis ullamcorper bibendum.

Phasellus et hendrerit mauris. Proin eget nibh a massa vestibulum pretium. Suspendisse eu nisl a ante aliquet bibendum quis a nunc.

### Some great subheading (h3)

Praesent varius interdum vehicula. Aenean risus libero, placerat at vestibulum eget, ultricies eu enim. Praesent nulla tortor, malesuada adipiscing adipiscing sollicitudin, adipiscing eget est.

> This quote will *change* your life. It will reveal the <i>secrets</i> of the universe, and all the wonders of humanity. Don't <em>misuse</em> it.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce bibendum neque eget nunc mattis eu sollicitudin enim tincidunt.

### Some great subheading (h3)

Vestibulum lacus tortor, ultricies id dignissim ac, bibendum in velit. Proin convallis mi ac felis pharetra aliquam. Curabitur dignissim accumsan rutrum.

```html
<html>
  <head>
  </head>
  <body>
    <p>Hello, World!</p>
  </body>
</html>
```


In arcu magna, aliquet vel pretium et, molestie et arcu. Mauris lobortis nulla et felis ullamcorper bibendum. Phasellus et hendrerit mauris.

#### You might want a sub-subheading (h4)

In arcu magna, aliquet vel pretium et, molestie et arcu. Mauris lobortis nulla et felis ullamcorper bibendum. Phasellus et hendrerit mauris.

In arcu magna, aliquet vel pretium et, molestie et arcu. Mauris lobortis nulla et felis ullamcorper bibendum. Phasellus et hendrerit mauris.

#### But it's probably overkill (h4)

In arcu magna, aliquet vel pretium et, molestie et arcu. Mauris lobortis nulla et felis ullamcorper bibendum. Phasellus et hendrerit mauris.

##### Could be a smaller sub-heading, `pacman` (h5)

In arcu magna, aliquet vel pretium et, molestie et arcu. Mauris lobortis nulla et felis ullamcorper bibendum. Phasellus et hendrerit mauris.

###### Small yet significant sub-heading  (h6)

In arcu magna, aliquet vel pretium et, molestie et arcu. Mauris lobortis nulla et felis ullamcorper bibendum. Phasellus et hendrerit mauris.

### Oh hai, an unordered list!!

In arcu magna, aliquet vel pretium et, molestie et arcu. Mauris lobortis nulla et felis ullamcorper bibendum. Phasellus et hendrerit mauris.

- First item, yo
- Second item, dawg
- Third item, what what?!
- Fourth item, fo sheezy my neezy

### Oh hai, an ordered list!!

In arcu magna, aliquet vel pretium et, molestie et arcu. Mauris lobortis nulla et felis ullamcorper bibendum. Phasellus et hendrerit mauris.

1. First item, yo
2. Second item, dawg
3. Third item, what what?!
4. Fourth item, fo sheezy my neezy



## Headings are cool! (h2)

Proin eget nibh a massa vestibulum pretium. Suspendisse eu nisl a ante aliquet bibendum quis a nunc. Praesent varius interdum vehicula. Aenean risus libero, placerat at vestibulum eget, ultricies eu enim. Praesent nulla tortor, malesuada adipiscing adipiscing sollicitudin, adipiscing eget est.

Praesent nulla tortor, malesuada adipiscing adipiscing sollicitudin, adipiscing eget est.

Proin eget nibh a massa vestibulum pretium. Suspendisse eu nisl a ante aliquet bibendum quis a nunc.

### Tables

Title 1               | Title 2               | Title 3               | Title 4
--------------------- | --------------------- | --------------------- | ---------------------
lorem                 | lorem ipsum           | lorem ipsum dolor     | lorem ipsum dolor sit
lorem ipsum dolor sit | lorem ipsum dolor sit | lorem ipsum dolor sit | lorem ipsum dolor sit
lorem ipsum dolor sit | lorem ipsum dolor sit | lorem ipsum dolor sit | lorem ipsum dolor sit
lorem ipsum dolor sit | lorem ipsum dolor sit | lorem ipsum dolor sit | lorem ipsum dolor sit


Title 1 | Title 2 | Title 3 | Title 4
--- | --- | --- | ---
lorem | lorem ipsum | lorem ipsum dolor | lorem ipsum dolor sit
lorem ipsum dolor sit amet | lorem ipsum dolor sit amet consectetur | lorem ipsum dolor sit amet | lorem ipsum dolor sit
lorem ipsum dolor | lorem ipsum | lorem | lorem ipsum
lorem ipsum dolor | lorem ipsum dolor sit | lorem ipsum dolor sit amet | lorem ipsum dolor sit amet consectetur
