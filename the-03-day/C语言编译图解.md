

一、C 语言编译过程  
1. 编写 C 语言源代码即 hello.c 程序  
2. 将源代码进行预处理：宏定义展开、头文件展开、条件编译、删除注释  
   命令为：`gcc -E hello.c -o hello.i`  
3. 编译程序：检查语法，将 C 语言转换成汇编语言  
   命令为：`gcc -S hello.i -o hello.s`  
4. 汇编：将汇编语言转换成机器语言  
   命令为： `gcc -c hello.s -o hello.o`  
5. 链接：将 C 语言执行需要的链接库进行链接  
   命令为：`gcc hello.o -o hello.exe`  
6. 一步命令为： gcc -o hello.exe hello1.c hello2.c  

![C语言编译过程](https://img-blog.csdnimg.cn/20200625103740468.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3UwMTM2NDc3NTk=,size_16,color_FFFFFF,t_70)  

二、程序执行过程  
1. 源代码从硬盘加载到内存的代码区，并与数据区的数据进入 CPU  
2. CPU 运算区进行计算，控制器执行命令  
3. CPU 通过总线将处理后的数据从到内存的堆区或栈区  
4. 数据从内存送往硬盘等外部存储设备进行保存。  

i[C语言程序执行过程](https://img-blog.csdnimg.cn/20200626170601742.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3UwMTM2NDc3NTk=,size_16,color_FFFFFF,t_70)  


