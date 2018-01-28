# CSS 预处理

## 原生 CSS 问题
- 网站复杂度日益加深
- CSS 语法能力不够

## 常用 CSS 预处理器
- Sass
- less
- Stylus

## CSS 预处理器功能特性 （Sass）

### 嵌套

```CSS
/* 原生 CSS */

.link-list{
  border-radius: 10px;
}

.link-list .link-item {
  text-decoration: none;
}

.link-list .link-item:hover{
  background-color: #188eee;
}

/* Sass 预处理器 */

.link-list {
  border-radius: 10px;

  .link-item {
    text-decoration: none;

    &hover {
      background-color: #188eee;
    }
  }
}


```

- [Sass 在线编译](http://www.sassmeister.com/)

### 变量

```CSS
/* 原生 CSS */

.tt {
  color: #188eee;
}
.link {
  color: #188eee;
}

.btn {
  background-color: #188eee;
}

/* Sass 预处理器 */

$blue: #188eee;

.tt {
  color:$blue;
}
.link {
  color: $blue;
}

.btn {
  background-color:$blue;
}


```

### mixin

```CSS

/* 原生 CSS */

.box {
  -moz-box-shadow: 2px 4px #ccc;
  -webkit-box-shadow: 2px 4px #ccc;
  box-shadow: 2px 4px #ccc;
}

.header {
  -moz-box-shadow: 3px 4px #ccc;
  -webkit-box-shadow: 3px 4px #ccc;
  box-shadow: 3px 4px #ccc;
}

/* Sass 预处理器 */

@mixin box-shadow($shadow...){
  -moz-box-shadow:$shadow;
  -webkit-box-shadow: $shadow;
  box-shadow: $shadow;
}

.box {
  @include box-shadow(2px 4px #ccc);
}

.header {
  @include box-shadow(3px 4px #ccc);
}

```

### 循环

```CSS
/* 原生 CSS */

item-1 {
  background-image: url(xxx/1.png);
}

item-2 {
  background-image: url(xxx/2.png);
}

item-3 {
  background-image: url(xxx/3.png);
}

/* Sass 预处理器 */
@for $i from 1 to 4 {
  item-#{$i} {
    background-image: url(xxx/#{$i}.png);
  }
}
```
