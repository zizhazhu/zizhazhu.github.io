---
title: Probability and Statistics Chapter 1-10 The Probability of a Union of Events
p: Probability\Probability_and_Statistics
date: 2019-06-11 13:41:46
mathjax: true
categories:
- Math
- Probability
tags:
- notes
- math
---

## 联合事件的概率

先考虑一系列互不相交的事件，
$$
Pr(\bigcup_{i=1}^{n}A_i)=\sum_{i=1}^{n}Pr(A_i)
$$
也就是，这些事件的并的概率，就是直接把每个事件的概率加起来。

如果是任意两个事件，
$$
Pr(A_1\cup A_2)=Pr(A_1)+Pr(A_2)-Pr(A_1 \cap A_2)
$$

### 三个事件

直接地说公式就是，定理1.10.1：
$$
\begin{split}
Pr(A_1 \cup A_2 \cup A_3) = &Pr(A_1)+Pr(A_2)+Pr(A_3) \\
&- [Pr(A_1 \cap A_2) + Pr(A_1 \cap A_3) + Pr(A_2 \cap A_3)] \\
&+ Pr(A_1 \cap A_2 \cap A_3)
\end{split}\tag{1.10.1}
$$
证明是令$A=A_1 \cup A_2\space, B=A_3$，然后利用两个事件的并展开公式。

### 有限个事件

定理1.10.2：
$$
\begin{split}
Pr(\bigcup_{i=1}^n A_i) = &\sum_{i=1}^n Pr(A_i)-\sum_{i<j}Pr(A_i \cap A_j)+\sum_{i<j<k}Pr(A_i\cap A_j \cap A_k) \\
&- \sum_{i<j<k<l}Pr(A_i \cap A_j \cap A_k \cap A_l) \\
&+(-1)^{n+1}Pr(\bigcap_{i=1}^{n}A_i)
\end{split}\tag{1.10.6}
$$
使用数学归纳法证明，找出$m$和$m+1$之间的差异项。

除此之外，也可以利用事件的补的交集来快速计算，
$$
Pr(\bigcup_{i=1}^n A_i) =1-Pr(\bigcap_{i=1}^n A_i^c )
$$