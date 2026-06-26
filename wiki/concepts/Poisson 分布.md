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

# Poisson 分布

Poisson 分布，也叫泊松分布，常用来描述单位时间或单位空间内某事件发生的次数。

如果随机变量 $X$ 表示某段时间内事件发生的次数，并且平均发生次数是 $\lambda$，那么：

$$
X\sim Poisson(\lambda)
$$

PMF 为：

$$
P(X=k)=\frac{e^{-\lambda}\lambda^k}{k!}
$$

其中：

$$
k=0,1,2,\dots
$$

且：

$$
\lambda>0
$$

## 参数含义

$\lambda$ 表示单位区间内事件发生的平均次数，不是概率。

## 与二项分布的关系

当 [[Binomial 分布|二项分布]] 的 $n$ 很大、$p$ 很小，并且 $np=\lambda$ 保持适中时：

$$
Binomial(n,p)\approx Poisson(np)
$$

直觉上，Poisson 分布描述大量独立小概率事件在单位时间或空间内发生的次数。

## 连接

Poisson 分布是一种 [[离散随机变量]]，其分布用 [[概率质量函数 PMF]] 描述。

