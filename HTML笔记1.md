





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



## 2. 常见的HTML标签

标签是由标签名、标签属性和文本内容三部分组成（注意：单标签没有文本内容）

标签属性是对标签的一种描述方式

标签属性分通用属性、自有属性和自定义属性。

### 通用属性

所有标签都具有的属性，如：

```
id 给标签一个唯一的名称

class 给标签一个类

style 设置标签的行内样式

title 鼠标移动到该标签所提示的内容
```

### 自定义标签

通常用来传值。

格式：data-*

```
<img data-src = "图片名" alt = "提示文本">
```



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
    <tr>//行
    	<th></th>//表头
    	<td></td>//列
    </tr>
</table>
```

行<tr>
列<td>
快捷方式

```
 table>tr*n>td*n{}
```

#### 属性

​		border:表格边框

​		width:表格宽度

​		align:表格对齐方式（left（默认），right，center）

​		cellpadding:单元格文本与边框的距离

​		cellspacing: 单元格边框间距

#### 表格合并

- 水平合并 保留左边

  ```
  colspan="" 
  ```

  

- 垂直合并 保留上边

  ```
  rowspan="" 
  ```

#### 完整的表格组成

​		caption（标题）、thead（表头）、tbody（表体）和tfoot（表尾）四部分组成。

```
<input>: 输入框 -> type = "submit" （有提交按钮）
<button> name </button> 按钮
alert("") 弹窗
```



## 3 Form 表单（用户输入的地方）

核心标签之一，实现前后端交互

常用属性：

action ：表单数据提交的服务器网址
name ：表单名称
method ：方式 （get（会暴露数据）/post（不会暴露））

### 1.input类

| 控件名称     | type属性值   | 描述                                                         |
| ------------ | :----------- | :----------------------------------------------------------- |
| 文本框       | text(默认值) | 默认。定义一个单行的文本字段（默认宽度为 20 个字符）。       |
| 密码框       | password     | 定义密码字段                                                 |
| 单选按钮     | radio        | 定义单选按钮。(性别等)                                       |
| 复选框       | checkbox     | 定义复选框。(爱好等)                                         |
| 提交按钮     | submit       | 定义提交按钮。                                               |
| 重置按钮     | reset        | 定义重置按钮（重置所有的表单值为默认值）。                   |
| 图片提交按钮 | image        | 定义图像作为提交按钮。                                       |
| 普通按钮     | button       | 定义可点击的按钮（通常与 JavaScript 一起使用来启动脚本）。   |
| 隐藏文本框   | hidden       | 定义隐藏输入字段，前后台交互非常有用。                       |
| 文件上传框   | file         | 定义文件选择字段和 “浏览…” 按钮，供文件上传。可以通过accept属性规范选取文件的类型。accept属性的值:<br/>image/* 接受所有的图像文件。<br/>image/png 表示只接受图片文件的png文件<br/>audio/* 接受所有的声音文件。<br/>video/* 接受所有的视频文件。<br/>multiple属性可以用来设置一次允许选择多个文件 multiple=“multiple” |

属性：

placeholder（提示）/ name（命名）/ minlength（最小长度）maxlength（最大长度）/ disabled（忽略）/ readonly（只读）

### 2.textarea

属性：

name / id / cols（行数）/ rows（列数）/ placeholder（提示）/ minlength（最小长度）maxlength（最大长度）/ required / value

定义文本域 (一个多行的输入控件)，输入大量的内容

文本区域中可容纳无限数量的文本，其中的文本的默认字体是等宽字体（通常是 Courier）。

可以通过 cols 和 rows 属性来规定 textarea 的尺寸大小，不过更好的办法是使用 CSS 的 height 和 width 属性。

缩放设置：

禁止缩放：resize: none;
水平缩放：resize: horizontal;
垂直缩放：resize: vertical;
水平垂直缩放：resize: both;

### 3.select类

下拉列表框，默认用于单项选择。用option呈现每个选项。

```
<form>
	<lable for="course">课程</lable>
	<select id="course" multiple = "multiple"//可以多选，没有只能单选>
		<option>语文</option>
        <option>数学</option>	
        <option>英语</option>	
	</select>//for和id对应，产生关联
</form>
```

multiple：表示可以多选。

size：最多显示的行数。

### 4.button类

普通按钮，具有提交功能。可以单独使用，若写在form表单时中具有提交功能。

#### 文本框：

```
<input type="text" name="textarea">
```

#### 密码框：

```
<input type="password">
```

#### 提交框：

```
<input type="submit" value="按钮文字 ">
```



### 5.iframe

框架集，用来将多个网页组合成一个文件

#### 属性：

- name：框架名
- src：引入的外部HTML文件
- width：宽度
- height：高度
- frameborder： 是否有边框
- marginheight：框架距离顶部和底部的距离
- marginwidth：框架距离左右的距离

#### 框架标签





## 4. 内联（行级）元素和块元素

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





## 5. HTML 5新增容器

```
<header><header>  头部
<nav><nav>  导航栏
<article><article> 
<section><section>
<aside><aside>  侧边栏
<footer><footer>  底部
```

