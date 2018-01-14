# 常用基本元素

## 标题元素
`<h1>`、 `<h2>`、 `<h3>`、 `<h4>`、 `<h5>`、 `<h6>`标签用来定义标题，其大小依次减小，`<h1>`为最大的标题，`<h6>`为最小的标题。

```HTML
<h1>这是标题 1</h1>
<h2>这是标题 2</h2>
<h3>这是标题 3</h3>
<h4>这是标题 4</h4>
<h5>这是标题 5</h5>
<h6>这是标题 6</h6>
```

**注意：** 标题具有明确的语义性，请根据文档结构合理使用，而不要只是用来标识字体大小。

## 段落元素
`<p>`标签定义段落，每一个`<p>`标签默认都另起一行。

```HTML
<p>这是段落文字</p>
<p>这是另一个段落文字，另起一行开始</p>

```

## 图片元素
`<img>`标签用来在网页中嵌入图片，该标签没有结束标签。`<img>`标签有两个必需的属性：`src`属性 和 `alt` 属性。其中`src`属性为图片地址，`alt`属性为如果图片加载失败显示的替换文字。除了必须属性外，还可以添加控制大小的属性`width`和`height`。

```HTML
<img src="//placehold.it/300" alt="我是图片加载失败后显示的文字" width="150" height="150">
```
## 链接元素
`<a>`标签定义超链接，用于网页之间的跳转（从一个网页到另一个网页），它有一个重要的属性`href`，用来指定链接的目标。如果需要新标签页打开，则要添加另一个属性`target`。如果图片也需要超链接，则可以通过元素嵌套实现.

```HTML
<a href="http://imweb.io" target="_blank">
    <img src="imweb-logo.png" alt="IMWeb 学院">
</a>
```

## 列表元素
列表分为无序列表及有序列表两种，其中无序列表标签为`<ul>`，有序列表标签为`<ol>`，其直接的子元素标签为`<li>`(不能是其他标签)。

```HTML
<!-- 无序列表 -->
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JS</li>
</ul>

<!-- 有序列表 -->
<ol>
    <li>首先把冰箱门打开</li>
    <li>然后把大象关进去</li>
    <li>最后把冰箱门关上</li>
</ol>

```

## div 元素
`<div>`标签用来分割为独立的、不同的部分，每一个`<div>`标签默认都另起一行。

```HTML
<div>
    <h2>区块标题/h2>
    <p>区块描述文字</p>
</div>
```

## span 元素
`<span>`标签被用来组合文档中的行内元素。

```HTML
<p>前端三大语言：<span>HTML</span>、<span>CSS</span>、<span>Javascript</span></p>
```

## 换行元素
`<br>`标签可插入一个简单的换行符，它是个空元素，没有结束标签，不包含任何内容。

#### 参考链接
- [HTML 元素参考 | MDN](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element)
- [HTML 参考手册 | W3cschool](http://www.w3school.com.cn/tags/)
- [HTML 元素 | 维基百科](https://www.wikiwand.com/en/HTML_element#/Document_structure_elements)
