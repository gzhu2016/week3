# 多媒体第三周资料：HTML

## 1 HTML 简介

```HTML
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>我是标题</title>
</head>
<body>
    <h1>我的第一个标题</h1>
    <p>我的第一个段落。</p>
</body>
</html>
```

> 注意：对于中文网页需要使用 `<meta charset="utf-8">` 声明编码，否则会出现乱码。

1. DOCTYPE 声明了文档类型
2. 位于标签 `<html>` 与 `</html>` 描述了文档类型
3. 位于标签 `<body>` 与 `</body>` 为可视化网页内容
4. 位于标签 `<h1>` 与 `</h1>` 作为一个标题使用
5. 位于标签 `<p>` 与 `</p>` 作为一个段落显示

## 2 HTML 网页结果

![](http://airing.ursb.me/image/2016091701.png)

> 注：只有 `<body>` 区域 (白色部分)才会在浏览器中显示。

## 3 HTML 基础

### 3-1 HTML 标题

HTML 标题（Heading）是通过`<h1>` - `<h6>` 标签来定义的。

```HTML
<h1>这是一个标题</h1>
<h2>这是一个标题</h2>
<h3>这是一个标题</h3>
```

### 3-2 HTML 段落

HTML 段落是通过标签 `<p>` 来定义的。

```HTML
<p>这是一个段落。</p>
<p>这是另外一个段落。</p>
```

### 3-3 HTML 链接

HTML 链接是通过标签 `<a>` 来定义的。

```HTML
<a href="http://www.runoob.com">这是一个链接</a>
```

超链接可以是一个字，一个词，或者一组词，也可以是一幅图像，您可以点击这些内容来跳转到新的文档或者当前文档中的某个部分。

当您把鼠标指针移动到网页中的某个链接上时，箭头会变为一只小手。

在标签`<a>`中使用了`href`属性来描述链接的地址。

### 3-4 HTML 图像

HTML 图像是通过标签 `<img>` 来定义的.

```HTML
<img src="w3cschool.png" width="104" height="142">
```

### 3-5 HTML 水平线

`<hr>` 标签在 HTML 页面中创建水平线。

```HTML
<p>这是一个段落。</p>
<hr>
<p>这是一个段落。</p>
<hr>
<p>这是一个段落。</p>
```

### 3-6 HTML 注释

```HTML
<!-- 这是一个注释 -->
```

### 3-7 HTML 换行

如果您希望在不产生一个新段落的情况下进行换行（新行），请使用 `<br/>` 标签：

```HTML
<p>这个<br>段落<br>演示了分行的效果</p>
```

`<br/>` 元素是一个空的 HTML 元素。由于关闭标签没有任何意义，因此它没有结束标签。

### 3-7 HTML 文本格式化

#### 3-7-1 HTML 文本格式化标签

|标签|描述|
|:--:|:--:|
|`<b>`|定义粗体文本|
|`<em>`|定义着重文字|
|`<i>`|定义斜体字|
|`<small>`|定义小号字|
|`<strong>`|定义加重语气|
|`<sub>`|定义下标字|
|`<sup>`|定义上标字|
|`<ins>`|定义插入字|
|`<del>`|定义删除字|

#### 3-7-2 HTML "计算机输出" 标签

> 注：了解即可。

|标签|描述|
|:--:|:--:|
|`<code>`|定义计算机代码|
|`<kbd>`|定义键盘码|
|`<samp>`|定义计算机代码样本|
|`<var>`|定义变量|
|`<pre>`|定义预格式文本|

#### 3-7-3 HTML 引文, 引用, 及标签定义

> 注：了解即可。

|标签|描述|
|:--:|:--:|
|`<abbr>`|定义缩写|
|`<address>`|定义地址|
|`<bdo>`|定义文字方向|
|`<blockquote>`|定义长的引用|
|`<q>`|定义短的引用语|
|`<cite>`|定义引用、引证|
|`<dfn>`|定义一个定义项目|

### 3-8 HTML 头部

#### 3-8-1 HTML `<head>` 元素

`<head>` 元素包含了所有的头部标签元素。在 `<head>`元素中你可以插入脚本（script）, 样式文件（CSS），及各种meta信息。

可以添加在头部区域的元素标签为: `<title>`, `<style>`, `<meta>`, `<link>`, `<script>`, `<base>`。

#### 3-8-2 HTML `<title>` 元素

`<title>` 标签定义了不同文档的标题。

`<title>` 在 HTML/XHTML 文档中是必须的。

1. 定义了浏览器工具栏的标题
2. 当网页添加到收藏夹时，显示在收藏夹中的标题
3. 显示在搜索引擎结果页面的标题

#### 3-8-3 HTML `<base>` 元素

`<base>` 标签描述了基本的链接地址/链接目标，该标签作为 HTML 文档中所有的链接标签的默认链接:

```HTML
<head>
<base href="http://www.runoob.com/images/" target="_blank">
</head>
```

#### 3-8-4 HTML `<link>` 元素

`<link>` 标签定义了文档与外部资源之间的关系。

`<link>` 标签通常用于链接到样式表。

```HTML
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```


#### 3-8-5 HTML `<style>` 元素

`<style>` 标签定义了HTML文档的样式文件引用地址。

在 `<style>` 元素中你需要指定样式文件来渲染 HTML 文档。

```HTML
<head>
<style type="text/css">
body {background-color:yellow}
p {color:blue}
</style>
</head>
```

#### 3-8-6 HTML `<meta>` 元素

1. `<meta>` 标签描述了一些基本的元数据。
2. `<meta>` 标签提供了元数据，元数据也不显示在页面上，但会被浏览器解析。
3. `<meta>` 标签通常用于指定网页的描述，关键词，文件的最后修改时间，作者，和其他元数据。
4. 元数据可以使用于浏览器（如何显示内容或重新加载页面），搜索引擎（关键词），或其他 Web 服务。
5. `<meta>` 一般放置于 `<head>` 区域

```HTML
<!--为搜索引擎定义关键词-->
<meta name="keywords" content="HTML, CSS, XML, XHTML, JavaScript">
<!--为网页定义描述内容-->
<meta name="description" content="Free Web tutorials on HTML and CSS">
<!--定义网页作者-->
<meta name="author" content="Hege Refsnes">
<!--每30秒中刷新当前页面-->
<meta http-equiv="refresh" content="30">
```

#### 3-8-7 HTML `<script>` 元素

`<script>` 标签用于加载脚本文件，如： JavaScript。

`<script>` 在以后的课程中会详细描述。

## 4 课堂练习

```HTML
<!DOCTYPE HTML>
<html>
    <head>
        <meta charset="utf-8"> 
        <title>多媒体技术</title>
    </head>


    <body>
        <h1>万年死神小学生的自白</h1>
        作者：<a href="http://baidu.com"><em>柯南</em><a/>
        <p>我的名字叫<del>工藤新一</del>，不，现在叫<strong>江户川柯南</strong>，原本是个名侦探，不幸被歹徒灌下毒药而变小。</p>
        <p>我的名人名言是：<blockquote>身体虽然缩小了，头脑还是一样的好。无论如何，真相只有一个！</blockquote></p>
        <p>我的身体已经<small>缩小了</small>！要是让他们知道工藤新一还活着，不但我的性命难保，还会危害到我周遭的亲人。在阿笠博士的建议下，我隐瞒了身份。当小兰问及我的名字时，情急之下，我化名为江户川柯南。为了搜集那些家伙的情报，于是便住进了父亲以侦探为业的小兰家中。但是这位叔叔却是个糊涂大侦探，看不下去的我于是便装成叔叔，利用我天生的推理能力解决了许多的悬疑案件。而叔叔也拜我所赐成了名号越来越响的大侦探。而我现在却变回了一个小学生，还被迫跟同班同学的步美，元太与光彦组成少年侦探团。</p>
        <p>接着就向大家介绍博士为我发明的道具。首先是<sup>手表型麻醉枪</sup>。透过瞄准器对准目标按下按钮就能发射麻醉针，能够在瞬间让人昏睡；接着是<sup>领结变声器</sup>。只要调整后放的转盘，不管是大人或是小孩，任何人的声音都可以模仿；接下来的秘密道具是<sup>脚力倍增鞋</sup>，利用电与磁力刺激脚的穴道，可使肌肉的力量发挥极限；若要追缉歹徒，则可使用涡轮引擎滑板，不过因为动力来自太阳能，只有在出太阳时才能使用，这是它唯一的缺点。对了，我差点忘记了。我们少年侦探团的胸章内藏了<sup>超小型无线电对讲机</sup>，同时还兼备发信机功能，简直无懈可击。除此之外虽然还有很多道具，不过最厉害的武器应该算是我这里（脑袋）。</p>
        <p><cite>身体虽变小，但头脑一样棒，无所不知的名侦探，真相永远只有一个！</cite> </p>
        <img src="http://airing.ursb.me/image/2016091702.jpeg" >
    </body>


	</html>
```

## 5 课后作业

1. 学习慕课网提供的[
《HTML+CSS基础课程》](http://www.imooc.com/learn/9)中的第1章到第5章的内容，并完成练习。

2. 学习慕课网提供的[
《HTML+CSS基础课程》](http://www.imooc.com/learn/9)中的第6章到第15章的内容，并完成练习。（选做）

> 要求：在[github.com/gzhu2016/week3](http://github.com/gzhu2016/week3)上提交作业，内容为慕课网学习进度截图。


