# week 1

> **定义 1.1.1** (度量空间) 设 $X$ 是一个非空集合，若对于 $X$ 中任意两个元素 $x,y$, 有一个实数 $d\left(x,y\right)$ 与它们对应，而且满足下面条件:<br>(i) **(非负性与正定性)** 对任意 $x,y\in X$, $d\left(x,y\right)\ge0$, 并且 $d\left(x,y\right)=0$ 的充要条件是 $x=y$;<br>(ii) **(对称性)** 对任意 $x,y\in X$, $d\left(x,y\right)=d\left(y,x\right)$;<br>(iii) **(三角不等式)** 对任意 $x,y,z\in X$, $d\left(x,y\right)\le d\left(x,z\right)+d\left(z,y\right)$,<br>则称 $\left(X,d\right)$ 是一个**度量空间** (或**距离空间**), $d$ 为 $X$ 上的**度量** (或**距离**), $d\left(x,y\right)$ 为**点 $x,y$ 之间的距离**.

> **定义 1.1.2** (极限) 设 $\left(X,d\right)$ 是度量空间, $\left\{x_n\right\}_{n=1}^\infty$ 是 $X$ 中点列, $x_0\in X$, 若 $$\lim_{n\to\infty}d\left(x_n,x_0\right)=0,$$ 则称**点列 $\left\{x_n\right\}_{n=1}^\infty$ 按照度量 $d$ 收敛于 $x_0$**, 记为 $\lim_{n\to\infty}x_n=x_0$.

> **例 1.1.2** (n 维 Euclid 空间) 在 $n$ 个有序实数组 $x=\left(x_1,x_2,\cdots,x_n\right)$ 全体组成的集合 $X$ 中，定义 $$d\left(x,y\right)=\sqrt{\sum_{i=1}^{n}\left(x_i-y_i\right)^2},$$ 则 $\left(X,d\right)$ 是度量空间，称为 $n$ 维 Euclid（欧几里得）空间，通常记为 $\mathbb R^n$.

> **例 1.1.10** (一致收敛与度量收敛) 由例 1.1.10 的讨论可知，$C\left[a,b\right]$ 中点列按度量 $d$ 收敛等价于区间 $\left[a,b\right]$ 上的函数列一致收敛.

> **例 1.1.11** (等价度量) 设 $\left(X,d\right)$ 是度量空间，我们还可以在 $X$ 上定义新的度量 $$d'\left(x,y\right)=\frac{d\left(x,y\right)}{1+d\left(x,y\right)},\quad d''\left(x,y\right)=\ln\left(1+d\left(x,y\right)\right),\quad\forall x,y\in X,$$ 它们是不同的度量. 但是容易验证，对于空间 $X$ 中的点列 $\left\{x_n\right\}$，$$\lim_{n\to\infty}x_n\overset d=x_0\Leftrightarrow\lim_{n\to\infty}x_n\overset{d'}=x_0\Leftrightarrow\lim_{n\to\infty}x_n\overset{d''}=x_0.$$

> **例 1.1.12** (可测函数等价类空间) 对于有限区间 $\left[a,b\right]$，记 $\mathfrak G=\left\{\left[a,b\right]\text{ 上几乎处处有限的 Lebesgue 可测函数}\right\}$. $\mathfrak G$ 中两个函数 $f,g$ 是**等价**的，是指它们满足 $f\underset{m}{\doteq}g$. 仍以 $f$ 来表示 Lebesgue 可测函数 $f$ 在 $\mathcal S=\mathfrak G/\sim$ 中对应的等价类. 对于 $f,g\in\mathcal S$，定义 $$d\left(f,g\right)=\int_{\left[a,b\right]}\frac{\left|f\left(t\right)-g\left(t\right)\right|}{1+\left|f\left(t\right)-g\left(t\right)\right|}\mathrm dm\left(t\right),$$ 容易验证这是一个度量，进而 $\left(\mathcal S,d\right)$ 是完备的度量空间.

## 1.1-2

