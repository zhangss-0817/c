#  1. Hello World

编写C语言代码：hello.c
```c
#include <stdio.h>

int main()
{
	//这是第一个C语言代码
	printf("hello world\n");

	return 0;
}
```
C语言的源代码文件是一个普通的文本文件，<font color=red>但扩展名必须是.c</font>。
## 代码分析
**1) include头文件包含**
 - #include的意思是头文件包含，#include <stdio.h>代表包含stdio.h这个头文件 
 - 使用C语言库函数需要提前包含库函数对应的头文件，如这里使用了printf()函数，需要包含stdio.h头文件
 
**#include< > 与 #include " "的区别：**
- < > 表示系统直接按系统指定的目录检索
- " " 表示系统先在 " " 指定的路径(没写路径代表当前路径)查找头文件，如果找不到，再按系统指定的目录检索

**2) main函数**
- 一个完整的C语言程序，是由一个、且只能有一个main()函数(又称主函数，必须有)和若干个其他函数结合而成（可选）。
- main函数是C语言程序的入口，程序是从main函数开始执行。

**3) { } 括号，程序体和代码块**
- { }叫代码块，一个代码块内部可以有一条或者多条语句
- C语言每句可执行代码都是";"分号结尾
- 所有的#开头的行，都代表预编译指令，预编译指令行结尾是没有分号的
- 所有的可执行语句必须是在代码块里面

**4) 注释**
- //叫行注释，注释的内容编译器是忽略的，注释主要的作用是在代码中加一些说明和解释，这样有利于代码的阅读
- /**/叫块注释
- 块注释是C语言标准的注释方法
- 行注释是从C++语言借鉴过来的

**5) printf函数**
- printf是C语言库函数，功能是向标准输出设备输出一个字符串
- printf(“hello world\n”)；//\n的意思是回车换行

**6) return语句**
- return代表函数执行完毕，返回return代表函数的终止
- 如果main定义的时候前面是int，那么return后面就需要写一个整数；如果main定义的时候前面是void，那么return后面什么也不需要写
- 在main函数中return 0代表程序执行成功，return -1代表程序执行失败
- int main()和void main()在C语言中是一样的，但C++只接受int main这种定义方式
# 2. 数据类型
**1. 关键字**

![alt](/picture/1.png "Magic")

<img src="/picture/1.png" width = "100" height = "100" div align=right />