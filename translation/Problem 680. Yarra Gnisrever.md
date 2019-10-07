### 680. Yarra Gnisrever

Let $N$ and $K$ be two positive integers.

$F_n$ is the $n$-th Fibonacci number: $F_1 = F_2 = 1$, $F_n = F_{n - 1} + F_{n - 2}$ for all $n \geq 3$.
Let $s_n = F_{2n - 1} \mod N$ and let $t_n = F_{2n} \mod N$.

Start with an array of integers $A = (A[0], \cdots, A[N - 1])$ where initially every $A\text{[}i]$ is equal to $i$.
Now perform $K$ successive operations on $A$, where the $j$-th operation consists of reversing the order of those elements in $A$ with indices between $s_j$ and $t_j$ (both ends inclusive).

Define $R(N,K)$ to be $\sum_{i = 0}^{N - 1}i \times A\text {[}i]$ after $K$ operations.

For example, $R(5, 4) = 27$, as can be seen from the following procedure:
Initial position: $(0, 1, 2, 3, 4)$

Step 1 - Reverse $A[1]$ to $A[1]$: $(0, 1, 2, 3, 4)$
Step 2 - Reverse $A[2]$ to $A[3]$: $(0, 1, 3, 2, 4)$
Step 3 - Reverse $A[0]$ to $A[3]$: $(2, 3, 1, 0, 4)$
Step 4 - Reverse $A[3]$ to $A[1]$: $(2, 0, 1, 3, 4)$

$R(5, 4) = 0 \times 2 + 1 \times 0 + 2 \times 1 + 3 \times 3 + 4 \times 4 = 27$

Also, $R(10^2, 10^2) = 246597$ and $R(10^4, 10^4) = 249275481640$.
Find $R(10^{18}, 10^6)$ giving your answer modulo $10^9$.

### 680. 数组翻转

令 $N$ 和 $K$ 为两个正整数。

$F_n$ 是第 $n$ 个斐波那契数，其中 $F_1 = F_2 = 1$，且对于 $n \geq 3$，$F_n = F_{n - 1} + F_{n - 2}$。
再令 $s_n = F_{2n - 1} \mod N$ 且 $t_n = F_{2n} \mod N$.

现在给定一个正整数数组 $A = (A[0], \cdots, A[N - 1])$，一开始的时候，$A\text{[}i]$ 等于 $i$。
现在接连对数组 $A$ 进行 $K$ 次操作，对于第 $j$ 次操作，你需要将 $A$ 中的 $[s_j, t_j]$ 这段区间翻转。 

然后，定义 $R(N,K)$ 为经过 $K$ 次操作后， $\sum_{i = 0}^{N - 1}i \times A\text {[}i]$ 的值。

比如说，$R(5, 4) = 27$，其过程如下：
初始位置：$(0, 1, 2, 3, 4)$

- 第一步 - 翻转 $[1,1]$：$(0, 1, 2, 3, 4)$
- 第二步 - 翻转 $[2,3]$：$(0, 1, 3, 2, 4)$
- 第三步 - 翻转 $[0,3]$：$(2, 3, 1, 0, 4)$
- 第四步 - 翻转 $[3,1]$：$(2, 0, 1, 3, 4)$

$R(5, 4) = 0 \times 2 + 1 \times 0 + 2 \times 1 + 3 \times 3 + 4 \times 4 = 27$

并且，$R(10^2, 10^2) = 246597$ 且 $R(10^4, 10^4) = 249275481640$。
请计算 $R(10^{18}, 10^6)$ 模 $10^9$ 的值。
