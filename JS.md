JS 数组可以设置  

    arr.length = 0 

清空数组。


通过（唯一方法） 

    Object.prototype.toString.call();
  
查看一个值得内部标签属性[[class]]

方法

    .toString()
    
不能访问内部[[class]],因为基本类型构造器中的 toString 被重写了。

例如

    console.log(Object.prototype.toString.call(666));// [object Number] 
    console.log(Object.prototype.toString.call("hello world"));//[object String]
    console.log(Object.prototype.toString.call(null));//[object Null]
    console.log(Object.prototype.toString.call(undefined));//[object Undefined]
    console.log(Object.prototype.toString.call([0,1,2]));//[object Array]
    console.log(Object.prototype.toString.call({a:"hello world"}));//[object Object]
    console.log(Object.prototype.toString.call(function(){return "hello world"}));//[object Function]
    console.log(Object.prototype.toString.call(new Error()));//[object Error]
    console.log(Object.prototype.toString.call(/ab+c/));//[object RegExp]
    
 <br><br>
 
 0x   16进制
 0o   8进制
 0b   2进制 
 <br><br>
 
 <b>强制类型转换测试</b>
    
