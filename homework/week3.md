# 第 3 周

> **定义** (弱导数) 设 $g,h\in L_{\mathrm{loc}}^2\left(\mathbb R\right)$. 若对一切 $\varphi\in C_c^\infty\left(\mathbb R\right)$ 成立 $$ \int_{\mathbb R}g\varphi'\mathrm dt=-\int_{\mathbb R}h\varphi\mathrm dt, $$ 则称 $h$ 是 $g$ 的弱导数, 记为 $g'=h$.

> **基本事实** (弱导数绝对连续) 设 $g\in L_{\mathrm{loc}}^2\left(\mathbb R\right)$, $h\in L^2\left(\mathbb R\right)$, 若 $h$ 是 $g$ 的弱导数, 即对一切 $\varphi\in C_c^\infty\left(\mathbb R\right)$ 成立 $$ \int_{\mathbb R}g\varphi'\mathrm dt=-\int_{\mathbb R}h\varphi\mathrm dt, $$ 则 $g$ 绝对连续, 且 $g'=h$ 几乎处处成立.

> **定义 1.1.1** (度量空间) 设 $X$ 是一个非空集合, 若对于 $X$ 中任意两个元素 $x,y$, 有一个实数 $d\left(x,y\right)$ 与它们对应, 而且满足下面条件:<br>(i) **(非负性与正定性)** 对任意 $x,y\in X$, $d\left(x,y\right)\ge0$, 并且 $d\left(x,y\right)=0$ 的充要条件是 $x=y$;<br>(ii) **(对称性)** 对任意 $x,y\in X$, $d\left(x,y\right)=d\left(y,x\right)$;<br>(iii) **(三角不等式)** 对任意 $x,y,z\in X$, $d\left(x,y\right)\le d\left(x,z\right)+d\left(z,y\right)$,<br>则称 $\left(X,d\right)$ 是一个**度量空间**(或**距离空间**), $d$ 为 $X$ 上的**度量**(或**距离**), $d\left(x,y\right)$ 为**点 $x,y$ 之间的距离**.

> **定义 1.1.2** (极限) 设 $\left(X,d\right)$ 是度量空间, $\left\{x_n\right\}_{n=1}^\infty$ 是 $X$ 中点列, $x_0\in X$, 若 $$\lim_{n\to\infty}d\left(x_n,x_0\right)=0,$$ 则称**点列 $\left\{x_n\right\}_{n=1}^\infty$ 按照度量 $d$ 收敛于 $x_0$**, 记为 $\lim_{n\to\infty}x_n=x_0$.

> **定义 1.2.1** (哈梅尔基与维数) 我们称线性空间 $X$ 上的一个极大线性无关组为空间 $X$ 的一组**哈梅尔基**, 若 $X$ 的某个哈梅尔基中只有有限个元素, 则称 $X$ 是**有限维线性空间**, 否则称其为**无限维线性空间**.

> **引理 1.2.1** (完备性与闭集) 设 $A$ 为完备的度量空间 $\left(X,d\right)$ 的一个子集. 度量空间 $\left(A,d\right)$ 是完备的当且仅当 $A$ 是 $X$ 的一个闭子集.

> **定义 1.2.2** (半范数与范数) 记 $\mathbb K$ 是实数域 $\mathbb R$ 或复数域 $\mathbb C$. 对于 $\mathbb K$ 上的线性空间 $X$, 若 $X$ 中的每个向量 $x$ 都对应一个实数 $\left\|x\right\|$, 且满足如下条件:<br>(i) 对任意 $x\in X$, $\left\|x\right\|\ge0$;<br>(ii) 对数 $\alpha$ 与 $x\in X$, $\left\|\alpha x\right\|=\left|\alpha\right|\left\|x\right\|$;<br>(iii) 对任意 $x,y\in X$, $\left\|x+y\right\|\le\left\|x\right\|+\left\|y\right\|$, <br>则称 $\left\|\cdot\right\|$ 为 $X$ 上的**半范数**, $X$ 称为半赋范空间. 若 $\left\|\cdot\right\|$ 还满足 $\left\|x\right\|=0$ 当且仅当 $x=0$, 则称 $\left\|\cdot\right\|$ 为 $X$ 上的**范数**, $\left(X,\left\|\cdot\right\|\right)$ 称为**赋范线性空间**.<br>线性空间上的范数诱导了这个空间上的度量 $d\left(x,y\right)=\left\|x-y\right\|$. 显然这个度量具有平移不变性, 即 $d\left(x,y\right)=d\left(x+z,y+z\right)$. 而且, 若 $x_n$ 按度量 $d$ 收敛于 $x_0$, 由三角不等式可得 $\left\|x_n\right\|\to\left\|x_0\right\|$. 换言之, $\left\|\cdot\right\|$ 在度量 $d$ 给出的拓扑下是连续的.

> **定理 1.2.2** (勾股定理, 毕达哥拉斯定理) 对内积空间 $H$ 中两个元素 $x,y$, 若 $x\perp y$, 则有 $$ \left\|x+y\right\|^2=\left\|x\right\|^2+\left\|y\right\|^2. $$

> **定义 1.2.3** (内积空间) 记 $\mathbb K$ 是实数域 $\mathbb R$ 或复数域 $\mathbb C$. 对于 $\mathbb K$ 上的线性空间 $H$, 如果 $H$ 中任何两个向量 $x,y$ 都对应着一个数 $\left\langle x,y\right\rangle\in\mathbb K$, 满足条件:<br>(i) **(共轭对称性)** 对任意 $x,y\in H$, $\left\langle x,y\right\rangle=\overline{\left\langle y,x\right\rangle}$;<br>(ii) **(对第一变元的线性性)** 对任意 $x,y,z\in H$, $\alpha,\beta\in\mathbb K$, $\left\langle\alpha x+\beta y,z\right\rangle=\alpha\left\langle x,z\right\rangle+\beta\left\langle y,z\right\rangle$;<br>(iii) **(正定性)** 对任意 $x\in H$, $\left\langle x,x\right\rangle\ge0$, 且 $\left\langle x,x\right\rangle=0$ 的充要条件是 $x=0$, <br>那么称 $\left\langle\cdot,\cdot\right\rangle$ 是 $H$ 中的**内积**, 称 $H$ 是实 (或复)**内积空间**.

> **引理 1.2.3** (柯西-施瓦茨不等式) 设 $x,y\in H$, 则成立不等式 $$ \left|\left\langle x,y\right\rangle\right|^2\le\left\langle x,x\right\rangle\left\langle y,y\right\rangle. $$

> **定义 1.2.4** (正交) 如果内积空间 $\left(H,\left\langle\cdot,\cdot\right\rangle\right)$ 中两个向量 $x,y$ 满足 $\left\langle x,y\right\rangle=0$, 就说 $x$ 与 $y$ **正交**, 记作 $x\perp y$.

> **例 1.2.8** ($L^p\left(E\right)$ 的完备性) 设 $E$ 是欧几里得空间 $\mathbb R^k$ 的勒贝格可测集. 对 $1\le p<\infty$, $L^p\left(E\right)$ 按范数 $\left\|f\right\|_p=\left(\int_E\left|f\right|^p\mathrm dm\right)^{1/p}$ 成为赋范线性空间, 其诱导度量 $d\left(f,g\right)=\left\|f-g\right\|_p$ 是完备的, 即 $L^p\left(E\right)$ 是巴拿赫空间.

> **例 1.2.12** ($C\left[a,b\right]$ 是巴拿赫空间) 由例 1.1.6, $C\left[a,b\right]$ 是巴拿赫空间.

> **例 1.2.13** ($l^p$ 是巴拿赫空间) 令 $1\le p<\infty$. 空间 $l^p$ 按范数 $\left\|x\right\|_p=\left(\sum_{n=1}^\infty\left|x_n\right|^p\right)^{1/p}$ 是完备的, 即 $l^p$ 是巴拿赫空间.

> **习题 1.2 第 13 题** (内积空间的可数直和) 设 $R_1,R_2,\cdots,R_n,\cdots$ 是一列内积空间. 令 $R=\left\{\left\{x_n\right\}:x_n\in R_n,\sum_{n=1}^\infty\left\|x_n\right\|^2<\infty\right\}$, 当 $\left\{x_n\right\},\left\{y_n\right\}\in R$ 时, 规定 $$ \alpha\left\{x_n\right\}+\beta\left\{y_n\right\}=\left\{\alpha x_n+\beta y_n\right\},\quad\left\langle\left\{x_n\right\},\left\{y_n\right\}\right\rangle=\sum_{n=1}^\infty\left\langle x_n,y_n\right\rangle. $$ 证明 $R$ 是内积空间. 如果 $R_n\left(n=1,2,\cdots\right)$ 都是希尔伯特空间, 证明 $R$ 也是希尔伯特空间.(空间 $R$ 常记为 $\bigoplus_n R_n$.)

> **定义 1.3.1** (正交系与标准正交系) 设 $\mathcal F$ 是希尔伯特空间 $H$ 中的一族非零向量.<br>(i) 如果 $\mathcal F$ 中任何两个不同的向量都正交, 就称 $\mathcal F$ 是 $H$ 的正交系;<br>(ii) 如果正交系 $\mathcal F$ 中每个向量的范数都等于 $1$, 就称 $\mathcal F$ 是标准正交系 (或规范正交系).

> **定理 1.3.1** (贝塞尔不等式) 设 $\mathcal F=\left\{e_\lambda:\lambda\in\Lambda\right\}$ 是希尔伯特空间 $H$ 中的标准正交系. 那么, 对于每个 $x\in H$, 它的傅里叶系数 $\left\{\left\langle x,e_\lambda\right\rangle:\lambda\in\Lambda\right\}$ 中最多只有可列个不为零, 并且还成立如下的贝塞尔不等式: $$ \sum_{\lambda\in\Lambda}\left|\left\langle x,e_\lambda\right\rangle\right|^2\le\left\|x\right\|^2. $$

> **定理 1.3.2** (标准正交基的等价条件) 设 $\mathcal E=\left\{e_\lambda:\lambda\in\Lambda\right\}$ 是希尔伯特空间 $H$ 中的标准正交系, 下列命题等价:<br>(i) 对 $H$ 中任意元素 $x$, 有 $x=\sum_{\lambda\in\Lambda}\left\langle x,e_\lambda\right\rangle e_\lambda$;<br>(ii) $\overline{\text{span}\left\{e_\lambda:\lambda\in\Lambda\right\}}=H$;<br>(iii) $\left\{e_\lambda:\lambda\in\Lambda\right\}$ 是**完全的**, 即: 若 $x\in H$ 满足 $x\perp e_\lambda\left(\forall\lambda\in\Lambda\right)$, 则 $x=0$;<br>(iv) $\left\{e_\lambda:\lambda\in\Lambda\right\}$ 是**完备的**, 即: 对 $H$ 中任意元素 $x$, 帕塞瓦尔等式 $\left\|x\right\|^2=\sum_{\lambda\in\Lambda}\left|\left\langle x,e_\lambda\right\rangle\right|^2$ 成立.<br>我们称满足上述条件之一的标准正交系为希尔伯特空间 $H$ 中的一组**标准正交基**(或规范正交基).

> **定理 1.3.3** (标准正交系可扩张为标准正交基) 设 $A$ 是希尔伯特空间 $H$ 的标准正交系, 则 $A$ 可扩张为 $H$ 的一组标准正交基.

> **例 1.3.9** (埃尔米特多项式构成完备标准正交系) 令 $H_n$ 为埃尔米特多项式 $\left(-1\right)^n\mathrm e^{t^2}\frac{\mathrm d^n}{\mathrm dt^n}\mathrm e^{-t^2}$, 作 $$ \psi_n\left(t\right)=\left(2^n n!\sqrt\pi\right)^{-\frac12}\mathrm e^{-\frac{t^2}{2}}H_n\left(t\right), $$ 则 $\psi_n\left(t\right)\left(n=0,1,2,\cdots\right)$ 组成 $L^2\left(\mathbb R,\mathrm e^{-t^2}\mathrm dm\left(x\right)\right)$ 中的完备标准正交系.

> **定义 1.4.1** (内点, 内部与开集) 设 $A$ 是度量空间 $\left(X,d\right)$ 中的点集, $x_0\in A$.<br>(i) 如果存在 $r>0$ 使得 $\left\{x\in X:d\left(x,x_0\right)<r\right\}\subseteq A$, 则称 $x_0$ 是 $A$ 的内点;<br>(ii) $A$ 的内点全体构成的点集称为 $A$ 的 (拓扑)内部, 记作 $A^\circ$;<br>(iii) 如果 $A$ 中每一点都是 $A$ 的内点, 就称 $A$ 是开集;<br>(iv) 规定空集也是开集.

