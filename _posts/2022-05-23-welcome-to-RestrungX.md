---
layout: post
---
随便玩玩，记录点好的东西。

一些简单的且使用的小技能

## Vue项目配置同一局域网可使用IP访问的操作

config文件中找到 index.js 文件的host改成 “本机网络ip地址”

**查看ip地址的方法**

 通过命令行

1、win + R 输入cmd 打开cmd命令框

2、输入ipconfig   得到 IPv4 地址 .....

# vue中(动画)第三方插件库的使用

首先安装模块
**npm install animate.css 命令**

考虑到我们会在多个路组件中使用 我这里直接引入到main.js 里面,输入以下

```html
import animated from 'animate.css' ;
Vue.use(animated);
```

# 通过对滚动条的监听实现animate的应用

```vue
  mounted() {
        // 监听滚动事件，用handleScroll这个方法进行相应的处理
        window.addEventListener("scroll", this.handleScroll);
    },
     beforeDestroy() {
    // 在组件生命周期结束的时候要销毁监听事件，否则其他页面也会使用这个监听事件
    window.removeEventListener("scroll", this.handleScroll);
  },
    methods:{
        handleScroll() {
  		// 监听到页面滚动后的处理事件
    	 var scrollTop = window.pageYOffset || document.documentElement.scrollTop || document.body.scrollTop;
      // console.log(scrollTop,offsetTop)
      //判断滚动距离，做相应的类名添加
        scrollTop >200 ? this.$refs.tabbarBox.classList.value= " textBox animate__animated animate__rubberBand":this.$refs.tabbarBox.classList.value=" textBox"
       
       },
```

# vue使用静态图片当作盒子背景

```vue-js
//在data里声明一个对象bg用来存储背景图片（当然对象bg里面可以设置其他的background属性，我这里只运用了img）
bg: {
                backgroundImage: "url(" + require("../assets/联系我们bg.jpg") + ")",
               },
               
//require是node语法
```

```
//在需要添加背景图片的盒子里使用
	:style="bg"（vue数据绑定）
```

<meta data-vue-meta-info="true" name="keywords" content="关键字">
<meta data-vue-meta-info="true" name="description" content="内容">
<title>标题</title>