设 $\left(X,d\right)$ 是度量空间, 在 $X$ 上定义

$$
d'\left(x,y\right)=\frac{d\left(x,y\right)}{1+d\left(x,y\right)},\quad\forall x,y\in X
$$

和

$$
d''\left(x,y\right)=\ln\left(1+d\left(x,y\right)\right),\quad\forall x,y\in X.
$$

证明: $d'$ 和 $d''$ 都是 $X$ 上的度量, 并且 $\left(X,d'\right)$, $\left(X,d''\right)$ 中点列的收敛性和在 $\left(X,d\right)$ 中是一致的.

### 解答 1.1-2

本题即**例 1.1.11** 所断言的结论, 下面给出证明.

**$d'$ 是 $X$ 上的度量**. 依据**定义 1.1.1 (度量空间)**, (i) (ii) 显然. (iii) 由三角不等式及函数 $t\mapsto\frac{t}{1+t}$ 在 $\left[0,\infty\right)$ 上单调递增得

$$
\frac{d\left(x,y\right)}{1+d\left(x,y\right)}\le\frac{d\left(x,z\right)+d\left(z,y\right)}{1+d\left(x,z\right)+d\left(z,y\right)}\le\frac{d\left(x,z\right)}{1+d\left(x,z\right)}+\frac{d\left(z,y\right)}{1+d\left(z,y\right)}.
$$

故 $d'$ 是度量.

**$d''$ 是 $X$ 上的度量**. 依据**定义 1.1.1 (度量空间)**, (i) (ii) 显然. (iii) 由三角不等式及 $\ln$ 的单调性得

$$
\ln\left(1+d\left(x,y\right)\right)\le\ln\left(1+d\left(x,z\right)+d\left(z,y\right)\right)\le\ln\left(1+d\left(x,z\right)\right)+\ln\left(1+d\left(z,y\right)\right).
$$

故 $d''$ 是度量.

**收敛性一致.** 依据**定义 1.1.2 (极限)**, $x_n\overset d\to x_0\iff\epsilon_n\to0$, 故只需证 $\epsilon_n\to0\iff d'\left(x_n,x_0\right)\to0\iff d''\left(x_n,x_0\right)\to0$. 即证: 对于空间 $X$ 中的点列 $\left\{x_n\right\}$,

$$
\lim_{n\to\infty}x_n\stackrel{d}{=}x_0\Leftrightarrow\lim_{n\to\infty} x_n\stackrel{d'}{=}x_0\Leftrightarrow\lim_{n\to\infty}x_n\stackrel{d''}{=}x_0.
$$

**$\Rightarrow$ 方向**: 若 $x_n\overset d\to x_0$, 即 $\epsilon_n\to0$, 则 $d'\left(x_n,x_0\right)=\frac{\epsilon_n}{1+\epsilon_n}\to0$, $d''\left(x_n,x_0\right)=\ln\left(1+\epsilon_n\right)\to0$, 故 $x_n\overset{d'}\to x_0$, $x_n\overset{d''}\to x_0$.

**$\Leftarrow$ 方向**: 若 $d'\left(x_n,x_0\right)\to0$, 即 $\frac{\epsilon_n}{1+\epsilon_n}\to0$. 若 $\epsilon_n\not\to0$, 则存在子列 $\epsilon_{n_k}\ge\delta>0$, 于是 $\frac{\epsilon_{n_k}}{1+\epsilon_{n_k}}\ge\frac{\delta}{1+\delta}>0$, 矛盾, 故 $\epsilon_n\to0$. 若 $d''\left(x_n,x_0\right)=\ln\left(1+\epsilon_n\right)\to0$, 同样得 $\epsilon_n\to0$.

综上, 三种度量下的收敛性是等价的.

## 1.1-4

设 $X$ 是 $\left[0,1\right]$ 上多项式全体. 对于 $P,Q\in X$, $P\left(x\right)-Q\left(x\right)=\sum_{i=0}^{n}a_ix^i$, 令