> **引理 1.4.1** (基本点列与完备性) (i) 度量空间 $X$ 中收敛点列是基本点列.<br>(ii) 设 $\left\{x_n\right\}_{n=1}^\infty$ 是度量空间 $X$ 中基本点列, 如果 $\left\{x_n\right\}_{n=1}^\infty$ 有子列 $\left\{x_{n_k}\right\}_{k=1}^\infty$ 收敛于 $X$ 中的点 $x$, 那么 $\left\{x_n\right\}_{n=1}^\infty$ 也收敛于 $x$.<br>(iii) 完备度量空间的闭子集是完备子空间.<br>(iv) 任何度量空间的完备子空间是闭子集.

> **定理 1.4.1** (连续映射的等价条件) 设 $f$ 是度量空间 $X$ 到度量空间 $Y$ 中的映射, 那么下面条件等价:<br>(i) 映射 $f$ 是连续的;<br>(ii) 对于任意 $x_0\in X,\varepsilon>0$, 存在 $\delta>0$, 使得对 $x_0$ 在 $X$ 中的邻域 $O\left(x_0,\delta\right)$, 有 $f\left(O\left(x_0,\delta\right)\right)\subset O\left(f\left(x_0\right),\varepsilon\right)$;<br>(iii) 空间 $Y$ 中的任一开集 $O$ 的原像 $f^{-1}\left(O\right)$ 是 $X$ 中的开集;<br>(iv) 空间 $Y$ 中的任一闭集 $F$ 的原像 $f^{-1}\left(F\right)$ 是 $X$ 中的闭集.

> **命题 1.4.1** (可分空间的子空间可分) 设度量空间 $\left(X,d\right)$ 是可分的, $A$ 为 $X$ 的子集, 则度量空间 $\left(A,d\right)$ 也是可分的.

> **例 1.4.1** (开球是开集) 在度量空间 $\left(X,d\right)$ 中, 对于 $x_0\in X,r>0$, 集 $O\left(x_0,r\right)=\left\{x\in X:d\left(x,x_0\right)<r\right\}$ 称为开球, 也叫做 $x_0$ 的 $r$-邻域. 容易看出, 开球 $O\left(x_0,r\right)$ 是开集.

> **注 1.4.1** (稠密子集) (i) 类似地, 可得 $L^p\left(\mathbb R^n\right)\left(1\le p<\infty\right)$ 中的简单函数全体, 阶梯函数全体以及 $C_c^\infty\left(\mathbb R^n\right)$ 均是稠密子集.<br>(ii) 然而, 在 $L^\infty\left[a,b\right]$ 中, 只有简单函数全体是稠密子集.

> **定理 1.4.2** (有限维的赋范线性空间是完备的) 有限维的赋范线性空间是完备的. 在证明中, 断言存在正实数 $c_1,c_2$, 使得对于 $X$ 中的每个 $x=\sum_{i=1}^n x_i e_i$, 成立 $$ c_1\sqrt{\sum_{i=1}^n\left|x_i\right|^2}\le\left\|x\right\|\le c_2\sqrt{\sum_{i=1}^n\left|x_i\right|^2}. \quad \left(1.21\right) $$

> **例 1.4.2** (闭球是闭集) 在度量空间 $\left(X,d\right)$ 中, 对于 $x_0\in X,r>0$, 集 $B\left(x_0,r\right)=\left\{x\in X:d\left(x,x_0\right)\le r\right\}$ 称为闭球. 显然闭球 $B\left(x_0,r\right)$ 是闭集.

> **定义 1.4.3** (极限点, 导集, 闭包与闭集) 设 $X$ 是度量空间, $A$ 是 $X$ 的子集.<br>(i) 设 $x_0\in X$, 如果存在一点列 $\left\{x_n\right\}_{n=1}^\infty$ 使得 $x_n\ne x_0$ 且 $x_n\to x_0$, 那么称 $x_0$ 是点集 $A$ 的极限点;<br>(ii) $A$ 的极限点全体构成的集称为 $A$ 的导集, 记作 $A'$. 称 $\overline A=A\cup A'$ 是 $A$ 的闭包;<br>(iii) 如果集合 $A$ 的极限点全体 $A'$ 都包含在 $A$ 中, 就称 $A$ 为闭集.

> **例 1.4.3** (距离函数连续) 设 $F$ 是度量空间 $\left(X,d\right)$ 的非空子集, 定义距离函数 $d\left(x,F\right)=\inf_{z\in F}d\left(x,z\right)$. 由度量的三角不等式可得 $$ \left|d\left(x_1,F\right)-d\left(x_2,F\right)\right|\le d\left(x_1,x_2\right), $$ 故 $x\mapsto d\left(x,F\right)$ 是 $X$ 上的连续函数. 显然它还是一致连续的.

> **定义 1.4.5** (稠密性) 在度量空间 $\left(X,d\right)$ 中, 对于 $B$ 中一个子集 $A$, 我们称 $A$ 在 $B$ 中稠密是指 $B\subset\overline A$.

> **例 1.4.5** (魏尔斯特拉斯第一逼近定理) 对直线上的有界闭区间 $\left[a,b\right]$, 由数学分析中的魏尔斯特拉斯第一逼近定理, 多项式全体 $P$ 在 $C\left[a,b\right]$ 中是稠密的.

> **定义 1.4.6** (可分性) 设 $X$ 是度量空间. 如果存在某个可数子集在 $X$ 中稠密, 就称 $X$ 是**可分空间**.

> **例 1.4.6** ($L^p$ 中的稠密子集) 对直线上有界闭区间 $\left[a,b\right]$ 及 $1\le p<\infty$, $L^p\left[a,b\right]$ 中的简单函数全体, 阶梯函数全体, $C_c^\infty\left(a,b\right)$, $C\left[a,b\right]$ 以及多项式全体 $P$ 均是 $L^p\left[a,b\right]$ 的稠密子集.

> **定义 1.4.7** (完备性) 设 $\left(X,d\right)$ 是度量空间.<br>(i) 设 $\left\{x_n\right\}_{n=1}^\infty$ 是 $X$ 中的点列. 如果对于任一正数 $\varepsilon$, 存在正整数 $N$, 使得当 $n,m\ge N$ 时, $d\left(x_n,x_m\right)<\varepsilon$, 就称 $\left\{x_n\right\}_{n=1}^\infty$ 是 $X$ 中的**基本点列**, 或者称为柯西点列;<br>(ii) 若度量空间 $X$ 中每个基本点列都收敛, 则称 $X$ 是**完备度量空间**;<br>(iii) 完备的赋范线性空间称为**巴拿赫空间**;<br>(iv) 完备的内积空间称为**希尔伯特空间**;<br>(v) 设 $A$ 是 $X$ 的子空间, 如果 $A$ 作为度量空间是完备的, 那么称 $A$ 是 $X$ 的**完备子空间**.

> **例 1.4.9** ($C$ 与 $L^p$ 的可分性) $C\left[a,b\right]$ 和 $L^p\left[a,b\right]\left(1\le p<\infty\right)$ 是可分空间.

> **例 1.4.10** ($l^\infty$ 不可分) 有界数列全体组成的空间 $l^\infty$ 是不可分的.

> **例 1.4.11** ($L^\infty$ 不可分) 空间 $L^\infty\left[a,b\right]$ 是不可分的.

> **例 1.4.13** ($L^p\left(E\right)$ 是巴拿赫空间) 设 $E$ 是 $\mathbb R^n$ 的一个勒贝格可测集, 则空间 $L^p\left(E\right)\left(1\le p<\infty\right)$ 是巴拿赫空间. 特别地, $L^2\left(E\right)$ 是希尔伯特空间.

> **定义 1.5.1** (不动点) 设 $X$ 为一集合, $\varphi$ 是 $X$ 到自身的映射. 如果 $x^*\in X$, 使得 $\varphi\left(x^*\right)=x^*$, 那么称 $x^*$ 为映射 $\varphi$ 的一个不动点.

> **定理 1.5.1** (巴拿赫) 完备度量空间 $X$ 到自身的压缩映射 $\varphi$ 有唯一不动点.

> **注 1.5.1** (迭代法) 不动点定理的证明不仅给出了压缩映射的不动点的存在性和唯一性, 同时也提供了求不动点的一种方法 — 迭代法. 就是说, 在完备度量空间中, 从任取的"初值" $x_0$ 出发, 逐次作点列 $x_n=\varphi^n\left(x_0\right),n=1,2,\cdots$, 它收敛到方程 $\varphi\left(x\right)=x$ 的解. 这种方法也称为逐次逼近法. 并且在 $\left(1.24\right)$ 式中令 $p\to\infty$, 得到 $$ d\left(x^*,x_n\right)\le\frac{\alpha^n}{1-\alpha}d\left(x_1,x_0\right). \quad \left(1.25\right) $$

> **定义 1.5.2** (压缩映射) 设 $\left(X,d\right)$ 是度量空间, $\varphi$ 是 $X$ 到它自身的一个映射, 如果存在数 $\alpha$, $0\le\alpha<1$, 使得对一切 $x,y\in X$, 成立 $$ d\left(\varphi\left(x\right),\varphi\left(y\right)\right)\le\alpha d\left(x,y\right), $$ 就称 $\varphi$ 是 $X$ 上的压缩映射, 对于线性空间 $X$ 上的情况往往称之为压缩算子.

> **定理 1.5.2** ($\varphi^n$ 压缩 $\Rightarrow$ 唯一不动点) 设度量空间 $X$ 是完备的, $\varphi$ 是 $X$ 到自身的映射. 如果存在一个自然数 $n$ 使得 $\varphi^n$ 是 $X$ 上的压缩映射, 那么映射 $\varphi$ 在 $X$ 中有唯一的不动点.

> **定理 1.5.3** (初值问题解的存在唯一性) 假设 $f\left(x,y\right)$ 是平面上某单连通区域 $D$ 上的二元连续函数, 我们考虑一阶常微分方程初值问题 $$\frac{\mathrm dy}{\mathrm dx}=f\left(x,y\right),\quad y|_{x=x_0}=y_0. \quad \left(1.28\right)$$ 假设 $f\left(x,y\right)$ 在 $D$ 的一个矩形子集 $D=\left\{\left(x,y\right):\left|x-x_0\right|\le a,\left|y-y_0\right|\le\lambda\right\}$ 上对 $y$ 满足利普希茨条件, 即存在常数 $L>0$, 使得当 $\left(x,y_i\right)\in D\left(i=1,2\right)$ 时, $\left|f\left(x,y_1\right)-f\left(x,y_2\right)\right|\le L\left|y_1-y_2\right|$, 记 $M=\max_{\left(x,y\right)\in D}\left|f\left(x,y\right)\right|$, 则当 $h<\min\left\{a,\frac{\lambda}{M},\frac{1}{L}\right\}$ 时, 初值问题 (1.28) 在区间 $\left[x_0-h,x_0+h\right]$ 上有唯一解.

> **例 1.6.1** ($\mathbb R^n$ 中有界集相对列紧) 由波尔查诺-魏尔斯特拉斯定理, $\mathbb R^n$ (或 $\mathbb C^n$)中的子集 $A$ 是相对列紧集等价于 $A$ 是有界的. 再由定理 1.4.2 的讨论知, 对任意的有限维赋范线性空间 $X$, 它的子集 $A$ 是相对列紧集等价于 $A$ 是有界集.

> **推论 1.6.3** (紧集上连续函数达到上下确界) 度量空间 $X$ 的紧子集 $K$ 上的连续函数 $f$ 是有界的, 且上, 下确界可达.

> **闵可夫斯基不等式** 对于勒贝格测度空间 $\left(\mathbb R^n,\mathrm dm\right)$ 中的可测集 $E$ 和其上的勒贝格可测函数 $f,g$, 若 $f,g$ 是 $p$ 次可积的, 其中 $p\ge1$, 则 $$ \left(\int_E \left|f\left(t\right)+g\left(t\right)\right|^p \mathrm dm\left(t\right)\right)^{\frac1p}\le\left(\int_E \left|f\left(t\right)\right|^p \mathrm dm\left(t\right)\right)^{\frac1p}+\left(\int_E \left|g\left(t\right)\right|^p \mathrm dm\left(t\right)\right)^{\frac1p}. \quad \left(1.6\right) $$

> **定义** (巴拿赫空间) 若赋范线性空间 $X$ 在诱导度量 $d\left(x,y\right)=\left\|x-y\right\|$ 下是完备的, 则称 $X$ 是**巴拿赫空间**.

---

## 1 (有限维赋范线性空间与 $\mathbb R^n$ 的等价)

设 $X$ 是 $n$ 维赋范线性空间 (数域为 $\mathbb R$), 证明 $X$ 与 $\mathbb R^n$ 在范数意义下等价.

### 解答 1

