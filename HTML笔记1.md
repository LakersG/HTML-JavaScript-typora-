

# HTML

## 1.搭建框架

<!DOCTYPE html>  ！+回车生成默认框架

<head></head> 头部
<title></title> 标题，显示在标签页
<p></p> 段落
<h1></h1>

<h6></h6>
1~6级标题 快速 h$*n(n代表几级标题)

<hr color= width= size= align=> 水平线
<img src="网址" alt="">图片
和HTML文件的位置关系
/ 子集  ./同集 ../父集 
超链接
<a herf="转跳的网址"> 可以是anything </a>
文本标签
<em></em> 着重文字
<b></b> 粗体文字
<i></i> 斜体文字
<del></del> 删除文字
<span></span> 无特殊含义

列表
<ol> 
    <li></li> 
</ol> 

有序标签

type= 1（1，2，3）
type= a (a,b,c)
type= A (A,B,C)
type= i 小写罗马数字
type= I 大写罗马数字

<ul> 
    <li></li> 
</ul> 
无序标签

type= dise '·' 
type= circle 'o'
type= suqare 方形
type= none ' '

表格
<table> </table>

行<tr>
列<td>
快捷方式 table>tr*n>td*n{}

表格合并
colspan="" 

水平合并 保留左边
rowspan="" 

垂直合并 保留上边

Form 表单（用户输入的地方）
1.容器
2.控件（输入框，按钮）
action ：服务器网址
name ：表单名称
method ：方式
{
  get url
  post
}
<input>: 输入框 -> type = "submit" （有提交按钮）
<button> name </button> 按钮
alert("") 弹窗

文本框：

<input type="text" name="textarea">
密码框：

<input type="password">
提交框：

<input type="submit" value="按钮文字 ">

内联元素和块元素

div(容器元素)
H5新增容器

<header><header> 头部
<nav><nav> 导航栏
<article><article> 
<section><section>
<aside><aside> 侧边栏
<footer><footer> 底部