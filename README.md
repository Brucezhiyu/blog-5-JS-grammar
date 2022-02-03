### JavaScript语法


1. 什么是表达式和语句
**表达式**
是由运算符和运算对象组成的,单独的一个运算对象(常量/变量)也可以叫做表达式，这是最简单的表达式.
eg:
1+2表达式的值为3
add(1,2)表达式的值为函数值的返回值
console.log表达式的值为函数本身
console.log(3)的值为 undefined
**语句**
var a=1 是一个语句

tips
两者的区别:
表达式一般都有值，语句可能有也可能没有，语句一般会改变环境(声明，赋值)(以上并不是绝对的)
不可以写错大小写.
大部分空格没有实际意义,但是return后不能加回车。
2. 标识符的规则 
规则:第一个字符,可以是Unicode字母或$或_或中文。后面的字符,除了上面所说，还可以有数字。
```JavaScript
var $9= 10
```

3. if else 语句 
语法:
```JavaScript
if(表达式){
    语句1
}else{语句2}
```
**问号冒号表达式(用来代替if...else)**
语法:
```JavaScript
表达式1?表达式2:表达式3
```
```JavaScript
function max(a,b){
    return a>b ? a:b
}//如果a>b结果等于a，否则为b
```
**&&短路逻辑**
A&&B&&C&&D 取第一个假值或D，并不取true/false
```JavaScript
window.f1&&console.log('f1存在')
//如果window.f1存在，则打印'f1存在'
```
**||短路逻辑**
A||B||C||D  取第一个真值或D，并不取true/false
```JavaScript
a= a || 100
//如果a=a成立则a=a，反之则a=100
```
4. while for 语句
while语句语法:
```JavaScript
while(表达式){语句}
```
for语句语法:
```JavaScript
for(语句1;表达式2;语句3){
    循环体
}
```

5. break continue  
break:退出当前循环
continue:退出所有循环

6. label
语法:
```JavaScript
foo:{
    console.log(1);
    break foo;
    console.log('什么都不输出')
}//foo是一个标签，这个语句是{...}
```
