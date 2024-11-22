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