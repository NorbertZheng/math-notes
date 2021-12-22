# Trace

## Are there non-commuting matrices for which $tr(ABC)=tr(BAC)$?

对于线性operator $A$和$B$，它们作用于$\mathbb{C}^{n}$，也就是指其列数为$n$。依据trace的循环性质，我们有：
$$
tr(AB)=tr(BA)
$$
更一般地来说，对于线性operator $A$、$B$、$C$，它们作用于$\mathbb{C}^{n}$上，我们有：
$$
tr(ABC)=tr(CAB)=tr(BCA)=tr(ABC)
$$
注意！$A$、$B$、$C$之间的顺序是要保留的，也就是一般情况下，其他顺序等式不成立：
$$
tr(ABC){\neq}tr(BAC)
$$
但这里，我们抛出一个问题，我们是否可以对$A$、$B$、$C$进行限制，使得等式成立？即：
$$
tr(ABC)=tr(BAC)
$$
当然，如果$A$和$B$是commute的话，上式显然是成立的，因为commute的定义为：
$$
AB=BA
$$
上面的定义没有针对$A$和$B$的可逆性做任何假设。当然，如果$A$和$B$中任意一个和$C$具备commute关系，我们可以充分地推导出上式，但必要性未知（好像上面$AB=BA$也只是一个充分条件），如$AC=CA$时可以有如下推导：
$$
tr(ABC)=tr(CAB)=tr(ACB)=tr(BAC)
$$
那么，对于$A$、$B$、$C$均为non-commuting matrix的时候，是否还存在一些约束让上面提到的等式成立？我们在这里**让$A$、$B$、$C$均为可逆矩阵，因为如果$A$、$B$、$C$具有zero-divisors，上面等式可以通过一种很简单的方式满足**。

现在，给定$C$和$A$，我们有${\varphi}: M_{n{\times}n}(\mathbb{C}){\rightarrow}R$：
$$
\varphi(B)&=tr(ABC)-tr(BAC)\\
&=tr(BCA)-tr(BAC)\\
&=tr(B(CA-AC))
$$
这是定义在$M_{n{\times}n}(\mathbb{C})$上的一个linear函数。$\varphi(B)$可能不会对$M_{n{\times}n}(\mathbb{C})$都为0，但会对$M_{n{\times}n}(\mathbb{C})$的线性子空间为0。比如，我们给出：
$$
\varphi(B_{1}+tB_{2})=0,{\forall}B_{1},B_{2}{\in}M_{n{\times}n}(\mathbb{C}),[{\varphi}(B_{1}){\neq}0\&\varphi(B_{2}){\neq}0]
$$
这样，在给定$t=-\frac{\varphi(B_{1})}{\varphi(B_{2})}$的情况下，我们可以令$\varphi(B)=0$，就得到了在给定$A$和$C$情况下，可以令等式满足的$B$，也就是下式在这种特定配置下成立：
$$
tr(ABC)=tr(BAC)
$$
