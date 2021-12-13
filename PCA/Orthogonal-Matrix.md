# Orthogonal Matrix

## The length(magnitude) of each eigenvalue of $Q$ is 1.

令$Q$为一个$n{\times}n$实正交矩阵。

令$\lambda$为$Q$的一个特征值，$\textbf{v}$为对应的特征向量。

于是，我们有：
$$
Q\textbf{v}={\lambda}\textbf{v}
$$
对两边取模有：
$$
||Q\textbf{v}||^{2}=||{\lambda}\textbf{v}||^{2}=|\lambda|^{2}||\textbf{v}||^{2}
$$
左式做如下化简：
$$
&||Q\textbf{v}||^{2}\\
=&\overline{(Q\textbf{v})}^{T}(Q\textbf{v})\\
=&\overline{\textbf{v}}^{T}Q^{T}Q\textbf{v}\\
=&\overline{\textbf{v}}^{T}\textbf{v}\\
=&||\textbf{v}||^{2}
$$
其中，第一步使用了向量模的定义，第二步是因为$Q$是一个实正交矩阵，第三步是因为$Q^{T}Q=I$，第四步使用了向量模的定义。于是，我们得到：
$$
|\lambda|^{2}||\textbf{v}||^{2}=||\textbf{v}||^{2}
$$
由于$\textbf{v}$是一个特征向量，其一定是非零的，于是$||\textbf{v}||^{2}{\neq}0$，两边消去$||\textbf{v}||$有：
$$
|\lambda|^{2}=1
$$
由于特征值的length（magnitude）非零，于是有：
$$
|\lambda|=1
$$
