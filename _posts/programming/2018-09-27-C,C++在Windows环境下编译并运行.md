---
published: true
layout: post
title: C,C++在Windows环境下编译并运行
date: 2018-09-27
categories: blog
tags: [编程随想]
---

**前提条件安装minGW编译器和java运行环境JDK（注意环境变量的配置）**

**①**Notepad++用法：
  第一步：打开notepad++，按F5，或者点击菜单栏“运行->运行”，弹出如下对话框，输入：

              cmd /k cd /d "$(CURRENT_DIRECTORY)" & g++ "$(FILE_NAME)" -o "$(NAME_PART)" & "$(NAME_PART).exe"

然后点击"保存"。
第二步：点击“保存”后，弹出如下对话框，设置此命令的名称与快捷键，例如：name输入“C/C++ compiler”,shortcut （快捷键）设置为自己习惯的即可。点击“OK”，大功告成。

**②***Sublime Text*用法：
                 在工具里面的编译选项

**③***Eclipse*直接打开用				 

译文（Translation）：

**Prerequisites to install minGW compiler and java runtime environment JDK (note the configuration of environment variables)**

**1**Notepad++ usage:
  The first step: open notepad++, press F5, or click the menu bar "Run -> Run", the following dialog box pops up, enter:

              Cmd /k cd /d "$(CURRENT_DIRECTORY)" & g++ "$(FILE_NAME)" -o "$(NAME_PART)" & "$(NAME_PART).exe"

Then click "Save".
Step 2: After clicking “Save”, the following dialog box pops up, set the name and shortcut key of this command, for example: name input “C/C++ compiler”, shortcut (shortcut) is set to your own habit. Click "OK" and you're done.

**2***Sublime Text* Usage:
                 Compile options in the tool

**3***Eclipse* open directly
