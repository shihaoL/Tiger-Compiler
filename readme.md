Tiger Compiler
====

## 构造编译器环境
Linux 	4.10
GCC 	5.4
Bison 	3.0
Flex 	2.6
Make 	4.1

## 文件清单
- `LJZ_TC/`
  - `include/`
    - balabala
  - `src/`
    - `tiger.lex` 
    - `tiger.y` 
  - `lib/`
    - `libtiger.c` , `libtiger.s` TIGER外部函数
    - `tigerMain.c`, `tigerMain.s` TIGER程序编译结果示例
  - `makefile`
  - `customtests/` 测试用例
  - `testcases/` 书本测试用例
  - `parsetest.tig`  语法测试TIGER程序

## 使用指南
- `make all` 

  生成可执行文件`parsetest.out`，并测试TIGER程序语法`parsetest.tig`

  *注意: 第一次生成时显示`没有那个文件或目录`为正常现象*

- `make clean`

  清除依赖文件、目标文件、可执行文件


## 运行时环境

OS: Debian-MIPS

  `ssh root@106.14.177.227 -p 10022`

  使用sftp交换文件

  ## 栈帧部分的寄存器相关函数可能有bug，还未调试
  ## 寄存器分配可以考虑线性扫描分配（图着色可能比较复杂）


