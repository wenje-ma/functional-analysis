# week9

> **定理 1.4.2 (有限维赋范线性空间完备)**
> 
> 有限维的赋范线性空间是完备的.

> **定义 1.6.1 (相对列紧集)**
> 
> 设 $X$ 是度量空间, $A$ 是 $X$ 的子集. 如果 $A$ 中的任何点列都有在 $X$ 中收敛的子列, 就称 $A$ 是 $X$ 中的相对列紧集; 如果 $X$ 自身是相对列紧集, 就称 $X$ 是列紧空间.

> **定理 1.6.1 (无限维空间的单位球不相对列紧)**
> 
> 如果赋范线性空间 $X$ 是无限维的, 那么 $X$ 的单位球不是相对列紧的.

> **定理 2.3.1 (哈恩-巴拿赫延拓定理)**
> 
> 设 $L_0$ 是实赋范线性空间 $L$ 的线性子空间. 若 $f_0$ 是 $L_0$ 上的有界线性泛函, 则存在 $L$ 上的有界线性泛函 $f$, $f|_{L_0}=f_0$, 且 $\left\|f\right\|=\left\|f_0\right\|$.

> **推论 2.3.4 (闭线性子空间与点的分离)**
> 
> 设 $M$ 是赋范线性空间 $\left(X,\left\|\cdot\right\|\right)$ 的闭线性子空间, $x\notin{}M$, 则存在 $f\in{}X^*$ 使得 $\left\|f\right\|=1$, $f\left(M\right)=0$, $f\left(x\right)=d\left(x,M\right)$.

> **定义 2.4.1 (凸集)**
> 
> 设 $V$ 是线性空间, $M$ 是 $V$ 的一个子集. 如果对于任意的 $x,y\in{}M$, 及数 $\alpha\in\left[0,1\right]$, 有 $\alpha{}x+\left(1-\alpha\right)y\in{}M$, 就称 $M$ 是一个凸集.

> **引理 2.4.1 (一点与凸集的分离)**
> 
> 设 $A$ 是实赋范线性空间 $L$ 中的凸子集, 如果 $A$ 的内部 $A^\circ$ 是非空的, 并且 $y_0\notin{}A^\circ$, 则 $L$ 上存在非零的连续线性泛函 $f$, 使得 $f\left(x\right)\le{}f\left(y_0\right)$ 对一切 $x\in{}A$ 成立.

> **定理 2.4.1 (凸集分离定理)**
> 
> 设 $M$ 与 $N$ 是实赋范线性空间 $L$ 中的凸集, 如果 $M$ 的内部 $M^\circ$ 是非空的, 并且 $M^\circ\cap{}N=\emptyset$, 则存在 $L$ 上非零的连续线性泛函 $f$ 分离 $M$ 与 $N$, 即 $\sup_{x\in{}M}f\left(x\right)\le\inf_{x\in{}N}f\left(x\right)$.

> **推论 2.4.1 (闭凸集与紧凸集的严格分离)**
> 
> 设 $M,N$ 是实赋范线性空间 $L$ 中的闭凸集, $d\left(M,N\right)=\inf_{x\in{}M,y\in{}N}d\left(x,y\right)>0$, 则存在 $L$ 上的非零连续线性泛函 $f$ 严格分离 $M$ 与 $N$, 即 $\sup_{x\in{}M}f\left(x\right)<\inf_{y\in{}N}f\left(y\right)$.

> **注 2.4.1 (复赋范线性空间的实部分离)**
> 
> 设 $A$ 是复赋范线性空间 $L$ 中的凸子集, 如果 $A^\circ$ 是非空的, 并且 $y_0\notin{}A^\circ$, 则 $L$ 上存在非零的连续线性泛函 $f$, 使得 $\sup_{x\in{}A}\operatorname{Re}f\left(x\right)\le\operatorname{Re}f\left(y_0\right)$.

> **例 2.4.2 (凸函数的上方图是凸集)**
> 
> 若 $\varphi$ 是直线 $\mathbb{R}$ 上的凸函数, 即 $\varphi\left(tx+\left(1-t\right)y\right)\le{}t\varphi\left(x\right)+\left(1-t\right)\varphi\left(y\right)$, $\forall{}x,y\in\mathbb{R}$, $t\in\left(0,1\right)$, 那么图形 $\left\{\left(x,y\right)\in\mathbb{R}^2:y\ge\varphi\left(x\right)\right\}$ 是平面中的一个凸集.

> **定义 2.4.3 (分离与严格分离)**
> 
> 设 $V$ 是实线性空间, $M$ 与 $N$ 是它的子集, $f$ 是 $V$ 上的线性泛函. (i) 如果存在常数 $C$, 使得 $f\left(x\right)\le{}C$, $\forall{}x\in{}M$ 与 $f\left(y\right)\ge{}C$, $\forall{}y\in{}N$, 即 $\sup\left\{f\left(x\right):x\in{}M\right\}\le\inf\left\{f\left(x\right):x\in{}N\right\}$, 则称线性泛函 $f$ 分离集 $M$ 与 $N$. (ii) 如果线性泛函 $f$ 满足 $\sup\left\{f\left(x\right):x\in{}M\right\}<\inf\left\{f\left(x\right):x\in{}N\right\}$, 则称 $f$ 严格分离 $M$ 与 $N$.

