# PCA

## Are all eigenvectors, of any matrix, always orthogonal?

我们知道PCA所操作的matrix($A$)都是positive semi-definite matrix，比如Matrix Cross-Product($X'X$)、Cov-Matrix和Cor-Matrix等，易知：
$$
A=A^{T}
$$
这是一个实对称矩阵，具备如下性质：

- 实对称矩阵$A$的不同特征值对应的特征向量是正交的。

- 实对称矩阵$A$的特征值都是实数，特征向量都是实向量。

- $n$阶实对称矩阵$A$必可相似对角化，且相似对角阵上的元素即为矩阵本身特征值。
  $$
  A=Q{\Lambda}Q^{T}=Q{\Lambda}Q^{-1}
  $$

- 若$A$具有$k$重特征值$λ_{0}$，必有$k$个线性无关的特征向量，或者说秩$r(λ_{0}I-A)$至多为$n-k$，其中$I$为单位矩阵。

我们可以对第一个性质进行探讨，可以如下验证：
$$
&(AX_{1})^{T}=({\lambda}_{1}X_{1})^{T}\\
{\Rightarrow}&X_{1}^{T}A^{T}={\lambda}_{1}X_{1}^{T}\\
{\Rightarrow}&X_{1}^{T}A^{T}X_{2}={\lambda}_{1}X_{1}^{T}X_{2}\\
{\Rightarrow}&X_{1}^{T}AX_{2}={\lambda}_{1}X_{1}^{T}X_{2}\\
{\Rightarrow}&X_{1}^{T}{\lambda}_{2}X_{2}={\lambda}_{1}X_{1}^{T}X_{2}\\
{\Rightarrow}&{\lambda}_{2}X_{1}^{T}X_{2}={\lambda}_{1}X_{1}^{T}X_{2}\\
{\Rightarrow}&({\lambda}_{2}-{\lambda}_{1})X_{1}^{T}X_{2}=0
$$
由于${\lambda}_{2}{\neq}{\lambda}_{1}$，$X_{1}^{T}X_{2}$必须为0。这建立了对应于两个不同特征值的特征向量的正交性。

