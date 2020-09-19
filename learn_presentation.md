#### html的语义标签
###### section
* 段落
* webkit.org 苹果开源的浏览器内核

##### html语法
* 元素（标签）
<script></script>

* 属性
##### js语法
* alert window里面弹出窗口
例如：alert("hello");

* this
> 谁调用this，this就指向谁，指向的是一个对象
>函数.call()
* 原型

#### 为什么会卡顿
1. 图片资源过大
2. 浏览器会下载很多文件（线程个数决定）

### 跨域
 面试必问
#### 基础知识
 - 同源策略
 浏览器故意设计的一个功能限制
 
#### 什么是同源? 为什么要同源？重点
 两个URL
 - 协议
 - 域名
 - 端口号

 #### 规避
  
 #### 怎么跨域
 - cros
 - websocket, nginx

### 具体语法

#### 不支持老的浏览器
 - 兼容性不好
###### jsonp
 - 和json没有半毛钱关系
 ` <script>`  不支持同源。

 ### 什么是跨域？为什么要跨域？
 ### 同源政策？避免同源的方法。

 ### js的事件处理机制
 #### 宏任务，微任务
  1. 同步代码
  2. 清空微任务列表
  3. 在从宏任务列表取出一个并执行
  4. 清空微任务列表
  5. 循环3、4
 
 script start
 promise start
 这是p改变
 script end
 hhhh reject
 hhh
 这是第一个settimeout
 p2start
 p2success
 这是第二个settiemout
 p3start
 p3success
 