> **定义 2.5.1 (自反空间)**
> 
> 设 $X$ 是赋范线性空间, $J$ 是典则映射. 如果 $J:X\to{}X^{**}$ 是同构, 就称 $X$ 是自反的.

> **注 2.5.1 (一般可测空间上 $L^p$ 的对偶)**
> 
> 设 $\left(X,\mathcal{R}\right)$ 是一个可测空间, $\mu$ 是它的一个 $\sigma$-有限测度. 对赋范线性空间 $L^p\left(X,\mu\right)$ ($1\le{}p<\infty$) 上的一个连续线性泛函 $\psi$, 都存在唯一的 $g\in{}L^q\left(X,\mu\right)$ ($\frac1p+\frac1q=1$), 使得 $\psi\left(f\right)=\int_Xf\left(x\right)g\left(x\right)\,\mathrm{d}\mu\left(x\right)$, $\forall{}f\in{}L^p\left(X,\mu\right)$, 且此时 $\left\|\psi\right\|=\left\|g\right\|_q$.

> **定理 2.5.2 (里斯表示定理)**
> 
> 设 $X$ 是紧度量空间. 对实 (复) 连续函数空间 $C\left(X\right)$ 上的一个连续线性泛函 $f$, 存在 $X$ 上唯一的全有限广义测度 (复测度) $\mu$ 使得 $f\left(x\right)=\int_Xx\left(t\right)\,\mathrm{d}\mu\left(t\right)$, $\forall{}x\in{}C\left(X\right)$, 并且 $\left\|f\right\|=\left|\mu\right|\left(X\right)$, 这里 $\left|\mu\right|$ 是 $\mu$ 的全变差测度.

> **例 2.5.2 (自反空间的对偶空间自反)**
> 
> 当 $X$ 是自反空间时, $X^*$ 也是自反的; 事实上这时 $\left(X^*\right)^{**}=X^{***}=\left(X^{**}\right)^*=X^*$.

> **定理 2.5.3 (典则映射的保范性)**
> 
> 设 $X$ 是赋范线性空间, 则典范映射 $J:x\mapsto{}x^{**}$ 一定是从 $X$ 到 $X^{**}$ 的保范的线性算子, 即 (i) $\left(\alpha{}x+\beta{}y\right)^{**}=\alpha{}x^{**}+\beta{}y^{**}$; (ii) $\left\|x^{**}\right\|=\left\|x\right\|$.

> **定义 3.1.1 (疏朗集)**
> 
> 设 $A$ 是度量空间 $X$ 的一个子集, 如果 $A$ 的闭包 $\overline{A}$ 不含有 $X$ 的非空开集, 即 $\overline{A}$ 没有内点, 则称 $A$ 在 $X$ 中是疏朗的.

> **定理 3.1.1 (贝尔纲定理)**
> 
> 完备度量空间是第二纲的.

> **注 3.1.1 (疏朗集的等价刻画)**
> 
> 从定义可以看出, $A$ 是疏朗集当且仅当 $\overline{A}$ 是疏朗的. 由此易得 $A$ 是疏朗集也等价于 $\overline{A}$ 的余集 $\overline{A}^c=X\setminus\overline{A}$ 是稠密的.

## 2.4-5 (有界闭凸集的上下边界函数)

设 $A$ 是 $\mathbb{R}^2$ 中有界闭凸集. $B$ 是 $A$ 在 $x$ 轴上的投影. 证明: $B$ 是一个闭区间, 且存在两个 $B$ 上的凹函数 $f_1\left(x\right)$ 和凸函数 $f_2\left(x\right)$, 使得

$$
A=\left\{\left(x,y\right):x\in{}B,f_2\left(x\right)\le{}y\le{}f_1\left(x\right)\right\}.
$$

### 解答 2.4-5

记 $\pi\left(x,y\right)=x$, 则 $B=\pi\left(A\right)$.

$B$ 是闭区间. $A$ 是**定义 2.4.1 (凸集)**, $\pi$ 是线性映射, 故 $B=\pi\left(A\right)$ 是凸集. 又 $A$ 有界闭, 故 $A$ 紧, 而 $\pi$ 连续, 故 $B=\pi\left(A\right)$ 紧, 特别地 $B$ 闭且有界.

$\blacksquare$

对每个 $x\in{}B$, 截面 $A_x=\left\{y:\left(x,y\right)\in{}A\right\}$ 是 $\mathbb{R}$ 中的非空紧凸集, 故 $A_x=\left[\min{}A_x,\max{}A_x\right]$. 令

$$
f_1\left(x\right)=\max{}A_x,\quad{}f_2\left(x\right)=\min{}A_x,\quad{}x\in{}B.
$$

则 $f_1,f_2$ 是 $B$ 上的实值函数, 且

$$
A_x=\left\{y:f_2\left(x\right)\le{}y\le{}f_1\left(x\right)\right\},\quad{}x\in{}B.
$$

再证 $f_1$ 凹, $f_2$ 凸. 设 $x_1,x_2\in{}B$, $t\in\left[0,1\right]$, $x=tx_1+\left(1-t\right)x_2$. 取 $y_1=f_1\left(x_1\right)$, $y_2=f_1\left(x_2\right)$, 则 $\left(x_1,y_1\right),\left(x_2,y_2\right)\in{}A$; 由 $A$ 凸, $\left(x,ty_1+\left(1-t\right)y_2\right)\in{}A$, 故

