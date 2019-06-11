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

对于任意两个事件，
$$
Pr(A_1\cup A_2)=Pr(A_1)+Pr(A_2)-Pr(A_1 \cap A_2)
$$

### 三个事件

直接地说公式就是，
$$
\begin{split}
Pr(A_1 \cup A_2 \cup A_3) = &Pr(A_1)+Pr(A_2)+Pr(A_3) \\
&- [Pr(A_1 \cap A_2) + Pr(A_1 \cap A_3) + Pr(A_2 \cap A_3)] \\
&+ Pr(A_1 \cap A_2 \cap A_3)
\end{split}\tag{1.10.1}
$$
证明就是令$A=A_1 \cup A_2\space B=A_3$，然后利用两个事件的并展开公式。

