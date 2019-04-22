# JavaScript简介

## JS简介

* 简介:

  ​	 JavaScript一种在浏览器中解释运行的脚本语言，它的解释器被称为JavaScript引擎，为浏览器的一部分，是广泛用于 客户端的脚本语言，最早是在HTML网页上使用，用来给HTML（HTML5）网页增加动态功能。在1995年时，由Netscape公 司的Brendan Eich，在网景导航者浏览器上首次设计实现而成。因为Netscape与Sun合作，Netscape管理层希望它外观看起 来像Java，因此取名为JavaScript。 可以实现：用户交互（表单验证）、网页特效（漂浮的广告）、客户端的显示（页面内容，速度快）、网页游戏、 地图搜索、股市信息查询、web聊天。。。 

## JS与H5的关系

* H5狭义上，指HTML的第五个版本；广义上指web前端的所有技术，由于web前端是在H5出现后开始火爆起来，所以， 习惯上把web前端也叫H5。web前端开发也叫H5开发。

* H5包括 HTML，CSS，JavaScript，等一切前端技术。

  ![1553936676305](C:\Users\ADMINI~1\AppData\Local\Temp\1553936676305.png) 



## JS的组成：三部分组成

###ECMAScript

>​	一种由Ecma国际(前身为欧洲计算机制造商协会),定立ECMA-262标准化的脚本程序设计语言。规定了 JavaScript 脚本的核心语法，如 数据类型、关键字、保留字、运算符、对象和语句等。 

###BOM

> 	定义了 JavaScript 操作浏览器的接口，提供了访问某些功能（如浏览器窗口大小、版本信息、浏览历史记录等） 的途径以及操作方法。 

###DOM

> 	定义了 JavaScript 操作 HTML 文档的接口，提供了访问 HTML 文档（如body、form、div、textarea等）的途径以及 操作方法。 

# JS基础

## JS在HTML中如何使用

```
<body>
	<script type="text/javascript">
 	//第一句javascript代码：
	 alert(“我用来弹出消息框！”) ;
 	//第二句：
	 document.write(“我会把内容显示在页面上，能够输出任何HTML代码！”);
	</script>
</body>
</html>
```

**tip:JS大小写敏感**

## script 标签的引入位置

### 1、script标签写在HTML中

​	script标签和属性可以写在HTML中任意位置，可以写多个。一般写在会<head>中。

```html
<script type="text/javascript" >
 	JS代码写在这里。
</script>
```

### 2、使用script标签引入外部javaScript文件 

```html
<script type="text/javascript" src="demo1.js" ></script>
```

**tip**：

>* 引入文件不可以使用单标签  
>
>  ```html
>  eg: <script type="text/javascript" src="demo1.js“/ >
>       //以上缺少结尾的</script>是不正确的
>  ```
>
>* 引入文件不可以在标签中写代码
>
>  ```html
>  eg: <script src="demo1.js">
>      	alert('xxxx') //不正确的
>  	</script>;
>  ```

## 注释

* 单行注释 //
*  多行注释 /* */ 
* 文档注释 /** */ 

## 运行顺序

> Javascript和HTML代码在同一个文件中写，它们的执行顺序是从上朝下，谁在前先执行谁。 

## JS变量

**变量用来在计算机中存储和表示数据。 **

### 变量定义（声明）

```html
var age; //var是关键字，age是变量名
```

### 赋值

```html
age=20; //20是数据 "="是赋值
```

### 定义的同时赋值

```html
var age=20; //定义一个变量
var myname="刘德华",age=20,weight=140; //可以一次性定义多个变量
```

# JS的数据类型

## Undefined类型

* Undefined类型只有一个值undefined，它是变量未被赋值时的值。

## Null类型

* Null类型也只有一个值null，Null类型的语义是“一个空的对象引用”，注意和空字符串区别开。 

## Boolean类型

* 布尔有两种取值true和false，表示真或假。非0代表真，0代表假 。

## String类型

* 又叫字符串类型，用双（单）引号括起来的一串字符。 

## Number类型

* 包含整数数± 9007199254740992 和浮点数±1.7976931348623157 × 10的308次方。 

## Object类型

* JavaScript中最为复杂的类型就是Object，它是一系列属性的无序集合。 

>使用typeof关键字查看变量类型 : var age=20; alert(typeof age) 

# JS变量的命名规则和关键字 

## 变量命名规则

* 不以数字开头，数字、字母以及下划线均可用来组成变量名，但不能使用关键字及保留字。 
* 尽量使用有意义的单词作为变量名，也尽量不要与HTML、CSS中的关键字冲突。有驼峰命名法和西班牙 命名法（以小写字母b,f,i,s开头表示类型，后接大写开头的有意义的单词）等等 

## 关键字及保留字 

![1554079408609](C:\Users\ADMINI~1\AppData\Local\Temp\1554079408609.png)

![1554079429567](C:\Users\ADMINI~1\AppData\Local\Temp\1554079429567.png)

# JS运算符

## 算数运算符

* 由算术运算符组成的式子叫算术表达式，结果是数值类型 

![1554079531834](C:\Users\ADMINI~1\AppData\Local\Temp\1554079531834.png)

## 关系运算符

* 由关系运算符组成的式子叫关系表达式，关系表达式返回的结果是布尔类型 

![1554079639643](C:\Users\ADMINI~1\AppData\Local\Temp\1554079639643.png)

## 逻辑运算符

![1554165425245](C:\Users\ADMINI~1\AppData\Local\Temp\1554165425245.png)

* 逻辑短路

  >​	当逻辑运算符的前面的变量或者表达式（式子）能够决定整个表达式的结果时，则逻辑运算符后面的变量或者 表达式（式子），不再进行运算。 

  

# JS变量类型的转换

## JS是弱类型语言

* 变量声明是不需要指明类型
  * eg： var age;   age=20; 
* 变量的类型在使用中可变
  * eg：age=“年龄:”+age; 

**Tip：注：JS变量的类型由其存放的数据类型确定** 

## JS的类型转换

### 隐式（自动）转换

* 当运算符两边的操作数（表达式、变量、值）的数据类型不一致时，浏览器首先会把类型转换成一样的

  **字符串与数字之间进行加法运算，会把数字转换成字符串**

  ```html
  var age=25;
  var str="我今年"+age
  alert(str);//输出：我今年25
  ```

  

  



