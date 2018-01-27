# HTML 语义化

- 没有语义化

  ```HTML
  <div class="header"></div>

  <div class="container">
    <div class="aside"></div>
    <div class="main"></div>
  </div>

  <div class="footer"></div>

  ```

- 语义化之后

  ```HTML
  <header class="header"></header>

  <div class="container">
    <aside class="aside"></aside>
    <main class="main"></main>
  </div>

  <footer class="footer"></footer>

  ```

## 优势

- 方便团队开发与维护
- 有利于 SEO
- 屏幕阅读软件（盲人）会根据结构来读页面

#### 参考文章

- [深入理解HTML5标签](https://segmentfault.com/a/1190000002695791)
- [HTML 语义](http://justineo.github.io/slideshows/semantic-html/#/2)


## 让 IE8 支持 HTML 5 新标签

> 默认情况下， IE8 不支持 HTML5 新标签

### 使用 `document.createElement`

```HTML
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <title>HTML5 test</title>
    <style media="screen">
    /*  重置样式 */

    article,
    aside,
    details,
    figcaption,
    figure,
    footer,
    header,
    hgroup,
    main,
    menu,
    nav,
    section,
    summary {
        display: block;
    }
    </style>
</head>

<body>
    <script>
    document.createElement('section');
    </script>
    <style>
    section {
        color: red;
    }
    </style>
    <section>
        Hello!
    </section>
</body>

</html>

```

### 借助 html5shiv.js 让 IE8 支持更多的 HTML5 特性

#### 参考链接

- [IE8 HTML5 surport](http://intertwingly.net/blog/2008/01/22/Best-Standards-Support#c1201006277)
- [HTML5 shiv](https://johnresig.com/blog/html5-shiv/)
- [html5shiv.js](https://github.com/aFarkas/html5shiv/)
- [github上html5shiv项目readme.md部分的翻译](http://www.zhangxinxu.com/wordpress/2013/02/github-html5shiv-readme-translate/)
- [HTML5 Shiv 的一些趣事](http://note.rpsh.net/posts/2011/05/25/story-of-html5-shiv/)
