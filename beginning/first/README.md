# 最开始的部分
## 目录
### [C++概览](#1-c-%e6%a6%82%e8%a7%88)
### [Hello, world!](#2-hello-world)
### [基本命令行](#%e5%9f%ba%e6%9c%ac%e5%91%bd%e4%bb%a4%e8%a1%8c)
### [OJ](#oj)
***
## 1. C++ 概览
其实，C++的本质是两部分：C和[STL](https://www.baidu.com/s?ie=utf-8&wd=STL) 。

C++的后缀名们
```
.cpp
.cc
.cxx
.c++
.c
.txt
(无后缀名)
... ...
```

C++ 的代码结构
```cpp
#include <iostream>           
                              //上一行是头文件
#define PI 3.14               //宏定义
using namespace std;          //命名空间
int abs(int a){               //自定义函数
    return a>0?a:-a;
}
int main(){                   //主函数
    int n;
    cin>>n;
    cout<<abs(n*PI);
    return 0;
}
```

## 2. Hello, world!
### 标准代码1
```cpp
#include <iostream>
using namespace std;
int main(){
    cout<<"Hello, world!";//流输出
    return 0;
}
```
输出：

![image.png](https://i.loli.net/2020/02/10/3wUSxiKW7ltgAoL.png)

### 标准代码2
```cpp
#include <cstdio>
using namespace std;
int main(){
    printf("Hello, World!");//C的标准输出
    return 0;
}
```

输出：

![image.png](https://i.loli.net/2020/02/10/3wUSxiKW7ltgAoL.png)

### 不标准代码1
```cpp
#include<stdio.h>
using namespace std;
int main(){
    string s="Hello, world!";
    puts(s);//输出一行
    return 0;
}
```
输出：

![image.png](https://i.loli.net/2020/02/10/3wUSxiKW7ltgAoL.png)

### 不标准代码2
```cpp
#include<stdio.h>
using namespace std;
int main(){
    string s="Hello, world!";
    for(int i=0;i<s.length();i++){
        putchar(s[i]);//逐个输出字符
    }
    return 0;
}
```
输出：

![image.png](https://i.loli.net/2020/02/10/3wUSxiKW7ltgAoL.png)

