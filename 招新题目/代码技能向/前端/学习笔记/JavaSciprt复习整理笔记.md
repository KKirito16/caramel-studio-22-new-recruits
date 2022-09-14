# JavaSciprt

## 1.引入JavaSciprt

### 1.内部标签

```javascript
<script>
    //......
</script>
```

### 2.外部引入

在h5文件的<head>标签内

```
<script src="abc.js"><script>
```

## 2.基本语法

1.申明变量

```
var 变量名=xxx
```

2.条件语句

```
if（条件）{

}if else（条件）{

}else（条件）{

}
```

3.程序员调试用，显示在控制台

```
consloe.log(xxx)
```

4.打印

```
document.write("xxx");
```

5.弹框弹出信息

```
alert("xxx")；
```

## 3.数据类型

#### 变量：

var

```
var a = 1；
```



#### number：

js不区分小数和整数

```js
123 //整数123
123.1 //浮点数123.1
1.123e3 //科学计数法
-99 //复数
NaN //not a number
Infinity //无限大
```

浮点数问题，尽量避免使用浮点数进行运算，因为存在精度损失问题。

#### 字符串''、"":

'abc'、"abc"

#### 布尔值：

true、flase

#### 逻辑运算：

```
&& 与

|| 或

！ 非
```

#### 比较运算符：

```
=
== 等于（类型不一样，值也一样，也会判定为true）
===  绝对等于（当且仅当类型一样，值一样，结果为ture）
```

所以最好用===来比较，而不用==

- 须知：NaN！=NaN，这个与所有的数值都不相等，包括自己
- 只能用isNaN(NaN)来判断这个数是否是NaN

#### null和undefined

- null 空
- undefined 未定义

#### 数组

C、Java数组里元素必须是相同类型的对象，JS不需要这样，这是它的不严谨性

取数组下标，如果越界了，就会报错undefined

#### 对象

对象是大括号，数组是中括号

每个属性之间使用逗号隔开，最后一个不需要添加

```
//Person person = new Person（1，2，3,4,5）；
var person={
    name：“qinjiang”，
    age：3，
    tags：['js','java','web','...']
}
```

### 4.严格审查模式：

'use strict';严格审查模式，预防JavaScript的随意性导致产生的一些问题（需要IDEA设置支持ES6语法

ES6中 用let定义变量，局部变量都建议用let定义
