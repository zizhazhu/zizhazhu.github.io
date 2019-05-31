---
title: Probability and Statistics Chapter 1-9 Multinomial Coefficients Exercise
p: Probability\Probability_and_Statistics
date: 2019-05-23 13:41:46
mathjax: true
categories:
- Math
- Probability
tags:
- notes
- math
---

1. 直接应用公式，把21个房子分到3类。

$$
{21\choose 7,7,7}=\frac{21!}{7!7!7!}
$$

2. 把50个位置分给4种珠子
   $$
   50\choose 18,12,8,12
   $$
   
3. 300个人里选5个再选8个

$$
300 \choose 5,8,287
$$

4. 先计算可能的排列数，把10个位置分给5种字母

$$
10\choose3,3,2,1,1
$$

而statistics只是其中的一种
$$
\frac{1}{10\choose3,3,2,1,1}=\frac{1}{50400}
$$

5. 把n次投掷分给6种结果，再除以总共的可能数
   $$
   \frac{n\choose n_1,n_2,n_3,n_4,n_5,n_6}{6^n}
   $$
   
6. 每个数字出现2次，总共6种情况，是对称的

   $$
   \frac{6{7\choose 2,1,1,1,1,1}}{6^7}
   $$

7. 25张卡里有12张红卡，分到三个人手里，分别是10, 8, 7张。计算红卡是6,2,4的概率。
   先计算卡分布的总数
   $$
   25\choose{10, 8, 7}
   $$
   然后计算红卡分布的总数
   $$
   12\choose{6,2,4}
   $$
   再考虑其他卡的分配数
   $$
   13\choose{4,6,3}
   $$
   

8. $$
   \frac{{12\choose{3,3,3,3}}{40\choose{10,10,10,10}}}{52\choose{13,13,13,13}}
   $$

9. $$
   \frac{4!}{52\choose{13,13,13,13}}
   $$

10. $$
    \frac{1}{9\choose{2,3,4}}=\frac{2!3!4!}{9!}
    $$

    9个位置里面，选两个放Davis，选3个放Jones，选4个放Smith。

    另一种解释，三个内部排列，除以全排列。