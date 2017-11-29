---
title: 神器 Emacs 神之编辑器使用入门(一)
---

# 简介（Introduction）

相信很多从事计算机软件开发的人都听说过emacs，但是真正掌握甚至入门emacs的都少之又少。emacs是"Editing MACros"的缩写, 是一款古老的文本编辑器，同时也是一个操作系统。emacs的默认配置相对于那些现代的文本编辑器显得十分不友好，但是经过一番折腾后也能配置成一个功能强大的IDE，本文仅做一些简单的入门介绍，让那些刚接触emacs的读者对emacs有个粗略的了解。

常见的文本编辑器学习曲线图

# 快速上手（Getting Started）

打开emacs后会呈现如下界面，很多刚接触emacs的人在这一步就被吓住了。

[神器] Emacs 神之编辑器使用入门(一)

Welcome to GNU Emacs

在emacs中规定了大写的C代表Control(键盘上的Ctrl键)，而M代表Meta(键盘上的Alt键)，S则代表Shift(键盘上的Shift键)。下面是一下常用的快捷键:

C-x C-f 打开/新建文件
C-x C-s 保存当前缓冲区
C-x C-c 关闭Emacs
C-f 前进一个字符
C-b 后退一个字符
C-p 上一行
C-n 下一行
M-f 前进一个单词
M-b 后退一个单词
C-a 行首
C-e 行尾
C-v 下翻一页
M-v 上翻一页
M-< 文件头
M-> 文件尾
C-Space 设置开始标记
C-@ 设置开始标记(C-space可能被操作系统拦截)
M-w 复制标记区内容
C-y 帖粘
M-u 使光标处的单词大写
M-l 使光标处的单词小写
M-c 使光标处单词首字母大写
C-k 删除一行
C-s 向下搜索
C-r 向上搜索
M-% 替换
C-x u 撤销操作