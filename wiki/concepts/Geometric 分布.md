---
type: concept
status: developing
created: 2026-06-24
updated: 2026-06-26
sources:
  - wiki/sources/概率论 第五讲：离散随机变量.md
tags:
  - 概率论
  - 分布
---

# Geometric 分布

Geometric 分布，也叫几何分布，描述第一次成功发生在第几次试验。

假设每次试验成功概率为 $p$，并且各次试验[[独立性|独立]]。定义 [[随机变量]] $X$ 为第一次成功所需的试验次数，则：

$$
X\sim Geometric(p)
$$

取值为：

$$
X\in\{1,2,3,\dots\}
$$

PMF 为：

$$
P(X=k)=(1-p)^{k-1}p
$$

其中：

$$
k=1,2,3,\dots
$$

## 无记忆性

Geometric 分布具有 [[无记忆性]]：

$$
P(X>s+t\mid X>s)=P(X>t)
$$

直觉是：已经失败了很多次，并不会改变未来第一次成功还要等多久的分布。

## 连接

Geometric 分布相当于不断重复 [[Bernoulli 分布|Bernoulli]] 试验，直到第一次成功；它的分布用 [[概率质量函数 PMF]] 描述。它是连续 [[指数分布]] 的离散对应物，两者都具有 [[无记忆性]]。

