# Interesting worked-out math problems

### Number 1.

Consider the matrix
$$
A(x) \;=\;
\begin{bmatrix}
x & 1 \\[6pt]
0 & x
\end{bmatrix}
\in M_{2}(\mathbb{R}[x]).
$$

Find the Smith normal form of $A$.

##### Solution:

Apply row and column operations:

1. $C_1 \leftarrow C_1 - x\,C_2$

$$
\begin{bmatrix}
x & 1\\
0 & x
\end{bmatrix}
\;\longrightarrow\;
\begin{bmatrix}
0 & 1\\
-x^2 & x
\end{bmatrix}
$$

2. Swap columns $C_1 \leftrightarrow C_2$
   
$$
\begin{bmatrix}
1 & 0\\
x & -x^2
\end{bmatrix}.
$$

4. $R_2 \leftarrow R_2 - x\,R_1$
   
$$
\begin{bmatrix}
1 & 0\\
0 & -x^2
\end{bmatrix}.
$$

6. Multiply $R_2$ by $-1$ which is a unit in $\mathbb{R}[x]$

$$
\operatorname{diag}(1,x^2).
$$

Thus, the Smith normal form is
$$
\operatorname{SNF}(A) =\operatorname{diag}(1,x^2),
$$

with invariant factors $d_1 = 1$, $d_2 = x^2$, satisfying $d_1 \mid d_2$.
