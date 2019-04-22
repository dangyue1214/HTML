# 属性

## 背景图片

1.background-color  背景颜色 

2.background-repeat  背景重复：有三个属性值

>a. repeat-x  横向重复 ：可用于渐变色图片插图横向平铺图片；
>
> b. repeat-y 纵向重复 ：可用于渐变色图片插图纵向平铺图片；
>
> c. no-repeat 不重复。

3.background-image  背景图片

4.background-position：向右偏移量px  向下偏移量px，属性值也可以为:top  left /center center/right bottom

>可用在雪碧图中应用
>
>tip:**雪碧图又称css精灵：作用是可以减少对服务器的请求，通过background-position位移显示出布局的位置**

5.background-attachment:fixed  背景固定

**tip：简写：background：url() no-repeat center top,能够使用简写使用简写**

## 文本属性

1.direction  设置文本方向

>属性值：ltr  从左向右        rtl   从右向左

2.letter-spacing  设置字符间距 ，可以为负值

3.text-align 设置文本水平对齐方式

>属性值：left（左对齐）、center（居中）、right（右对齐），justify（两边对齐）
>
>tip：**此属性对图片也是有效果的，但是图片不能是块级元素，不能产生浮动。**

4.text-decoration 给文本添加修饰

>属性值：none 取消文本的默认样式         underline  给文本添加一条下划线
>
>​             overline 给文本添加一条上划线     line-through 穿过文本的一条线

5.text-indent  缩进元素文本的首行

>px是具体长度 ， 百分比是基于父元素宽度的百分比

6.text-transform 控制元素中的字母，设置字母的样式

>capitalize  每个字母的首字母大写
>
>uppercase  每个字母都大写
>
>lowercase  每个字母都小写

7.word-spacing 控制英文单词词距

8.vertical-align 垂直对齐方式（基线为准）

> 属性值 :top（上）、middle（中）、bottom（下）、baseline（默认状态）
>
> tip:**基线的产生来自内容，如果没有内容，则元素自动以底部为基线对齐**

9.line-height  行高

>当行高等于容器（父元素）的高时，可以实现文本垂直居中（**只适用于单行文本**）
>
>当单行文本的行高小于容器的高时，可实现单行文本在容器中垂直中齐以上；
>
>当单行文本的行高大于容器的高时，可实现单行文本在容器中垂直中齐以下；
>
>多行文本垂直居中：
>
>a.padding-top=(高度-总行高)/2；b.盒子的高度-padding-top=盒子的新高度

10.layout-flow 控制文本流

>属性值：horizontal（自左向右）、vertical-ideographic（自上而下）
>
>tip：**专门用于IE的一个属性**

## 字体属性

1.font-size 字体大小

2.color  字体颜色

>三种表示颜色属性值：英文   十六进制   rgb

3.font-family  字体样式/字体族科

>tip：**若要同时设置字体，英文字体必须在中文字体的前面**

4.font-weight  字体粗细

>属性值：bold(字体变粗)、bolder(更粗)、normal（正常）
>
>也可以设置值：100-900

5.font-style 字体倾斜

>属性值：italic(斜体字)、oblique(让现有字体发生倾斜)、normal 字体倾斜





























  



