
# 1. Clopper-Pearson confidence interval

Let
\\[ X \sim Bin(n,p) \\].
We want to find all the values p \\( ([l,u]) \\)that are not rejected at level \\( \alpha \\):
\\[ \sum_{k=X}^{n} \binom{n}{k} l^k (1-l)^{n-k} = \frac{\alpha}{2} \\]
\\[ \sum_{k=0}^{X} \binom{n}{k} u^k (1-u)^{n-k} = \frac{\alpha}{2} \\]

The association between beta and binomial distribution:
\\[ \sum_{k=X}^{n} \binom{n}{k} p^k (1-p)^{n-k} = \int_{0}^{p} f (t|X,n-X+1)dt \\]

Therefore,

$$ \begin{equation}
    l=
    \begin{cases}
      0, & \text{if}\ X=0 \\
      B(\frac{\alpha}{2},X,n-X+1), & \text{otherwise}
    \end{cases}
  \end{equation} $$

$$ \begin{equation}
    u=
    \begin{cases}
      1, & \text{if}\ X=n \\
      B(1-\frac{\alpha}{2},X+1,n-X), & \text{otherwise}
    \end{cases}
  \end{equation} $$




# 2. Finite domain

Assume that we can build a C-P CI for $p(x)$ for any x. Our goal is to build simultaneous bands of $1- \beta$ for $p(x)$:

\\[ P(p(x_k) \in [l(x_k),u(x_k)],\forall i = 1,2,...,n) \geq 1- \beta \\]

\\[ P(p(x_k) \in [l(x_k),u(x_k)],\forall i = 1,2,...,n) \\]
\\[ = 1 - P(\exists k, p(x_k) \notin [l(x_k),u(x_k)]) \\]
\\[ = 1 - P(\bigcup_{k=1,2,...,n} p(x_k) \notin [l(x_k),u(x_k)]) \\]
\\[ \geq 1 - P(\sum_{k=1}^{n} p(x_k) \notin [l(x_k),u(x_k)]) \\]
\\[ \geq 1 - n \alpha \\]

Therefore, \\( \beta = n \alpha \\).

# 3. Infinite domain

$B_{x,r} = \left{ y \mid \| y-x \| \leq r \right}$ contains all the neighbors of $x$.

Suppose we have a set $S= { x_1,x_2,...,x_n } \subseteq D$, our assumption is that:
For any $x \in D$, there exists $x_i,x_j \in S \cap B_{x,r}$, $p(x_i)\leq p(x) \leq p(x_j)$

