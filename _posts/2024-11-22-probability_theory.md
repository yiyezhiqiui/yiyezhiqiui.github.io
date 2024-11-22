---
layout: post
title: "概率论知识总结"
date:   2024-11-22
tags: [geek]
comments: true
author: yiyezhiqiu
---


# 概率论的基本概念
## 样本空间、随机事件
样本空间:随机试验E的可能结果集合
样本点:E的每个结果

随机事件:试验E的样本空间S的子集为E的随机事件

$若A\subseteq B,B\subset A,则A=B$

$事件A-B称为事件A与B的差事件$

$若A\cap B=\phi,则称事件A与B互斥(互不相容)$

$若A\cup B=S且A\cap B=\phi,则称事件A与B为逆事件,又称对立事件$

## 等可能概型
等可能概型(古典概型):试验的样本空间只包含有限个元素,试验中每个基本事件发生的可能性相同

## 条件概率
条件概率:事件A已发生的条件下事件B发生的概率$P(B|A)=P(AB)/P(A)$

全概率公式:试验E的样本空间为S,A为E的事件,$B_1,B_2……B_n$为S的一个划分,且P(B_i)>0(i=1,2……,n)则全概率公式为

$$

P(A)=P(A|B_1)P(B_1)+P(A|B_2)P(B_2)+……+P(A|B_n)P(B_n)
$$


贝叶斯公式:试验E的样本空间为S,A为E的事件,$B_1,B_2……B_n$为S的一个划分,且P(A)>0,P(B_i)>0(i=1,2……,n)则，贝叶斯公式为

$$

P(B_i|A)=P(A|B_i)P(B_i)/ \sum_{j=1}^n P(A|B_j)P(B_j)
$$


## 独立性
若$P(AB)=P(A)P(B)$则称事件A与B为独立事件

# 随机变量及其分布
## 离散型随机变量及其分布

### (0-1)分布

### 伯努利试验

### 泊松分布
$\sum_{k=0}^\infty P\{X=k\}=\sum_{k=0}^\infty \frac{e^{-\lambda}\lambda^k}{k!}$

## 随机变量的分布函数
函数$F(x)=P\{X\leq x\},-\infty<x<\infty$称为X的分布函数

对于任意实数$x_1,x_2(x_1<x_2),有$

$P\{x_1\leq X\leq x_2\}=P\{X\leq x_2\}-P\{X\leq x_1\}=F(x_2)-F(x_1)$

分布函数具有一下性质
1.F(x)是一个不减函数

2.$0\leq F(x)\leq1 且F(-\infty)=lim_{x\to-\infty}F(x)=0.F(\infty)=lim_{x\to\infty}F(x)=1$

3.$F(x+0)=F(x)$

## 连续型随机变量及其概率密度
概率密度f(x)有以下性质：
1.$f(x)\geq0$

2.$\int_{-\infty}^{\infty}f(x)dx=1$

3.对于任意实数$x_1,x_2(x_1\leq x_2),有P\{x_1\leq X\leq x_2\}=F(x_2)-F(x_1)=\int_{x_1}^{x_2}f(x)dx$

4.若f(x)在点x处连续,则有$F'(x)=f(x)$

下面介绍三种重要的连续型随机变量
### 1.均匀分布

$$
f(x)=\begin{cases}
\frac{1}{b-a},   a<x<b\\
0,其他
\end{cases}
$$

### 2.指数分布

$$
f(x)=\begin{cases}
\frac{1}{\theta}e^{-\frac{x}{\theta}},   x>0\\
0,其他
\end{cases}
$$

### 3.正态分布

$$
f(x)=\frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{(x-\mu)^2}{2\sigma^2}},-\infty<x<\infty\\
$$

标准正态分布
$f(x)=\frac{1}{\sqrt{2\pi}}e^{-\frac{x^2}{2}}$

# 多维随机变量
## 二维随机变量
$我们称P\{X=x_i,Y=y_i\}=p_{ij},j,j=1,2……为二维离散型随机变量(X,Y)的分布率,或称为随机变量X和Y的联合分布律$

$F(x,y)=\int_{-\infty}^y\int_{-\infty}^x f(u,v)dudv$,则称(X,Y)是二维连续型随机变量,函数f(x,y)称为二维连续型随机变量(X,Y)的概率密度,或称为随机变量X和Y的联合概率密度
