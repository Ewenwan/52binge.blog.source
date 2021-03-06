---
title: one-hot encoding 与 dummy encoding（not finish）
toc: true
date: 2018-04-05 16:43:21
categories: machine-learning
tags: feature_project
---

One-Hot编码和哑变量应该怎么用考虑一个具有三个类别的离散型特征，采用 One-Hot 编码后：

<!-- more -->


其中





因此有





从上面的公式可以看出，参数(θ0, θ1, θ2, θ3) 与参数(θ0 + αθ3, θ1 − αθ3, θ2 − αθ3, (1 − α)θ3) 等价，α 可以取任意值。此时模型很难学到靠谱的参数，此问题被称为虚拟陷阱（dummy variable trap）。产生这种问题的原因是因为偏置项θ0 与其它变量之间有线性相关关系，解决这个问题有以下三种方法：

>（1）去掉偏置项θ0 。此时上面公式中θ0=0，此时模型只有唯一解（思考下为什么）。
>（2）引入正则项。既然有很多等价的参数，那我们可以考虑从这些等价的参数中选择我们最想要的，常用的做法就是使用正则项，控制参数的取值范围。
>（3）使用哑变量替代One-Hot编码。此时上面公式中x3=0，模型只有唯一解.

此问题思考的关键点在于，对于特征变量的引入，要保证参数之间不存在线性相关关系，如果存在线性相关关系，则容易出现虚拟陷阱的问题。上面考虑的是一个离散型特征的情况，如果有很多种不同类型的离散型特征，例如三个离散型特征，分别是M类、N类和P类，那么最终我们要用多少个变量来表示他们并且不出问题呢？

## Reference

- [One-Hot编码和哑变量应该怎么用][1]

[1]: https://www.jianshu.com/p/08a5396ca2ed