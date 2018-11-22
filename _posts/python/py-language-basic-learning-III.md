---
title: Python Basic Learning III (not finish)
toc: true
date: 2017-06-05 11:00:21
categories: python
tags: [python]
description: 廖雪峰的 Python 教程 - Functional Programming
mathjax: true
list_number: true
---

## 1. 函数式编程

函数就是面向过程的程序设计的基本单元。

Functional Programming 其思想更接近数学计算。

在计算机的层次上，CPU执行的是加减乘除的指令代码，以及各种条件判断和跳转指令，所以，汇编语言是最贴近计算机的语言。

而计算则指数学意义上的计算，越是抽象的计算，离计算机硬件越远。

对应到编程语言，就是越低级的语言，越贴近计算机，抽象程度低，执行效率高，比如C语言；越高级的语言，越贴近计算，抽象程度高，执行效率低，比如Lisp语言。

函数式编程就是一种抽象程度很高的编程范式，`纯粹的函数式编程语言编写的函数没有变量`，因此，任意一个函数，只要输入是确定的，输出就是确定的，这种纯函数我们称之为没有副作用。而允许使用变量的程序设计语言，由于函数内部的变量状态不确定，同样的输入，可能得到不同的输出，因此，这种函数是有副作用的。

函数式编程的一个特点就是，允许把函数本身作为参数传入另一个函数，还允许返回一个函数！

Python对函数式编程提供部分支持。由于Python允许使用变量，因此，Python不是纯函数式编程语言。

### 1.1 高阶函数

Higher-order function


## 2. 模块

> Python内置的模块 和 来自第三方的模块。

> 每一个包目录下面都会有一个__init__.py的文件，这个文件是必须存在的，否则，Python就把这个目录当成普通目录，而不是一个包。

## Reference article

- [廖雪峰的官方网站 liaoxuefeng][2]

[1]: https://docs.python.org/2/library/functions.html#abs
[2]: http://www.liaoxuefeng.com/wiki/001374738125095c955c1e6d8bb493182103fac9270762a000/001386819196283586a37629844456ca7e5a7faa9b94ee8000