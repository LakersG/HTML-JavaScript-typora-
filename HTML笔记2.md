# CSS操作

## 关联方式

### 1 内联样式

（杂乱、不易维护）

### 2 内部样式

（多个页面容易混乱）

```
<style></style>标签
```

### 3 外部样式

（运用于多个页面）

一般使用link，可以通过 javaScript 的DOM操作去修改

```
<link herf="css文件">标签
```

## CSS 语法组成

选择器+声明

选择器可以继承

### 1.全局选择器（级别最低）

```
*{} 
```

一般用作初始化

### 2.元素选择器

p、b、div 等标签
选择同种元素

```
<span></span>标签选择器
```

### 3.类选择器（灵活）

例 

```
<h2 class = "name">
```

索引方式

```
· "类名"{} 
```

多个类名中间用 ， 分隔
同个标签可以用多个类选择器（用空格分开）

### 4.ID选择器

例

```
<h2 id="name"> 
```

一个id只能使用一次，不能以数字开头
索引方式

```
#"id名"{}
```

-------------------------------------------------

## 字体属性

### 字体颜色（三种方式）

1.对应十六进制数字
2.英文单词
3.RGB三原色通道

### 字体大小

```
font-size 接受最小值：12px
```

### 字体粗细

```
font-weight（bold bolder lighter）
100-900px （400为默认）
```

### 字体样式

```
font-style
normal 正常
italic 斜体字
```

### 行高

```
line-height (px/数字/em等)
```

### 文字修饰

```
text-decoration：（none/underline/overline/linethrough）
```

### 字体

font-family （宋体、黑体······）

-------------------------------------------------

## 背景属性

### 主要属性

```
background-color 背景颜色
```

```
background-image （url="图片链接"）
```

```
background-position 渲染起始位置
{ left、 right、 center、 top、 button }
```

```
background-repeat（设置如何平铺背景图像）
{
  repeat-x
  repeat-y
  no-repeat
}
```

```
background-size
{
  1.设置像素大小
  2.设置百分比大小
  3.cover 保持图片横纵比并将图片缩放成完全覆盖的最小大小
  4.contain 保持图片横纵比并将图片缩放成适合背景定位的最大大小
}
```

----------------------------------------------------

### 文本属性

text-align（center left right）

```
text-decoration
{  
  overline    //上划线
  linethrough //下划线
  underline   //下划线
}
```

```
text-transform
{
  captialize //每个单词开头大写
  uppercase  //全部大写
  lowercase  //全部小写
}
```

```
text-indent
{
  正值，右缩进
  负值，左缩进
}
```



----------------------------------------------------

## 表格属性

```
border: _px(粗细) solid（实线） color（颜色）
table，td.(内部线)
border-collapse(单边框)
```



### 表格填充

```
padding: 内边距
```



### 表格颜色

```
backgroundcolor：背景颜色
color：字颜色

宽 width
高 height
```



### 表格文字属性

```
水平： text-align
垂直： height, vertical-align
```



-----------------------------------------------------

## CSS伪类选择器

伪类：专门用来表示元素的一种特殊状态。（用冒号）

常用的伪类选择器：

1. a标签的伪类：:link（初始状态） / :visited（访问过后） / :hover（鼠标经过时） / :active（单击下去）
2. :focus ：获得焦点
3. :first-child/ :last-child / :nth-child（number）



## 关系选择器

### 1.后代选择器

选择E下被F包含的元素

```
E F
{  } 多重包含也生效
```



### 2.子代选择器

只对直接子代元素有用

```
E>F
{ }
```



### 3.相邻兄弟选择器

紧跟E后的F

```
E+F
{ }
```



### 4.通用兄弟选择器

```
E~F
{ } E下面所有同类型的兄弟
```



## CSS伪元素

用于向某些选择器设置特殊效果

伪元素和伪类的区别：

根本区别在于：它们是否创造了新的元素。

伪元素/伪对象：前面必须有选择器，不存在在DOM文档中，是虚拟的元素，是创建新元素。代表某个元素的子元素，这个子元素虽然在逻辑上存在，但却并不实际存在于文档树中。



伪类只能使用“：”
而伪元素既可以使用“:”，也可以使用“::”

因为伪类是类似于添加类所以可以是多个，而伪元素在一个选择器中只能出现一次，并且只能出现在末尾



常用：

:before  / :after / :first-letter /:first-line 可以是一个冒号也可以是双冒号

::selection / ::placeholder / :: backdrop 前面只能是双冒号

```
<style>
	p:first-letter{
	//添加特性
	}
</style>
```



-------------------------------------------------------