欲证明 $X$ 与 $\mathbb R^n$ 在范数意义下等价. 依据**定理 1.4.2** (有限维的赋范线性空间是完备的) 证明中的式 (1.21), 即证明存在正实数 $c_1,c_2$, 使得对 $X$ 中每个 $x=\sum_{i=1}^n x_i e_i$ 成立

$$
c_1\sqrt{\sum_{i=1}^n\left|x_i\right|^2}\le\left\|x\right\|\le c_2\sqrt{\sum_{i=1}^n\left|x_i\right|^2}. \quad \left(1.21\right)
$$

**第一步: 建立坐标同构.** 由 $X$ 是 $n$ 维线性空间, 依据**定义 1.2.1 (哈梅尔基与维数)**, 取 $X$ 的一组基 $e_1,e_2,\cdots,e_n$. 定义映射

$$
T\colon\mathbb R^n\to X,\quad T\left(\left(x_1,x_2,\cdots,x_n\right)\right)=\sum_{i=1}^n x_i e_i.
$$

由于 $\left\{e_i\right\}$ 是基, $T$ 是 $\mathbb R^n$ 到 $X$ 上的一一对应.

**第二步: 下界估计.** 在 $\mathbb R^n$ 的单位球面 $S^{n-1}=\left\{\left(x_i\right):\sum_{i=1}^n x_i^2=1\right\}$ 上作函数

$$
f\left(\left(x_i\right)\right)=\left\|T\left(\left(x_i\right)\right)\right\|=\left\|\sum_{i=1}^n x_i e_i\right\|.
$$

由**定义 1.2.2** (半范数与范数) 的注, 范数 $\left\|\cdot\right\|$ 在度量诱导的拓扑下连续; 而 $T$ 是线性映射, 故 $f$ 是 $\mathbb R^n$ 上的连续函数. 又 $S^{n-1}$ 是 $\mathbb R^n$ 中的有界闭集, 依据**例 1.6.1** ($\mathbb R^n$ 中子集相对列紧等价于有界, 闭的相对列紧集即紧集), $S^{n-1}$ 是紧集. 故由**推论 1.6.3** (紧集上连续函数达到上下确界), 连续函数 $f$ 在 $S^{n-1}$ 上达到下确界, 即存在 $\left(x_i^0\right)\in S^{n-1}$ 使 $f\ge f\left(\left(x_i^0\right)\right)$ 于 $S^{n-1}$ 上. 因 $\left\{e_i\right\}$ 线性无关, $\sum_{i=1}^n x_i e_i\ne0$ 对一切 $\left(x_i\right)\ne0$ 成立, 特别在 $S^{n-1}$ 上 $f>0$, 记 $c_1=f\left(\left(x_i^0\right)\right)>0$, 则对一切 $\left(x_i\right)\in S^{n-1}$ 有 $f\left(\left(x_i\right)\right)\ge c_1$. 再由齐性 (**定义 1.2.2 (ii)** (半范数与范数))对任意 $\left(x_i\right)\ne0$ 有

$$
\left\|T\left(\left(x_i\right)\right)\right\|\ge c_1\left\|\left(x_i\right)\right\|_2,
$$

此式对 $\left(x_i\right)=0$ 也平凡成立.

**第三步: 上界估计.** 同理, 由**推论 1.6.3** (紧集上连续函数达到上下确界), 连续函数 $f$ 在 $S^{n-1}$ 上达到上确界, 即存在 $\left(x_i^1\right)\in S^{n-1}$ 使 $f\le f\left(\left(x_i^1\right)\right)$ 于 $S^{n-1}$ 上. 记 $c_2=f\left(\left(x_i^1\right)\right)$ 为 $f$ 在 $S^{n-1}$ 的上确界, 则对一切 $\left(x_i\right)\in S^{n-1}$ 有 $f\left(\left(x_i\right)\right)\le c_2$. 再由齐性 (**定义 1.2.2 (ii)** (半范数与范数))对任意 $\left(x_i\right)\ne0$ 有

$$
\left\|T\left(\left(x_i\right)\right)\right\|\le c_2\left\|\left(x_i\right)\right\|_2,
$$

此式对 $\left(x_i\right)=0$ 也平凡成立.

**第四步: 结论.** 由第二, 三步得

$$
c_1\left\|\left(x_i\right)\right\|_2\le\left\|T\left(\left(x_i\right)\right)\right\|\le c_2\left\|\left(x_i\right)\right\|_2,
$$

即 $X$ 上的范数与 $\mathbb R^n$ 上的欧几里得范数互相控制, 这正是**定理 1.4.2** (有限维的赋范线性空间是完备的) 证明中的式 (1.21). $\blacksquare$

> 实际上, 本题正是书中**定理 1.4.2** (有限维的赋范线性空间是完备的)证明中首先确立的事实; 由上述等价及 $\mathbb R^n$ 的完备性, 也可立即得到 $X$ 的完备性.

---

## 2 (习题 1.4)

### 2. 习题 1.4-2

设 $B$ 是度量空间中的闭集, 证明存在一个递减开集列 $\left\{O_1,O_2,\cdots,O_n,\cdots\right\}$, 使得每个 $O_n$ 包含 $B$ 且 $\bigcap_{n=1}^{\infty}O_n=B$.

#### 解答 1.4-2

对每个正整数 $n$, 令

$$
O_n=\left\{x\in X:d\left(x,B\right)<\frac1n\right\}.
$$

**第一步: 每个 $O_n$ 是开集.** 由**例 1.4.3** (距离函数连续), 函数 $x\mapsto d\left(x,B\right)$ 是连续的. 而开区间 $\left(-\infty,\frac1n\right)$ 是 $\mathbb R$ 中的开集, 依据**定理 1.4.1 (iii)** (连续映射把开集的原像映为开集), $O_n=\left(d\left(\cdot,B\right)\right)^{-1}\left(\left(-\infty,\frac1n\right)\right)$ 是 $X$ 中的开集.

**第二步: $\left\{O_n\right\}$ 递减.** 因 $\frac1n$ 随 $n$ 递减, 故 $d\left(x,B\right)<\frac1{n+1}$ 能推出 $d\left(x,B\right)<\frac1n$, 即 $O_{n+1}\subset O_n$, 故 $\left\{O_n\right\}$ 是递减开集列.

**第三步: $B\subset O_n$ ($\forall n$).** 对 $x\in B$, $d\left(x,B\right)=\inf_{z\in B}d\left(x,z\right)=0<\frac1n$, 故 $x\in O_n$.

**第四步: $\bigcap_{n=1}^\infty O_n\subset B$.** 设 $x\in\bigcap_{n=1}^\infty O_n$, 则 $d\left(x,B\right)<\frac1n$ 对一切 $n$ 成立, 故 $d\left(x,B\right)=0$. 于是对每个 $n$, 由 $d\left(x,B\right)=0=\inf$, 存在 $z_n\in B$ 使 $d\left(x,z_n\right)<\frac1n$, 故 $z_n\to x$. 依据**定义 1.4.3 (ii)** (极限点, 导集, 闭包与闭集), $x$ 是 $B$ 的极限点, 故 $x\in B'$; 又 $B$ 是闭集, 由**定义 1.4.3 (iii)** (极限点, 导集, 闭包与闭集), $B'\subset B$, 故 $x\in B$.

综上, $\left\{O_n\right\}$ 是递减开集列, 每个 $O_n$ 包含 $B$, 且由第三步与第四步得 $\bigcap_{n=1}^\infty O_n=B$. $\blacksquare$

---

### 4. 习题 1.4-4

设 $E,F$ 是度量空间 $X$ 中的两个子集并且 $d\left(E,F\right)\stackrel{\text{def}}{=}\inf_{x\in E,y\in F}d\left(x,y\right)>0$. 证明: 存在两个互不相交的开集 $O_1,O_2$ 分别包含 $E$ 和 $F$.

#### 解答 1.4-4

记 $\delta=d\left(E,F\right)>0$, 令

$$
O_1=\left\{x\in X:d\left(x,E\right)<\frac{\delta}{2}\right\},\quad
O_2=\left\{x\in X:d\left(x,F\right)<\frac{\delta}{2}\right\}.
$$

**第一步: $O_1,O_2$ 是开集.** 由**例 1.4.3** (距离函数连续), $x\mapsto d\left(x,E\right)$ 与 $x\mapsto d\left(x,F\right)$ 连续; 再由**定理 1.4.1 (iii)** (连续映射的等价条件), 开区间 $\left(-\infty,\frac{\delta}{2}\right)$ 的原像 $O_1,O_2$ 是 $X$ 中的开集.

**第二步: $E\subset O_1$, $F\subset O_2$.** 对 $x\in E$, $d\left(x,E\right)=\inf_{z\in E}d\left(x,z\right)\le d\left(x,x\right)=0$, 故 $d\left(x,E\right)=0<\frac{\delta}{2}$, 即 $x\in O_1$; 同理 $F\subset O_2$.

**第三步: $O_1\cap O_2=\varnothing$.** 反设 $x\in O_1\cap O_2$, 则 $d\left(x,E\right)<\frac{\delta}{2}$ 且 $d\left(x,F\right)<\frac{\delta}{2}$. 由下确界的定义, 存在 $y\in E$ 与 $z\in F$ 使得 $d\left(x,y\right)<\frac{\delta}{2}$, $d\left(x,z\right)<\frac{\delta}{2}$. 由度量的三角不等式 (**定义 1.1.1 (iii)** (度量空间)),

$$
d\left(y,z\right)\le d\left(y,x\right)+d\left(x,z\right)<\frac{\delta}{2}+\frac{\delta}{2}=\delta,
$$

这与 $\delta=\inf_{x\in E,y\in F}d\left(x,y\right)\le d\left(y,z\right)$ 矛盾. 故 $O_1\cap O_2=\varnothing$.

故存在互不相交的开集 $O_1,O_2$ 分别包含 $E,F$. $\blacksquare$

---

### 5. 习题 1.4-5

设 $f\left(x\right)$ 是度量空间 $X$ 上的实函数. 如果对于任意点 $x_0\in X$, 有

$$
\lim_{r\to0}\sup_{x\in O\left(x_0,r\right)}f\left(x\right)\le f\left(x_0\right),
$$

就称 $f\left(x\right)$ 在 $X$ 上是**上半连续**的. 证明: 当 $f\left(x\right)$ 是 $X$ 上的上半连续函数时, 对任何常数 $a$, 集合 $X\left(f\ge a\right)\stackrel{\text{def}}{=}\left\{x:f\left(x\right)\ge a\right\}$ 是闭集. 反之也真.

#### 解答 1.4-5

**先证 $\Rightarrow$ (上半连续 $\Rightarrow$ $X\left(f\ge a\right)$ 闭).** 设 $f$ 上半连续, 固定 $a$. 我们用"闭集 $\Leftrightarrow$ 补集为开集"(**集合论的直接事实**)来证明. 设 $x_0\notin X\left(f\ge a\right)$, 即 $f\left(x_0\right)<a$. 记

$$
\overline{\lim_{x\to x_0}}f\left(x\right)\stackrel{\text{def}}{=}\lim_{r\to0}\sup_{x\in O\left(x_0,r\right)}f\left(x\right)\le f\left(x_0\right)<a.
$$

由于 $\lim_{r\to0}\sup_{x\in O\left(x_0,r\right)}f\left(x\right)<a$, 存在 $r_0>0$ 使 $\sup_{x\in O\left(x_0,r_0\right)}f\left(x\right)<a$, 即对一切 $x\in O\left(x_0,r_0\right)$ 有 $f\left(x\right)<a$, 故 $O\left(x_0,r_0\right)\subset X\setminus X\left(f\ge a\right)$. 由**例 1.4.1** (开球是开集), $O\left(x_0,r_0\right)$ 是开集, 故 $x_0$ 是 $X\setminus X\left(f\ge a\right)$ 的内点 (**定义 1.4.1 (i)** (内点, 内部与开集)). 由于 $x_0$ 任取, $X\setminus X\left(f\ge a\right)$ 是开集, 故 $X\left(f\ge a\right)$ 是闭集.

**再证 $\Leftarrow$ ($X\left(f\ge a\right)$ 对一切 $a$ 闭 $\Rightarrow$ 上半连续).** 固定 $x_0$, 对任意 $a>f\left(x_0\right)$, 因 $f\left(x_0\right)<a$, 故 $x_0\notin X\left(f\ge a\right)$. 由 $X\left(f\ge a\right)$ 闭, 其补集 $X\setminus X\left(f\ge a\right)$ 是开集, 而 $x_0$ 属于该开集, 依据**定义 1.4.1 (i)** (内点, 内部与开集) 与**例 1.4.1** (开球是开集), 存在 $r_0>0$ 使 $O\left(x_0,r_0\right)\subset X\setminus X\left(f\ge a\right)$, 即对一切 $x\in O\left(x_0,r_0\right)$ 有 $f\left(x\right)<a$, 故 $\sup_{x\in O\left(x_0,r_0\right)}f\left(x\right)\le a$. 于是

