---
type: concept
status: developing
created: 2026-06-26
updated: 2026-06-26
sources:
  - wiki/sources/概率论 第六讲：连续随机变量.md
tags:
  - 概率论
  - 随机变量
---

# 累积分布函数 CDF

累积分布函数（Cumulative Distribution Function）记作 $F_X(x)$，定义为随机变量落在 $x$ 左边的概率：

$$
F_X(x)=P(X\le x)
$$

## 与 PDF 的关系

对 [[连续随机变量]]，CDF 是 [[概率密度函数 PDF]] 从负无穷积分到 $x$ 的面积：

$$
F_X(x)=\int_{-\infty}^{x} f_X(t)\,dt
$$

如果 $F_X(x)$ 可导，PDF 就是 CDF 的导数：

$$
f_X(x)=F_X'(x)
$$

## 用 CDF 求区间概率

$$
P(a<X\le b)=F_X(b)-F_X(a)
$$

对连续随机变量端点是否包含不影响结果（单点概率为 0），所以也等于 $P(a<X<b)$。

## CDF 的性质

1. 取值有界：$0\le F_X(x)\le 1$
2. 单调不减：$x_1<x_2 \Rightarrow F_X(x_1)\le F_X(x_2)$
3. 左端极限为 0：$\lim_{x\to-\infty}F_X(x)=0$
4. 右端极限为 1：$\lim_{x\to+\infty}F_X(x)=1$

## 连接

- 离散世界对应的是 [[概率质量函数 PMF]]，而 CDF 对离散和连续都适用。
- 典型推导见 [[指数分布]] 的 CDF。
