# html
### 第1章 html结构 
* 利于SEO search engine optimization
* html是文本文档
* 标签与<b>元素</b>（经常互换使用）
* 特性与<i>特性值</i>
* 注意现在html的发展迅速，现在要多看看开发文档
* 开始标签与结束标签<></>
* 学习 html 学习 标签 作用 用在何处

### 第二章 文本
#### 结构化标记
  * 标题 ``` <h1> <h2> <h3> <h4> <h5> <h6>```
  * 段落  ` <p>`
  * 粗体与斜体 ` <b> <i>`
  * 上标与下标 ` <sup> <sub>`
<i>example: 3<sup>rd</sup> ,CO<sub>2</sub></i>

* 空白（遇到多个空白折叠成一个）
* 换行符` <br />`
<i>假如<br />生活欺骗了你</i>

* 水平线` <hr />`
<i><hr />假如生活欺骗了你</i>

#### 语义化标记
上面都是结构化标记
语义化标记用来给网页添加额外信息
* 加粗和强调 ` <storng> <em>` 
* 引用 ` <blockquote> <q>`
* 缩写词 ` <abbr>`
* 引文和定义 ` <cite> <dfn>`
* 设计者详细信息 ` <address>`
* 内容的修改 ` <ins> <del> <s>`
<i>example:<ins>hi</ins><del>bye</del></i>

### 列表
#### 有序列表
```
<ol>this is an orderedlist
<li>zhangsan</li>
<li>lisi</li>
<li>wangwu</li>
</ol> 
```
<ol>this is an orderedlist
<li>zhangsan</li>
<li>lisi</li>
<li>wangwu</li>
</ol> 

#### 无序列表
` <ul> <li>`
#### 定义列表

*` <dl>` 定义列表
*` <dt>` 术语
*` <dd>` 定义

```
<dl>
<dt>春天</dt>
<dd>春天是一个季节</dd>
</dl>
```
<dl>
<dt>春天</dt>
<dd>春天是一个季节</dd>
</dl>

#### 嵌套列表
```
<ul>
<li>春天在哪里？</li>
<ul>
<li>小朋友眼睛里</li>
</ul>
</ul>
```
<ul>
<li>春天在哪里？</li>
<ul>
<li>小朋友眼睛里</li>
</ul>
</ul>

### 链接
``` <a href="www.scut.cn">华南理工官网</a>```

<a href="www.scut.cn">华南理工官网</a>

#### URL(unified resource locator)
* 绝对URL
域名+资源位置
* 相对URL
在相同文件夹内（例如同一网站），可以只使用相对URL
子文件夹访问链接父文件夹/祖父文件夹的文件：


margin //外边距
padding//内边距

##### chrome f12 on mac
> option + command + i

#### 添加图像
 <b>标签：</b>` <img>`
 <b>特性：</b>
 1. src(告诉浏览器哪里可以找到图片) 
 2. alt(图像的文本说明) 
 3. title（图像的附加说明）
 4. height
 5. width

 #### 表格
  1. 标签：` <table> <tr>:table row <td>:table data`
  2. 表格的标题： ` <th>`
  3. 特性： colspan 跨列 rowspan 跨行
  <br>
  ``` 
  <table width="400" cellpadding="10" cellspacing="5">
   <tr>
    <th width="150"></th>
    <th>Alice</th>
    <th>Tom</th>
    <th>Bob</th>
  </tr>
  <tr>
    <th>age</th>
      <td colspan="2">5</td>  <td>4</td>
      <td>17</td>
  </tr>
  </table>
  ```
  <table width="400" cellpadding="10" cellspacing="5">
  <tr>
  <th width="150"></th>
  <th>Alice</th>
  <th>Tom</th>
  <th>Bob</th>
  </tr>
  <tr>
  <th>age</th>
  <td colspan="2">5</td> 
  <td>4</td>
  
  </tr>
  </table>

#### 表单
* 标签
` <textarea> <input> `

## 学习CSS
 
