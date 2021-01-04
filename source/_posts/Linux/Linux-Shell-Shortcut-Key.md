---
title: Linux Shell快捷键
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

**1.控制命令**

Ctrl + l：清屏（与clear命令效果相同）

Ctrl + c：终止当前正在执行的命令

Ctrl + z：挂起命令，把当前进程转到后台运行，使用fg命令恢复，bg命令继续后台运行，jobs命令查询后台进程。

Ctrl + d : 退出当前 Shell

**2.编辑命令**

**光标移动**

Ctrl + a ：移到命令行首

Ctrl + e ：移到命令行尾

Ctrl + f ：前移（向右移动）一个字符

Ctrl + b ：后退（向左移动）一个字符

Alt + f ：前移（向右移动）一个单词

Alt + b ：后退（向左移动）一个单词

Ctrl + xx：在命令行首和光标之间移动

**3.文本修改**

**补全、删除、粘贴**

tab : 自动补全命令

Ctrl + u ：从光标处删除至命令行首

Ctrl + k ：从光标处删除至命令行尾

Ctrl + w ：从光标处删除至字首

Alt + d ：从光标处删除至字尾

Ctrl + d ：删除光标处（或光标后）的字符（如果光标前后都没有字符，即命令行为空的时候，则会退出shell）

Ctrl + h ：删除光标前的字符(与backspace键相同)

Alt + Backspace：与 Ctrl + w 类似，分隔符有些差别

Ctrl + y ：粘贴至光标后

**4.改变大小写**

Alt + c ：从光标处更改为首字母大写的单词

Alt + u ：从光标处更改为全部大写的单词

Alt + l ：从光标处更改为全部小写的单词

**5.交换字符、单词位置**

Ctrl + t ：交换光标处和之前的字符（ESC+t相同）

Alt + t ：交换光标处和之前的单词

**6.重新执行命令**

Ctrl + p：历史中的上一条命令

Ctrl + n：历史中的下一条命令

Alt + .：使用上一条命令的最后一个参数（会直接在当前光标位置显示）

Ctrl + r：搜索之前使用过的命令

Ctrl + g：从历史搜索模式退出

**7.Bang (!) 命令**

Bang命令算不上快捷键键，但是使用可以快捷的进行一些操作，比如重新执行之前命令、修改上一条命令并执行等等。

!!：执行上一条命令

!cc：执行最近的以cc开头的命令，如!l会执行ls命令

!$：打印上一条命令的最后一个参数，并回车执行。与Alt + .相似，但是会自动执行

!\*：上一条命令的所有参数 !cc:p：仅打印以!cc的输出，但不执行，如!l:p会显示ls

!\$:p：打印输出!\$的输出

^blah：删除上一条命令中第一个blah，然后执行

^blah^foo：将上一条命令中的 blah 替换为 foo，然后执行

^blah^foo^：将上一条命令中所有的 blah 都替换为 foo，然后执行

**补充**
Ctrl + -: 撤回上一次修改
Alt + r: 撤回所有修改
man bash: 查找Commands for Moving查看所有快捷键