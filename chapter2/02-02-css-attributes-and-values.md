# 属性和值

## 属性

### 属性参考

- [CSS 参考 - CSS | MDN](https://developer.mozilla.org/zh-CN/docs/Web/CSS/Reference)
- [CSS 参考手册](http://www.w3school.com.cn/cssref/)
- [如何阅读 CSS 属性值定义语法](https://developer.mozilla.org/zh-CN/docs/Web/CSS/Value_definition_syntax)

### 字体相关属性

- `font-family`: 定义文本的字体，如:`font-family: arial;`
- `font-size`: 字体尺寸, 如 `font-size: 18px;`
- `font-style` ：字体样式，如：`font-style: italic;`
- `font-weight`：字体的粗细，如：`font-weight: bold;`

### 文本相关属性

- `color`：定义文字颜色，如：`color: red;`
- `line-height`：设置行高，如：`line-height: 1.5;`
- `text-align`：文本的水平对齐方式，如：`text-aligin: center;`
- `text-decoration`：文本的装饰效果，如：`text-decoration: underline;`
- `text-indent`：首行的缩进，如：`text-indent: 2em;`
- `text-shadow`：文本的阴影效果，如：`text-shadow: 0 0 5px #ff0000;`

### 列表属性

- `list-style`：在一个声明中设置所有的列表属性
- `list-style-image`：将图象设置为列表项标记
- `list-style-position`：设置列表项标记的放置位置
- `list-style-type`：设置列表项标记的类型

  ```CSS
  ul, ol {
      /* 第一个none表示image，outside表示position，第二个none表示type */  
      list-style: none outside none;
  }

  ```

### 表格属性

- `border-collapse`：是否合并表格边框
- `border-spacing`：相邻单元格边框之间的距离
- `table-layout`：设置表格的布局算法

  ```CSS
  /* 三个属性，只作用于 table 元素，其余元素都没有作用 */
  table {
      border-collapse:collapse;
      border-spacing: 0;
      table-layout: fixed;
  }
  ```

### 盒子相关

#### 盒子大小

主要是宽高及最小和最大宽高。

- width
- min-width
- max-width
- height
- min-height
- max-height
- box-sizing

#### 盒子边框

- border：简写模式，四边边框
- border-width：边框宽度
- border-style：边框样式，常用的为solid和dashed
- border-color：边框颜色
- border-top：上边框
- border-right：右边框
- border-bottom：下边框
- border-left：左边框

#### 盒子内外边距

- margin
- margin-top
- margin-right
- margin-bottom
- margin-left
- padding
- padding-top
- padding-right
- padding-bottom
- padding-left

#### 盒子背景

设置背景图片，背景颜色，图片位置及是否平铺等，一般也采用简写形式。

- background：总的简写形式，包括了下面各个单条属性
- background-color：背景色
- background-image：背景图片
- background-position：背景图片起始位置
- background-repeat：背景图片平铺方式
- background-size：背景图片大小
- background-clip：背景图片绘制区域
- background-origin：背景图片的定位区域

#### 盒子显示隐藏

- overflow：指定当内容溢出其块级容器时,是否剪辑内容，渲染滚动条或显示内容
- visibility：是否可见

#### 盒子其他

- border-radius：圆角
- box-shadow：阴影

### 空间位置相关

- display
- float
- clear
- position
- top
- right
- bottom
- left
- transform
- z-index
- opacity

### 动画相关

- transition
- animation

## 属性值

- 关键词
- 数字
- 数值 + 单位
- 多个值
- 颜色值
