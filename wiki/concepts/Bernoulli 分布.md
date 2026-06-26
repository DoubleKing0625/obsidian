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

# Bernoulli 分布

Bernoulli 分布描述一次二选一试验，例如成功/失败、正面/反面、点击/不点击。

如果 [[随机变量]] $X$ 只有两个取值 0 和 1，并且：

$$
P(X=1)=p
$$

$$
P(X=0)=1-p
$$

那么：

$$
X\sim Bernoulli(p)
$$

PMF 为：

$$
P(X=x)=p^x(1-p)^{1-x}
$$

其中：

$$
x\in\{0,1\}
$$

Bernoulli 分布是 [[Binomial 分布]] 在 $n=1$ 时的特殊情况。

