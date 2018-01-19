# CSS 样式计算

### 浏览器的默认样式

### 样式的继承

### 样式的层叠
- 元素声明的样式的权重高于浏览器默认样式
- 浏览器默认样式的权重高于继承的样式

### 样式优先级

！important > style > id 选择器 > 类选择器 > 元素选择器 > *  > 浏览器默认 > 继承

###  CSS 重置

- 作用
  - 消除浏览器默认样式的影响

- CSS Reset 方案
  - 纠正
    - normalize.css
  - 清零
    - Eric Meyer's Reset CSS 2.0

- 推荐方案
  - normalize.css + 部分清零

### 浏览器兼容

一般来说兼容问题我们可以分两步走：第一步是确定浏览器是否支持，第二步是如果表现不一致，怎么去修复。

#### 浏览器是否支持

- [Can I Use](http://caniuse.com/#index)

#### 如何针对修复

- [考各个浏览器hack详细](http://browserhacks.com/)
