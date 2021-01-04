---
title: Linux VIM Tips
top: false
cover: true
toc: true
mathjax: true
date: 2021-1-4
password:
summary:
tags: Linux
categories: Linux
---

# Online Help
:help x -> Normal mode command
:help v_u -> Visual mode command
:help i_ -> Insert mode command

# 常用快捷键
C-f -> 向前翻页
C-b -> 往回翻页
C-d -> 向前翻半页
C-u -> 往回翻半页
C-e -> 向前翻一行
C-y -> 往回翻一行

M -> 光标跳到屏幕中间
L -> 光标跳到屏幕底部
H -> 光标跳到屏幕顶部

w -> 光标往前跳一个单词
b -> 光标往回跳一个单词
d -> +d删一行，+w往前删一个单词, +b往回删一个单词
y -> +y拷贝一行
p -> 粘贴
u -> 撤回修改
C-r -> 重复撤回的修改

. -> 重复上一次的命令
; -> 重复正向查找或反向查找t/T/f/F
, -> 反向t/T/f/F

:split -> 上下分屏
:vsplit -> 左右分屏
vi -p test1.cpp test2.cpp -> 分标签页
:tabe test3.cpp -> 打开第3个标签页
:tabn -> 下一个标签页
:tabp -> 上一个标签页
vi -o test1.cpp test2.cpp -> 上下分屏
vi -O test1.cpp test2.cpp -> 左右分屏
C-w -> 加方向键或w在窗格间跳转