$$
\begin{aligned}
d_1\left(P,Q\right)&=\max_{x\in\left[0,1\right]}\left|P\left(x\right)-Q\left(x\right)\right|,\\
d_2\left(P,Q\right)&=\sum_{i=0}^{n}\left|a_i\right|.
\end{aligned}
$$

证明

(1) $d_1,d_2$ 都是 $X$ 上的度量.

(2) 多项式按 $d_1$ 收敛等价于在 $\left[0,1\right]$ 上一致收敛于某一多项式.

(3) 按 $d_2$ 收敛可以推出按 $d_1$ 收敛, 但反之不真 (即存在多项式列 $\left\{P_k\right\},d_1\left(P_k,0\right)\to 0$, 但 $d_2\left(P_k,0\right)\not\rightarrow 0$).

### 解答 1.1-4

(1) **$d_1$ 是度量**. 依据**定义 1.1.1 (度量空间)**, (i) (ii) 显然. (iii) 对任意 $R\in X$ 与 $x\in\left[0,1\right]$,

$$
\left|P\left(x\right)-Q\left(x\right)\right|\le\left|P\left(x\right)-R\left(x\right)\right|+\left|R\left(x\right)-Q\left(x\right)\right|\le d_1\left(P,R\right)+d_1\left(R,Q\right).
$$

对 $x$ 取最大值即得 $d_1\left(P,Q\right)\le d_1\left(P,R\right)+d_1\left(R,Q\right)$.

**$d_2$ 是度量**. 依据**定义 1.1.1 (度量空间)**, (i) (ii) 显然. (iii) 设 $P-R=\sum_{i=0}^{n}a_ix^i$, $R-Q=\sum_{i=0}^{n}b_ix^i$, 则 $P-Q=\sum_{i=0}^{n}\left(a_i+b_i\right)x^i$, 于是

$$
d_2\left(P,Q\right)=\sum_{i=0}^{n}\left|a_i+b_i\right|\le\sum_{i=0}^{n}\left|a_i\right|+\sum_{i=0}^{n}\left|b_i\right|=d_2\left(P,R\right)+d_2\left(R,Q\right).
$$

故 $d_1,d_2$ 都是 $X$ 上的度量. $\blacksquare$

(2) 由题设 $d_1$ 的定义,

$$
d_1\left(P_k,P\right)\to0\Leftrightarrow\max_{x\in\left[0,1\right]}\left|P_k\left(x\right)-P\left(x\right)\right|\to0.
$$

这正是 $\left\{P_k\right\}$ 在 $\left[0,1\right]$ 上一致收敛于多项式 $P$ 的定义, 两者等价. (此即**例 1.1.10** 的结论在多项式子空间上的情形: $C\left[a,b\right]$ 中点列按度量 $d$ 收敛等价于函数列一致收敛.) $\blacksquare$

(3) **$d_1$ 推出 $d_2$**. 设 $d_2\left(P_k,Q\right)\to0$, 记 $P_k-Q=\sum_{i=0}^{n_k}a_i^{\left(k\right)}x^i$, 则 $\sum_{i=0}^{n_k}\left|a_i^{\left(k\right)}\right|\to0$. 对一切 $x\in\left[0,1\right]$ 有 $x^i\le1$, 故

$$
\left|P_k\left(x\right)-Q\left(x\right)\right|\le\sum_{i=0}^{n_k}\left|a_i^{\left(k\right)}\right|x^i\le\sum_{i=0}^{n_k}\left|a_i^{\left(k\right)}\right|=d_2\left(P_k,Q\right)\to0.
$$

上式对 $x$ 一致成立, 故 $d_1\left(P_k,Q\right)\to0$.

**反之不真**. 取 $P_k\left(x\right)=x^k\left(1-x\right)^k=\sum_{j=0}^{k}\binom{k}{j}\left(-1\right)^jx^{k+j}$. 则

$$
d_1\left(P_k,0\right)=\max_{x\in\left[0,1\right]}\left[x\left(1-x\right)\right]^k=\left(\frac14\right)^k\to0.
$$