$$
\lim_{r\to0}\sup_{x\in O\left(x_0,r\right)}f\left(x\right)=\inf_{r>0}\sup_{x\in O\left(x_0,r\right)}f\left(x\right)\le\sup_{x\in O\left(x_0,r_0\right)}f\left(x\right)\le a.
$$

由于这对一切 $a>f\left(x_0\right)$ 成立, 令 $a\downarrow f\left(x_0\right)$ 得 $\lim_{r\to0}\sup_{x\in O\left(x_0,r\right)}f\left(x\right)\le f\left(x_0\right)$, 故 $f$ 上半连续. $\blacksquare$

---

### 7. 习题 1.4-7

设 $X$ 是可分的度量空间, $A\subset X$, $\left\{O_\lambda:\lambda\in\Lambda\right\}$ 是 $A$ 的开覆盖. 证明: 可从 $\left\{O_\lambda:\lambda\in\Lambda\right\}$ 中选出至多可列个开集 $\left\{O_{\lambda_n}\right\}$, 使得 $\bigcup_n O_{\lambda_n}\supset A$.

#### 解答 1.4-7

**第一步: 取可数稠密子集.** 因 $X$ 可分, 依据**定义 1.4.6 (可分性)**, 存在可数子集 $D=\left\{x_1,x_2,\cdots\right\}$ 在 $X$ 中稠密, 即依据**定义 1.4.5 (稠密性)**, $\overline D=X$.

**第二步: 一族可数开球构成"开基".** 我们证明: 对任意开集 $G$ 及 $x\in G$, 存在 $x_n\in D$ 与正有理数 $r$ 使 $x\in O\left(x_n,r\right)\subset G$. 事实上, 由**定义 1.4.1 (i)** (内点, 内部与开集), 存在 $\varepsilon>0$ 使 $O\left(x,\varepsilon\right)\subset G$. 由 $\overline D=X$ 及 $x\in X$, 存在 $x_n\in D$ 使 $d\left(x,x_n\right)<\frac{\varepsilon}{2}$ (否则 $x$ 不是 $D$ 的极限点也不属于 $D$, 矛盾); 取有理数 $r$ 满足 $d\left(x,x_n\right)<r<\frac{\varepsilon}{2}$ (有理数在 $\mathbb R$ 中稠密), 则对 $y\in O\left(x_n,r\right)$, 由三角不等式 $d\left(y,x\right)\le d\left(y,x_n\right)+d\left(x_n,x\right)<r+\frac{\varepsilon}{2}<\varepsilon$, 故 $O\left(x_n,r\right)\subset O\left(x,\varepsilon\right)\subset G$, 且 $x\in O\left(x_n,r\right)$.

**第三步: 构造至多可列子覆盖.** 考虑可数族

$$
\mathscr B=\left\{O\left(x_n,r\right):n=1,2,\cdots;\ r\in\mathbb Q,\ r>0\right\}.
$$

对每个 $B\in\mathscr B$, 若存在 $\lambda\in\Lambda$ 使 $B\subset O_\lambda$ 且 $B\cap A\ne\varnothing$, 则任取一个这样的 $\lambda$, 记为 $\lambda_B$. 令 $\mathscr B'=\left\{B\in\mathscr B:\text{存在}\ \lambda_B\right\}$, 则 $\left\{O_{\lambda_B}:B\in\mathscr B'\right\}$ 至多可列 (因为 $\mathscr B$ 可数).

对任意 $x\in A$, 因 $\left\{O_\lambda\right\}$ 是 $A$ 的开覆盖, 存在 $\lambda$ 使 $x\in O_\lambda$, 且 $O_\lambda$ 是开集. 由第二步, 存在 $B=O\left(x_n,r\right)\in\mathscr B$ 使 $x\in B\subset O_\lambda$, 且 $B\cap A\ni x\ne\varnothing$, 故 $B\in\mathscr B'$ 且 $x\in B\subset O_{\lambda_B}$. 因此 $\bigcup_{B\in\mathscr B'}O_{\lambda_B}\supset A$, 即从 $\left\{O_\lambda\right\}$ 中选出了至多可列个开集覆盖 $A$. $\blacksquare$

---

### 9. 习题 1.4-9

对 $1\le p<\infty$, 定义巴拿赫空间

$$
L^p\left(\mathbb R,\mathrm e^{-t^2}\mathrm dt\right)=\left\{f\text{ 在 }\mathbb R\text{ 上勒贝格可测}:\left\|f\right\|_p=\left(\int_{\mathbb R}\left|f\left(t\right)\right|^p\mathrm e^{-t^2}\mathrm dt\right)^{1/p}<\infty\right\}.
$$

证明: $C_c^\infty\left(\mathbb R\right)$ 在 $L^p\left(\mathbb R,\mathrm e^{-t^2}\mathrm dt\right)$ 中稠密. 判断多项式全体是否为稠密集 (无须证明).

#### 解答 1.4-9

**第一步: 化归为支集有界.** 对 $f\in L^p\left(\mathbb R,\mathrm e^{-t^2}\mathrm dt\right)$, 令 $f_N=f\cdot\chi_{\left[-N,N\right]}$. 由**数学分析**可知 $\left|f\right|^p\mathrm e^{-t^2}\in L^1\left(\mathbb R\right)$, 其无穷远尾积分趋于 $0$, 即

$$
\left\|f-f_N\right\|_p^p=\int_{\left|t\right|>N}\left|f\left(t\right)\right|^p\mathrm e^{-t^2}\mathrm dt\to0\quad\left(N\to\infty\right).
$$

故对给定 $\varepsilon>0$, 取 $N$ 使 $\left\|f-f_N\right\|_p<\frac{\varepsilon}{2}$.

**第二步: 支集有界的函数可用 $C_c^\infty$ 逼近.** 对 $t\in\left[-N,N\right]$, 有 $\mathrm e^{-t^2}\le1$, 故对任意勒贝格可测 $g$,

$$
\int_{\mathbb R}\left|g\right|^p\mathrm e^{-t^2}\mathrm dt\le\int_{\mathbb R}\left|g\right|^p\mathrm dt.
$$

特别地, 对 $f_N$ (支集含于 $\left[-N,N\right]$), 在 $\left[-N,N\right]$ 上 $\mathrm e^{-t^2}\ge\mathrm e^{-N^2}>0$, 故 $\int_{\mathbb R}\left|f_N\right|^p\mathrm dt\le\mathrm e^{N^2}\int_{\mathbb R}\left|f_N\right|^p\mathrm e^{-t^2}\mathrm dt\le\mathrm e^{N^2}\int_{\mathbb R}\left|f\right|^p\mathrm e^{-t^2}\mathrm dt<\infty$, 故 $f_N\in L^p\left(\mathbb R\right)$. 由**注 1.4.1 (i)** (稠密子集), $C_c^\infty\left(\mathbb R\right)$ 在 $L^p\left(\mathbb R\right)$ 中稠密, 依据**定义 1.4.5 (稠密性)**, 存在 $\varphi\in C_c^\infty\left(\mathbb R\right)$ 使 $\left\|f_N-\varphi\right\|_{L^p\left(\mathbb R\right)}<\frac{\varepsilon}{2}$. 再由上述 $\mathrm e^{-t^2}\le1$ 得

$$
\left\|f_N-\varphi\right\|_{L^p\left(\mathbb R,\mathrm e^{-t^2}\mathrm dt\right)}\le\left\|f_N-\varphi\right\|_{L^p\left(\mathbb R\right)}<\frac{\varepsilon}{2}.
$$

**第三步: 合拢.** 由三角不等式 (**定义 1.2.2 (iii)** (半范数与范数)),

$$
\left\|f-\varphi\right\|_p\le\left\|f-f_N\right\|_p+\left\|f_N-\varphi\right\|_p<\frac{\varepsilon}{2}+\frac{\varepsilon}{2}=\varepsilon.
$$

故对任意 $f\in L^p\left(\mathbb R,\mathrm e^{-t^2}\mathrm dt\right)$ 与 $\varepsilon>0$ 存在 $\varphi\in C_c^\infty\left(\mathbb R\right)$ 使 $\left\|f-\varphi\right\|_p<\varepsilon$, 依据**定义 1.4.5** (稠密性), $C_c^\infty\left(\mathbb R\right)$ 在 $L^p\left(\mathbb R,\mathrm e^{-t^2}\mathrm dt\right)$ 中稠密. $\blacksquare$

**关于多项式全体:** 是稠密集. 事实上, 由**例 1.3.9** (埃尔米特多项式构成完备标准正交系), $\psi_n\left(t\right)=\left(2^n n!\sqrt\pi\right)^{-1/2}\mathrm e^{-t^2/2}H_n\left(t\right)$ ($H_n$ 为埃尔米特多项式)组成 $L^2\left(\mathbb R,\mathrm e^{-t^2}\mathrm dm\right)$ 中的完备标准正交系, 而 $\psi_n=\mathrm e^{-t^2/2}\times$ (多项式), 故多项式全体在 $L^2\left(\mathbb R,\mathrm e^{-t^2}\mathrm dt\right)$ 中稠密; 对一般 $1\le p<\infty$ 亦然.

---

### 10. 习题 1.4-10

设 $C_{2\pi}=\left\{f\in C\left[0,2\pi\right]:f\left(0\right)=f\left(2\pi\right)\right\}$, 并按范数 $\left\|f\right\|=\max_{0\le t\le2\pi}\left|f\left(t\right)\right|$ 成一赋范空间. 证明:

(i) 令 $\mathcal P=\left\{f\in C_{2\pi}:\text{存在多项式}\ P\ \text{使得}\ f\left(t\right)=P\left(t\right),\ \forall0\le t\le2\pi\right\}$, 则 $\mathcal P$ 在 $C_{2\pi}$ 中稠密.

(ii) $C_{2\pi}$ 在 $L^p\left[0,2\pi\right]\left(1\le p<\infty\right)$ 中稠密, 但不在 $L^\infty\left[0,2\pi\right]$ 中稠密.

(iii) 将 $C_{2\pi}$ 中函数零延拓为 $\left[0,4\pi\right]$ 上的函数, 则 $C_{2\pi}$ 在 $L^p\left[0,4\pi\right]\left(1\le p<\infty\right)$ 中不稠密.

#### 解答 1.4-10

**(i) $\mathcal P$ 在 $C_{2\pi}$ 中稠密.** 设 $f\in C_{2\pi}$, $\varepsilon>0$. 由**例 1.4.5** (魏尔斯特拉斯第一逼近定理), 多项式全体在 $C\left[0,2\pi\right]$ 中稠密, 故存在多项式 $Q$ 使 $\left\|f-Q\right\|_{C\left[0,2\pi\right]}<\frac{\varepsilon}{4}$. 记 $\delta=Q\left(2\pi\right)-Q\left(0\right)$, 则

$$
\left|\delta\right|\le\left|Q\left(2\pi\right)-f\left(2\pi\right)\right|+\left|f\left(2\pi\right)-f\left(0\right)\right|+\left|f\left(0\right)-Q\left(0\right)\right|<\frac{\varepsilon}{4}+0+\frac{\varepsilon}{4}=\frac{\varepsilon}{2}.
$$

作多项式 $P\left(t\right)=Q\left(t\right)-\frac{\delta}{4\pi^2}t^2$. 则 $P\left(0\right)=Q\left(0\right)$, $P\left(2\pi\right)=Q\left(2\pi\right)-\delta=Q\left(0\right)$, 故 $P\left(0\right)=P\left(2\pi\right)$, 即 $P\in\mathcal P$. 且

$$
\left\|P-Q\right\|_{C\left[0,2\pi\right]}=\max_{0\le t\le2\pi}\left|\frac{\delta}{4\pi^2}t^2\right|=\left|\delta\right|<\frac{\varepsilon}{2},
$$

故 $\left\|f-P\right\|\le\left\|f-Q\right\|+\left\|Q-P\right\|<\frac{\varepsilon}{4}+\frac{\varepsilon}{2}<\varepsilon$. 依据**定义 1.4.5** (稠密性), $\mathcal P$ 在 $C_{2\pi}$ 中稠密. $\blacksquare$

**(ii) $C_{2\pi}$ 在 $L^p\left[0,2\pi\right]$ 中稠密.** 设 $f\in L^p\left[0,2\pi\right]$, $\varepsilon>0$. 由**例 1.4.6** ($L^p$ 中的稠密子集), $C\left[0,2\pi\right]$ 在 $L^p\left[0,2\pi\right]$ 中稠密, 故存在 $g\in C\left[0,2\pi\right]$ 使 $\left\|f-g\right\|_p<\frac{\varepsilon}{2}$. 现在把 $g$ 在端点处稍作修改以令其满足 $h\left(0\right)=h\left(2\pi\right)$: 取 $\eta>0$ 充分小, 令

