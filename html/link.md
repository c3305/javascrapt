javascrapt

1.常量与变量
2.数据类型
3.运算符
4.表达式与语句
5.转义字符
6.注释

一:变量
## 1.申明变量  
var apple = 10;
## 2.申明多个变量
var temp, apple2 = "青苹果", apple1 = "红苹果";  变量可以使用 , 号隔开  从而定义多个变量名和值

## 3.转化变量值
// 变量名 = 值  赋值（apple) 给temp 临时变量
apple1 = apple2;
apple2 = temp;
console.log(apple1);
console.log(apple2);
## 小知识
<!-- // 变量是临时调用内存空间存储 //-->
二:数据类型
## 数据类型
(1).js是动态语言  变量的数据类型是可以变换的
 javascript 数据类型是自由的 
如  var x = 10; 
    x = "pink"  这里是把数字类型转化或者覆盖变成字符串型数据

(2).简单数据类型：
    1.number: 数字类型数据  包括整数型和浮点型（小数点）
    2.Boolean:布尔型类型  就是对与错 true和false
    3.string:字符串类型数据  就是""  字符串带引号
    4.Undefined:声明变量  没有给值 就是Undefined
    5.null: (空) 申明变量但是a的值为空
        1.number:
            1.  
                所有的数字都叫数字类型
                八进制加上0表示八进制 0 ~ 7
                十六进制  0 ~ 9,  a ~f前面加上0x
                最大值console.log(number.max_vulue);表示
                最小值console.log(number.min_vulue);表示
                无穷大console.log(number.min_vulue * 2);
                无穷小console.log(-number.min_vulue * 2);
                Nan表示非数字类型数据
            2.isNan()
                用来判断是否是数字类型  返回true或者false
                x 是数字返回false 不是就是false
        2.string:
            1.
                字符串可以是引用引号里任意文本，语法是"" ''
                推荐js里面使用 单引号
                js里面用引号得嵌套“ ‘ ’ ”
            2.
                转化符 \n换行;  \\ 显示\; \' 单引号; \' 双引号; \t tab缩进; \b 空格;
            3.
                length  检测字符串的长度
                字符串的加上 alert（ "大帅哥" + " 有钱 " ）
                            alert("12"+12)  1212
                            数值相加,字符相连
            4.                
                字符串拼接加强
                var age = 10;
                console.log('大帅哥' + age);
                console.log('大帅哥' + age + '有钱');

                交互：
                    var age = prompt('请输入您的年纪');
                    var str = "您今年已经 + age + 岁了";
                    alert(str);
        3.布尔型
            flase  (错)
            true    （对）
            用于结构的条件判断
        4.undefined
            未定义的数据类型
            var cc = undefined;
            console.log(c)
        5.null
            空值
(3)获取变量的数据类型
        var num = 10;
        console.log(typeof num);  查看数据类型输出为数字类型数据
        var str = 'cxl';
        console.log(typeof str); 字符串类型
            小案例
                var age = prompt('请输入您的年龄');
                console.log(age);      
                console.log(typeof age);  字符串类型数据
        字面量
            字面量表示如何表达这个值
                在控制台
                    蓝色的数据是数字类型数据（0，1，2）
                    黑色的数据是字符串类型数据（'名字')
                    灰色的数据是undefined或null数据 （true, false)
(4)数据类型转化
        把一种数据类型转化另外一种
            1.转化字符串类型
                toSting()       var num = 10; var str = num.toSting();  console.log(str);
                String(变量)强制转换    console.log(String(num));
            2.转化数字类型
            3.转化布尔类型         