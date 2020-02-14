# 配置Marlin

Marlin is a huge C++ program composed of many files, but here we'll only be talking about the two files that contain all of Marlin's compile-time configuration options:

- `Configuration.h` contains the core settings for the hardware, language and controller selection, and settings for the most common features and components.
- `Configuration_adv.h` serves up more detailed customization options, add-ons, experimental features, and other esoterica.

These two files contain all of Marlin's build-time configuration options. Simply edit or replace these files before building and uploading Marlin to the board. A variety of pre-built configurations are included in the `config/examples` folder to get you started.

To use configurations from an earlier version of Marlin, try dropping them into the newer Marlin and building. As part of the build process, the `SanityCheck.h` will print helpful error messages explaining what needs to be changed.

Also a tool like [Winmerge](http://winmerge.org/) is usefull to compare the old file to the new one and you can copy over the settings.

## Compiler Directives

![image](https://raw.githubusercontent.com/Apex-yuan/Documents/master/source/Marlin/images/1565056497193.png)

---

sdf|sdfsd|

- [ ] 

sd |dfds|sdfs



项目     | Value 

-------- | ----- 

电脑  | $1600 

手机  | $12 

导管  | $1

| 名称          | 作用                                                    |
| ------------- | ------------------------------------------------------- |
| EQU           | 给数字常量取一个符号名                                  |
| AREA          | 汇编一个新的代码段或数据段                              |
| SPACE         | 分配内存空间                                            |
| PRESERVE8     | 当前文件堆栈需要按照8字节对齐                           |
| IMPORT        | 声明标号来自外部文件                                    |
| EXPORT        | 声明一个标号具有全局属性，可被外部的文件使用            |
| DCD           | 以字为单位分配内存，要求4字节对齐，并要求初始化这些内存 |
| PROC          | 定义子程序，与**ENDP**成对使用，表示子程序结束          |
| B             | 跳转到一个标号                                          |
| END           | 到达文件末尾，文件结束                                  |
| IF,ELSE,ENDIF | 汇编条件分支语句                                        |