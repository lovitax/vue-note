# Vue 小黄鸭学习法

```
总需要个开始
这句话其实是说学习的开始，也是这个文章的开始
我终于也是实现了用前端开发工具和环境进行
但是呢觉得Gitbook有点局限性，样式比较少，但是markdown支持的样式就是这些么。这个点可以想一想能不能扩展下
谈到扩展就涉及到改写Gitbook的源码了，或者重写算了
哦哦，刚才保存的时候刷新了一下页面会先白再变黄（因为我现在是晚上23：56所以页面设置成了Sepia）。解决这个问题的方式我首先想到的是热重载。
重写Gitbook或者就干脆自己做一个脚手架，首先需要有个markdown翻译成HTML的过程。抽象语法树么，AST。然后还想可以扩展，这个终极目标就是实现可以用html+css排版了。
或者这样，可以自己设计配色和各种元素样式，但是写markdown的时候一定还要简单。要不干脆写html算了。。。

啊啊啊，这个区域里面是pre/code 所以没有自动换行，感觉又想改它了
```

其实是想写Vue的，怎么说了那么多乱七八糟有的没的
啊，困了呢

<a href="#">写个标签会显示么</a>
开始了啊

## Vue组件生命周期
```
new Vue()  
        beforeCreated  
Observe Data  
Init Events  
        created  
    *has el option*  n-> when vm.$mount(el) is called  
            |  
        *has template option*  
`compile template into render function `  /  `compile el's outerHTML as template`
beforeMount
        Create vm.$el and repalce 'el' with it
mounted
                                    beforeUpdate
                when data changes   virtual DOM re-render and patch
                                    updated

destroy 
        Teardown watchers, child components and event listeners

        destroyed
```

```js
let a = 1
```

