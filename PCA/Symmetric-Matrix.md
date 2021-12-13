# Symmetric Matrix

## $(A^{T}A=AA^{T}){\nRightarrow}(A=A^{T})$

显然，$AA^{T}$和$A^{T}A$都是对称矩阵$S$。但是，这无法推导出$A$也是对称矩阵$S$。关于对这两者等价的猜想主要来自于，对于对称矩阵$S$存在正交特征值分解：
$$
S=Q{\Lambda}Q^{T}
$$
同时特征分解的特征向量正交的充要条件为：
$$
&A=Q{\Lambda}Q^{T}\\
{\Leftrightarrow}&A^{T}A=AA^{T}
$$
于是，我们猜想：
$$
&A=A^{T}\\
{\Leftrightarrow}&A^{T}A=AA^{T}
$$
当然，这一推理是不对的，或者说不完全对，这一关系仅在$A$为$2{\times}2$矩阵时成立，毕竟一个normal matrix不必须是symmetric matrix。比如，我们考虑一个$3{\times}3$矩阵：
$$
A=\begin{bmatrix}
1 & 1 & 0\\
0 & 1 & 1\\
1 & 0 & 1
\end{bmatrix}
$$
这里$A$中的每一项都只包含$0$和$1$，这是一个non-negative matrix，然后我们有：
$$
A^{T}A=\begin{bmatrix}
2 & 1 & 1\\
1 & 2 & 1\\
1 & 1 & 2
\end{bmatrix}=AA^{T}
$$
但是对于$A$来说，$A_{31}{\neq}A_{13}$，所以$A^{T}{\neq}A$。但是，我们考虑一个$2{\times}2$矩阵：
$$
A=\begin{bmatrix}
a & b\\
c & d
\end{bmatrix}
$$
$A^{T}A=AA^{T}$意味着$b^{2}=c^{2}$。由于$b$和$c$都是non-negative的，于是有$b=c$，从而$A=A^{T}$。