$$
h\left(t\right)=\begin{cases}
\left(1-\frac{t}{\eta}\right)g\left(2\pi\right)+\frac{t}{\eta}g\left(\eta\right),&0\le t<\eta,\\
g\left(t\right),&\eta\le t\le2\pi,
\end{cases}
$$

则 $h$ 连续, $h\left(0\right)=g\left(2\pi\right)$, $h\left(2\pi\right)=g\left(2\pi\right)$, 故 $h\left(0\right)=h\left(2\pi\right)$, 即 $h\in C_{2\pi}$. 又 $g,h$ 在 $\left[0,\eta\right]$ 上均有界 (设 $\left|g\right|,\left|h\right|\le M$), 故 $\left\|g-h\right\|_p^p\le\int_0^\eta\left(2M\right)^p\mathrm dt=\left(2M\right)^p\eta$, 取 $\eta$ 足够小使 $\left\|g-h\right\|_p<\frac{\varepsilon}{2}$. 于是

$$
\left\|f-h\right\|_p\le\left\|f-g\right\|_p+\left\|g-h\right\|_p<\varepsilon.
$$

依据**定义 1.4.5** (稠密性), $C_{2\pi}$ 在 $L^p\left[0,2\pi\right]$ 中稠密. $\blacksquare$

**(ii) $C_{2\pi}$ 不在 $L^\infty\left[0,2\pi\right]$ 中稠密.** $C_{2\pi}\subset C\left[0,2\pi\right]$, 由**例 1.4.9** ($C$ 与 $L^p$ 的可分性), $C\left[0,2\pi\right]$ 可分; 再由**命题 1.4.1** (可分空间的子空间可分), 其子空间 $C_{2\pi}$ 可分, 故存在可数子集 $D$ 在 $C_{2\pi}$ 中稠密. 若 $C_{2\pi}$ 在 $L^\infty\left[0,2\pi\right]$ 中稠密, 则 $D$ 也在 $L^\infty\left[0,2\pi\right]$ 中稠密 (**稠密的稠密仍稠密**, 证明详见后文), 即 $L^\infty\left[0,2\pi\right]$ 可分, 这与**例 1.4.11** ($L^\infty\left[a,b\right]$ 不可分)矛盾. 故 $C_{2\pi}$ 不在 $L^\infty\left[0,2\pi\right]$ 中稠密. $\blacksquare$

**(iii) 零延拓不稠.** 记 $Z=\left\{\widetilde f:f\in C_{2\pi}\right\}$, 其中 $\widetilde f$ 是 $f$ 零延拓到 $\left[0,4\pi\right]$ 的函数, 则 $\widetilde f\equiv0$ 于 $\left(2\pi,4\pi\right]$. 取 $h=\chi_{\left[3\pi,4\pi\right]}\in L^p\left[0,4\pi\right]$. 对任意 $\widetilde f\in Z$, 因 $\widetilde f\equiv0$ 于 $\left(2\pi,4\pi\right]$,

$$
\left\|h-\widetilde f\right\|_p^p\ge\int_{\left[3\pi,4\pi\right]}\left|1-\widetilde f\right|^p\mathrm dt+\int_{\left(2\pi,3\pi\right)}\left|\widetilde f\right|^p\mathrm dt\ge\int_{\left[3\pi,4\pi\right]}1\,\mathrm dt=\pi,
$$

故 $\left\|h-\widetilde f\right\|_p\ge\pi^{1/p}>0$ 对一切 $\widetilde f\in Z$ 成立, 即 $h$ 不在 $Z$ 的闭包中. 依据**定义 1.4.5** (稠密性), $Z$ 在 $L^p\left[0,4\pi\right]$ 中不稠密. $\blacksquare$

---

### 12. 习题 1.4-12

令 $C_b\left(\mathbb R\right)$ 为 $\mathbb R$ 上有界的连续函数全体构成的巴拿赫空间, 它的范数 $\left\|x\right\|=\sup_{t\in\mathbb R}\left|x\left(t\right)\right|$. 令 $C_0\left(\mathbb R\right)=\left\{f\in C_b\left(\mathbb R\right):\lim_{t\to\pm\infty}x\left(t\right)=0\right\}$ 为 $C_b\left(\mathbb R\right)$ 的线性子空间. 证明:

(i) $C_0\left(\mathbb R\right)$ 是可分的.

(ii) $C_b\left(\mathbb R\right)$ 不是可分的.

#### 解答 1.4-12

**(i) $C_0\left(\mathbb R\right)$ 可分.**

**第一步: $C_c\left(\mathbb R\right)$ (紧支撑连续函数)在 $C_0\left(\mathbb R\right)$ 中稠密.** 设 $f\in C_0\left(\mathbb R\right)$, $\varepsilon>0$. 因 $\lim_{t\to\pm\infty}f\left(t\right)=0$, 存在 $M>0$ 使对 $\left|t\right|\ge M$ 有 $\left|f\left(t\right)\right|<\varepsilon$. 取连续函数 $\varphi$ 满足 $0\le\varphi\le1$, $\varphi\equiv1$ 于 $\left[-M,M\right]$, $\varphi\equiv0$ 于 $\left(-\infty,-M-1\right]\cup\left[M+1,\infty\right)$ (例如分段线性函数). 令 $g=f\varphi$, 则 $g\in C_c\left(\mathbb R\right)$, 且 $\left\|f-g\right\|_\infty=\sup_t\left|f\left(t\right)\right|\left|1-\varphi\left(t\right)\right|<\varepsilon$ (在 $\left[-M,M\right]$ 上为 $0$, 在 $\left|t\right|\ge M$ 上 $<\varepsilon$). 依据**定义 1.4.5** (稠密性), $C_c\left(\mathbb R\right)$ 在 $C_0\left(\mathbb R\right)$ 中稠密.

**第二步: $C_c\left(\mathbb R\right)$ 可分.** 记 $C_c\left(\left[-n,n\right]\right)=\left\{f\in C\left[-n,n\right]:\text{支集 }f\subset\left[-n,n\right]\right\}$, 则 $C_c\left(\mathbb R\right)=\bigcup_{n=1}^\infty C_c\left(\left[-n,n\right]\right)$. 由**例 1.4.9** ($C$ 与 $L^p$ 的可分性), $C\left[-n,n\right]$ 可分; 由**命题 1.4.1** (可分空间的子空间可分), 其子空间 $C_c\left(\left[-n,n\right]\right)$ 可分.

**第三步: $C_0\left(\mathbb R\right)$ 可分.** 由前两步, $C_c\left(\mathbb R\right)$ 可分且在 $C_0\left(\mathbb R\right)$ 中稠密; 故设 $\left\{y_k\right\}$ 是 $C_c\left(\mathbb R\right)$ 中的可数稠密子集, 则对任意 $f\in C_0\left(\mathbb R\right)$ 与 $\varepsilon>0$, 先取 $g\in C_c\left(\mathbb R\right)$ 使 $\left\|f-g\right\|<\frac{\varepsilon}{2}$, 再取 $y_k$ 使 $\left\|g-y_k\right\|<\frac{\varepsilon}{2}$, 故 $\left\{y_k\right\}$ 也在 $C_0\left(\mathbb R\right)$ 中稠密, 即 $C_0\left(\mathbb R\right)$ 可分. $\blacksquare$

> 第三步实际上证明了前文结论 (**稠密的稠密仍稠密**).

**(ii) $C_b\left(\mathbb R\right)$ 不可分.**

**第一步: $l^\infty$ 等距嵌入 $C_b\left(\mathbb R\right)$.** 对 $a=\left(a_n\right)_{n\in\mathbb Z}\in l^\infty$, 定义 $f_a\in C_b\left(\mathbb R\right)$ 为分片线性函数: $f_a\left(n\right)=a_n$ ($n\in\mathbb Z$), 且 $f_a$ 在每个区间 $\left[n,n+1\right]$ 上为线性. 则 $f_a$ 连续, 有界, 且 $\left\|f_a\right\|_\infty=\sup_{t\in\mathbb R}\left|f_a\left(t\right)\right|=\sup_{n\in\mathbb Z}\left|a_n\right|=\left\|a\right\|_{l^\infty}$ (**线性组合不放大最大值**), 即 $a\mapsto f_a$ 是 $l^\infty$ 到 $C_b\left(\mathbb R\right)$ 子空间的等距映射.

**第二步: 用反证.** 若 $C_b\left(\mathbb R\right)$ 可分, 则由**命题 1.4.1** (可分空间的子空间可分), 其子空间 (即 $l^\infty$ 的等距像)也可分, 从而 $l^\infty$ 可分, 这与**例 1.4.10** ($l^\infty$ 不可分)矛盾. 故 $C_b\left(\mathbb R\right)$ 不可分. $\blacksquare$

> $C_0\left(\mathbb R\right)$ 可分而 $C_b\left(\mathbb R\right)$ 不可分的原因是, $C_0\left(\mathbb R\right)$ 中的函数在远处必须变小, 自由度有限; 而 $C_0\left(\mathbb R\right)$ 中的函数在远处可以任意大, 自由度太大, 甚至能容下不可分子空间 $l^\infty$, 因此也变得不可分了.

---

### 13. 习题 1.4-13

设 $H$ 是希尔伯特空间, 证明 $H$ 可分等价于 $H$ 存在一组可数的正交基.

#### 解答 1.4-13

**先证 $\Leftarrow$: $H$ 有可数正交基 $\Rightarrow$ $H$ 可分.** 设 $\left\{e_n:n=1,2,\cdots\right\}$ 是 $H$ 的一组可数标准正交基. 由**定理 1.3.2 (ii)** (标准正交基的等价条件), $\overline{\text{span}\left\{e_n\right\}}=H$. 令

$$
D=\left\{\sum_{k=1}^m\left(a_k+\mathrm i b_k\right)e_k:m\ge1,\ a_k,b_k\in\mathbb Q\right\},
$$

