# 单位

## 绝对单位
### 像素 px
  - px 是 pixels（像素）的缩写，是一种绝对单位

  ```CSS
  .box {
    width: 200px;
    font-size: 16px;
  }

  ```

#### in
#### cm
#### pt
#### mm

### 相对单位
#### %
  - 如果对 html 元素设置 font-size 为百分比值，则是以浏览器默认的字体大小16px为参照计算的（所有浏览器的默认字体大小都为 16px），如62.5%即等于10px（62.5% * 16px = 10px）

#### em
em 也是一种相对单位,不过其参照值并不是固定不变的，而是不同的属性有不同的参照值。

- font-size
  - em 的计算方式是相对于父元素的字体大小，1em 等于父元素设置的字体大小。如果父元素没有设置字体大小，则继续往父级元素查找，直到有设置大小的，如果都没有设置大小，则使用浏览器默认的字体大小。
- 其他属性（border, width, height, padding, margin, line-height）
  - 使用em单位的计算方式是参照该元素的 font-size，1em 等于该元素设置的字体大小。同理如果该元素没有设置，则一直向父级元素查找，直到找到，如果都没有设置大小，则使用浏览器默认的字体大小。

总之em的计算单位相对来说比较复杂，现在已经不建议使用，如果你要兼容的浏览器是现代浏览器的话，那么可以使用下面要介绍的 rem 单位。

#### rem

rem 也是一种相对单位，rem 是相对于根元素 html 的 font-size 来计算的，所以其参照物是固定的。由于是新技术，不支持IE8以下（包括IE8）,不过幸喜的是移动端可以放心使用。

#### vw, vh, vmin, vmax

 v 系单位，也是相对单位，是基于视窗大小（浏览器用来显示内容的区域大小）来计算的。

- vw：基于视窗的宽度计算，1vw 等于视窗宽度的百分之一
- vh：基于视窗的高度计算，1vh 等于视窗高度的百分之一
- vmin：基于vw和vh中的最小值来计算，1vmin 等于最小值的百分之一
- vmax：基于vw和vh中的最大值来计算，1vmax 等于最大值的百分之一


## 单位运算

使用 calc 来进行单位运算，单位运算时可以使用各种单位进行加减乘除运算。

```CSS
.box {
 height: calc(50vh - 20px); /* 50% 的视窗高度减掉20px */
 width: calc(100% / 3);  /* 三分之一的父容器宽度 */
 background: red;
}

```

calc 也存在兼容问题，详细介绍可参考：[calc | MDN](https://developer.mozilla.org/zh-CN/docs/Web/CSS/calc)


**注：chrome 浏览器最小的字体为 12px，如果设置 10px 也会渲染成 12px 。**