而

$$
d_2\left(P_k,0\right)=\sum_{j=0}^{k}\binom{k}{j}=2^k\to\infty.
$$

故存在 $d_1\left(P_k,0\right)\to0$ 而 $d_2\left(P_k,0\right)\not\to0$ 的多项式列. $\blacksquare$

> **反之不真** 的构造思路: 要找一个函数, 函数值很小但是系数很大, 因此联想到要找能够包含大量正负抵消的函数——要是函数中出现了 $\left(-1\right)^n$ 就很合适. 而二项式天然适配这种需求, 因此尝试构造 $x^k\left(1-x\right)^k$, 其写作二项式后系数为 $2^k$, 果然无穷大.

## 1.1-5

对 $0<p<1$, 记 $L^p\left[0,1\right]$ 是区间 $\left[a,b\right]$ 上勒贝格可测且 $p$ 次可积的函数全体. 令

$$
d\left(f,g\right)=\int_{0}^{1}\left|f\left(t\right)-g\left(t\right)\right|^p\mathrm dt.
$$

证明:

(1) 当数 $a,b>0$ 时, $\left(a+b\right)^p \le a^p+b^p$.

(2) $d$ 是伪度量, 即 $d$ 是非负的且满足定义 1.1.1 (ii) 及 (iii).

(3) 若等价关系 $f\sim g$ 是指两个函数 $f,g$ 满足 $f\underset{m}{\doteq}g$, 仍以 $f$ 来表示 $p$ 次可积函数 $f$ 在 $L^p\left[a,b\right]=L^p\left[a,b\right]/\sim$ 中对应的等价类, 则 $\left(L^p\left[a,b\right],d\right)$ 是度量空间.

### 解答 1.1-5

(1) 不妨设 $a\le b$. 易知 $\left(1+t\right)^p\le1+t^p$ ($t\ge0$). 于是

$$
\left(a+b\right)^p=b^p\left(1+\frac{a}{b}\right)^p\le b^p\left[1+\left(\frac{a}{b}\right)^p\right]=a^p+b^p\quad\blacksquare
$$

(2) 依据**定义 1.1.1 (度量空间)**, (i) 非负性、(ii) 对称性显然. (iii) 对任意可测函数 $h$, 由 (1) 逐点地有

$$
\left|f\left(t\right)-g\left(t\right)\right|^p\le\left(\left|f\left(t\right)-h\left(t\right)\right|+\left|h\left(t\right)-g\left(t\right)\right|\right)^p\le\left|f\left(t\right)-h\left(t\right)\right|^p+\left|h\left(t\right)-g\left(t\right)\right|^p.
$$

积分即得 $d\left(f,g\right)\le d\left(f,h\right)+d\left(h,g\right)$. 故 $d$ 是伪度量. $\blacksquare$

(3) 依据**定义 1.1.1 (度量空间)**, 由 (2) 已知非负性、对称性与三角不等式成立, 只需再验证正定性 (商空间构造方式同**例 1.1.12**). 若 $d\left(f,g\right)=0$, 即 $\int_{0}^{1}\left|f-g\right|^p\mathrm dt=0$. 因被积函数 $\left|f-g\right|^p\ge0$ 且可测, 由积分的性质,

$$
\int_{0}^{1}\left|f-g\right|^p\mathrm dt=0\Leftrightarrow\left|f-g\right|^p=0\text{ a.e.}\Leftrightarrow f=g\text{ a.e.}\Leftrightarrow f\sim g.
$$

故在等价类空间 $L^p\left[0,1\right]/\sim$ 上, $d\left(\left[f\right],\left[g\right]\right)=0\Leftrightarrow\left[f\right]=\left[g\right]$, 因此 $\left(L^p\left[0,1\right]/\sim,d\right)$ 是度量空间. $\blacksquare$

## 1.1-7

在三维欧几里得空间 $\mathbb R^3$ 中, 考虑单位球面

