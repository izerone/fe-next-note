# 元素层级 —— z-index

## 优先级顺序

- 默认 HTML 结构顺序
- position(非 static 值) 元素高于其他元素
- position(非 static 值) 元素之间先通过 z-index 值判断
- 如果 z-index 相同则按照 HTML结构顺序

## z-index 总结

- z-index 属性用于描述定位元素在垂直于页面方向上的排列顺序
- z-index 一般比较规则是值大在上，值相同则排后面的在上
- 元素在设置了某些属性的时候会创建层叠上下文，z-index 值比较大小只有在同一个层叠上下文才有效
