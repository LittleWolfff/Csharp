# 前言：快捷的学习方法
1、理解语法构成和含义
2、必要的死记硬背
3、多敲多练（这个是重点）
# 一、程序文件的基础结构
一个代码块可以简单分成三个部分
​​​​​​​​​​![alt text](image.png)
***
看下图，不同的颜色代表不同的部分，还可以发现，这三者首字母都是大写的，如果是变量名称，首字母就不大写了，可以有这么些印象
![alt text](image-1.png)
写代码常常需要引用命名空间，例如，只有引用了System这个命名空间，Console才能在别的命名空间Lesson1里使用，也就是说，Console其实就是System工具包里的一个工具
***
# 二、控制台输入输出语句
## 1、学习
（开头的四段代码是为了方便复习，请先看后面的内容来理解）
```csharp
Console WriteLine("...");
Console Write("...");
Console ReadLine();
Console ReadKey();
```
## 2、理解
![alt text](image-2.png)
其实WriteLine可以理解为占用了一整行，无论你输入什么，都会用看不见的空格把那一整行填满
另外，引号内的内容对符号没有特殊要求，也就是说里面输入中文的标点符号也没有问题
![alt text](image-3.png)
![alt text](image-4.png)
![alt text](image-5.png)
## 3、习题
![alt text](image-6.png)
![alt text](image-7.png)
![alt text](image-8.png)
***
# 三、变量
分类：整型（分有无符号），浮点型，布尔型bool，字符型char，字符串型string
## 1、折叠代码
![alt text](image-9.png)
在折叠的代码里还可以继续折叠代码
![alt text](image-10.png)
本质是 编辑器提供给我们的 预处理指令
它只会在编辑时有用 发布了代码 或执行代码 它会被自动删除
## 2、变量类型
![alt text](image-11.png)
![alt text](image-12.png)
共有14种变量类型，都尽量记一记
### 有符号的整型变量
变量的使用不能无中生有，必须先声明
![alt text](image-13.png)
![alt text](image-14.png)
“+”只是把两个东西连在一起，不会在中间产生空格
![alt text](image-15.png)
![alt text](image-16.png)
### 无符号的整型变量
![alt text](image-17.png)
### 浮点数（小数）
![alt text](image-18.png)
且这个f是有小数的时候才加，如果没有小数，就可以直接float f=80;不用加f
![alt text](image-19.png)
![alt text](image-20.png)
![alt text](image-21.png)
![alt text](image-22.png)
![alt text](image-23.png)
### 特殊类型
![alt text](image-24.png)
![alt text](image-25.png)
char类型是16位无符号整数
![alt text](image-26.png)
## 3、为什么有那么多不同类型的变量
![alt text](image-27.png)
![alt text](image-28.png)
## 4、变量要先初始化
![alt text](image-29.png)
## 5、练习
![alt text](image-30.png)
![alt text](image-31.png)
***
# 四、变量的本质
## 1、变量的存储空间（内存中）（字节数要记，会卡面试题）
![alt text](image-32.png)
![alt text](image-33.png)
sizeof()的结果是int类型的
### 有符号
![alt text](image-34.png)
![alt text](image-35.png)
### 无符号
![alt text](image-36.png)
![alt text](image-37.png)
### 浮点数
![alt text](image-38.png)
![alt text](image-39.png)
### 特殊类型
![alt text](image-40.png)
![alt text](image-41.png)
## 2、变量的本质是什么
![alt text](image-42.png)
## 3、二进制和十进制的相互转化
### 十进制转二进制
![alt text](image-43.png)
![alt text](image-44.png)
补充一下：所得余数 倒序数出来后，前面还要加最后的一个商（其实就是图中计算后，从下往上看 右边的数）
### 二进制转十进制
![alt text](image-45.png)
注意从右往左看的第一个数在第0位，如果是二进制的1，则转换成2的0次方
### 字节的存储
![alt text](image-46.png)
![alt text](image-47.png)
![alt text](image-48.png)
![alt text](image-49.png)
### 有无符号的原因
![alt text](image-50.png)
![alt text](image-51.png)
现在只需理解整数的二进制就行了，理解了它，就能理解为什么 不同的存储空间就意味着它的存储范围不一样
## 4、练习
![alt text](image-52.png)
![alt text](image-53.png)
![alt text](image-54.png)
可用电脑自带计算机验证结果
![alt text](image-55.png)
![alt text](image-56.png)
![alt text](image-57.png)
![alt text](image-58.png)
calculate就是计算的英文
***
# 五、变量的命名规则
## 1、必须遵守的规则
![alt text](image-59.png)
“.”和“ ”都算是特殊符号（点和空格）
## 2、常用命名规范
![alt text](image-60.png)
***
# 六、常量
## 1、基础语法
![alt text](image-61.png)
## 2、常量的特点
![alt text](image-62.png)
![alt text](image-63.png)
![alt text](image-64.png)
![alt text](image-65.png)
![alt text](image-66.png)
***
# 七、转义字符
## 1、什么是转义字符
![alt text](image-67.png)
![alt text](image-68.png)
注意对角线的方向，是向右倾斜的
![alt text](image-69.png)
## 2、常用的转义字符（必记）
![alt text](image-70.png)
![alt text](image-71.png)
## 3、不常用的转义字符（了解）
![alt text](image-72.png)
![alt text](image-73.png)
alarm就是警报的意思，所以是\a
## 4、如何禁用转义字符
![alt text](image-74.png)
当我们想要在字符串中打印斜杠时，会因为斜杆的转义作用而报错
![alt text](image-75.png)
这个时候可以双斜杠，第一条斜杠负责转义，第二条斜杠负责打印出来
不过，我们也可以直接禁用转义字符
![alt text](image-76.png)
![alt text](image-77.png)
## 5、练习
![alt text](image-78.png)
![alt text](image-79.png)
***
# 附快捷键
按住Ctrl、K+C——注释

按住Ctrl、K+U——取消注释

Ctrl+F5——运行代码








