$$
f_1\left(x\right)\ge{}tf_1\left(x_1\right)+\left(1-t\right)f_1\left(x_2\right),
$$

即 $f_1$ 是 $B$ 上的凹函数. 同理, $f_2$ 是 $B$ 上的凸函数.

$\blacksquare$

最后证恒等式. 设 $\left(x,y\right)\in{}A$, 则 $x\in{}B$ 且 $y\in{}A_x$, 故 $f_2\left(x\right)\le{}y\le{}f_1\left(x\right)$, 即 $A$ 含于右端.

反之设 $x\in{}B$, $f_2\left(x\right)\le{}y\le{}f_1\left(x\right)$. 因 $A$ 紧, $\left(x,f_1\left(x\right)\right)$ 与 $\left(x,f_2\left(x\right)\right)$ 都属于 $A$; 若 $f_1\left(x\right)=f_2\left(x\right)$, 则 $y$ 就等于这个值, $\left(x,y\right)\in{}A$. 否则有 $t\in\left[0,1\right]$ 使 $y=tf_1\left(x\right)+\left(1-t\right)f_2\left(x\right)$, 由 $A$ 凸得

$$
\left(x,y\right)=t\left(x,f_1\left(x\right)\right)+\left(1-t\right)\left(x,f_2\left(x\right)\right)\in{}A.
$$

故 $A$ 等于右端.

$\blacksquare$

## 2.4-6 (凸函数在一点处的支撑直线)

设 $\varphi$ 是直线 $\mathbb{R}$ 上的凸函数. 使用**定理 2.4.1 (凸集分离定理)** 证明: 对任意点 $x\in\mathbb{R}$, 存在常数 $m$ 使得

$$
\varphi\left(y\right)-\varphi\left(x\right)\ge{}m\left(y-x\right),\quad\forall{}y\in\mathbb{R}.
$$

### 解答 2.4-6

记 $\varphi$ 的上方图为

$$
M=\left\{\left(u,v\right)\in\mathbb{R}^2:v\ge\varphi\left(u\right)\right\},
$$

并取单点集 $N=\left\{\left(x,\varphi\left(x\right)\right)\right\}$. 按**例 2.4.2 (凸函数的上方图是凸集)**, $M$ 是凸集; 按**定义 2.4.1 (凸集)**, $N$ 也是凸集, 且 $M^\circ\cap{}N=\emptyset$.

由**定理 2.4.1 (凸集分离定理)**, 存在 $\mathbb{R}^2$ 上非零的连续线性泛函 $f$, 使

$$
\sup_{\left(u,v\right)\in{}M}f\left(u,v\right)\le\inf_{\left(u,v\right)\in{}N}f\left(u,v\right)=f\left(x,\varphi\left(x\right)\right).
$$

$\mathbb{R}^2$ 上的连续线性泛函必形如 $f\left(u,v\right)=au+bv$, 其中 $a,b$ 不全为零. 对 $y\in\mathbb{R}$ 取 $\left(u,v\right)=\left(y,\varphi\left(y\right)\right)\in{}M$, 上式给出

$$
ay+b\varphi\left(y\right)\le{}ax+b\varphi\left(x\right),
$$

整理得

$$
\varphi\left(y\right)-\varphi\left(x\right)\ge\frac{a}{b}\left(x-y\right)=\left(-\frac{a}{b}\right)\left(y-x\right).
$$

取 $m=-a/b$ 证毕.

$\blacksquare$

## 2.4-7 (凸集与子空间的分离)

设 $V$ 是实赋范线性空间, $M$ 是 $V$ 的凸子集, $M^\circ$ 非空, $F$ 是 $V$ 的线性子空间, $M^\circ\cap{}F=\emptyset$. 则存在非零的 $f\in{}V^*$, 满足

$$
f\left(x\right)\le0,\quad\forall{}x\in{}M;\quad{}f\left(x\right)=0,\quad\forall{}x\in{}F.
$$

### 解答 2.4-7

按**定义 2.4.3 (分离与严格分离)**, 由**定理 2.4.1 (凸集分离定理)** 与题设 $M^\circ\cap{}F=\emptyset$, 存在非零的 $f\in{}V^*$ 使

$$
f\left(x\right)\le{}f\left(y\right),\quad\forall{}x\in{}M,\quad\forall{}y\in{}F.
$$

记 $d=\inf_{y\in{}F}f\left(y\right)$. 因 $0\in{}F$, 有 $d\le{}f\left(0\right)=0$; 于是

$$
f\left(x\right)\le{}d\le0,\quad\forall{}x\in{}M.
$$

$\blacksquare$

再证 $f$ 在 $F$ 上恒为零. 任给 $y\in{}F$ 与正整数 $n$, 由 $ny\in{}F$ 得 $f\left(ny\right)=nf\left(y\right)\ge{}d$; 若 $f\left(y\right)<0$, 则当 $n$ 充分大时 $nf\left(y\right)<{d}$, 与 $nf\left(y\right)\ge{}d$ 矛盾. 故 $f\left(y\right)\ge0$; 同样有 $-f\left(y\right)\ge0$. 于是 $f\left(y\right)=0$.

$\blacksquare$

## 2.4-8 (凸集作为半空间之交)

设 $V$ 是实赋范线性空间, $M$ 是 $V$ 的凸子集. 证明:

(i) 若 $M$ 是闭的, 则 $M$ 是一些闭半空间的交.

