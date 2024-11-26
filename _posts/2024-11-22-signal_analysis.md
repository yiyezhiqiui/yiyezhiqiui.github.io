---
layout: post
title: "信号分析处理与分析"
date:   2024-11-22
tags: [geek]
comments: true
author: yiyezhiqiu
---

# 第一章 连续信号的分析

## 第一节连续信号的时域描述和分析

### 一、连续信号的时域描述

#### (一)普通信号的时域描述

##### 1.正弦信号
$ x(t)=A\sin(\omega_0 t+\phi_0)=A\cos(\omega_0 t+\phi_0-\frac{\pi}{2})    -\infty<t<\infty$

##### 2.指数信号
$x(t)=Ae^{st}  -\infty<t<\infty$

#### (二)奇异信号的描述

##### 1.单位斜坡信号
$$
r(t)=\begin{cases}
t,t\geq 0\\
0,t<0
\end{cases}
$$

##### 2.单位斜坡信号
$$
u(t)=\begin{cases}
1,t>0\\
0,t<0
\end{cases}
$$
![信号图片](../images/signal_analysis/1.png "信号图片")
由单位斜坡信号可以得到矩形信号$x(t)=A[u(t+\frac{\tau}{2})-u(t-\frac{\tau}{2})]\\$
![矩形信号](../images/signal_analysis/2.png "矩形信号")

##### 3.单位冲激信号
$$
\begin{cases}
\delta(t),t\neq0\\
\int_{-\infty}^{\infty}\delta(t)dt=1,t=0
\end{cases}
$$

冲激信号的性质
$$
1.若\delta(t)在x=0处连续，则有\int_{-\infty}^{\infty}x(t)\delta(t)dt=x(0)\\
2.冲激信号具有偶函数特性
3.冲激信号于阶跃信号互为积分和微分得到关系\\
\int_{-\infty}^t\delta(\tau)d\tau=u(t)\\
\frac{du(t)}{dt}=\delta(t)
$$

### 二、连续信号的时域分析
#### (一)基本运算
##### 1.尺度变换
##### 2.翻转
##### 3.平移
#### (二)叠加和相乘
#### (三)微分和积分
#### (三)卷积运算
$x_1(t)*x_2(t)=\int_{-\infty}^{\infty}x_1(\tau)x_2(t-\tau)d\tau=\int_{-\infty}^{\infty}x_1(t-\tau)x_2(\tau)d\tau$

### 三、连续信号的时域分析
#### (一)分解成冲激函数之和
#### (二)
