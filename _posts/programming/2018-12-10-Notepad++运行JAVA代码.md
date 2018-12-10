---
published: true
layout: post
title: Notepad++运行JAVA代码
date: 2018-12-10
categories: blog
tags: [编程随想]
---

Notepad++运行JAVA有两种方法：

第一种：调用cmd终端命令执行。

第二种：安装NppExec插件。

版本：npp.7.5.9.bin.x64  

前提：已配置JAVA环境变量。

# 第一种方法：

工具栏->运行  点击后选择运行
1、在运行窗口中输入：

cmd /k javac "$(FULL_CURRENT_PATH)" & echo 编译成功！ & PAUSE & EXIT

点击保存后，在弹出的窗口中设置名称：取名为JAVA编译

2、重复上面的步骤，增加运JAVA的方法
在运行窗口中输入：

cmd /k java -cp "$(CURRENT_DIRECTORY)" "$(NAME_PART)" & PAUSE & EXIT

点击保存后，在弹出的窗口中设置名称：取名为JAVA运行

打开.java文件 点击 编译JAVA，成功后再点击 运行JAVA，即可实现调用CMD命令运行JAVA代码

手动点击 运行 比较麻烦，可以设置 快捷键，编译JAVA ：Alt+Shift+B    运行JAVA：Alt+Shift+R

# 第二种方法：

工具栏->插件->Plugin Manager->Show Plugin Manger  

如果没有Plugin Manager可以手动安装

{ ##notepad++64位添加plugin manager   


（测试下载 v1.4.11下的 PluginManager_v1.4.11_x64.zip   32位的下载PluginManager_v1.4.12_UNI.zip）

- 下载解压后，将两个文件放到对应的文件夹，再打开notepad++，plugin manager就有了。

- 添加PluginManager.dll文件到plugins文件夹里：

- 添加gpup.exe文件到updater文件夹里：

点击 Show Plugin Manager 选择 NppExec 再点击Install 开始安装

打开JAVA代码，按F6执行，首次使用要配置编译器，输入如下代码：

NPP_SAVE
cd "$(CURRENT_DIRECTORY)"
javac.exe "$(FILE_NAME)"
java.exe "$(NAME_PART)"

点击OK 运行JAVA代码，控制台输出结果

--------------------- 
作者：JoLon7 
来源：CSDN 
原文：https://blog.csdn.net/qq_16149125/article/details/82909977 
版权声明：本文为博主原创文章，转载请附上博文链接！

译文(Translation):

 