(ii) 若 $M$ 是开的, 则 $M$ 是一些开半空间的交.

### 解答 2.4-8

(i) 记 $\mathcal{H}$ 为一切包含 $M$ 的闭半空间之族, 显然 $M\subset\bigcap\mathcal{H}$. 反之设 $x\notin{}M$. 因 $M$ 闭, $d\left(x,M\right)=:\delta>0$. 取 $N=\left\{x\right\}$, 由**推论 2.4.1 (闭凸集与紧凸集的严格分离)**, 存在 $f\in{}V^*$ 与实数 $\beta$, 使

$$
f\left(y\right)\le\beta<{f}\left(x\right),\quad\forall{}y\in{}M.
$$

令 $H=\left\{z:f\left(z\right)\le\beta\right\}$, 则 $H$ 是闭半空间, 而 $x\notin{}H$. 故 $x\notin\bigcap\mathcal{H}$, 即 $\bigcap\mathcal{H}\subset{}M$. 结合 $M\subset\bigcap\mathcal{H}$ 得 $M=\bigcap\mathcal{H}$.

$\blacksquare$

(ii) 记 $\mathcal{H}'$ 为一切包含 $M$ 的开半空间之族, 显然 $M\subset\bigcap\mathcal{H}'$. 反之设 $x\notin{}M$. 因 $M$ 开凸, $M^\circ=M$ 非空而 $x\notin{}M^\circ$; 由**引理 2.4.1 (一点与凸集的分离)**, 存在非零的 $f\in{}V^*$ (否则开半空间不存在), 使

$$
f\left(y\right)\le{}f\left(x\right),\quad\forall{}y\in{}M.
$$

下证左端对 $y\in{}M$ 是严格的. 若某个 $y_0\in{}M$ 使 $f\left(y_0\right)=f\left(x\right)$, 则对任意 $u\in{}V$ 与充分小的 $t>0$, 由 $M$ 开得 $y_0\pm{}tu\in{}M$, 于是

$$
f\left(y_0\right)\pm{}tf\left(u\right)\le{}f\left(x\right)=f\left(y_0\right),
$$

故 $f\left(u\right)\le0$ 且 $-f\left(u\right)\le0$, 即 $f\left(u\right)=0$; 由 $u$ 任意得 $f=0$, 与 $f\ne0$ 矛盾. 所以

$$
f\left(y\right)<{f}\left(x\right),\quad\forall{}y\in{}M,
$$

