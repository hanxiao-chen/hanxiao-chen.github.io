
# 1. Clopper-Pearson confidence interval

Let
\\[ X ~ Bin(n,p) \\].
We want to find all the values p \\( ([l,u]) \\)that are not rejected at level \\( \alpha \\):
\\[ \sum_{k=X}^{n} \binom(n,k) l^k (1-l)^{n-k} = \frac{\alpha}{2} \\]
\\[ \sum_{k=0}^{X} \binom(n,k) u^k (1-u)^{n-k} = \frac{\alpha}{2} \\]

The association between beta and binomial distribution:
\\[ \sum_{k=X}^{n}\begin{pmatrix} n\\ k \end{pmatrix} p^k (1-p)^{n-k} = \int_{0}^{p} f (t|X,n-X+1)dt \\]

Therefore,

\\[ \begin{document}
  \begin{equation}
    l=
    \begin{cases}
      0, & \text{if}\ X=0 \\
      B(\frac{\alpha}{2},X,n-X+1), & \text{otherwise}
    \end{cases}
  \end{equation}
\end{document} \\]

\\[ \begin{document}
  \begin{equation}
    u=
    \begin{cases}
      1, & \text{if}\ X=n \\
      B(1 - \frac{\alpha}{2},X+1,n-X), & \text{otherwise}
    \end{cases}
  \end{equation}
\end{document} \\]




# 2. Finite domain

\\[ P(p(x_k) \in [l(x_k),u(x_k)],\forall i = 1,2,...,n) \geq 1- \beta \\]

\\[ P(p(x_k) \in [l(x_k),u(x_k)],\forall i = 1,2,...,n) \\]
\\[ = 1 - P(\exists k, p(x_k) \notin [l(x_k),u(x_k)]) \\]
\\[ = 1 - P(\bigcup_{k=1,2,...,n} p(x_k) \notin [l(x_k),u(x_k)]) \\]
\\[ \geq 1 - P(\sum_{k=1}^{n} p(x_k) \notin [l(x_k),u(x_k)]) \\]
\\[ \geq 1 - n \alpha \\]

Therefore, \\( \beta = n \alpha \\).

# 3. Infinite domain


