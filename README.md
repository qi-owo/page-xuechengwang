# 制作时的某些问题
#### 1.子盒子宽度可以大于父盒子

eg：本来 1 2 3盒子想在一排 三个盒子都有右外边距。但是3盒子加上外边距就超了。此时要给1 2 3的盒子**加上合适的宽度**（大于父盒子的）

#### 2.清除浮动的代码（写CSS开头）

```css
/*清除浮动的*/
.clearfix:before,
.clearfix:after{
    content: "";
    display: table;
}
.clearfix:after{
    clear: both;
}
.clearfix{
    *zoom: 1;
}
/*然后在对应元素的class加上clearfix*/
```

[网址入口](https://github.com/qi-owo/page-xuechengwang/blob/master/index.html)