令 $H'=\left\{z:f\left(z\right)<{f}\left(x\right)\right\}$, 则 $H'$ 是闭半空间, 而 $x\notin{H'}$. 故 $x\notin\bigcap\mathcal{H'}$, 即 $\bigcap\mathcal{H'}\subset{}M$. 结合 $M\subset\bigcap\mathcal{H'}$ 得 $M=\bigcap\mathcal{H'}$.

$\blacksquare$

## 2.4-9 (均衡凸开集与凸集的分离)

设集合 $A$ 是复赋范线性空间 $V$ 中的一个均衡凸开集, $B$ 是一个和 $A$ 不相交的非空凸子集. 证明: 存在一个复线性泛函 $f$ 和 $c>0$, 使得在 $A$ 上 $\left|f\left(x\right)\right|<{c}$, 在 $B$ 上 $\left|f\left(x\right)\right|\ge{}c$.

### 解答 2.4-9

先说明 $0\in{}A$: 取 $a\in{}A$, 由 $A$ 均衡得 $-a\in{}A$, 由 $A$ 凸得

$$
0=\frac12a+\frac12\left(-a\right)\in{}A,
$$

又 $A$ 开, 故 $A^\circ=A\ne\emptyset$.

由**定理 2.4.1 (凸集分离定理)**, 并按**注 2.4.1 (复赋范线性空间的实部分离)** 以复线性泛函的实部作分离泛函, 存在非零复线性连续泛函 $f$, 使

$$
\sup_{x\in{}A}\operatorname{Re}f\left(x\right)\le\inf_{y\in{}B}\operatorname{Re}f\left(y\right)=:c.
$$

记 $s=\sup_{x\in{}A}\operatorname{Re}f\left(x\right)$. 因 $A$ 均衡, 对 $x\in{}A$ 与 $\left|\lambda\right|=1$ 有 $\lambda{}x\in{}A$, 故

$$
\left|f\left(x\right)\right|=\sup_{\left|\lambda\right|=1}\operatorname{Re}\left(\lambda{}f\left(x\right)\right)=\sup_{\left|\lambda\right|=1}\operatorname{Re}f\left(\lambda{}x\right)\le{}s,
$$

从而 $0\le{}s\le{}c$, 即 $\operatorname{Re}f$ 在 $A$ 的内点 $\lambda{}x$ 处取到上确界 $s=c$. 于是对任意 $u\in{}V$ 与充分小的 $t>0$, 有 $\lambda{}x\pm{}tu\in{}A$,

$$
\operatorname{Re}f\left(\lambda{}x\pm{}tu\right)=s\pm{}t\operatorname{Re}f\left(u\right),
$$

而左端总不超过 $s$, 故 $\operatorname{Re}f\left(u\right)=0$; 由 $u$ 任意得 $\operatorname{Re}f=0$, 从而 $\operatorname{Im}f\left(u\right)=-\operatorname{Re}f\left(\mathrm{i}u\right)=0$, 即 $f=0$, 与 $f\ne0$ 矛盾. 故

$$
\left|f\left(x\right)\right|<{c},\quad\forall{}x\in{}A.
$$

$\blacksquare$

最后, 对 $y\in{}B$ 有

$$
\left|f\left(y\right)\right|\ge\operatorname{Re}f\left(y\right)\ge{}c.
$$

$\blacksquare$

## 2.4-11 (闭凸集的距离公式)

设 $M$ 是实赋范线性空间 $X$ 的凸子集.

(i) 证明: 若 $M$ 是闭的, 则对任意 $x\notin{}M$, 我们有

$$
d\left(x,M\right)=\sup_{f\in{}X^*,\left\|f\right\|=1}\left(f\left(x\right)-\sup_{z\in{}M}f\left(z\right)\right).
$$

(ii) 当 $M$ 不是闭的时候, (i) 的结论是否成立? 考虑

$$
E=\left\{x\in{}l^2:\exists{}N\ge1,x_N>0;\forall{}n>{N},x_n=0\right\},
$$

我们承认: 不存在非零的 $f\in\left(l^2\right)^*$ 分离 $E$ 与 $\left\{0\right\}$.

### 解答 2.4-11

(i) 设 $M$ 非空闭凸, $x\notin{}M$, $\delta=d\left(x,M\right)>0$. 记上式右端为 $s$.

先证 $s\le\delta$. 任给 $f\in{}X^*$, $\left\|f\right\|=1$ 与 $z\in{}M$, 有

$$
f\left(x\right)-f\left(z\right)\le\left\|f\right\|\left\|x-z\right\|=\left\|x-z\right\|,
$$

对 $z\in{}M$ 取下确界得 $f\left(x\right)-\sup_{z\in{}M}f\left(z\right)\le\delta$, 再对 $f$ 取上确界得 $s\le\delta$.

$\blacksquare$

再证 $s\ge\delta$. 令 $C=M-x=\left\{z-x:z\in{}M\right\}$, 它是 $X$ 中的闭凸集, 且 $d\left(0,C\right)=\delta$; 于是开球 $B\left(0,\delta\right)$ 与 $C$ 不交. 由**定理 2.4.1 (凸集分离定理)**, 存在非零的 $f\in{}X^*$, 使

$$
\sup_{\left\|u\right\|<\delta}f\left(u\right)\le\inf_{c\in{}C}f\left(c\right).
$$

左端等于 $\delta\left\|f\right\|$, 故

$$
\delta\left\|f\right\|\le\inf_{z\in{}M}\left(f\left(z\right)-f\left(x\right)\right),
$$

即对一切 $z\in{}M$,

$$
f\left(z\right)-f\left(x\right)\ge\delta\left\|f\right\|.
$$

令 $g=-f/\left\|f\right\|$, 则 $\left\|g\right\|=1$, 且对 $z\in{}M$,

$$
g\left(x\right)-g\left(z\right)=\frac{f\left(z\right)-f\left(x\right)}{\left\|f\right\|}\ge\delta,
$$

对 $z\in{}M$ 取下确界得 $g\left(x\right)-\sup_{z\in{}M}g\left(z\right)\ge\delta$, 再对 $f$ 取上确界得 $s\ge\delta$.

$\blacksquare$

(ii) 结论不成立. 考虑

$$
E=\left\{x\in{}l^2:\exists{}N\ge1,x_N>0;\forall{}n>{N},x_n=0\right\}.
$$

即 $l^2$ 中只有有限个坐标非零, 且最后一个非零坐标为正的点之全体. 易知对 $\lambda>0$ 有 $\lambda{}E=E$. 又 $0\notin{}E$, $0\in\overline{E}$, 即 $E$ 不闭, 且 $d\left(0,E\right)=0$.

由于不存在非零的 $f\in\left(l^2\right)^*$ 分离 $E$ 与 $\left\{0\right\}$; 按**定义 2.4.3 (分离与严格分离)**, 这等价于不存在非零的 $f$ 使 $f\le0$ 在 $E$ 上成立. 于是对每个 $f\ne0$ 都存在 $z\in{}E$ 使 $f\left(z\right)>0$; 又 $\lambda{}z\in{}E$ 对一切 $\lambda>0$ 成立, 故

$$
\sup_{z\in{}E}f\left(z\right)=+\infty,\quad\forall{}f\ne0.
$$

因此对每个 $f\in\left(l^2\right)^*$, $\left\|f\right\|=1$, 都有

$$
f\left(0\right)-\sup_{z\in{}E}f\left(z\right)=-\infty,
$$

对 $f$ 取上确界时, 右侧并不等于 $d\left(0,E\right)=0$. 故 (i) 的结论在 $M$ 不闭时不成立.

$\blacksquare$

## 2.5-1 ($L^p\left(\mathbb{R}\right)$ 的对偶空间)

设 $F\in{}L^p\left(\mathbb{R}\right)^*\left(1\le{}p<\infty\right)$. 证明: 存在唯一的 $\beta\in{}L^q\left(\mathbb{R}\right)$ ($\frac1p+\frac1q=1$), 使得

$$
F\left(f\right)=\int_{\mathbb{R}}f\left(t\right)\beta\left(t\right)\,\mathrm{d}t,\quad\forall{}f\in{}L^p\left(\mathbb{R}\right),
$$

并且 $\left\|F\right\|=\left\|\beta\right\|_q$. 从而映射 $F\mapsto\beta$ 是 $L^p\left(\mathbb{R}\right)^*$ 到 $L^q\left(\mathbb{R}\right)$ 的保范线性同构, 即在这个意义下 $L^p\left(\mathbb{R}\right)^*=L^q\left(\mathbb{R}\right)$.

### 解答 2.5-1

勒贝格测度是 $\mathbb{R}$ 上的 $\sigma$-有限测度, 由**注 2.5.1 (一般可测空间上 $L^p$ 的对偶)**, 存在唯一的 $\beta\in{}L^q\left(\mathbb{R}\right)$ 使上式成立, 且

$$
\left\|F\right\|=\left\|\beta\right\|_q.
$$

$\blacksquare$

再证这个对应是同构 (单满线性保范). 任给 $\beta\in{}L^q\left(\mathbb{R}\right)$, 令

$$
F_\beta\left(f\right)=\int_{\mathbb{R}}f\left(t\right)\beta\left(t\right)\,\mathrm{d}t,\quad{}f\in{}L^p\left(\mathbb{R}\right).
$$

定义该映射为 $\Phi$:

$$
\Phi:L^p(\mathbb{R})^*\to{}L^q(\mathbb{R}),\quad\Phi(F)=\beta.
$$

从**注 2.5.1 (一般可测空间上 $L^p$ 的对偶)** 知其满射且保范; 积分的线性性易知 $\Phi$ 的线性性; 唯一性又给出其单射: 若 $\beta_1=\beta_2$, 即 $\Phi(F_1)=\Phi(F_2)$, 则由唯一性可知 $F_1(f)=F_2(f)$. 故 $F\mapsto\beta$ 是 $L^p\left(\mathbb{R}\right)^*$ 到 $L^q\left(\mathbb{R}\right)$ 的保范线性同构, 即在这个意义下 $L^p\left(\mathbb{R}\right)^*=L^q\left(\mathbb{R}\right)$.

$\blacksquare$

## 2.5-2 (几乎处处有限可测函数空间上的泛函)

设 $S$ 是区间 $\left[0,1\right]$ 上几乎处处有限可测函数的全体组成的线性空间, 如果对于任意的 $f,g\in{}S$, 定义度量

$$
d\left(f,g\right)=\int_0^1\frac{\left|f\left(t\right)-g\left(t\right)\right|}{1+\left|f\left(t\right)-g\left(t\right)\right|}\,\mathrm{d}t.
$$

证明:

(i) $L^1\left[0,1\right]$ 在 $\left(S,d\right)$ 中稠密.

(ii) $\left(S,d\right)$ 上不存在非零的连续线性泛函.

### 解答 2.5-2

(i) 设 $f\in{}S$, $n\ge1$, 令

$$
f_n=f\chi_{\left\{\left|f\right|\le{}n\right\}}.
$$

则 $\left|f_n\right|\le{}n$ 且 $f_n$ 可测, 故 $f_n\in{}L^1\left[0,1\right]$. 因 $f$ 几乎处处有限, $\left|f-f_n\right|\to0$ 几乎处处成立; 又

$$
\frac{\left|f-f_n\right|}{1+\left|f-f_n\right|}\le\chi_{\left\{\left|f\right|>{n}\right\}},
$$

由控制收敛定理得 $d\left(f,f_n\right)\to0$. 故每个 $f\in{}S$ 都是 $L^1\left[0,1\right]$ 中一列元素的 $d$-极限, 即 $L^1\left[0,1\right]$ 在 $\left(S,d\right)$ 中稠密.

$\blacksquare$

(ii) 示性函数. 设 $\Lambda$ 是 $\left(S,d\right)$ 上的连续线性泛函. 由 $\Lambda$ 在 $0$ 处连续, 对于任意的 $\varepsilon>0$, 存在 $\delta>0$, 使

$$
d\left(g,0\right)<\delta\Rightarrow\left|\Lambda{}g\right|\le1.
$$

这里取 $\varepsilon=1$. 设 $A\subset\left[0,1\right]$ 可测, $m\left(A\right)<\delta$, $c$ 是常数. 取 $g=c\chi_A$, 因 $d\left(c\chi_A,0\right)<\delta$, 则 $\left|\Lambda\left(c\chi_A\right)\right|\le1$. 但线性有 $\Lambda\left(c\chi_A\right)=c\Lambda\left(\chi_A\right)$, 对任意的 $c$ 都有上界 $1$ 只能 $\Lambda\left(\chi_A\right)=0$.

示性函数的线性组合即为简单 (阶梯) 函数, 将阶梯函数加和即为 $S$ 中有界函数, 由 (i) 知有界函数能逼近 $S$ 中任意函数, 因此对于任意的 $g(S)$, $\Lambda(g)=0$, 即 $\left(S,d\right)$ 上不存在非零的连续线性泛函.

$\blacksquare$

## 2.5-4 ($C_0\left(\mathbb{R}\right)$ 上的泛函与有界变差函数)

对巴拿赫空间 $C_0\left(\mathbb{R}\right)=\left\{f\in{}C\left(\mathbb{R}\right):\lim_{\left|x\right|\to\infty}f\left(x\right)=0\right\}$, 设 $F\in{}C_0\left(\mathbb{R}\right)^*$, 证明: 存在直线上的有界变差函数 $\alpha\left(x\right)$, 使得

$$
F\left(f\right)=\int_{\mathbb{R}}f\left(x\right)\,\mathrm{d}\alpha\left(x\right),\quad\forall{}f\in{}C_0\left(\mathbb{R}\right).
$$

### 解答 2.5-4

把 $\mathbb{R}$ 两端紧化为 $\overline{\mathbb{R}}=\left[-\infty,+\infty\right]$, 则 $\overline{\mathbb{R}}$ 是紧度量空间. 每个 $f\in{}C_0\left(\mathbb{R}\right)$ 按 $f\left(\pm\infty\right)=0$ 延拓后属于 $C\left(\overline{\mathbb{R}}\right)$, 且

$$
C_0\left(\overline{\mathbb{R}}\right)=\left\{g\in{}C\left(\overline{\mathbb{R}}\right):g\left(\pm\infty\right)=0\right\}
$$

是 $C\left(\overline{\mathbb{R}}\right)$ 的闭线性子空间, 两者范数相同.

对实赋范线性空间 $C\left(\overline{\mathbb{R}}\right)$ 上的实线性泛函 $\operatorname{Re}F$, 有 $\left\|\operatorname{Re}F\right\|=\left\|F\right\|$. 由**定理 2.3.1 (哈恩-巴拿赫延拓定理)**, 存在 $\widetilde{g}\in{}C\left(\overline{\mathbb{R}}\right)^*$, 使 $\widetilde{g}$ 延拓 $\operatorname{Re}F$ 且 $\left\|\widetilde{g}\right\|=\left\|F\right\|$. 令

$$
\widetilde{F}\left(g\right)=\widetilde{g}\left(g\right)-\mathrm{i}\widetilde{g}\left(\mathrm{i}g\right),\quad{}g\in{}C\left(\overline{\mathbb{R}}\right),
$$

则 $\widetilde{F}$ 是复线性的, 在 $C_0\left(\mathbb{R}\right)$ 上与 $F$ 一致, 且 $\left\|\widetilde{F}\right\|=\left\|F\right\|$.

由**定理 2.5.2 (里斯表示定理)**, 存在 $\overline{\mathbb{R}}$ 上唯一的全有限广义测度 $\mu$, 使

$$
\widetilde{F}\left(g\right)=\int_{\overline{\mathbb{R}}}g\,\mathrm{d}\mu,\quad\forall{}g\in{}C\left(\overline{\mathbb{R}}\right),
$$

且 $\left\|\widetilde{F}\right\|=\left|\mu\right|\left(\overline{\mathbb{R}}\right)$.

令

$$
\alpha\left(x\right)=\mu\left(\left[-\infty,x\right]\right),\quad{}x\in\mathbb{R}.
$$

对 $\mathbb{R}$ 的任一分割 $x_0<{x}_1<\cdots<{x}_n$, 有

$$
\sum_{i=1}^{n}\left|\alpha\left(x_i\right)-\alpha\left(x_{i-1}\right)\right|=\sum_{i=1}^{n}\left|\mu\left(\left(x_{i-1},x_i\right]\right)\right|\le\left|\mu\right|\left(\left(x_0,x_n\right]\right)\le\left\|\widetilde{F}\right\|,
$$

故 $\alpha$ 是有界变差函数, 其全变差不超过 $\left\|F\right\|$.

$\blacksquare$

最后, 设 $f\in{}C_0\left(\mathbb{R}\right)$. 因 $f\left(\pm\infty\right)=0$,

$$
F\left(f\right)=\widetilde{F}\left(f\right)=\int_{\overline{\mathbb{R}}}f\,\mathrm{d}\mu=\int_{\mathbb{R}}f\,\mathrm{d}\mu=\int_{\mathbb{R}}f\left(x\right)\,\mathrm{d}\alpha\left(x\right),
$$

其中 $\mathrm{d}\alpha$ 表示 $\alpha$ 诱导的 $\mathbb{R}$ 上的广义测度, 它正是 $\mu$ 在 $\mathbb{R}$ 上的限制.

$\blacksquare$

## 2.5-8 (有限维空间的自反性)

$X$ 是有限维赋范线性空间, 证明: $X$ 是自反空间.

### 解答 2.5-8

由**定理 2.5.3 (典则映射的保范性)**, 典则映射 $J:X\to{}X^{**}$ 是线性的且 $\left\|Jx\right\|=\left\|x\right\|$. 则核空间

$$
\ker{}J=\{\|Jx\|=0\}=\{\|x\|=0\}=\{0\},
$$

故 $J$ 是单射. $X$ 与 $X^{**}$ 都是 $n$ 维线性空间, 而从 $n$ 维空间到 $n$ 维空间的单射线性映射必为满射, 故 $J$ 是同构. 按**定义 2.5.1 (自反空间)**, $X$ 是自反的.

$\blacksquare$

## 2.5-9 (自反性与对偶空间的自反性)

设 $X$ 是巴拿赫空间, 证明: $X$ 是自反的充要条件是 $X^*$ 是自反的.

### 解答 2.5-9

由**例 2.5.2 (自反空间的对偶空间自反)**: 若 $X\cong{}X^{**}$, 则

$$
\left(X^*\right)^{**}=X^{***}=\left(X^{**}\right)^*\cong{}X^*.
$$

$\blacksquare$

## 3.1-1 (疏朗集的补开集刻画)

设 $A$ 是度量空间 $\left(X,d\right)$ 的子集. 证明: $A$ 是疏朗集的充要条件是对任意非空开集 $U$, 存在一个非空开子集 $V$ 使得 $V\cap{}A=\emptyset$.

### 解答 3.1-1

按**定义 3.1.1 (疏朗集)**, $A$ 疏朗即 $\overline{A}$ 没有内点.

必要性. 设 $A$ 疏朗, $U$ 是非空开集. 若 $U\subset\overline{A}$, 则 $\overline{A}$ 有内点, 矛盾; 故存在 $x\in{}U\setminus\overline{A}$. 因 $\overline{A}$ 闭, $X\setminus\overline{A}$ 开, 故

$$
V=U\cap\left(X\setminus\overline{A}\right)
$$

是含 $x$ 的非空开集, 且 $V\cap{}A\subset{}V\setminus\overline{A}=\emptyset$.

$\blacksquare$

充分性. 设对任意非空开集 $U$ 都存在非空开集 $V\subset{}U$ 使 $V\cap{}A=\emptyset$. 若 $\overline{A}$ 有内点, 即存在非空开集 $U\subset\overline{A}$, 取相应的 $V$, 但 $V\cap{}A\ne\emptyset$, 矛盾. 所以 $\overline{A}$ 没有内点, $A$ 疏朗.

$\blacksquare$

## 3.1-2 (闭疏朗集作为两个集合的边界)

设 $A$ 是完备度量空间 $\left(X,d\right)$ 中的闭疏朗集. 证明: 存在开集 $U$ 以及闭集 $V$, 使得 $A=\partial{}U=\partial{}V$.

### 解答 3.1-2

由**定义 3.1.1 (疏朗集)**, 闭集 $A=\overline{A}$ 没有内点; 由**注 3.1.1 (疏朗集的等价刻画)**, $X\setminus{}A$ 是稠密集. 取 $U=X\setminus{}A$, 它是开集; 取 $V=A$, 它是闭集. 于是

$$
A=\partial{}U=\partial{}V.
$$

$\blacksquare$

## 3.1-4 (巴拿赫空间与可列个相对列紧集)

证明无限维的巴拿赫空间不能分解成可列个相对列紧集的并集.

### 解答 3.1-4

设 $X$ 是无限维巴拿赫空间, 且

$$
X=\bigcup_{n=1}^{\infty}K_n,
$$

其中每个 $K_n$ 是相对列紧集 (按**定义 1.6.1 (相对列紧集)**). 则 $\overline{K_n}$ 中任一点列有收敛于 $X$ 中某点的子列, 而 $\overline{K_n}$ 闭, 故极限属于 $\overline{K_n}$, 即 $\overline{K_n}$ 是紧集.

先证每个 $\overline{K_n}$ 没有内点. 若存在球 $B\left(x_0,r\right)\subset\overline{K_n}$, $r>0$, 则 $\overline{B}\left(x_0,r\right)$ 是紧集 $\overline{K_n}$ 的闭子集, 故紧; 平移与伸缩不改变紧性, 故 $\overline{B}\left(0,1\right)$ 紧, 从而 $B\left(0,1\right)$ 相对列紧, 与**定理 1.6.1 (无限维空间的单位球不相对列紧)** 矛盾.

$\blacksquare$

于是每个 $K_n$ 的闭包没有内点, 按**定义 3.1.1 (疏朗集)**, $K_n$ 是疏朗集; 故 $X$ 是可数个疏朗集之并, 即 $X$ 是第一纲集. 但 $X$ 是巴拿赫空间, 完备, 由**定理 3.1.1 (贝尔纲定理)**, $X$ 是第二纲集, 矛盾. 故 $X$ 不能分解成可列个相对列紧集的并集.

$\blacksquare$

## 3.1-5 (巴拿赫空间与可列个有限维子空间)

设 $X$ 是无限维的巴拿赫空间. 证明不存在一列有限维的子空间 $\left\{L_n\right\}$, 使得

$$
X=\bigcup_{n=1}^{\infty}L_n.
$$

### 解答 3.1-5

设 $L_n$ 是 $X$ 的有限维子空间. 由**定理 1.4.2 (有限维赋范线性空间完备)**, $L_n$ 完备, 从而是 $X$ 的闭子空间; 又 $X$ 无限维, 故 $L_n\ne{}X$.

证 $L_n$ 没有内点. 若存在球 $B\left(x_0,r\right)\subset{}L_n$, 因 $x_0\in{}L_n$, 由 $L_n$ 的线性得

$$
B\left(0,r\right)=B\left(x_0,r\right)-x_0\subset{}L_n.
$$

于是对任意 $x\ne0$, 有 $\left\|\frac{r}{2\left\|x\right\|}x\right\|=\frac{r}{2}<{r}$, 故 $\frac{r}{2\left\|x\right\|}x\in{}L_n$, 再由 $L_n$ 线性得 $x\in{}L_n$; 于是 $X=L_n$, 矛盾.

按**定义 3.1.1 (疏朗集)**, $L_n$ 是疏朗集. 若 $X=\bigcup_{n=1}^{\infty}L_n$, 则 $X$ 是可数个疏朗集之并, 即第一纲集, 与**定理 3.1.1 (贝尔纲定理)** (完备度量空间是第二纲的) 矛盾. 故不存在这样的 $\left\{L_n\right\}$.

$\blacksquare$
