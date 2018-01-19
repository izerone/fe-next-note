# CSS 颜色的使用

## 取色工具
- [马克鳗](http://www.getmarkman.com/)
- [ColorZilla](http://www.colorzilla.com/)

## 如何定义颜色

### 颜色关键词

- [颜色名](http://www.w3school.com.cn/cssref/css_colornames.asp)
- 新的颜色关键字
  - transparent : 透明
  - currentColor
    - 使用该元素 color 的计算值。如果该元素设置了 color 颜色值，则使用该 color；如果该元素没有设置 color，则继承父级元素的 color。

### rgb
- 表示使用红-绿-蓝模式来定义颜色
- rgb 函数表示为：rgb(red, green, blue)。每个参数 (red、green 以及 blue) 定义颜色的强度，可以是介于 0 与 255 之间的整数，或者是百分比值（从 0% 到 100%）。

### rgba
在 rgb 的基础上，还可以添加一个 alpha 透明度表示半透明值，构成了我 rgba，其函数表示为：rgb(red, green, blue, alpha)，其中 alpha 参数是介于 0.0（完全透明）与 1.0（完全不透明）的数字。


### 十六进制
- “#” 后跟6位十六进制字符（0-9, A-F）
- “#” 后跟3位十六进制字符（0-9, A-F）

### hsl
- 可以通过 hue（色调）、saturation（饱和度）、lightness（亮度）模式定义颜色，其语法为：hsl(hue, saturation, lightness)
  - Hue 是色盘上的度数（从 0 到 360） - 0 (或 360) 是红色，120 是绿色，240 是蓝色。Saturation 是百分比值；0% 意味着灰色，而 100% 是全彩。Lightness 同样是百分比值；0% 是黑色，100% 是白色。

### hsla
- 语法为hsla(hue, saturation, lightness, alpha)，alpha 取值同样为介于0.0到1.0的数字

#### 参考链接

- [css color | MDN](https://developer.mozilla.org/zh-CN/docs/Web/CSS/color_value)
- [CSS 合法值](http://www.w3school.com.cn/cssref/css_colors_legal.asp)
