---
title: LDA Topic Model
toc: true
date: 2017-09-22 07:08:21
categories: nlp
tags: LDA
---

Latent Dirichlet Allocation 主题模型理论:

 1. 直观版
 2. 标准版
 3. 公式版

<!-- more -->

>                                           据我推测，大部分人是可以撑过前两个版本的

## 1. 什么是主题模型

<img src="/images/nlp/lda-01.png" width="420" height="400"/img>

### 1.1 直观版

`场景` : 假设某企业想要招聘一个工程师，他们收到了一把简历，他们想直接通过简历来看谁是大牛，谁是彩笔 ?

`特征` :

简历里通常包含这些个人特征 :

<img src="/images/nlp/lda-02.png" width="490" height="400" /img>

`判断基础` :

<img src="/images/nlp/lda-04.png" width="400" height="200" /img>

`总结公式` :

<img src="/images/nlp/lda-05.png" width="700" height="400" /img>

> ？

### 例子与理论的关系

<img src="/images/nlp/lda-04.png" width="400" height="200" /img>

<img src="/images/nlp/lda-06.png" width="400" height="200" /img>

## 2. 什么是 LDA ?

Latent Dirichlet Allocation

            是一种无监督的贝叶斯模型

  1. 是一种主题模型，它可以将文档集中每篇文档的主题按照概率分布的形式给出。
  2. 无监督学习算法，训练时需要手工标注训练集，需要的是文档集以及主题数量k即可。

此外LDA的另一个优点则是: 每一个主题均可找出词语来描述它。                 

是一种词袋模型，即它认为一篇文档是由一组词构成的一个集合，一篇 Doc 可以包含多个Topic，文档中每个词都由其中一个主题生成。

## Reference

[1]: /images/nlp/lda-01.png
[2]: /images/nlp/lda-02.png
[3]: /images/nlp/lda-03.png
[4]: /images/nlp/lda-04.png
[5]: /images/nlp/lda-05.png
