---
type: concept
status: developing
created: 2026-06-24
updated: 2026-06-26
sources:
  - wiki/sources/概率论 第五讲：离散随机变量.md
  - wiki/sources/概率论 第四讲：计数方法.md
tags:
  - 概率论
  - 分布
---

# Binomial 分布

Binomial 分布，也叫二项分布。

如果进行 $n$ 次独立重复 [[Bernoulli 分布|Bernoulli]] 试验，每次成功概率为 $p$，定义 $X$ 为成功次数，那么：

$$
X\sim Binomial(n,p)
$$

PMF 为：

$$
P(X=k)=\binom{n}{k}p^k(1-p)^{n-k}
$$

其中：

$$
k=0,1,2,\dots,n
$$

## 直觉

- $\binom{n}{k}$（[[二项系数]]）：从 $n$ 个位置中选 $k$ 个成功位置。
- $p^k$：$k$ 次成功的概率贡献。
- $(1-p)^{n-k}$：$n-k$ 次失败的概率贡献。

## 使用信号

固定做 $n$ 次独立试验，问成功了几次。

## 连接

Binomial 分布是一种 [[离散随机变量]]，分布用 [[概率质量函数 PMF]] 描述；当 $n=1$ 时退化为 [[Bernoulli 分布]]。

