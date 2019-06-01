# Python FAQ

+ Python是一门通用编程语言，现在被广泛地应用在人工智能&爬虫&数据科学等领域。
+ Python有许多不同的**实现**：PyPy，Jython，IronPython以及官方的标准实现CPython。
  - 目前（2019.6.1）这些实现都可以免费下载。
  - CPython即[https://python.org](https://python.org)上的Python。
  - 所谓的「语言」，不严谨地说，即是一（大）组形如「我需要按这种格式写」和「我这么写会有这样的效果」的规则；而「实现」则是根据程序员写的东西按某种方式去产生效果的东西。
+ Anaconda是一个「Python+一堆数据科学的库」的一键安装包。
+ 「编辑器」跟「编译器」是不同的东西。不严谨地说，前者是用来写代码的，后者是将代码变成可以用来跑的程序的。
  - 大部分（几乎所有）的Python实现都是直接跑代码的。采用这种运行方式的东西叫作「解释器」。
  - Python for Windows自己有一个带语法高亮的编辑器。
+ PyCharm不是Python实现，它是一个**IDE**。你可以（不严谨地）把IDE看作比普通的编辑器要厉害很多的编辑器。

## 学Python 2还是Python 3？

学Python 3，因为Python 2已经过时，快要停止维护了。

## Python版本是越新越好吗？

是的。除非有特殊需求，否则建议使用最新的稳定版。

CPython以外的实现一般都会有说明「兼容Python X.Y」，简单点说就是「使用该版本（几乎）等同于使用Python X.Y」的意思。

## Python能够做[某个需求]吗？

一般而言，有这么几种情况：

+ 你想要的东西已经有人做了，只需要直接用别人写好的库就好了。
+ 你想要的东西已经有人做了，但是在Python里并没有对应的库。这种情况下，借助FFI绕一下还是能做。
+ 你想要的东西还暂时没有人做，但是你随时都可以自己干。
+ 你想要的东西不适合用一般的编程语言做，但是还是可以绕一下然后在Python里面做，只是你可能需要接受「这并不是Python本身的功能」这一事实。
  - （包括但不限于用Python代替HTML/Markdown/SQL）
+ 你想要的东西不适合用编程的方式做。

### 做GUI

`tkinter`。或者如果你不喜欢TK，还有`pyqt5`。

### 做网页

后端主要有Django和Flask。

前端暂时没有。（但是technically可以做一个Python to Javascript的编译器）

### 访问数据库

Redis/MySQL(MariaDB)都有对应的库。CPython本身自带SQLite。

看你是要访问什么数据库，比较流行的数据库一般都会有。

### 爬虫/自动化办公/机器学习

都有的。请参阅相关资料。

## 有关FAQ的其他内容

### 许可
本文按CC-BY 4.0进行许可。

### 我想加新东西！
来[这里](https://github.com/bctnry/public/issues)提issue。
