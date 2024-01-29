





# HTML

HTML是一种超文本**标记语言**，标识性语言，而非**编程语言**，不能使用逻辑运算。通过标签将网络上的文档格式进行统一，是分散的网络资源成为完整的整体。

具备简易性、可扩展性、平台无关性和通用性等特点。

## 1. 搭建框架

```
<!DOCTYPE html> ！+回车生成默认框架
<head></head>   头部
<title></title> 标题，显示在标签页
<p></p>         段落
```

```
1~6级标题 快速 h$*n(n代表几级标题)
<h1></h1>
<h6></h6>
```



## 2. 常见的HTML元素

### 2.1 水平线

```
<hr color=black width= size= align=> 
```


### 2.2 图片

```
<img src="" alt="">
```

### 2.3 和HTML文件的位置关系

/ 子集  ./同集 ../父集 

### 2.4 超链接

```
<a herf="转跳的网址"> 可以是anything </a>
```

### 2.5 文本标签

<em>王干饭</em> 

```
<em></em>
```

着重文字

<b>王干饭</b> 

```
<b></b>
```

粗体文字

<i>王干饭</i> 

```
<i></i>
```

斜体文字

<del>王干饭</del> 

```
<del></del>
```

删除文字

<span>王干饭</span> 

```
<span></span>
```

无特殊含义

### 2.6 列表

#### 有序标签

```
<ol>
	<li></li>
</ol>
```

<ol> 
    <li>王干饭</li> 
    <li>陈干饭</li>
</ol> 
```
type= 1（1，2，3）
type= a (a,b,c)
type= A (A,B,C)
type= i 小写罗马数字
type= I 大写罗马数字
```



### 无序标签

```
<ul>
	<li></li>
</ul>
```

<ul> 
    <li>王干饭</li> 
    <li>陈干饭</li>
</ul> 
```
type= dise '·'`
type= circle 'o'
type= suqare 方形
type= none ' '
```



### 2.7 表格

```
<table> 
    <tr>111</tr>
    <tr>222</tr>
</table>
```

行<tr>
列<td>
快捷方式

```
 table>tr*n>td*n{}
```



#### 表格合并

- 水平合并 保留左边

  ```
  colspan="" 
  ```

  

- 垂直合并 保留上边

  ```
  rowspan="" 
  ```



### 2.8 Form 表单（用户输入的地方）

1.容器
2.控件（输入框，按钮）
action ：服务器网址
name ：表单名称
method ：方式
{
  get url
  post
}

```
<input>: 输入框 -> type = "submit" （有提交按钮）
<button> name </button> 按钮
alert("") 弹窗
```



#### 文本框：

```
<input type="text" name="textarea">
```

#### 密码框：

```
<!--<input type="password">-->
```

#### 提交框：

```
<!--<input type="submit" value="按钮文字 ">-->
```



## 3. 内联（行级）元素和块元素

​		块级元素独占一行，识别宽高，如果不设置，宽度为整行宽度，高度为实际内容高度。

​		行级不独占一行，不能设置宽高，宽高分别为内容实际的宽高。

​		块级标签可通过设置样式：

```
display：inline
```

​		转换为行级标签，而行级标签可通过设置样式：

```
display：block
```

​		转换为块级标签。



### 块级标签

```
div p h1-h6 ul ol pre table adress 等
```

### 行级标签

```
span a b strong i em sup sub
```

img属于行块级标签，相当于执行了

```
display: inline-block
```



### 嵌套规范

1.块级元素可以包含行级元素或块级元素，但是行级元素只能包含行级元素。

2.p,h1-h6,dt标签中只能包含行级标签，不能再包含块级标签。

3.块级元素和块级元素并列，行级元素和行级元素并列。



## 4. div(容器元素) 

## 5. HTML 5新增容器

```
<header><header>  头部
<nav><nav>  导航栏
<article><article> 
<section><section>
<aside><aside>  侧边栏
<footer><footer>  底部
```

