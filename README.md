# Homepage about index.html and homestyle.css

<img id="dx" src="http://home.ustc.edu.cn/~rdx1017/main/dx.png">

## homestyle.css 设置了我的页面的板式

```
div#left_side{
    float: left;
    font-family: Consolas,"Comic Sans MS";
    text-align: left;
    font-size: 80%;
    width: 20%;
    margin-right: 10px;
    padding: 10px;
    background-color: #4d505b;
    color: azure;
}

div#right_side{
    float: right;
    font-family: Tahoma,Georgia,"Times New Roman";
    font-size: 76%;
    width: 18%;
    margin-left: 10px;
    padding: 10px;
    background-color: #4d505b;
    color: azure;
}

div#middle{
    margin: 10px auto;
    padding-left: 40px;
    padding-right: 20px;
    width: 58%;
}
```
这一段代码设置

```
div#left_side
```
我的页面左栏占20%的页面，并且向左浮动，也就是靠在页面最左面。

```
div#right_side
```
我的页面右栏占18%的宽度，并且浮动在页面最右面。

中间的页面自动居中显示，宽度是58%。


**homestyle.css中其他的代码设置的就是一些细节的东西了**


## index.html 是我的网页格式和内容

### 7 - 13行是我的head的设置

```
<title>Ren Dexin</title>
```
这段代码设置网页标题。

```
<link type="image/x-icon" rel="shortcut icon" href="http://home.ustc.edu.cn/~rdx1017/main/dx.ico" />
```
这段代码设置网页小图标，其中href关键字是图标的绝对地址。
**icon格式的图标怎么做呢？百度一下就有在线制作的。**

```
<link rel="stylesheet" type="text/css" href="homestyle.css">
```
这段代码链接网页格式，也就是homestyle.css，假如这两个文件在一个文件夹，href关键字就不用添加绝对路径了，我的建议还是添加绝对路径比较好，因为全网页都使用这个板式。


### 17 - 34行是header部分，也就是网页最上面那一栏。

```
<img id="dx" src="http://home.ustc.edu.cn/~rdx1017/main/dx.png">
```
这段代码添加了我的网页左上角图标的链接地址。

```
<div id="nav_container">
    <ul>
        <li><a href="http://home.ustc.edu.cn/~rdx1017/">HOME</a></li>
        <li><a href="https://github.com/Rdx1017">GITHUB</a></li>
        <li><a href="http://home.ustc.edu.cn/~rdx1017/main/idl/idl.html">IDL</a></li>
        <li><a href="#fortran">FORTRAN</a></li>
        <li><a href="#about">MATLAB</a></li>
        <li><a href="#others">OTHERS</a> </li>
    </ul>
</div>
```
这段代码添加了访问列表分栏。他的属性设置在homestyle.css 67 - 97行。

```
div#nav_container{
    margin-left: 50px;
}

div#nav_container ul{
    list-style-type:none;
    margin:0;
    padding:0;
    overflow:hidden;
}

div#nav_container li
{
    float: left;
}
div#nav_container a:link,div#nav_container a:visited
{
    display:block;
    width:120px;
    font-weight:bold;
    color:#FFFFFF;
    background-color:#bebebe;
    text-align:center;
    padding:4px;
    text-decoration:none;
    text-transform:uppercase;
}
div#nav_container a:hover,div#nav_container a:active
{
    background-color:#cc0000;
}
```

#### <div id="contents"></div>
这一块添加的我的网页的主要内容部分，其中包括left_side,right_side和middle

**注意：left_side,right_side必须要在middle之前，因为他们是相对浮动的，要是不相信，可以试试换个位置。**

中间栏列表样式设置是：
```
div#contents ul{
    list-style-type: circle;
}
```

左右栏列表样式设置是：
```
div#right_side ul,div#left_side ul{
    margin: 0;
    list-style-type: square;
    padding: 1em;
}
```


# SOME TIPS

这是一个只用了很基础的一些html元素设置的一个简单的网页。
那么一般常用的html标签有哪些呢：

1.```<p>内容</p>```：这个标签里面是一个段落

2.```<a href="链接地址">提示字符串</a>```：这个标签里面是一个链接

3.```<img src='链接地址'/>```：这个标签里面是一个图片

4.```<ul></ul>```:这是一个列表，里面添加```<li>内容</li>```来加入每一个选项。

其他的还有很多，你应该去看书了解的，或者是访问w3school去学习.

<hr/>

<p>Copyright &copy; 2016 - 2017 -DX. All rights reserved.</p>
