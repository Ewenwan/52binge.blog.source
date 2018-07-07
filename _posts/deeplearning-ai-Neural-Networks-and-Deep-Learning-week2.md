---
title: deeplearning.ai Neural Networks and Deep Learning (week2)
toc: true
date: 2018-07-07 09:55:21
categories: deeplearning
tags: deeplearning.ai
mathjax: true
---

<script type="text/x-mathjax-config">
  MathJax.Hub.Config({
    extensions: ["tex2jax.js"],
    jax: ["input/TeX"],
    tex2jax: {
      inlineMath: [ ['$','$'], ['\\(','\\)'] ],
      displayMath: [ ['$$','$$']],
      processEscapes: true
    }
  });
</script>
<script type="text/javascript" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS_HTML,http://myserver.com/MathJax/config/local/local.js">
</script>

本周我们将要学习 Logistic Regression, 它是神经网络的基础. 

Logistic Regression 可以看成是一种只有输入层和输出层(没有隐藏层)的神经网络. 

我们将使用 **Python** 来实现一个这样的模型, 并将其应用在 **cat** 和 **non-cat** 的图像识别上.

<!-- more -->

## 1. Notation

更多关于本系列课程的符号点[这里][1]同样地, 参数也有所变化($bias$ 单独拿出来作为$b$, 而不是添加 $\theta\_0$

## 2. Logistic Regression

<img src="/images/deeplearning/C1W2-4_1.jpg" width="750" />

 - 一个是 **Loss function**, 即损失函数, 它代表了对于一个样本估计值与真实值之间的误差; 
 - 一个是 **Cost function**, 它代表了所有样本loss的平均值.

<img src="/images/deeplearning/C1W2-6_1.jpg" width="750" />

## 3. Logistic Regression Cost Function

<img src="/images/deeplearning/C1W2-8_1.jpg" width="750" />

## 4. Gradient Descent

<img src="/images/deeplearning/C1W2-9_1.jpg" width="750" />

<img src="/images/deeplearning/C1W2-10_1.jpg" width="750" />

## 5. Derivatives

<img src="/images/deeplearning/C1W2-11_1.png" width="750" />

<img src="/images/deeplearning/C1W2-12_1.png" width="750" />

## 7. Computation Graph

<img src="/images/deeplearning/C1W2-13_1.jpg" width="750" />

## 8. Computation Graph Derivatives

<img src="/images/deeplearning/C1W2-14_1.png" width="750" />

## 9. Logistic regression recap

有了计算图的概念之后, 我们将其运用到Logistic Regression上. 下面标注了计算图的表达.

<img src="/images/deeplearning/C1W2-15_1.jpg" width="750" />

有了上面的图之后, 我们现在来计算反向传播.

## 2 计算图与前向反向传播

## Reference

[img4]: /images/deeplearning/C1W2-4.jpg

[1]: http://7xrrje.com1.z0.glb.clouddn.com/deeplearningnotation.pdf