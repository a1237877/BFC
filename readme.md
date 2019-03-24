# bfc的概念
Block Formatting Context  块级格式化上下文
#bfc 功能
1.使 BFC 内部浮动元素不会到处乱跑；
2。和浮动元素产生边界。

#BFC的渲染规则
1.bfc在页面上是一个独立的容器，最显著的效果就是建立一个隔绝的空间，外面的元素不会影响bfc里面的元素，反之，里面的元素也不会影响外面的元素，当加上BFC效果后，该容器就是一个独立的空间，但不是脱离文档流。
2.bfc的区域不会浮动元素的box重叠
3.垂直方向的外边距会发生边距折叠（包括父子元素，兄弟元素）。水平方向的外边距不存在边距折叠
margin-bottom :30px;   margin-top:20px; 则会取30px为外边距

#创建条件
1.overflow 的值不为 visible时
2.float的值不为none
3.行内快 inline-block
4.表格单元display：table 
5.绝对定位（absolute,fixed)