则 $D$ 可数. 对任意 $x\in H$ 与 $\varepsilon>0$, 因 $\text{span}\left\{e_n\right\}$ 稠密, 存在有限组合 $y=\sum_{k=1}^m c_k e_k$ 使 $\left\|x-y\right\|<\frac{\varepsilon}{2}$; 又 $\mathbb Q$ 在 $\mathbb R$ 中稠密, 可取 $c'_k=a_k+\mathrm i b_k$ ($a_k,b_k\in\mathbb Q$)使 $\left\|y-\sum_{k=1}^m c'_k e_k\right\|=\left\|\sum_{k=1}^m\left(c_k-c'_k\right)e_k\right\|\le\sum_{k=1}^m\left|c_k-c'_k\right|<\frac{\varepsilon}{2}$. 故 $D$ 在 $H$ 中稠密, 依据**定义 1.4.6** (可分性), $H$ 可分. $\blacksquare$

**再证 $\Rightarrow$: $H$ 可分 $\Rightarrow$ $H$ 有可数正交基.** 由**定理 1.3.3** (标准正交系可扩张为标准正交基) (取 $A=\varnothing$), $H$ 存在一组标准正交基 $\mathcal E=\left\{e_\lambda:\lambda\in\Lambda\right\}$. 我们证明 $\mathcal E$ 可数. 对 $\lambda\ne\mu\in\Lambda$, $e_\lambda\perp e_\mu$ 且 $\left\|e_\lambda\right\|=\left\|e_\mu\right\|=1$, 依据**定理 1.2.2 (勾股定理)**, $\left\|e_\lambda-e_\mu\right\|^2=\left\|e_\lambda\right\|^2+\left\|e_\mu\right\|^2=2$, 故 $\left\|e_\lambda-e_\mu\right\|=\sqrt2$. 因 $H$ 可分, 存在可数稠密子集 $\left\{x_n\right\}$ (**定义 1.4.6** (可分性)). 定义映射 $n\colon\Lambda\to\mathbb N$, 欲证明 $\mathcal E$ 可数只需证明映射 $n\colon\Lambda\to\mathbb N$ 为单射. 则对每个 $\lambda$, 依据**定义 1.4.5** (稠密性) 取 $n\left(\lambda\right)$ 使 $\left\|e_\lambda-x_{n\left(\lambda\right)}\right\|<\frac{1}{3}$. 对于 $n\left(\mu\right)$ 同理. 反证法, 若其不是单射, 即 $n\left(\lambda\right)=n\left(\mu\right)$ 而 $\lambda\ne\mu$, 则

$$
\left\|e_\lambda-e_\mu\right\|\le\left\|e_\lambda-x_{n\left(\lambda\right)}\right\|+\left\|x_{n\left(\mu\right)}-e_\mu\right\|<\frac{1}{3}+\frac{1}{3}=\frac{2}{3},
$$

与 $\left\|e_\lambda-e_\mu\right\|=\sqrt2$ 矛盾. 故 $n\colon\Lambda\to\mathbb N$ 是单射, $\Lambda$ 可数. 于是 $H$ 存在一组可数 (标准)正交基. $\blacksquare$

---

### 14. 习题 1.4-14

(傅里叶变换的黎曼-勒贝格引理)对 $f\in L^1\left(\mathbb R\right)$, 证明:

$$
\lim_{\left|\xi\right|\to\infty}\int_{\mathbb R}f\left(x\right)\mathrm e^{-\mathrm i2\pi\xi x}\mathrm dx=0.
$$

#### 解答 1.4-14

记 $F\left(\xi\right)=\int_{\mathbb R}f\left(x\right)\mathrm e^{-\mathrm i2\pi\xi x}\mathrm dx$.

**第一步: 对区间的特征函数成立.** 对 $f=\chi_{\left[a,b\right]}$, 直接计算

$$
F\left(\xi\right)=\int_a^b\mathrm e^{-\mathrm i2\pi\xi x}\mathrm dx=\frac{\mathrm e^{-\mathrm i2\pi\xi b}-\mathrm e^{-\mathrm i2\pi\xi a}}{-\mathrm i2\pi\xi},
$$

故 $\left|F\left(\xi\right)\right|\le\frac{2}{2\pi\left|\xi\right|}\to0$ ($\left|\xi\right|\to\infty$).

**第二步: 对阶梯函数成立.** 设 $s=\sum_{k=1}^m c_k\chi_{\left[a_k,b_k\right]}$ 是有限个区间特征函数的线性组合 (阶梯函数), 由第一步及线性性, $\int_{\mathbb R}s\left(x\right)\mathrm e^{-\mathrm i2\pi\xi x}\mathrm dx\to0$.

**第三步: 对一般 $f\in L^1\left(\mathbb R\right)$ 成立.** 由**注 1.4.1 (i)** (稠密子集), 阶梯函数全体在 $L^1\left(\mathbb R\right)$ 中稠密, 故对任意 $\varepsilon>0$, 依据**定义 1.4.5** (稠密性) 存在阶梯函数 $s$ 使 $\left\|f-s\right\|_1<\varepsilon$. 于是

$$
\left|F\left(\xi\right)\right|\le\int_{\mathbb R}\left|f-s\right|\mathrm dx+\left|\int_{\mathbb R}s\left(x\right)\mathrm e^{-\mathrm i2\pi\xi x}\mathrm dx\right|<\varepsilon+\left|\int_{\mathbb R}s\left(x\right)\mathrm e^{-\mathrm i2\pi\xi x}\mathrm dx\right|.
$$

由第二步, $\limsup_{\left|\xi\right|\to\infty}\left|F\left(\xi\right)\right|\le\varepsilon$. 因 $\varepsilon>0$ 任意, $\lim_{\left|\xi\right|\to\infty}\left|F\left(\xi\right)\right|=0$. $\blacksquare$

---

### 15. 习题 1.4-15

(平均连续性)对 $f\in L^p\left(\mathbb R\right),1\le p<\infty$, 证明:

$$
\lim_{\left|h\right|\to0}\int_{\mathbb R}\left|f\left(x+h\right)-f\left(x\right)\right|^p\mathrm dx=0.
$$

#### 解答 1.4-15

记平移算子 $\left(\tau_h f\right)\left(x\right)=f\left(x+h\right)$, 并记 $\left\|g\right\|_p=\left(\int_{\mathbb R}\left|g\right|^p\mathrm dx\right)^{1/p}$.

**第一步: 对 $C_c^\infty$ 函数成立.** 设 $\varphi\in C_c^\infty\left(\mathbb R\right)$, 支集含于 $\left[-M,M\right]$. $\varphi$ 在紧集 $\left[-M-1,M+1\right]$ 上连续, 故一致连续 (**紧支集上的连续函数必定一致连续**), 即对任意 $\varepsilon>0$ 存在 $\delta>0$, 当 $\left|h\right|<\delta$ 时 $\sup_x\left|\varphi\left(x+h\right)-\varphi\left(x\right)\right|<\varepsilon$. 对 $\left|h\right|<1$, 被积函数仅在 $\left[-M-1,M+1\right]$ 上可能非零, 故

$$
\left\|\tau_h\varphi-\varphi\right\|_p^p=\int_{\mathbb R}\left|\varphi\left(x+h\right)-\varphi\left(x\right)\right|^p\mathrm dx\le\left(2M+2\right)\varepsilon^p\to0.
$$

即 $\lim_{h\to0}\left\|\tau_h\varphi-\varphi\right\|_p=0$.

**第二步: 对一般 $f\in L^p\left(\mathbb R\right)$ 成立.** 由**注 1.4.1 (i)** (稠密子集), $C_c^\infty\left(\mathbb R\right)$ 在 $L^p\left(\mathbb R\right)$ 中稠密, 故对任意 $\varepsilon>0$, 依据**定义 1.4.5** (稠密性) 存在 $\varphi\in C_c^\infty\left(\mathbb R\right)$ 使 $\left\|f-\varphi\right\|_p<\varepsilon$. 由闵可夫斯基不等式 (式 (1.6))及勒贝格测度的平移不变性 ($\int_{\mathbb R}\left|g\left(x+h\right)\right|^p\mathrm dx=\int_{\mathbb R}\left|g\left(x\right)\right|^p\mathrm dx$),

$$
\left\|\tau_h f-f\right\|_p\le\left\|\tau_h f-\tau_h\varphi\right\|_p+\left\|\tau_h\varphi-\varphi\right\|_p+\left\|\varphi-f\right\|_p=2\left\|f-\varphi\right\|_p+\left\|\tau_h\varphi-\varphi\right\|_p.
$$

令 $h\to0$, 由第一步 $\lim_{h\to0}\left\|\tau_h \varphi-\varphi\right\|_p=0$, 即 $\lim_{\left|h\right|\to0}\int_{\mathbb R}\left|f\left(x+h\right)-f\left(x\right)\right|^p\mathrm dx=0$. $\blacksquare$

---

### 16. 习题 1.4-16

对赋范线性空间 $X$, 证明: $X$ 是完备的当且仅当对任意 $X$ 中点列 $\left\{x_n\right\}$, 当 $\sum_{n=1}^\infty\left\|x_n\right\|<\infty$ 时, $\sum_{n=1}^\infty x_n$ 在 $X$ 中收敛.

#### 解答 1.4-16

**先证 $\Rightarrow$: $X$ 完备且 $\sum\left\|x_n\right\|<\infty$ $\Rightarrow$ $\sum x_n$ 收敛.** 设 $\left\{x_n\right\}$ 满足 $\sum_{n=1}^\infty\left\|x_n\right\|<\infty$, 记部分和 $S_n=\sum_{k=1}^n x_k$. 对 $m>n$, 由范数的三角不等式 (**定义 1.2.2 (iii)** (半范数与范数)),

$$
\left\|S_m-S_n\right\|=\left\|\sum_{k=n+1}^m x_k\right\|\le\sum_{k=n+1}^m\left\|x_k\right\|\le\sum_{k=n+1}^\infty\left\|x_k\right\|\to0\quad\left(n\to\infty\right),
$$

故 $\left\{S_n\right\}$ 是基本点列 (**定义 1.4.7 (i)** (完备性)). 因 $X$ 完备, $\left\{S_n\right\}$ 收敛, 即 $\sum_{n=1}^\infty x_n$ 收敛. $\blacksquare$

**再证 $\Leftarrow$: 对任意 $\sum\left\|x_n\right\|<\infty$ 的 $\left\{x_n\right\}$, $\sum x_n$ 收敛 $\Rightarrow$ $X$ 完备.** 设 $\left\{y_n\right\}$ 是 $X$ 中基本点列. 依次取子列 $y_{n_1}<y_{n_2}<\cdots$ (下指标递增)使

$$
\left\|y_{n_{k+1}}-y_{n_k}\right\|<\frac{1}{2^k},\quad k=1,2,\cdots
$$

(由基本点列性质, **定义 1.4.7 (i)** (完备性), 可行). 令 $z_1=y_{n_1}$, $z_k=y_{n_k}-y_{n_{k-1}}$ ($k\ge2$), 则 $\sum_{k=1}^\infty\left\|z_k\right\|<\infty$ (几何级数收敛), 故由假设级数 $\sum_{k=1}^\infty z_k$ 收敛, 其部分和恰为 $y_{n_m}$, 故子列 $\left\{y_{n_m}\right\}$ 收敛于某点 $x\in X$. 由**引理 1.4.1 (ii)** (基本点列与完备性), 基本点列 $\left\{y_n\right\}$ 有收敛子列则自身收敛于 $x$, 故 $X$ 中每个基本点列收敛, 即 $X$ 完备. $\blacksquare$

---

### 18. 习题 1.4-18

设 $H$ 是直线上勒贝格平方可积, 且导函数也平方可积的绝对连续函数全体. 按通常的线性运算及范数

$$
\left\|f\right\|=\sqrt{\int_{\mathbb R}\left|f\left(t\right)\right|^2\mathrm dt+\int_{\mathbb R}\left|f'\left(t\right)\right|^2\mathrm dt},
$$

$H$ 成为赋范线性空间. 证明: $H$ 是希尔伯特空间.

#### 解答 1.4-18

**第一步: $H$ 是内积空间.** 对 $f,g\in H$, 定义 $\left\langle f,g\right\rangle=\int_{\mathbb R}f\left(t\right)\overline{g\left(t\right)}\mathrm dt+\int_{\mathbb R}f'\left(t\right)\overline{g'\left(t\right)}\mathrm dt$. 由 $f,f'\in L^2\left(\mathbb R\right)$ 及柯西-施瓦茨不等式 (**引理 1.2.3** 在 $L^2$ 上的情形), $\left\langle f,g\right\rangle$ 有限, 且显然满足**定义 1.2.3** (内积空间) 的内积三条件, 其中正定性由 $\left\langle f,f\right\rangle=0\Rightarrow f=f'=0$ 几乎处处, 再由 $f$ 绝对连续得 $f$ 为常数几乎处处, 而 $f\in L^2$ 故 $f\equiv0$. 又 $\left\langle f,f\right\rangle^{1/2}=\left\|f\right\|$, 故 $H$ 是内积空间, 其范数即题给范数. 由**定义 1.4.7 (iv)** (完备性), 只须证 $H$ 完备.

**第二步: 把 $H$ 等距嵌入 $L^2\left(\mathbb R\right)\times L^2\left(\mathbb R\right)$.** 令 $L^2\left(\mathbb R\right)\times L^2\left(\mathbb R\right)$ 的范数为 $\left\|\left(u,v\right)\right\|=\sqrt{\left\|u\right\|_2^2+\left\|v\right\|_2^2}$. 由**例 1.4.13** ($L^p\left(E\right)$ 是巴拿赫空间), $L^2\left(\mathbb R\right)$ 是希尔伯特空间; 由**习题 1.2 第 13 题** (内积空间的可数直和) (取 $R_1=R_2=L^2\left(\mathbb R\right)$), $L^2\left(\mathbb R\right)\times L^2\left(\mathbb R\right)$ 是希尔伯特空间. 作映射

$$
T\colon H\to L^2\left(\mathbb R\right)\times L^2\left(\mathbb R\right),\quad f\mapsto\left(f,f'\right).
$$

则 $T$ 是保范的线性映射, $T\left(H\right)\subset L^2\times L^2$ 是其线性子空间 ($H$ 的线性性显然).

**第三步: 证明 $T\left(H\right)$ 是闭的.** 设 $\left(f_n,f'_n\right)\to\left(g,h\right)$ 于 $L^2\times L^2$, 即 $f_n\to g$, $f'_n\to h$ 于 $L^2$. 对任意 $\varphi\in C_c^\infty\left(\mathbb R\right)$, 因 $f_n$ 绝对连续, 分部积分得 $\int_{\mathbb R}f_n\varphi'\mathrm dt=-\int_{\mathbb R}f'_n\varphi\mathrm dt$. 令 $n\to\infty$, 由 $f_n\to g$, $f'_n\to h$ 于 $L^2$ 及 $\varphi,\varphi'\in L^2$, 得

$$
\int_{\mathbb R}g\varphi'\mathrm dt=-\int_{\mathbb R}h\varphi\mathrm dt,\quad\forall\varphi\in C_c^\infty\left(\mathbb R\right).
$$

依据**定义** (弱导数), $g$ 的弱导数为 $h\in L^2$. 由**实变函数基本事实** (弱导数绝对连续), 得 $g\in H$ 且 $g'=h$, 故 $\left(g,h\right)=T\left(g\right)\in T\left(H\right)$. 因此 $T\left(H\right)$ 是 $L^2\times L^2$ 的闭线性子空间.

**第四步: 结论.** $L^2\times L^2$ 是希尔伯特空间 (第二步), $T\left(H\right)$ 是它的闭子集, 由**引理 1.4.1 (iii)** (基本点列与完备性), $T\left(H\right)$ 是完备子空间. 又 $T$ 是保范线性同构 ($T$ 单射: $T\left(f\right)=0$ 则 $f=f'=0$ 几乎处处, $f$ 绝对连续故 $f\equiv0$), 故 $H$ 完备. 由**定义 1.4.7 (iv)** (完备性), $H$ 是希尔伯特空间. $\blacksquare$

---

## 3 (习题 1.5)

### 2. 习题 1.5-2

设 $X$ 为完备度量空间, $\varphi$ 是 $X$ 到自身的映射, 记

$$
\alpha_n=\sup_{x\ne y}\frac{d\left(\varphi^n\left(x\right),\varphi^n\left(y\right)\right)}{d\left(x,y\right)},
$$

(i) 若级数 $\sum_{n=1}^{\infty}\alpha_n<\infty$, 则对任何一个初值 $x_0$, 迭代程序 $\left\{\varphi^n\left(x_0\right)\right\}$ 收敛于映射 $\varphi$ 的唯一不动点, 并求出第 $n$ 次近似解与准确解 $\varphi\left(x\right)=x$ 的逼近程度.

(ii) 若 $\inf_n\alpha_n<1$, 则 $\varphi$ 有唯一的不动点, 并给出一种收敛于准确解 $\varphi\left(x\right)=x$ 的迭代程序以及 $n$ 次近似解与准确解的逼近程度.

#### 解答 1.5-2

**(i) $\sum\alpha_n<\infty$ 的情形.**

**第一步: 不动点的存在与唯一性.** 因 $\sum\alpha_n<\infty$, $\alpha_n\to0$, 故存在正整数 $N$ 使 $\alpha_N<1$, 即 $d\left(\varphi^N\left(x\right),\varphi^N\left(y\right)\right)\le\alpha_N d\left(x,y\right)$ 对一切 $x,y$ 成立, 故 $\varphi^N$ 是压缩映射 (**定义 1.5.2**). 由**定理 1.5.2** ($\varphi^n$ 压缩 $\Rightarrow$ 唯一不动点), $\varphi$ 在 $X$ 中有唯一不动点 $x^*$.

**第二步: 迭代收敛.** 记 $x_n=\varphi^n\left(x_0\right)$. 对任意 $n$, 由 $\alpha_n$ 的定义,

$$
d\left(x_{n+1},x_n\right)=d\left(\varphi^n\left(\varphi\left(x_0\right)\right),\varphi^n\left(x_0\right)\right)\le\alpha_n d\left(\varphi\left(x_0\right),x_0\right)=\alpha_n d\left(x_1,x_0\right).
$$

对 $m>n$, 由三角不等式 (**定义 1.1.1 (iii)** (度量空间)),

$$
d\left(x_m,x_n\right)\le\sum_{k=n}^{m-1}d\left(x_{k+1},x_k\right)\le d\left(x_1,x_0\right)\sum_{k=n}^{m-1}\alpha_k\le d\left(x_1,x_0\right)\sum_{k=n}^{\infty}\alpha_k\to0\quad\left(n\to\infty\right),
$$

故 $\left\{x_n\right\}$ 是基本点列 (**定义 1.4.7 (i)** (完备性)). 因 $X$ 完备, $x_n\to y\in X$. 又由 $\alpha_1$ 有限, $d\left(\varphi(x),\varphi(x')\right)\le\alpha_1 d\left(x,x'\right)$, $\varphi$ 连续, 故极限与函数可以交换顺序:

$$
\varphi\left(y\right)=\varphi\left(\lim x_n\right)=\lim\varphi\left(x_n\right)=\lim x_{n+1}=y,
$$

即 $y$ 是 $\varphi$ 的不动点, 由唯一性 $y=x^*$. 故 $\left\{\varphi^n\left(x_0\right)\right\}$ 收敛于唯一不动点 $x^*$.

**第三步: 逼近程度.** 在第二步的不等式中令 $m\to\infty$, 由距离函数的连续性得

$$
d\left(x^*,x_n\right)=\lim_{m\to\infty}d\left(x_m,x_n\right)\le d\left(x_1,x_0\right)\sum_{k=n}^{\infty}\alpha_k.
$$

故第 $n$ 次近似解 $x_n=\varphi^n\left(x_0\right)$ 与准确解 $x^*$ 的逼近程度为 $d\left(x^*,x_n\right)\le d\left(x_1,x_0\right)\sum_{k=n}^{\infty}\alpha_k$. $\blacksquare$

**(ii) $\inf_n\alpha_n<1$ 的情形.**

因 $\inf_n\alpha_n<1$, 存在正整数 $N$ 使 $\alpha_N<1$, 即 $\varphi^N$ 是压缩映射 (**定义 1.5.2**). 由**定理 1.5.1** (巴拿赫), $\varphi^N$ 有唯一不动点 $x^*$: $\varphi^N\left(x^*\right)=x^*$.

**第一步: $x^*$ 是 $\varphi$ 的唯一不动点.** 因为 $\varphi\varphi^N=\varphi^{N+1}=\varphi^N\varphi$, 故 $\varphi^N\left(\varphi\left(x^*\right)\right)=\varphi\left(\varphi^N\left(x^*\right)\right)=\varphi\left(x^*\right)$, 即 $\varphi\left(x^*\right)$ 也是 $\varphi^N$ 的不动点; 由 $\varphi^N$ 不动点唯一, $\varphi\left(x^*\right)=x^*$, 即 $x^*$ 是 $\varphi$ 的不动点. 若 $y^*$ 是 $\varphi$ 的另一不动点, 则 $\varphi^N\left(y^*\right)=y^*$, $y^*$ 也是 $\varphi^N$ 的不动点, 由唯一性 $y^*=x^*$. 故 $\varphi$ 有唯一不动点 $x^*$.

**第二步: 迭代程序与逼近程度.** 取迭代程序 $x_{n+1}=\varphi^N\left(x_n\right)$, 即考察子序列 $\left\{\varphi^{Nk}\left(x_0\right)\right\}$. 因 $\varphi^N$ 是压缩映射 (压缩常数 $\alpha_N<1$) 且 $X$ 完备, 由**定理 1.5.1** (巴拿赫) 及**注 1.5.1** (迭代法) 的式 (1.25), 迭代 $\left\{\left(\varphi^N\right)^k\left(x_0\right)\right\}=\left\{\varphi^{Nk}\left(x_0\right)\right\}$ 收敛于 $x^*$, 且

$$
d\left(x^*,\varphi^{Nk}\left(x_0\right)\right)\le\frac{\alpha_N^k}{1-\alpha_N}d\left(\varphi^N\left(x_0\right),x_0\right).
$$

故 $\left\{\varphi^{Nk}\left(x_0\right)\right\}$ 即是一种收敛于准确解 $\varphi\left(x\right)=x$ 的迭代程序, 其 $k$ 次近似与准确解的逼近程度由上式给出. $\blacksquare$

---

### 4. 习题 1.5-4

写出并利用不动点原理证明, 关于方程组

$$
\frac{\mathrm dy_k}{\mathrm dx}=f_k\left(x,y_1,y_2,\cdots,y_n\right),\quad k=1,2,\cdots,n
$$

的解的存在性与唯一性定理.

#### 解答 1.5-4

**定理 (常微分方程组初值问题解的存在唯一性)** 设 $f_k\left(x,y_1,\cdots,y_n\right)$ ($k=1,\cdots,n$)在 $\mathbb R^{n+1}$ 的某区域上连续, 且关于 $\left(y_1,\cdots,y_n\right)$ 满足利普希茨条件, 即存在常数 $L>0$ 使得当 $\left(x,y\right),\left(x,z\right)$ 在此区域中时,

$$
\sum_{k=1}^n\left|f_k\left(x,y_1,\cdots,y_n\right)-f_k\left(x,z_1,\cdots,z_n\right)\right|\le L\sum_{k=1}^n\left|y_k-z_k\right|,
$$

则初值问题

$$
\frac{\mathrm dy_k}{\mathrm dx}=f_k\left(x,y_1,\cdots,y_n\right),\quad y_k\left(x_0\right)=y_k^0,\quad k=1,\cdots,n
$$

在 $x_0$ 的某个邻域上有唯一解 $y\left(x\right)=\left(y_1\left(x\right),\cdots,y_n\left(x\right)\right)$.

**证明** 取 $h>0$ 充分小, 考虑空间

$$
C_D=\left\{y=\left(y_1,\cdots,y_n\right)\in C\left(\left[x_0-h,x_0+h\right],\mathbb R^n\right):\left|y_k\left(x\right)-y_k^0\right|\le\lambda\ \forall x,\ y\left(x_0\right)=y_0\right\},
$$

其中范数为 $\left\|y\right\|=\max_{k=1,\cdots,n}\max_{x\in\left[x_0-h,x_0+h\right]}\left|y_k\left(x\right)\right|$, $y_0=\left(y_1^0,\cdots,y_n^0\right)$.

**第一步: 问题化为积分方程.** 由微积分基本定理, 初值问题等价于积分方程组

$$
y_k\left(x\right)=y_k^0+\int_{x_0}^x f_k\left(t,y_1\left(t\right),\cdots,y_n\left(t\right)\right)\mathrm dt,\quad k=1,\cdots,n.
$$

**第二步: 在 $C_D$ 上作压缩映射.** 记 $M=\max\left\{\left|f_k\left(x,y\right)\right|:k=1,\cdots,n,\ \left|x-x_0\right|\le h,\left|y_k-y_k^0\right|\le\lambda\right\}<\infty$ ($f_k$ 连续故在紧集上有界), 定义

$$
\left(Ay\right)_k\left(x\right)=y_k^0+\int_{x_0}^x f_k\left(t,y_1\left(t\right),\cdots,y_n\left(t\right)\right)\mathrm dt.
$$

仿照**定理 1.5.3** (初值问题解的存在唯一性) (取 $h<\min\left\{a,\frac{\lambda}{M},\frac{1}{L}\right\}$): 当 $\left|x-x_0\right|\le h$ 时, $\left|\left(Ay\right)_k\left(x\right)-y_k^0\right|\le Mh<\lambda$, 故 $Ay\in C_D$, 即 $A$ 把 $C_D$ 映入自身; 且对 $y,z\in C_D$, 由利普希茨条件,

$$
\left\|Ay-Az\right\|=\max_k\max_x\left|\int_{x_0}^x\left(f_k\left(t,y\right)-f_k\left(t,z\right)\right)\mathrm dt\right|\le Lh\left\|y-z\right\|,
$$

故当 $Lh<1$ 时 $A$ 是 $C_D$ 上的压缩映射 (**定义 1.5.2** (压缩映射)).

**第三步: 应用不动点原理.** $C_D$ 是 $C\left(\left[x_0-h,x_0+h\right],\mathbb R^n\right)$ 的闭子集. 由**例 1.2.12** ($C\left[a,b\right]$ 是巴拿赫空间), $C\left[a,b\right]$ 按最大范数完备; 因 $\left\|y\right\|=\max_{k=1,\cdots,n}\left\|y_k\right\|_\infty$ 且各分量 $y_k\in C\left[a,b\right]$, 故 $C\left(\left[x_0-h,x_0+h\right],\mathbb R^n\right)$ 按上述范数也是巴拿赫空间. 于是 $C_D$ 作为其闭子集, 由**引理 1.4.1 (iii)** (基本点列与完备性) 是完备度量空间. 由**定理 1.5.1** (巴拿赫), $A$ 在 $C_D$ 中有唯一不动点 $y$, 即 $y$ 满足积分方程, 由第一步即得初值问题的唯一解. $\blacksquare$

---

### 5. 习题 1.5-5

设从完备度量空间 $X$ 到自身的映射 $T$ 满足如下条件: 在开球 $O\left(x_0,r\right)\left(r>0\right)$ 内成立

$$
d\left(Tx,Tx'\right)<\theta d\left(x,x'\right),\quad 0<\theta<1,\ x\ne x',
$$

并且

$$
d\left(x_0,Tx_0\right)\le\alpha r.
$$

那么,

(i) 当 $\alpha$ 满足怎样的条件时, $T$ 在 $O\left(x_0,r\right)$ 内有不动点, 并且唯一?

(ii) 当 $\alpha\le1-\theta$ 时, 若 $T$ 在闭球 $B\left(x_0,r\right)$ 上连续, 则 $T$ 在 $B\left(x_0,r\right)$ 内有不动点. 这时这唯一性是否成立? 证明你的结论.

#### 解答 1.5-5

**(i) 条件为 $\alpha<1-\theta$.**

**第一步: 选取闭子球.** 设 $\alpha<1-\theta$, 则 $\frac{\alpha r}{1-\theta}<r$. 取 $\rho$ 满足 $\frac{\alpha r}{1-\theta}<\rho<r$, 作闭球 $B\left(x_0,\rho\right)\subset O\left(x_0,r\right)$.

**第二步: $T\left(B\left(x_0,\rho\right)\right)\subset B\left(x_0,\rho\right)$.** 对 $x\in B\left(x_0,\rho\right)$, 由开球内的压缩条件, $d\left(x_0,Tx_0\right)\le\alpha r$ 及三角不等式 (**定义 1.1.1 (iii)** (度量空间)),

$$
d\left(Tx,x_0\right)\le d\left(Tx,Tx_0\right)+d\left(Tx_0,x_0\right)<\theta d\left(x,x_0\right)+\alpha r\le\theta\rho+\alpha r\le\rho,
$$

故 $Tx\in B\left(x_0,\rho\right)$. 同时 $T$ 在 $B\left(x_0,\rho\right)$ 上仍满足压缩条件 ($B\left(x_0,\rho\right)\subset O\left(x_0,r\right)$), 且 $B\left(x_0,\rho\right)$ 是完备度量空间 $X$ 的闭子集, 由**引理 1.4.1 (iii)** (基本点列与完备性) 与**例 1.4.2** (闭球是闭集), $B\left(x_0,\rho\right)$ 是完备的.

**第三步: 存在唯一不动点.** 由**定理 1.5.1** (巴拿赫), $T$ 在 $B\left(x_0,\rho\right)\subset O\left(x_0,r\right)$ 内有唯一不动点. 若 $x',x''\in O\left(x_0,r\right)$ 都是 $T$ 的不动点且 $x'\ne x''$, 则由压缩条件 $d\left(x',x''\right)=d\left(Tx',Tx''\right)<\theta d\left(x',x''\right)<d\left(x',x''\right)$, 矛盾, 故 $T$ 在 $O\left(x_0,r\right)$ 内不动点唯一.

故当 $\alpha<1-\theta$ 时, $T$ 在 $O\left(x_0,r\right)$ 内有唯一不动点. $\blacksquare$

> 为什么是 $1-\theta$? 为了 (1) $T$ 能把闭球映到自己里面; (2) 闭球在 $O(x_0,r)$ 内, 我们希望有 $\theta\rho+\alpha r\le\rho<r$, 因此解得 $\alpha<1-\theta$.

**(ii) 当 $\alpha\le1-\theta$, $T$ 在 $B\left(x_0,r\right)$ 上连续时, $T$ 在 $B\left(x_0,r\right)$ 内有不动点, 且唯一性成立.**

**第一步: $T\left(B\left(x_0,r\right)\right)\subset B\left(x_0,r\right)$.** 对 $x\in O\left(x_0,r\right)$, $d\left(x,x_0\right)<r$, 由压缩条件与 $\alpha\le1-\theta$,

$$
d\left(Tx,x_0\right)\le d\left(Tx,Tx_0\right)+d\left(Tx_0,x_0\right)<\theta d\left(x,x_0\right)+\alpha r<\theta r+\left(1-\theta\right)r=r,
$$

故 $Tx\in O\left(x_0,r\right)\subset B\left(x_0,r\right)$. 对边界上的 $x\in B\left(x_0,r\right)\setminus O\left(x_0,r\right)$, 取 $x_m\in O\left(x_0,r\right)$ 使 $x_m\to x$, 由 $T$ 连续 $Tx_m\to Tx$, 而 $Tx_m\in B\left(x_0,r\right)$ 且 $B\left(x_0,r\right)$ 闭 (**例 1.4.2** (闭球是闭集)), 故 $Tx\in B\left(x_0,r\right)$. 故 $T\left(B\left(x_0,r\right)\right)\subset B\left(x_0,r\right)$.

**第二步: $T$ 在 $B\left(x_0,r\right)$ 上是压缩映射.** 对 $x,y\in B\left(x_0,r\right)$, 取 $x_m,y_m\in O\left(x_0,r\right)$ 使 $x_m\to x$, $y_m\to y$. 因 $T$ 连续且压缩条件在 $O\left(x_0,r\right)$ 内成立, $d\left(Tx_m,Ty_m\right)<\theta d\left(x_m,y_m\right)$, 令 $m\to\infty$ 得 $d\left(Tx,Ty\right)\le\theta d\left(x,y\right)$, 故 $T$ 是 $B\left(x_0,r\right)$ 上的压缩映射 (**定义 1.5.2**, 常数 $\theta<1$).

**第三步: 应用不动点原理.** $B\left(x_0,r\right)$ 是完备度量空间 $X$ 的闭子集, 由**引理 1.4.1 (iii)** (基本点列与完备性) 与**例 1.4.2** (闭球是闭集) 是完备的, 且由第一步 $T\left(B\left(x_0,r\right)\right)\subset B\left(x_0,r\right)$. 由**定理 1.5.1** (巴拿赫), $T$ 在 $B\left(x_0,r\right)$ 内有唯一不动点. $\blacksquare$

---

### 6. 习题 1.5-6

设 $F$ 是 $n$ 维欧几里得空间 $\mathbb R^n$ 中的有界闭集, $\varphi$ 是 $F$ 到自身的映射并且满足如下条件: 对于任何 $x,y\in F\left(x\ne y\right)$, 有

$$
d\left(\varphi\left(x\right),\varphi\left(y\right)\right)<d\left(x,y\right),\quad x\ne y.
$$

证明: 映射 $\varphi$ 在 $F$ 中存在唯一的不动点. 对于不闭的有界集这个事实能否成立?

#### 解答 1.5-6

**第一步: $F$ 是紧集, $\varphi$ 连续.** $F$ 是 $\mathbb R^n$ 中的有界闭集, 由**例 1.6.1** ($\mathbb R^n$ 中有界集相对列紧), $\mathbb R^n$ 中子集相对列紧等价于有界, 故 $F$ 是有界闭集即相对列紧的闭集, 从而是紧集. 由题设条件, $\varphi$ 是严格压缩的, 故 $\varphi$ 连续 (**定义 1.1.2** (极限) 意义下: $x_m\to x$ 时 $d\left(\varphi\left(x_m\right),\varphi\left(x\right)\right)<d\left(x_m,x\right)\to0$).

**第二步: 定义连续函数 $g$ 并取最小值.** 令 $g\left(x\right)=d\left(x,\varphi\left(x\right)\right)$ ($x\in F$). 因 $d$ 连续 (**例 1.4.3** (距离函数连续), 取 $F=\left\{\varphi\left(x\right)\right\}$ 或由 $d$ 的三角不等式) 且 $\varphi$ 连续, $g$ 是紧集 $F$ 上的连续函数, 由**推论 1.6.3** (紧集上连续函数达到上下确界), $g$ 在 $F$ 上达到下确界, 即存在 $x_0\in F$ 使 $g\left(x_0\right)=\min_{x\in F}g\left(x\right)$.

**第三步: $x_0$ 是不动点.** 反设 $g\left(x_0\right)>0$, 即 $\varphi\left(x_0\right)\ne x_0$. 由题设条件 ($\varphi\left(x_0\right)\in F$, 且 $x_0\ne\varphi\left(x_0\right)$),

$$
g\left(\varphi\left(x_0\right)\right)=d\left(\varphi\left(x_0\right),\varphi\left(\varphi\left(x_0\right)\right)\right)<d\left(x_0,\varphi\left(x_0\right)\right)=g\left(x_0\right),
$$

这与 $g\left(x_0\right)$ 是 $g$ 在 $F$ 上的最小值矛盾. 故 $g\left(x_0\right)=0$, 即 $d\left(x_0,\varphi\left(x_0\right)\right)=0$, 由正定性 (**定义 1.1.1 (i)** (度量空间)) $\varphi\left(x_0\right)=x_0$.

**第四步: 唯一性.** 若 $x,y\in F$ 都是不动点且 $x\ne y$, 则 $d\left(x,y\right)=d\left(\varphi\left(x\right),\varphi\left(y\right)\right)<d\left(x,y\right)$, 矛盾. 故不动点唯一.

故 $\varphi$ 在 $F$ 中存在唯一的不动点. $\blacksquare$

**关于不闭的有界集:** 不成立. 取 $F=\left(0,1\right]$ ($\mathbb R$ 中的有界非闭集), 映射 $\varphi\left(x\right)=\frac{x}{2}$. 对 $x\ne y\in F$, $d\left(\varphi\left(x\right),\varphi\left(y\right)\right)=\frac{\left|x-y\right|}{2}<d\left(x,y\right)$, 满足条件; 但 $\varphi$ 在 $F$ 中无不动点 ($\frac{x}{2}=x$ 得 $x=0\notin F$). 故对不闭的有界集该事实不成立. $\blacksquare$

> 不闭的有界集正是因为其不闭, 故不紧, 迭代序列的集合会跑到集合外, 此时压缩映射原理失效.

---

### 7. 习题 1.5-7

(牛顿迭代法) 设 $f$ 是定义在 $\left[a,b\right]$ 上的二次连续可微实函数, $\left[a,b\right]$ 中点 $\overline x$ 满足 $f\left(\overline x\right)=0,f'\left(\overline x\right)\ne0$. 证明: 存在点 $\overline x$ 的一个邻域 $U$, 使得对任意 $x_0\in U$, 迭代序列

$$
x_{n+1}=x_n-\frac{f\left(x_n\right)}{f'\left(x_n\right)},\quad n=0,1,2,\cdots
$$

都收敛于 $\overline x$.

#### 解答 1.5-7

**第一步: 牛顿映射及其导数.** 令 $N\left(x\right)=x-\frac{f\left(x\right)}{f'\left(x\right)}$, 其中 $x$ 属于使 $f'\left(x\right)\ne0$ 的开集. 因 $f$ 二次连续可微且 $f'\left(\overline x\right)\ne0$, $N$ 在 $\overline x$ 的某邻域内有定义且连续可微, 且

$$
N'\left(x\right)=1-\frac{f'\left(x\right)^2-f\left(x\right)f''\left(x\right)}{f'\left(x\right)^2}=\frac{f\left(x\right)f''\left(x\right)}{f'\left(x\right)^2},
$$

故 $N'\left(\overline x\right)=\frac{f\left(\overline x\right)f''\left(\overline x\right)}{f'\left(\overline x\right)^2}=0$ (因 $f\left(\overline x\right)=0$).

**第二步: 找压缩区间.** 因 $N'$ 连续且 $N'\left(\overline x\right)=0$, 存在 $\delta>0$ 使对 $\left|x-\overline x\right|\le\delta$ 有 $\left|N'\left(x\right)\right|\le\frac12<1$ (取 $\theta=\frac12$). 由微分中值定理, 对 $x,y\in\left[\overline x-\delta,\overline x+\delta\right]$ 存在 $\xi$ 介于其间, 使

$$
\left|N\left(x\right)-N\left(y\right)\right|=\left|N'\left(\xi\right)\right|\left|x-y\right|\le\frac12\left|x-y\right|,
$$

故 $N$ 在闭区间 $\left[\overline x-\delta,\overline x+\delta\right]$ 上是压缩映射 (**定义 1.5.2**, 压缩常数 $\frac12$).

**第三步: 取不变闭区间并迭代.** 记 $B=\left[\overline x-\rho,\overline x+\rho\right]$, 其中 $0<\rho\le\delta$ 待定. 因 $N$ 在 $\left[\overline x-\delta,\overline x+\delta\right]$ 上以 $\frac12$ 为压缩常数且 $N\left(\overline x\right)=\overline x$, 对 $x\in B$ ($B\subset\left[\overline x-\delta,\overline x+\delta\right]$), 由第二步的压缩估计得

$$
\left|N\left(x\right)-\overline x\right|=\left|N\left(x\right)-N\left(\overline x\right)\right|\le\frac12\left|x-\overline x\right|\le\frac{\rho}{2}<\rho,
$$

故 $N\left(B\right)\subset B$. $B$ 是完备度量空间 $\mathbb R$ 的闭子集, 由**引理 1.4.1 (iii)** (基本点列与完备性) 是完备的. 由**定理 1.5.1** (巴拿赫), $N$ 在 $B$ 内有唯一不动点; 又 $N\left(\overline x\right)=\overline x$, 故该不动点为 $\overline x$, 且由**注 1.5.1** (迭代法), 从任意 $x_0\in B$ 出发的迭代 $x_{n+1}=N\left(x_n\right)$ 收敛于 $\overline x$.

故取 $U=B\left(\overline x,\rho\right)$ (即 $\overline x$ 的邻域), 对任意 $x_0\in U$, 迭代序列收敛于 $\overline x$. $\blacksquare$
