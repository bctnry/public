# 新人指南

## 总体方针

1. 搜索引擎能搜得到的就不要问了。（请bing起步，不要用百度。）
2. 文档里有写的就不要问了（特别是关于`str.format()`的东西。老是帮人读文档很麻烦很痛苦的）。对文档的内容的疑问除外，这种可以随意问。
3. 代码跑不了，无论是你自己的代码还是搜到的别人的代码，按下一节中的方法处理。
4. 要学会自己读懂错误信息。即，知道「程序错了」是不够的，还要知道是「怎么样的错」。
5. 不要因为别人没有帮你而发脾气，大家都很忙的，就算有人很闲，他们也是在忙着闲，所以technically闲人也很忙（？）。

## 如何避免问了别人无法回答的有关代码的问题

以下举几个做得不是很对（或者直白点说，就是不对）的例子，请自行对号入座：

### 场景一

```
A（唐突地，毫无预兆地）：我的代码跑不了/报错了，有谁能帮帮我吗？
（然后没有下文了。一·点·下·文·都·没·有·了。）
A：……怎么没人帮我？！
```

在这里，最大的问题是「跑不了」的原因有**非常非常非常非常非常非常非常多**，包括但不限于：没有装Python；Python版本不对（例如，A复制粘贴了网上的Python2的例子，但是用Python3来跑）；运行的方式不对（例如，A复制粘贴了网上的例子后直接在REPL里粘贴）；用Microsoft Word/WPS Office来写Python（！）；语法错误等。甚至（经常地）有人会把「运行中异常退出」和「输出结果不对」这两种technically并不算跑不了的结果也叫做「跑不了」。这会给想要解答的人带来困难，因为代码在A那里，代码的行为在A那里，代码的结果也在A那里，这个「跑不了」究竟是怎样的跑不了，别人是不知道的。

### 场景二

```
A：我的代码跑不了，有谁能帮帮我吗？
A：*错误信息，包括但不限于截图、拍照和直接复制粘贴得到的文本*
B：*提了几个建议*
C：*也提了几个建议*
A：你们说的我都试过了，都跑不了，你们到底懂不懂啊？
```

场景二中A的做法要稍微比场景一中的A好一点，因为至少别人不再是什么都不知道了。在某些情况下，熟悉初学者错误的人可能会一眼看出问题所在（比如说用了中文的标点符号）或者是根据经验预测出问题所在（比如说，一个抱怨`str`不能和`int`相加的`TypeError`可能来自于某个地方忘记加`int()`转换，一个有关`None`的错误可能来自于某些corner case没有处理好，etc），但是从别人的角度来看，由于没有更多的信息，能做的事情也只有这些了。

### 场景三

```
A：我的代码跑不了，有谁能帮帮我吗？
A：*代码本身，包括但不限于截图、拍照和直接复制粘贴得到的文本*
A：*错误信息，包括但不限于截图、拍照和直接复制粘贴得到的文本*
```

这种相比起前两种来要好很多，至少别人能够开始分析究竟是代码中的哪一个环节出了错误。但是这样还是不够的：假如A写了这份代码本身是想要做出某种效果的（比如说，A希望将一组数字加起来计算它们的平均值、众数和中位数），即使A知道他的程序跑不了，别人也是**没有办法知道怎样才算跑不了**的。在这种情况下，别人能够帮到的其实比起场景二来并没有多很多。

### 场景四

```
A：我的代码跑不了，有谁能帮帮我吗？
A：*代码本身，包括但不限于截图、拍照和直接复制粘贴得到的文本*
A：*错误信息，包括但不限于截图、拍照和直接复制粘贴得到的文本*
A：我希望这样：这个程序会从命令行获取一组数字，并输出它们的平均数、众数和中位数。
```

只有这种情况才算是真正地问了一个清晰的问题。事实上，在某些程序员社区里，只有详细到这种程度以上的问题才是被允许的。假如A能够再进一步解释（比如说，解释一下究竟要什么样的数字，例如是否支持小数/二进制/十六进制等），可以获得加分。

### 总结

规则只有一句话：

> 从别人的角度看来，自己问的问题是否清晰？如果不清晰，就补充细节，直到清晰为止。

## 有关指南的其他内容

### 许可

本文按[CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/)进行许可。

### 我想加新东西！

来[这里](https://github.com/bctnry/public/issues)提issue。
