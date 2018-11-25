---
layout: post
title: C,C++在Windows环境下编译并运行
date: 2018-09-27
categories: blog
tags: [编程随想]
---

*前提条件安装minGW编译器和java运行环境JDK（注意环境变量的配置）*

①Notepad++用法：
第一步：打开notepad++，按F5，或者点击菜单栏“运行->运行”，弹出如下对话框，输入：

              cmd /k cd /d "$(CURRENT_DIRECTORY)" & g++ "$(FILE_NAME)" -o "$(NAME_PART)" & "$(NAME_PART).exe"

然后点击"保存"。
第二步：点击“保存”后，弹出如下对话框，设置此命令的名称与快捷键，例如：name输入“C/C++ compiler”,shortcut （快捷键）设置为自己习惯的即可。点击“OK”，大功告成。

②Sublime Text用法：
                 在工具里面的编译选项

③Eclipse直接打开用				 
