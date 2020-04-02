
# 1 Finite domain

\\[ P(p(x_k) \in [l(x_k),u(x_k)],\forall i = 1,2,...,n) \geq 1- \beta \\]

\\[ P(p(x_k) \in [l(x_k),u(x_k)],\forall i = 1,2,...,n) \\]
\\[ = 1 - P(\exists k, p(x_k) \notin [l(x_k),u(x_k)]) \\]
\\[ = 1 - P(\bigcup_{k=1,2,...,n} p(x_k) \notin [l(x_k),u(x_k)]) \\]
\\[ \geq 1 - P(\sum_{k=1}^{n} p(x_k) \notin [l(x_k),u(x_k)]) \\]
\\[ \geq 1 - n \alpha \\]

Therefore, \\( \beta = n \alpha \\).
