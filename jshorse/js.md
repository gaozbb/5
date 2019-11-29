### 运算

前置：先自加，后运算
后置：先运算，后自加

### 逻辑运算符

| 逻辑运算符 | 说明 | 案例 |
| - | - | - | - |
| && | 逻辑与 | true&&true |
| \|\| | 或 | true||true |
| ! | 非 | !true |

&&(逻辑与)
> 一侧为假即为假

||(逻辑或)
> 一侧为真即为真

!(逻辑非)

> 取反


### 构造函数、对象函数
语法规范
~~~javascript
var obj = {
	属性=值,
	属性=值
}
for (var k in obj){
	console.log(obj[k]);
}



var obj = new Object();
obj.属性=值；
obj.方法 = function(){
	console.log("方法值");
}





function 构造函数名(){
	this.属性 = 值;
	this.方法 = function(){}
}
new 构造函数名();

1.构造函数名字首字母大写
2.构造函数不需要return
3.调用构造函数必须用new
~~~


### JavaScript内置对象
JavaScript对象分为三种：自定义对象、内置对象、浏览器对象
内置对象指JS语言自带的对象
JavaScript提供多个内置对象：Math、Date、Array、String


Math概述
~~~
Math.PI									圆周率
Math.floor()						向下取整
Math.ceil()							  向上取整
Math.round()					  四舍五入
Math.abs()							 绝对值
Math.max()/Math.min()			求最大和最小值
~~~

Date
~~~javascript
var now = new Date();
console.log(now);

括号里面参数可以使('2019-5-1')

获取时间戳
var date = new Date();
console.log(date.valueOf());
console.log(date.getTime());
简单的写法，最常用的写法
var date1 = +new Date();
console.log(date1);
H5新增的 获取总毫秒
console.log(Date.now());


时间戳转换公式
d = parseInt(总秒数 /60 /60 /24);			//计算天数
h = parseInt(总秒数 /60 /60 %24);		  //计算小时
m = parseInt(总秒数 /60 %60);				 //计算分
s = parseInt(总秒数%60)；							//计算秒
~~~