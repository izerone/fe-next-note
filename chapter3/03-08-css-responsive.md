# 响应式设计

[响应式站点欣赏](https://mediaqueri.es/popular/)

## 简介

- 响应式设计
  - viewport
  - media queries
  - 内容布局
  - 图片大小

## viewport

```html
<meta name="viewport" content="width=device-width,initial-scale=1.0">

```

[viewport 详解](http://www.cnblogs.com/2050/p/3877280.html)

## 媒体查询

```css

/*  关键词 媒体类型  逻辑操作符  媒体条件  媒体属性 */

@@media screen and (min-width: 768px) and (max-width: 1024px){
  .demo {
    color: red;
  }
}

```

```html

<link rel="stylesheet" href="style.css" media="(min-width:1024px)">

```

## 响应式布局

- [内容流式布局](http://coding.imweb.io/demo/p3/responsive/fluid.html)
- [固体 + 流式](http://coding.imweb.io/demo/p3/responsive/fixed.html)
- [切换显示形式](http://coding.imweb.io/demo/p3/responsive/style.html)

## 响应式图片

```html
<img src="img/small.png" srcset="img/large.png 960w,img/medium.png 640w.img/small.png 320w"
sizes="(max-width:414px) 100vw,640px" alt="响应式图片">

```

### 响应式资源参考

#### 基本认识

- [什么是响应式布局设计](https://www.zhihu.com/question/20976405)
- [viewport 深入理解](https://www.cnblogs.com/2050/p/3877280.html)
- [CSS 媒体查询](https://developer.mozilla.org/zh-CN/docs/Web/Guide/CSS/Media_queries)
- [下手响应式及断点设置分析](http://imweb.io/topic/56dff5121a5f05dc506430da)

#### 整体布局

- [浮动布局精华 Layout Gala](https://blog.html.it/layoutgala/index.html)
- [Flexbox Grid](http://flexboxgrid.com/)
- [How to build a responsive grid system](https://zellwk.com/blog/responsive-grid-system/)

#### 内容处理相关

- [响应式导航解析](http://mux.alimama.com/posts/785)
- [video 自适应问题](http://alistapart.com/article/creating-intrinsic-ratios-for-video)
- [响应式图片处理101系列](https://www.w3cplus.com/blog/tags/509.html)
- [table 处理](https://css-tricks.com/responsive-data-table-roundup/)
- [图片滚动](http://www.swiper.com.cn/)


#### 框架相关

- [Bootstrap](http://v3.bootcss.com/)
- Foundation

#### 工具相关

- [使用Chrome测试页面响应性](https://segmentfault.com/a/1190000000581601)
- [测试响应和设备特定可视窗口](http://www.css88.com/doc/chrome-devtools/device-mode/emulate-mobile-viewports/)
- [Screensiz.es](http://screensiz.es/phone)
- [Respond.js](https://github.com/scottjehl/Respond)

#### 其他

- [响应式案例](https://mediaqueri.es/)
- [响应式资源汇总](https://bradfrost.github.io/this-is-responsive/resources.html)
- [《响应式Web设计-HTML5和CSS3实践》](https://www.gitbook.com/book/jobrest/web-html5-css3/details)

注：一般来说复杂的站点都会单独处理移动端，而不是全兼容从 PC 到 移动端的全兼容，毕竟移动端还是以轻快为主。

## 常见 CSS 框架

- [Bootstrap](https://v4-alpha.getbootstrap.com/)
- [Pure CSS](https://purecss.io/start/)
- [WE UI](https://github.com/Tencent/weui/wiki)