$$
S^2=\left\{x\in\mathbb R^3:x=\left(x_1,x_2,x_3\right),x_1^2+x_2^2+x_3^2=1\right\}.
$$

对于 $x,y\in S^2$, 规定 $d\left(x,y\right)$ 为过 $x,y$ 两点的大圆上以 $x,y$ 为端点的劣弧的弧长, 它在三维欧几里得空间的正交变换下是保持不变的.

(1) 对于 $x_1^2+x_2^2=1$, 计算 $d\left(\left(1,0,0\right),\left(x_1,x_2,0\right)\right)$.

(2) 如果用 $\rho\left(x,y\right)$ 表示欧几里得距离, 证明:

$$
\rho\left(x,y\right)\le d\left(x,y\right)\le\frac{\pi}{2}\rho\left(x,y\right).
$$

(3) 证明: $d$ 是 $S^2$ 上的度量.

### 解答 1.1-7

(1) 易知

$$
d\left(\left(1,0,0\right),\left(x_1,x_2,0\right)\right)=\arccos x_1=\arcsin x_2\quad\blacksquare
$$

(2) **左边** (其中 $\rho$ 为**例 1.1.2** 的欧氏度量):

设 $\theta=d\left(x,y\right)\in\left[0,\pi\right]$ 为 $x,y$ 的中心角, 则 $\rho\left(x,y\right)=\left\|x-y\right\|=2\sin\frac{\theta}{2}\le\theta=d\left(x,y\right)$.

**右边**:

$u=\frac{\theta}{2}\in\left[0,\frac{\pi}{2}\right]$. $\sin$ 在 $\left[0,\frac{\pi}{2}\right]$ 上是凹函数, 其图像位于连接 $\left(0,0\right)$ 与 $\left(\frac{\pi}{2},1\right)$ 的弦 $y=\frac{2}{\pi}u$ 之上方, 即 $\sin u\ge\frac{2}{\pi}u$, 故

$$
d\left(x,y\right)=\theta=2u\le\pi\sin u=\frac{\pi}{2}\cdot2\sin\frac{\theta}{2}=\frac{\pi}{2}\rho\left(x,y\right).
$$

合并即得 $\rho\left(x,y\right)\le d\left(x,y\right)\le\frac{\pi}{2}\rho\left(x,y\right)$. $\blacksquare$

(3) 依据**定义 1.1.1 (度量空间)**, (i) (ii) 显然. (iii) 设 $\alpha=d\left(x,y\right)$, $\beta=d\left(y,z\right)$, $\gamma=d\left(x,z\right)\in\left[0,\pi\right]$.

若 $\alpha+\beta\ge\pi$, 则 $\gamma\le\pi\le\alpha+\beta$, 不等式显然成立.

若 $\alpha+\beta<\pi$: 取单位向量 $u,v\perp y$ 使得

$$
\begin{aligned}
x&=\cos\alpha y+\sin\alpha u,\\
z&=\cos\beta y+\sin\beta v.
\end{aligned}
$$

则

$$
\begin{aligned}
\cos\gamma=x\cdot z&=\cos\alpha\cos\beta+\sin\alpha\sin\beta\left(u\cdot v\right)\\
&\ge\cos\alpha\cos\beta-\sin\alpha\sin\beta=\cos\left(\alpha+\beta\right).
\end{aligned}
$$

由于 $\gamma,\alpha+\beta\in\left[0,\pi\right]$ 且 $\cos$ 在 $\left[0,\pi\right]$ 上严格递减, 得 $\gamma\le\alpha+\beta$. 故三角不等式成立, $d$ 是 $S^2$ 上的度量. $\blacksquare$

> **证明技巧**: 把 $x$, $z$ 沿 $y$ 正交分解, 拆成平行于 $y$ 的和垂直于 $y$ 的部分, 而 $x$ 与 $z$ 各自垂直于 $y$ 的那部分分量的内积必然 $\ge-1$, 由此放缩证毕.
