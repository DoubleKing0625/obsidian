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

# 概率密度函数 PDF

概率密度函数（Probability Density Function）用来描述 [[连续随机变量]] 的分布，记作：

$$
f_X(x)
$$

## 关键：PDF 不是概率

$f_X(x)$ 是**概率密度**，不是概率。真正的概率要通过积分（曲线下面积）得到：

$$
P(a<X<b)=\int_a^b f_X(x)\,dx
$$

因此密度值可以大于 1。例如 $X\sim Uniform(0,0.5)$ 的密度是 2，但概率是面积 $2\times0.5=1$。

## 合法性条件

非负性：

$$
f_X(x)\ge 0
$$

总面积为 1：

$$
\int_{-\infty}^{+\infty} f_X(x)\,dx=1
$$

## 与 PMF 的对照

[[概率质量函数 PMF]] 是离散世界的对应物：离散用求和、连续用积分。

| | 离散 | 连续 |
|---|---|---|
| 描述函数 | [[概率质量函数 PMF]] | PDF |
| 区间概率 | 求和 | 积分 |
| 单点 | $P(X=x)$ 可大于 0 | $P(X=x)=0$ |

## 连接

- [[累积分布函数 CDF]] 是 PDF 从负无穷积分到 $x$ 的结果；反过来 PDF 是 CDF 的导数。
- 常见 PDF：[[均匀分布]]、[[指数分布]]、[[正态分布]]。
