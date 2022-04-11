---
layout: post
---
随便玩玩，记录点好的东西。

一些简单的且使用的小技能

## Vue项目配置同一局域网可使用IP访问的操作

config文件中找到 index.js 文件的host改成 “本机网络ip地址”

**查看ip地址的方法**

 通过命令行

1、win + R 打开[cmd](https://so.csdn.net/so/search?q=cmd&spm=1001.2101.3001.7020)

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

