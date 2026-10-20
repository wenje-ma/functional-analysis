# week5

> **基础知识: 紧度量空间的性质**<br>紧的度量空间是完备的且完全有界的.

> **基础知识: 闵可夫斯基不等式**<br>设 $1\le p<\infty$, $f,g\in L^{p}$, 则 $\|f+g\|_{p}\le\|f\|_{p}+\|g\|_{p}$.

> **例 1.2.8 ($L^{p}$ 是巴拿赫空间)**<br>设 $1\le p<\infty$, 则 $L^{p}(\mathbb{R})$ 按范数 $\|f\|_{p}=\left(\int_{\mathbb{R}}|f|^{p}\,\mathrm dm\right)^{1/p}$ 是巴拿赫空间.

> **例 1.2.12 ($C[a,b]$ 是巴拿赫空间)**<br>设 $[a,b]$ 是有限闭区间, 则 $C[a,b]$ 按范数 $\|f\|=\max_{x\in[a,b]}|f(x)|$ 是巴拿赫空间.

> **引理 1.4.1 (基本点列与完备性)**<br>设 $X$ 是度量空间, 则:<br>(i) 基本点列是有界的;<br>(ii) 若 $X$ 完备, 则点列收敛当且仅当它是基本点列;<br>(iii) 完备度量空间的闭子集是完备的.

> **习题 1.4-15 (平均连续性)**<br>设 $f\in L^{p}(\mathbb{R})$, $1\le p<\infty$, 则 $\lim_{h\to0}\left(\int_{\mathbb{R}}|f(x+h)-f(x)|^{p}\,\mathrm dm\right)^{1/p}=0$.

> **定义 1.5.1 (不动点)**<br>设 $T$ 是集合 $X$ 到自身的映射. 若存在 $x\in X$ 使得 $Tx=x$, 则称 $x$ 是 $T$ 的不动点.

> **定义 1.5.2 (压缩映射)**<br>设 $X$ 是度量空间, $T:X\to X$. 若存在 $0<\theta<1$, 使得 $d(Tx,Ty)\le \theta d(x,y)$ ($\forall x,y\in X$), 则称 $T$ 是 $X$ 上的压缩映射, $\theta$ 称为压缩系数.

> **定理 1.5.1 (巴拿赫不动点定理)**<br>设 $X$ 是完备的度量空间, $T:X\to X$ 是压缩映射, 则 $T$ 在 $X$ 中存在唯一的不动点 $x$; 且对任意的 $x_0\in X$, 迭代序列 $x_n=T^{n}x_0$ 收敛于 $x$, 误差估计 $d(x_n,x)\le \frac{\theta^{n}}{1-\theta}d(x_0,Tx_0)$.

> **定义 1.6.1 (相对列紧集)**<br>设 $A$ 是度量空间 $X$ 的子集. 若 $A$ 的闭包 $\overline{A}$ 是紧集, 则称 $A$ 是相对列紧集.

> **推论 1.6.1 (相对列紧集可分且有界)**<br>相对列紧集是可分的有界集.

> **例 1.6.1 (有限维空间中相对列紧 $\Leftrightarrow$ 有界)**<br>在有限维赋范线性空间 (特别地 $\mathbb{R}^n$) 中, $A$ 是相对列紧集当且仅当 $A$ 是有界集.

> **注 1.6.1 (网中的点不必属于集合本身)**<br>$\epsilon$-网中的点可以不必属于 $A$ 本身.

> **定理 1.6.2 (列紧 $\Leftrightarrow$ 覆盖紧)**<br>度量空间 $X$ 是紧集当且仅当它是列紧集 (即 $X$ 中任意点列都有收敛子列).

> **定义 1.6.3 ($\epsilon$-网与完全有界集)**<br>设 $A$ 是度量空间 $X$ 的子集, $\epsilon>0$. 若存在 $X$ 的有限子集 $\{x_1,\dots,x_N\}$, 使得 $A\subset \bigcup_{i=1}^{N}U(x_i,\epsilon)$, 则称 $\{x_1,\dots,x_N\}$ 是 $A$ 的一个 $\epsilon$-网. 若对每个 $\epsilon>0$, $A$ 都有有限的 $\epsilon$-网, 则称 $A$ 是完全有界集.

> **定理 1.6.3 (豪斯多夫定理)**<br>设 $X$ 是完备的度量空间, $A\subset X$, 则 $A$ 是相对列紧集当且仅当 $A$ 是完全有界集.

> **推论 1.6.3 (连续函数达到上下确界)**<br>设 $X$ 是紧度量空间, $f\in C(X)$, 则 $f$ 在 $X$ 上达到上确界与下确界.

> **例 1.6.3 ($\mathbb{R}^n$ 中有界集完全有界)**<br>设 $A$ 是 $\mathbb{R}^n$ 中的有界集, 则 $A$ 是完全有界集.

> **定义 1.6.5 (一致连续与等度连续)**<br>(i) 设 $f:X\to Y$ 是度量空间之间的映射. 若对每个 $\epsilon>0$ 存在 $\delta>0$, 使得 $d_X(x_1,x_2)<\delta$ 蕴含 $d_Y(f(x_1),f(x_2))<\epsilon$, 则称 $f$ 一致连续.<br>(ii) 设 $X$ 是紧度量空间, $\mathscr{F}\subset C(X)$. 若对每个 $\epsilon>0$ 存在 $\delta>0$, 使得对一切 $f\in\mathscr{F}$ 及 $x_1,x_2\in X$, 由 $d(x_1,x_2)<\delta$ 可推出 $|f(x_1)-f(x_2)|<\epsilon$, 则称 $\mathscr{F}$ 是等度连续的.

> **定理 1.6.5 (阿泽拉-阿斯卡里定理)**<br>设 $A\subset C[a,b]$, 则 $A$ 是相对列紧集当且仅当 $A$ 是有界的且等度连续的.

> **定理 1.6.7 (科尔莫戈罗夫-里斯-弗雷歇定理)**<br>设 $A\subset L^{p}(\mathbb{R})$, $1\le p<\infty$. 则 $A$ 是完全有界集当且仅当下列三条件同时成立:<br>(i) $A$ 是有界集;<br>(ii) (等度 $L^{p}$-胎紧) 对每个 $\epsilon>0$, 存在 $M>0$, 使得 $\int_{\{|x|>M\}}|f(x)|^{p}\,\mathrm dm<\epsilon^{p}$, $\forall f\in A$;<br>(iii) (等度 $L^{p}$-范数连续) 对每个 $\epsilon>0$, 存在 $\delta>0$, 使得 $\|f(x+h)-f(x)\|_{p}\le\epsilon$, $\forall f\in A$, $\forall |h|<\delta$.

> **定理 1.6.9 (紧度量空间上的性质)**<br>设 $X$ 是紧的度量空间, 则:<br>(i) $X$ 上的连续函数是一致连续的;<br>(ii) $C(X)$ 按范数 $\|f\|=\max_{x\in X}|f(x)|$ 构成巴拿赫空间;<br>(iii) (阿泽拉-阿斯卡里定理) $A\subset C(X)$ 是相对列紧集当且仅当 $A$ 是有界的且等度连续的.

---

## 1.5-8 (隐函数存在定理)

设函数 $F:U\times V\to\mathbb{R}^{m}$, 其中 $U$ 和 $V$ 分别是 $\mathbb{R}^{n}$ 和 $\mathbb{R}^{m}$ 中的开区域, $(x_0,y_0)\in U\times V$. 如果 $F$ 在 $U\times V$ 中连续, 并且对于任意的 $x\in U$, $F(x,\cdot)$ 在 $V$ 中是连续可微的, 同时满足

$$
F(x_0,y_0)=0,\quad \det\left(\frac{\partial F}{\partial y}\right)(x_0,y_0)\neq 0,
$$

其中 $\frac{\partial F}{\partial y}$ 是 $F$ 关于 $y$ 的 Jacobi 矩阵. 对于 $r>0$, 令 $C(B(x_0,r),\mathbb{R}^{m})$ 表示定义在闭球 $B(x_0,r)$ 上、取值在 $\mathbb{R}^{m}$ 中的向量值连续函数空间, 它按范数

$$
\|\varphi\|=\max_{x\in B(x_0,r),\,1\le i\le m}|\varphi_i(x)|,\quad \varphi=(\varphi_1,\dots,\varphi_m),
$$

构成了一个巴拿赫空间. 证明:

(i) 存在 $r>0$ 与 $\delta>0$, 使得在 $C(B(x_0,r),\mathbb{R}^{m})$ 的子集

$$
E=\left\{\varphi\in C(B(x_0,r),\mathbb{R}^{m}):\ \varphi(x_0)=y_0,\ |\varphi(x)-y_0|\le\delta,\ \forall x\in B(x_0,r)\right\}
$$

中, $(T\varphi)(x)=\varphi(x)-\left(\frac{\partial F}{\partial y}(x_0,y_0)\right)^{-1}F(x,\varphi(x))$ 是良定义的压缩映射;

(ii) 存在 $x_0$ 的邻域 $U_0\subset U$ 以及唯一的连续函数 $\varphi:U_0\to\mathbb{R}^{m}$, 满足

$$
F(x,\varphi(x))=0,\ \forall x\in U_0,\quad \varphi(x_0)=y_0.
$$

### 解答 1.5-8

记 $A=\left(\frac{\partial F}{\partial y}\right)(x_0,y_0)$. 由线性代数知识, $\det A\neq0$ 蕴含 $A$ 是可逆矩阵; 于是 $A^{-1}$ 存在且按算子范数有界, 记其范数为 $\|A^{-1}\|$.

由于 $F(x_0,y_0)=0$ 且 $F$ 在 $U\times V$ 中连续, 故对任意 $\epsilon>0$, 存在 $r_1>0$、$\delta_1>0$, 使得 $B(x_0,r_1)\subset U$、$B(y_0,\delta_1)\subset V$, 并且当 $|x-x_0|\le r_1$、$|y-y_0|\le\delta_1$ 时有 $|F(x,y)|<\epsilon$. 取 $\epsilon=\frac{\delta_1}{2\|A^{-1}\|}$, 可找到 $r_1,\delta_1>0$ 使

$$
\|A^{-1}\|\cdot|F(x,y)|<\frac{\delta_1}{2},\quad |x-x_0|\le r_1,\ |y-y_0|\le\delta_1. \tag{1}
$$

另一方面, 由于 $F(x,\cdot)$ 对每个 $x\in U$ 连续可微, $\frac{\partial F}{\partial y}$ 在 $U\times V$ 上连续, 且 $\frac{\partial F}{\partial y}(x_0,y_0)=A$, 故存在 $0<r\le r_1$、$0<\delta\le\delta_1$, 使得当 $|x-x_0|\le r$、$|y-y_0|\le\delta$ 时有

$$
\left\|A^{-1}\frac{\partial F}{\partial y}(x,y)-I\right\|<\theta<1 \tag{2}
$$

对某个 $0<\theta<1$ 成立 (例如取 $\theta=\frac12$).

现在验证 $T$ 良定义. 取 $\varphi\in E$. 因 $F$ 连续、$\varphi$ 连续, 故 $T\varphi=\varphi-A^{-1}F(\cdot,\varphi(\cdot))$ 是 $B(x_0,r)$ 上的连续函数, 即 $T\varphi\in C(B(x_0,r),\mathbb{R}^{m})$. 又因 $F(x_0,y_0)=0$, 故

$$
(T\varphi)(x_0)=\varphi(x_0)-A^{-1}F(x_0,\varphi(x_0))=y_0-A^{-1}F(x_0,y_0)=y_0.
$$

再由 (1), 对一切 $x\in B(x_0,r)$ 有 $|(T\varphi)(x)-y_0|=|A^{-1}F(x,\varphi(x))|\le\|A^{-1}\|\cdot|F(x,\varphi(x))|<\delta$. 于是 $T\varphi\in E$, 即 $T:E\to E$ 良定义.

下证 $T$ 是压缩映射. 设 $\varphi_1,\varphi_2\in E$, $x\in B(x_0,r)$. 由于 $F(x,\cdot)$ 在包含线段 $[\varphi_2(x),\varphi_1(x)]$ 的开集 $V$ 上连续可微, 由向量值函数的微分中值定理,

$$
F(x,\varphi_1(x))-F(x,\varphi_2(x))=\left(\int_0^{1}\frac{\partial F}{\partial y}(x,\varphi_2(x)+t(\varphi_1(x)-\varphi_2(x)))\,\mathrm dt\right)(\varphi_1(x)-\varphi_2(x)).
$$

因为 $\varphi_1,\varphi_2\in E$, 故 $\varphi_2(x)+t(\varphi_1(x)-\varphi_2(x))\in B(y_0,\delta)$, 故由 (2),

$$|(T\varphi_1)(x)-(T\varphi_2)(x)|=\left|\left(I-A^{-1}\int_0^{1}\frac{\partial F}{\partial y}(x,\varphi_2(x)+t(\varphi_1(x)-\varphi_2(x)))\,\mathrm dt\right)(\varphi_1(x)-\varphi_2(x))\right|\le\theta|\varphi_1(x)-\varphi_2(x)|.
$$

对 $x$ 取最大值, 得到 $\|T\varphi_1-T\varphi_2\|\le\theta\|\varphi_1-\varphi_2\|$, 其中 $0<\theta<1$. 故 $T$ 是 $E$ 上的压缩映射. 而 $E$ 关于条件 $\varphi(x_0)=y_0$、$|\varphi(x)-y_0|\le\delta$ ($\forall x$) 是闭集, 故 $E$ 是巴拿赫空间 $C(B(x_0,r),\mathbb{R}^{m})$ 的闭子集, 由**引理 1.4.1 (基本点列与完备性)(iii)**, $E$ 是完备的. 由**定理 1.5.1 (巴拿赫不动点定理)**, $T$ 在 $E$ 中存在唯一的不动点 $\varphi$, 即 $T\varphi=\varphi$. 于是对一切 $x\in B(x_0,r)$,

$$
\varphi(x)-A^{-1}F(x,\varphi(x))=\varphi(x)\ \Rightarrow\ A^{-1}F(x,\varphi(x))=0\ \Rightarrow\ F(x,\varphi(x))=0
$$

(最后一步用到 $A^{-1}$ 可逆, 故 $A^{-1}F=0$ 蕴含 $F=0$). 且 $\varphi(x_0)=y_0$.

取 $U_0=B(x_0,r)\cap U$, 则 $U_0$ 是 $x_0$ 在 $U$ 中的邻域, $\varphi|_{U_0}$ 连续, 满足 $F(x,\varphi(x))=0$ ($\forall x\in U_0$) 且 $\varphi(x_0)=y_0$. 唯一性: 若在 $U_0'\subset U$ 上还有连续解 $\psi$, 满足 $F(x,\psi(x))=0$、$\psi(x_0)=y_0$, 则由 $\psi$ 的连续性和 $\psi(x_0)=y_0$, 适当缩小邻域可设 $B(x_0,r)\subset U_0\cap U_0'$ 且 $|\psi(x)-y_0|\le\delta$ 对 $x\in B(x_0,r)$ 成立, 于是 $\psi|_{B(x_0,r)}\in E$ 且 $T\psi=\psi$, 由不动点的唯一性得 $\psi=\varphi$ 于 $B(x_0,r)$, 进而于 $U_0\cap U_0'$. 证毕.

---

## 1.6-1

设 $A$ 是紧的度量空间, $\{F_\lambda\}$ 是 $A$ 的一族闭子集, 如果 $\{F_\lambda\}$ 中任意有限个 $F_{\lambda_1},\dots,F_{\lambda_n}$ 的交集都不空, 那么 $\bigcap_\lambda F_\lambda$ 也不空. 反之, 如果度量空间 $A$ 具有如下性质: 对于 $A$ 中任意的闭子集族 $\{F_\lambda\}$, 从任意有限交集不空可推出 $\bigcap_\lambda F_\lambda$ 不空, 那么 $A$ 是紧的度量空间.

### 解答 1.6-1

先证第一句. 用反证法, 假设 $\bigcap_\lambda F_\lambda=\emptyset$. 由德摩根律, $\{A\setminus F_\lambda\}$ 是 $A$ 的开覆盖: 每个 $A\setminus F_\lambda$ 都是开集 (因 $F_\lambda$ 是闭集), 且 $\bigcup_\lambda(A\setminus F_\lambda)=A\setminus\bigcap_\lambda F_\lambda=A$. 由**定理 1.6.2 (列紧 $\Leftrightarrow$ 覆盖紧)**, 紧的度量空间 $A$ 的每个开覆盖都有有限子覆盖, 故存在有限个指标 $\lambda_1,\dots,\lambda_n$ 使

$$
A=\bigcup_{i=1}^{n}(A\setminus F_{\lambda_i})=A\setminus\bigcap_{i=1}^{n}F_{\lambda_i},
$$

从而 $\bigcap_{i=1}^{n}F_{\lambda_i}=\emptyset$, 这与 $\{F_\lambda\}$ 的任意有限交集不空矛盾. 故 $\bigcap_\lambda F_\lambda\neq\emptyset$.

再证第二句. 设度量空间 $A$ 具有所述有限交性质, 证明 $A$ 是紧的. 由**定理 1.6.2 (列紧 $\Leftrightarrow$ 覆盖紧)**, 只须证明 $A$ 是列紧的, 即 $A$ 中任意点列都有收敛子列. 用反证法, 设存在点列 $\{x_n\}\subset A$ 没有收敛子列. 令 $F_n=\overline{\{x_k:k\ge n\}}$ ($A$ 中从第 $n$ 项起的尾集的闭包). 则每个 $F_n$ 是闭集, 且 $F_1\supset F_2\supset\cdots$, 故任意有限个 $F_{n_1},\dots,F_{n_m}$ (设 $n=\max\{n_i\}$) 的交 $\bigcap_{i=1}^{m}F_{n_i}=F_n\neq\emptyset$ (因为 $x_n\in F_n$). 由有限交性质, $\bigcap_{n=1}^{\infty}F_n\neq\emptyset$. 取 $x\in\bigcap_{n=1}^{\infty}F_n$. 由 $x\in F_n=\overline{\{x_k:k\ge n\}}$, 对每个 $n$ 与 $\epsilon=\frac1m$, 存在 $k_m\ge n$ 使 $d(x_{k_m},x)<\frac1m$, 于是取子列 $k_1<k_2<\cdots$ 即得 $x_{k_m}\to x$, 这与 $\{x_n\}$ 没有收敛子列矛盾. 故 $A$ 列紧, 由**定理 1.6.2 (列紧 $\Leftrightarrow$ 覆盖紧)**, $A$ 是紧的. 证毕.

---

## 1.6-3

对 $\mathbb{R}^{n}$ 的有界子集 $E$ 及数 $\epsilon>0$, 给出它的一个有限 $\epsilon$-网.

### 解答 1.6-3

因 $E$ 有界, 故存在 $M>0$ 使 $E\subset[-M,M]^{n}$. 把 $\mathbb{R}^{n}$ 按平行于坐标轴的方向分割成边长为 $a=\frac{\epsilon}{\sqrt{n}}$ 的小方体

$$
\left\{\prod_{i=1}^{n}[k_i a,\ (k_i+1)a]:\ k_i\in\mathbb{Z},\ i=1,\dots,n\right\}.
$$

每个小方体的直径不超过 $\sqrt{n}\,a=\epsilon$. 因为 $E\subset[-M,M]^{n}$, 故与 $E$ 相交的小方体只有有限多个 (事实上至多 $\left(\left\lfloor\frac{2M}{a}\right\rfloor+2\right)^{n}$ 个). 对这有限多个小方体, 每个与 $E$ 相交的方体 $Q_j$ 中取一个点 $x_j\in E\cap Q_j$, 得到有限集 $\{x_1,\dots,x_N\}$. 对任意 $x\in E$, $x$ 属于某个与 $E$ 相交的方体 $Q_j$, 故 $|x-x_j|\le\operatorname{diam}Q_j\le\epsilon$, 即 $x\in U(x_j,\epsilon)$. 所以 $\{x_1,\dots,x_N\}$ 是 $E$ 的有限 $\epsilon$-网. 证毕.

---

## 1.6-5

设 $L$ 是赋范线性空间, $A$ 是 $L$ 的有界子集. 证明: $A$ 是完全有界集的充要条件是: 对任何 $\epsilon>0$, 存在 $L$ 的有限维子空间 $M$, 使 $A$ 中每个点与 $M$ 的距离都小于 $\epsilon$.

### 解答 1.6-5

先证充分性. 设 $A$ 完全有界. 由**定义 1.6.3 ($\epsilon$-网与完全有界集)**, 对 $\epsilon>0$, $A$ 有有限的 $\epsilon$-网 $\{a_1,\dots,a_N\}\subset A$. 令 $M=\operatorname{span}\{a_1,\dots,a_N\}$, 则 $M$ 是 $L$ 的有限维子空间. 对任意 $a\in A$, 存在 $a_i$ 使 $\|a-a_i\|<\epsilon$, 而 $a_i\in M$, 故 $d(a,M)=\inf_{m\in M}\|a-m\|\le\|a-a_i\|<\epsilon$. 故 $A$ 中每个点与 $M$ 的距离小于 $\epsilon$.

再证必要性. 设对任何 $\epsilon>0$ 存在有限维子空间 $M$, 使 $A$ 中每个点与 $M$ 的距离小于 $\epsilon$. 给定 $\epsilon>0$, 取 $M$ 使 $d(a,M)<\frac{\epsilon}{2}$ 对一切 $a\in A$ 成立. 对每个 $a\in A$, 由 $d(a,M)<\frac{\epsilon}{2}$ 可取 $m(a)\in M$ 使 $\|a-m(a)\|<\frac{\epsilon}{2}$. 因 $A$ 有界且 $\|m(a)\|\le\|m(a)-a\|+\|a\|$, 故集合 $\{m(a):a\in A\}\subset M$ 有界. 由**例 1.6.1 (有限维空间中相对列紧 $\Leftrightarrow$ 有界) 与例 1.6.3 ($\mathbb{R}^n$ 中有界集完全有界)**, 有限维赋范线性空间 $M$ 中的有界集是完全有界集, 故存在有限集 $\{m_1,\dots,m_N\}\subset M$ 使 $\{m(a):a\in A\}\subset\bigcup_{i=1}^{N}U(m_i,\epsilon/2)$. 于是对任意 $a\in A$, 存在 $i$ 使 $\|m(a)-m_i\|<\frac{\epsilon}{2}$, 故

$$
\|a-m_i\|\le\|a-m(a)\|+\|m(a)-m_i\|<\frac{\epsilon}{2}+\frac{\epsilon}{2}=\epsilon.
$$

所以 $\{m_1,\dots,m_N\}$ 是 $A$ 的有限 $\epsilon$-网 (由**注 1.6.1 (网中的点不必属于集合本身)**, 网点不必属于 $A$). 由 $\epsilon$ 的任意性, $A$ 完全有界. 证毕.

---

## 1.6-6

设 $0<\alpha\le1$. $C_\alpha[a,b]$ 是由在 $[a,b]$ 上满足 $\mathrm{H\ddot{o}lder}$ 条件 $|f(x)-f(x')|\le M_f|x-x'|^{\alpha}$, 并且 $f(a)=0$ 的函数组成的线性空间, 其范数定义为

$$
\|f\|=\sup_{x,x'\in[a,b],\,x\neq x'}\frac{|f(x)-f(x')|}{|x-x'|^{\alpha}}.
$$

试写出 $C_\alpha[a,b]$ 中的点集是完全有界集的一些条件.

### 解答 1.6-6

我给出如下的充分条件: 若 $A\subset C_\alpha[a,b]$ 满足

(i) $A$ 在 $C_\alpha[a,b]$ 中有界, 即存在 $M>0$ 使 $\|f\|\le M$ ($\forall f\in A$) ;

(ii) 对每个 $\epsilon>0$, 存在 $\delta>0$, 使得

$$
\sup_{f\in A}\ \sup_{0<|x-x'|<\delta}\frac{|f(x)-f(x')|}{|x-x'|^{\alpha}}<\epsilon,
$$

则 $A$ 是完全有界集.

先由 (i) 推出 $A$ 在 $C[a,b]$ 中一致有界且等度连续. 事实上, 对 $f\in A$ 与 $x\in[a,b]$, 由 $f(a)=0$ 得 $|f(x)|=|f(x)-f(a)|\le\|f\||x-a|^{\alpha}\le M(b-a)^{\alpha}$, 故 $A$ 在 $C[a,b]$ 中一致有界; 且 $|f(x)-f(x')|\le\|f\||x-x'|^{\alpha}\le M|x-x'|^{\alpha}$, 故 $A$ 在 $C[a,b]$ 中等度连续. 由**定理 1.6.5 (阿泽拉-阿斯卡里定理)**, $A$ 在 $C[a,b]$ 中相对列紧, 从而是完全有界的 (由**定理 1.6.3 (豪斯多夫定理)**, 因 $C[a,b]$ 完备).

下面用 $\epsilon$-网直接证明 $A$ 在 $C_\alpha[a,b]$ 中完全有界. 给定 $\epsilon>0$, 由条件 (ii) 取 $\delta>0$ 使

$$
\sup_{f\in A}\ \sup_{0<|x-x'|<\delta}\frac{|f(x)-f(x')|}{|x-x'|^{\alpha}}<\frac{\epsilon}{4}. \tag{1}
$$

取 $[a,b]$ 的一个分划 $a=t_0<t_1<\cdots<t_N=b$, 使网格长 $h=\max_j(t_{j+1}-t_j)<\delta$, 且 $h$ 小到

$$
\frac{\epsilon h^{\alpha}}{\delta^{\alpha}}<\frac{\epsilon}{4}. \tag{2}
$$

由 (i) 得到的一致有界性, 求值向量集 $\{(f(t_0),\dots,f(t_N)):f\in A\}\subset\mathbb{R}^{N+1}$ 有界, 由**例 1.6.3 ($\mathbb{R}^n$ 中有界集完全有界)** 它在 $\mathbb{R}^{N+1}$ (按最大坐标范数) 中完全有界, 故存在有限集 $\{f_1,\dots,f_K\}\subset A$ 使: 对每个 $f\in A$, 存在 $i$ 满足

$$
\max_{0\le j\le N}|f(t_j)-f_i(t_j)|<\frac{\epsilon\delta^{\alpha}}{8}. \tag{3}
$$

下证 $\{f_1,\dots,f_K\}$ 是 $A$ 在 $C_\alpha[a,b]$ 中的有限 $\epsilon$-网. 任取 $f\in A$, 取 $i$ 使 (3) 成立, 对任意 $x\neq x'\in[a,b]$ 估计 $\frac{|(f-f_i)(x)-(f-f_i)(x')|}{|x-x'|^{\alpha}}$.

若 $|x-x'|<\delta$, 则由 (1) 分别用于 $f$ 与 $f_i$ (均属于 $A$):

$$
|(f-f_i)(x)-(f-f_i)(x')|\le|f(x)-f(x')|+|f_i(x)-f_i(x')|<\frac{\epsilon}{4}|x-x'|^{\alpha}+\frac{\epsilon}{4}|x-x'|^{\alpha}=\frac{\epsilon}{2}|x-x'|^{\alpha}.
$$

若 $|x-x'|\ge\delta$, 先估计 $|(f-f_i)(z)|$ ($z\in[a,b]$). 设 $z\in[t_j,t_{j+1}]$, 则 $|z-t_j|\le h<\delta$, 由 (1) 得 $|f(z)-f(t_j)|<\frac{\epsilon}{4}|z-t_j|^{\alpha}\le\frac{\epsilon}{4}h^{\alpha}$, 同理 $|f_i(z)-f_i(t_j)|<\frac{\epsilon}{4}h^{\alpha}$; 再由 (3) 得 $|f(t_j)-f_i(t_j)|<\frac{\epsilon\delta^{\alpha}}{8}$. 故

$$
|(f-f_i)(z)|\le|f(z)-f(t_j)|+|f(t_j)-f_i(t_j)|+|f_i(t_j)-f_i(z)|<\frac{\epsilon}{2}h^{\alpha}+\frac{\epsilon\delta^{\alpha}}{8}.
$$

于是由 (2),

$$
\frac{|(f-f_i)(x)-(f-f_i)(x')|}{|x-x'|^{\alpha}}\le\frac{|(f-f_i)(x)|+|(f-f_i)(x')|}{\delta^{\alpha}}\le\frac{2\left(\frac{\epsilon}{2}h^{\alpha}+\frac{\epsilon\delta^{\alpha}}{8}\right)}{\delta^{\alpha}}=\frac{\epsilon h^{\alpha}}{\delta^{\alpha}}+\frac{\epsilon}{4}<\frac{\epsilon}{2}.
$$

综合两情形, $\|f-f_i\|_{C_\alpha[a,b]}<\epsilon$, 故 $\{f_1,\dots,f_K\}$ 是 $A$ 的有限 $\epsilon$-网. 由 $\epsilon$ 的任意性, $A$ 完全有界. 证毕.

---

## 1.6-7

证明**定理 1.6.7 (科尔莫戈罗夫-里斯-弗雷歇定理)** 中的必要性, 即若 $A\subset L^{p}(\mathbb{R})$ ($1\le p<\infty$) 是完全有界集, 则:

(i) $A$ 是有界集;

(ii) 对每个 $\epsilon>0$, 存在 $M>0$, 使得 $\int_{\{|x|>M\}}|f(x)|^{p}\,\mathrm dm<\epsilon^{p}$, $\forall f\in A$;

(iii) 对每个 $\epsilon>0$, 存在 $\delta>0$, 使得 $\|f(x+h)-f(x)\|_{p}\le\epsilon$, $\forall f\in A$, $\forall |h|<\delta$.

### 解答 1.6-7

先证 (i). 由**定理 1.6.3 (豪斯多夫定理)**, $L^{p}(\mathbb{R})$ 完备且 $A$ 完全有界, 故 $A$ 相对列紧; 由**推论 1.6.1 (相对列紧集可分且有界)**, 相对列紧集是有界的, 故 $A$ 有界.

再证 (ii). 由**定义 1.6.3 ($\epsilon$-网与完全有界集)**, $A$ 完全有界, 故对给定的 $\epsilon>0$, $A$ 有有限的 $\frac{\epsilon}{2}$-网 $\{f_1,\dots,f_N\}\subset A$. 因为每个 $f_i\in L^{p}(\mathbb{R})$ 满足 $\int_{\{|x|>M\}}|f_i(x)|^{p}\,\mathrm dm\to0$ ($M\to\infty$), 故存在 $M>0$ 使对一切 $i$ 有

$$
\left(\int_{\{|x|>M\}}|f_i(x)|^{p}\,\mathrm dm\right)^{1/p}<\frac{\epsilon}{2}.
$$

对任意 $f\in A$, 存在 $i$ 使 $\|f-f_i\|_{p}<\frac{\epsilon}{2}$. 由**闵可夫斯基不等式**,

$$
\left(\int_{\{|x|>M\}}|f(x)|^{p}\,\mathrm dm\right)^{1/p}\le\left(\int_{\{|x|>M\}}|f(x)-f_i(x)|^{p}\,\mathrm dm\right)^{1/p}+\left(\int_{\{|x|>M\}}|f_i(x)|^{p}\,\mathrm dm\right)^{1/p}\le\|f-f_i\|_{p}+\frac{\epsilon}{2}<\epsilon.
$$

于是 $\int_{\{|x|>M\}}|f(x)|^{p}\,\mathrm dm<\epsilon^{p}$ ($\forall f\in A$), (ii) 得证.

最后证 (iii). 对给定的 $\epsilon>0$, 由**定义 1.6.3 ($\epsilon$-网与完全有界集)**, $A$ 有有限的 $\frac{\epsilon}{3}$-网 $\{f_1,\dots,f_N\}\subset A$. 由**习题 1.4-15 (平均连续性)**, 每个 $f_i$ 满足 $\|f_i(x+h)-f_i(x)\|_{p}\to0$ ($h\to0$), 故存在 $\delta>0$ 使 $|h|<\delta$ 时对一切 $i$ 有 $\|f_i(x+h)-f_i(x)\|_{p}<\frac{\epsilon}{3}$. 对任意 $f\in A$, 存在 $i$ 使 $\|f-f_i\|_{p}<\frac{\epsilon}{3}$; 由 $L^{p}$ 范数的平移不变性和**闵可夫斯基不等式**,

$$
\|f(x+h)-f(x)\|_{p}\le\|f(x+h)-f_i(x+h)\|_{p}+\|f_i(x+h)-f_i(x)\|_{p}+\|f_i(x)-f(x)\|_{p}<\frac{\epsilon}{3}+\frac{\epsilon}{3}+\frac{\epsilon}{3}=\epsilon
$$

对一切 $|h|<\delta$ 成立. 故 (iii) 得证. 综上, 必要性成立. 证毕.

---

## 1.6-8

设

$$
C_0(\mathbb{R})=\left\{f:\ f\ \text{在}\ \mathbb{R}\ \text{上连续且}\ \lim_{|x|\to\infty}f(x)=0\right\}
$$

按范数 $\|f\|=\sup_{x\in\mathbb{R}}|f(x)|$ 构成巴拿赫空间. 证明 $A\subset C_0(\mathbb{R})$ 是相对列紧集的充要条件是 $A$ 有界、等度连续, 且对任意 $\epsilon>0$ 存在 $N>0$, 使得 $|f(x)|\le\epsilon$ ($\forall |x|>N$, $f\in A$).

### 解答 1.6-8

先证必要性. 设 $A\subset C_0(\mathbb{R})$ 相对列紧. 由**定理 1.6.3 (豪斯多夫定理)** ($C_0(\mathbb{R})$ 完备), $A$ 完全有界, 故由**推论 1.6.1 (相对列紧集可分且有界)**, $A$ 有界.

由**定义 1.6.3 ($\epsilon$-网与完全有界集)**, 对 $\epsilon>0$, $A$ 有有限的 $\frac{\epsilon}{3}$-网 $\{f_1,\dots,f_N\}\subset A$. 每个 $f_i\in C_0(\mathbb{R})$ 连续且 $\lim_{|x|\to\infty}f_i(x)=0$, 故存在 $M_i>0$ 使 $|f_i(x)|<\frac{\epsilon}{3}$ 当 $|x|>M_i$. 令 $M=\max_iM_i$, 则 $|f_i(x)|<\frac{\epsilon}{3}$ 对 $|x|>M$ 及一切 $i$ 成立. 对任意 $f\in A$, 存在 $i$ 使 $\|f-f_i\|<\frac{\epsilon}{3}$, 于是当 $|x|>M$ 时

$$
|f(x)|\le|f(x)-f_i(x)|+|f_i(x)|<\frac{\epsilon}{3}+\frac{\epsilon}{3}=\frac{2\epsilon}{3}\le\epsilon.
$$

(此处可将 $\epsilon$ 换成 $\frac{3\epsilon}{2}$ 使右端恰为 $\epsilon$. ) 故对任意 $\epsilon>0$ 存在 $N=M$ 使 $|f(x)|\le\epsilon$ ($\forall|x|>N$, $f\in A$).

再证 $A$ 等度连续. 每个 $f_i\in C_0(\mathbb{R})$ 在 $\mathbb{R}$ 上一致连续 (见**习题 1.6-16**: 紧区间外函数趋于 $0$, 紧区间上连续则一致连续), 故存在 $\delta>0$ 使 $|x-x'|<\delta$ 时 $|f_i(x)-f_i(x')|<\frac{\epsilon}{3}$ 对一切 $i$ 成立. 对任意 $f\in A$, 存在 $i$ 使 $\|f-f_i\|<\frac{\epsilon}{3}$, 故 $|x-x'|<\delta$ 时

$$
|f(x)-f(x')|\le|f(x)-f_i(x)|+|f_i(x)-f_i(x')|+|f_i(x')-f(x')|<\frac{\epsilon}{3}+\frac{\epsilon}{3}+\frac{\epsilon}{3}=\epsilon.
$$

故 $A$ 等度连续. 必要性得证.

再证充分性. 设 $A$ 有界、等度连续, 且对任意 $\epsilon>0$ 存在 $N$ 使 $|f(x)|\le\epsilon$ 对 $|x|>N$、$f\in A$. 证明 $A$ 完全有界, 再由**定理 1.6.3 (豪斯多夫定理)** ($C_0(\mathbb{R})$ 完备) 得 $A$ 相对列紧.

给定 $\epsilon>0$, 由假设取 $N>0$ 使 $|f(x)|\le\frac{\epsilon}{3}$ 对 $|x|>N$、$f\in A$. 在紧区间 $[-N,N]$ 上, $A$ 作为 $C[-N,N]$ 的子集有界且等度连续, 由**定理 1.6.5 (阿泽拉-阿斯卡里定理)**, $A|_{[-N,N]}$ 在 $C[-N,N]$ 中相对列紧, 从而是完全有界的, 故存在有限个函数 $g_1,\dots,g_K$ 使: 对每个 $f\in A$, 存在 $k$ 满足

$$
\max_{|x|\le N}|f(x)-g_k(x)|<\frac{\epsilon}{3}.
$$

把每个 $g_k$ 线性延拓为 $\widetilde g_k\in C_0(\mathbb{R})$: $\widetilde g_k=g_k$ 于 $[-N,N]$, 在 $[N,N+1]$ 与 $[-N-1,-N]$ 上从 $g_k(\pm N)$ 线性过渡到 $0$, 在 $|x|\ge N+1$ 上取 $0$. 则 $\{\widetilde g_1,\dots,\widetilde g_K\}\subset C_0(\mathbb{R})$. 对任意 $f\in A$, 存在 $k$ 使 $\max_{|x|\le N}|f-g_k|<\frac{\epsilon}{3}$. 当 $|x|\le N$ 时 $|f(x)-\widetilde g_k(x)|=|f(x)-g_k(x)|<\frac{\epsilon}{3}$; 当 $|x|>N$ 时 $|f(x)|\le\frac{\epsilon}{3}$, 且 $|\widetilde g_k(x)|\le\max\{|g_k(N)|,|g_k(-N)|\}$, 而 $|g_k(\pm N)|\le|f(\pm N)-g_k(\pm N)|+|f(\pm N)|<\frac{\epsilon}{3}+\frac{\epsilon}{3}=\frac{2\epsilon}{3}$, 故 $|f(x)-\widetilde g_k(x)|\le|f(x)|+|\widetilde g_k(x)|<\frac{\epsilon}{3}+\frac{2\epsilon}{3}=\epsilon$. 于是 $\|f-\widetilde g_k\|<\epsilon$, 故 $\{\widetilde g_1,\dots,\widetilde g_K\}$ 是 $A$ 的有限 $\epsilon$-网. 由 $\epsilon$ 的任意性, $A$ 完全有界, 从而相对列紧. 证毕.

---

## 1.6-9

设 $X$ 是巴拿赫空间, $A$ 是 $X$ 中的相对列紧集, 证明它的凸包 $\operatorname{co}(A)$ 也是相对列紧集.

### 解答 1.6-9

因 $X$ 完备且 $A$ 相对列紧, 由**定理 1.6.3 (豪斯多夫定理)**, $A$ 完全有界. 故对 $\epsilon>0$, $A$ 有有限的 $\epsilon$-网 $\{a_1,\dots,a_N\}\subset A$.

下证 $\operatorname{co}(A)\subset\operatorname{co}\{a_1,\dots,a_N\}+B(0,\epsilon)$. 任取 $z\in\operatorname{co}(A)$, 则存在 $x_1,\dots,x_m\in A$ 与非负实数 $\lambda_1,\dots,\lambda_m$ ($\sum_{j=1}^{m}\lambda_j=1$) 使 $z=\sum_{j=1}^{m}\lambda_jx_j$. 对每个 $j$, 由 $\{a_1,\dots,a_N\}$ 是 $A$ 的 $\epsilon$-网, 存在 $i_j\in\{1,\dots,N\}$ 使 $\|x_j-a_{i_j}\|<\epsilon$. 于是

$$
z=\sum_{j=1}^{m}\lambda_ja_{i_j}+\sum_{j=1}^{m}\lambda_j(x_j-a_{i_j}),
$$

其中 $\sum_{j=1}^{m}\lambda_ja_{i_j}\in\operatorname{co}\{a_1,\dots,a_N\}$, 且

$$
\left\|\sum_{j=1}^{m}\lambda_j(x_j-a_{i_j})\right\|\le\sum_{j=1}^{m}\lambda_j\|x_j-a_{i_j}\|<\sum_{j=1}^{m}\lambda_j\epsilon=\epsilon.
$$

故 $z\in\operatorname{co}\{a_1,\dots,a_N\}+B(0,\epsilon)$.

记 $K=\operatorname{co}\{a_1,\dots,a_N\}=\left\{\sum_{i=1}^{N}\lambda_ia_i:\lambda_i\ge0,\ \sum_{i=1}^{N}\lambda_i=1\right\}$. 它是 $\mathbb{R}^{N}$ 中的单形 $\Delta_{N-1}=\{\lambda_i\ge0,\ \sum\lambda_i=1\}$ 在连续映射 $(\lambda_1,\dots,\lambda_N)\mapsto\sum\lambda_ia_i$ 下的像, 故 $K$ 是紧集, 由**例 1.6.3 ($\mathbb{R}^n$ 中有界集完全有界)** 知 $K$ 完全有界, 故对 $\epsilon>0$, $K$ 有有限的 $\epsilon$-网 $\{y_1,\dots,y_M\}\subset K$. 于是对任意 $z\in\operatorname{co}(A)$, 存在 $u\in K$ 使 $\|z-u\|<\epsilon$, 且存在 $l$ 使 $\|u-y_l\|<\epsilon$, 故 $\|z-y_l\|<2\epsilon$. 所以 $\{y_1,\dots,y_M\}$ 是 $\operatorname{co}(A)$ 的有限 $2\epsilon$-网. 由 $\epsilon$ 的任意性, $\operatorname{co}(A)$ 完全有界, 再由**定理 1.6.3 (豪斯多夫定理)** ($X$ 完备) 得 $\operatorname{co}(A)$ 相对列紧. 证毕.

---

## 1.6-10 (格罗滕迪克定理)

设 $X$ 是巴拿赫空间, $K$ 是 $X$ 中的相对列紧集. 证明存在 $X$ 中的点列 $\{x_n\}$, 使得 $\lim_{n\to\infty}x_n=0$, 且

$$
K\subset\left\{\sum_{n=1}^{\infty}a_nx_n:\ \sum_{n=1}^{\infty}|a_n|\le1\right\}.
$$

### 解答 1.6-10

本解的构造严格按书末提示"在**推论 1.6.1 (相对列紧集可分且有界)** 稠密子集 $B$ 给出的点列中, 点之间的距离是越来越小的", 所得系数的精确条件为 $|a_n|\le1$ (即 $K\subset\overline{\operatorname{co}}\{\pm x_n\}$) ; 见解答末尾的说明.

因 $K$ 相对列紧, 由**定理 1.6.3 (豪斯多夫定理)** ($X$ 完备) $K$ 完全有界, 故由**定义 1.6.3 ($\epsilon$-网与完全有界集)**, 对每个 $n$, $K$ 有有限的 $\frac{1}{n}$-网, 记作 $\{y_{n,1},\dots,y_{n,m_n}\}\subset K$. 令

$$
B=\bigcup_{n=1}^{\infty}\{y_{n,1},\dots,y_{n,m_n}\},
$$

则 $B$ 是可数集, 且 $B$ 在 $K$ 中稠密 (因 $B$ 以任意精度逼近 $K$ 中每点). 把 $B$ 依序排列成点列 $\{z_1,z_2,\dots\}$, 使先排 $\frac{1}{n}$-网、再排 $\frac{1}{n+1}$-网……由于后加入的点属于更细的网, 与已有点的距离至多约 $\frac{1}{n}+\frac{1}{n-1}$, 故可排得相邻点距离递减且满足

$$
\|z_k-z_{k-1}\|\to0,\quad \sum_{k=2}^{\infty}\|z_k-z_{k-1}\|<\infty. \tag{1}
$$

(若有必要, 在每层网间插入更细的有限点使 (1) 成立, 这不改变 $B$ 的稠密性. ) 因 $B$ 在 $K$ 中稠密, 故 $B$ 在 $\overline{K}$ 中稠密, 于是

$$
\overline{K}\subset\overline{B}\subset\overline{\operatorname{co}}(B)=\overline{\operatorname{co}}\{z_k\}. \tag{2}
$$

定义点列 $\{x_n\}$:

$$
x_1=z_1,\quad x_n=z_n-z_{n-1}\ \ (n\ge2).
$$

由 (1), $\|x_n\|=\|z_n-z_{n-1}\|\to0$, 故 $\lim_{n\to\infty}x_n=0$; 且 $\sum_{n=1}^{\infty}\|x_n\|\le\|z_1\|+\sum_{n=2}^{\infty}\|z_n-z_{n-1}\|<\infty$, 即 $\{x_n\}$ 绝对可和.

下面证明 $K\subset\overline{\operatorname{co}}\{\pm x_n\}$. 任取 $w\in\overline{K}$, 由 (2), 存在 $w^{(m)}\in\operatorname{co}\{z_k\}$ 使 $w^{(m)}\to w$. 每个 $w^{(m)}$ 形如有限凸组合 $w^{(m)}=\sum_{k=1}^{p_m}\lambda_k^{(m)}z_k$, 其中 $\lambda_k^{(m)}\ge0$、$\sum_k\lambda_k^{(m)}=1$. 由于 $z_k=\sum_{i=1}^{k}x_i$ (望远镜求和), 故

$$
w^{(m)}=\sum_{k=1}^{p_m}\lambda_k^{(m)}\sum_{i=1}^{k}x_i=\sum_{i=1}^{p_m}\left(\sum_{k=i}^{p_m}\lambda_k^{(m)}\right)x_i.
$$

记 $c_i^{(m)}=\sum_{k=i}^{p_m}\lambda_k^{(m)}$, 则 $0\le c_i^{(m)}\le\sum_k\lambda_k^{(m)}=1$, 故 $c_i^{(m)}\in[0,1]$. 于是每个 $w^{(m)}$ 是 $\{\pm x_i\}$ 的有限凸组合 (系数在 $[-1,1]$ 内), 即

$$
w^{(m)}\in\operatorname{co}\{\pm x_1,\dots,\pm x_{p_m}\}\subset\overline{\operatorname{co}}\{\pm x_n\}.
$$

因 $w^{(m)}\to w$ 且 $\overline{\operatorname{co}}\{\pm x_n\}$ 是闭集, 故 $w\in\overline{\operatorname{co}}\{\pm x_n\}$. 所以 $\overline{K}\subset\overline{\operatorname{co}}\{\pm x_n\}$, 特别地 $K\subset\overline{\operatorname{co}}\{\pm x_n\}$.

最后说明 $\overline{\operatorname{co}}\{\pm x_n\}=\left\{\sum_{n=1}^{\infty}a_nx_n:\ |a_n|\le1\right\}$. 一方面, $\{\pm x_n\}$ 的每个有限凸组合 $\sum\epsilon_i\lambda_ix_i$ ($\lambda_i\ge0,\sum\lambda_i=1,\epsilon_i\in\{\pm1\}$) 满足 $|\epsilon_i\lambda_i|\le1$, 且由于 $\sum\|x_n\|<\infty$ 级数绝对收敛, 故 $\overline{\operatorname{co}}\{\pm x_n\}\subset\left\{\sum a_nx_n:|a_n|\le1\right\}$. 另一方面, $\left\{\sum a_nx_n:|a_n|\le1\right\}$ 是闭集 (若 $u^{(m)}=\sum a_n^{(m)}x_n\to u$, $|a_n^{(m)}|\le1$, 则由对角线抽取与控制收敛可得子列 $a_n^{(m_k)}\to a_n$ (逐 $n$) 且 $u=\sum a_nx_n$, $|a_n|\le1$), 且含 $\{\pm x_n\}$ 的凸包, 故 $\overline{\operatorname{co}}\{\pm x_n\}\supset\left\{\sum a_nx_n:|a_n|\le1\right\}$. 两方向合起来得等号. 于是

$$
K\subset\overline{\operatorname{co}}\{\pm x_n\}=\left\{\sum_{n=1}^{\infty}a_nx_n:\ |a_n|\le1,\ n=1,2,\dots\right\},\quad \lim_{n\to\infty}x_n=0.
$$

**说明 (关于系数条件)** 由上述望远镜构造, 所得系数的精确条件为逐项 $|a_n|\le1$ (即 $K\subset\overline{\operatorname{co}}\{\pm x_n\}$). 教材习题中写为 $\sum_{n=1}^{\infty}|a_n|\le1$ 处, 按本构造应理解为逐项 $|a_n|\le1$; 这也正与书末提示"在推论 1.6.1 稠密点列 $B$ 中相邻点距离越来越小"的望远镜求和构造一致. 证毕.

---

## 1.6-11

设 $B_1=\left\{f\in L^{1}[a,b]:\ \|f\|_1\le1\right\}$ 是实 $L^{1}[a,b]$ 的闭单位球, $g\in L^{\infty}[a,b]$ 是实值函数. 对 $f\in B_1$, 定义 $F_g(f)=\int_a^{b}fg\,\mathrm dm$. 证明 $F_g$ 在 $B_1$ 上是连续的, 并且

$$
\sup_{f\in B_1}F_g(f)=\|g\|_{\infty};
$$

又说明当 $g(x)=x-a$ 时, $\sup$ 不能达到.

### 解答 1.6-11

先证 $F_g$ 连续. 对 $f,h\in B_1$, 由 $L^{1}$-范数定义与 $|g|\le\|g\|_{\infty}$ (a.e.),

$$
|F_g(f)-F_g(h)|=\left|\int_a^{b}(f-h)g\,\mathrm dm\right|\le\int_a^{b}|f-h||g|\,\mathrm dm\le\|g\|_{\infty}\int_a^{b}|f-h|\,\mathrm dm=\|g\|_{\infty}\|f-h\|_1.
$$

故 $F_g$ 是 $B_1$ 上的 Lipschitz 映射, 从而是连续的.

再证 $\sup_{f\in B_1}F_g(f)=\|g\|_{\infty}$. 先看上界: 对任意 $f\in B_1$, 同样有

$$
F_g(f)=\int_a^{b}fg\,\mathrm dm\le\int_a^{b}|f||g|\,\mathrm dm\le\|g\|_{\infty}\|f\|_1\le\|g\|_{\infty},
$$

故 $\sup_{f\in B_1}F_g(f)\le\|g\|_{\infty}$.

再看下界. 对 $\epsilon>0$, 因 $\|g\|_{\infty}$ 是 $g$ 的本质上确界, 集合 $E_\epsilon=\left\{x\in[a,b]:\ |g(x)|>\|g\|_{\infty}-\epsilon\right\}$ 具有正测度 $m(E_\epsilon)>0$. 取

$$
f_\epsilon(x)=\frac{\operatorname{sign}(g(x))}{m(E_\epsilon)}\chi_{E_\epsilon}(x),
$$

其中 $\operatorname{sign}(g)$ 是 $g$ 的符号函数 (可测). 则 $\|f_\epsilon\|_1=\int_{E_\epsilon}\frac{|\operatorname{sign}(g)|}{m(E_\epsilon)}\,\mathrm dm=\frac{m(E_\epsilon)}{m(E_\epsilon)}=1$, 故 $f_\epsilon\in B_1$. 于是

$$
F_g(f_\epsilon)=\int_{E_\epsilon}\frac{g(x)\operatorname{sign}(g(x))}{m(E_\epsilon)}\,\mathrm dm=\frac{1}{m(E_\epsilon)}\int_{E_\epsilon}|g(x)|\,\mathrm dm\ge\frac{(\|g\|_{\infty}-\epsilon)\,m(E_\epsilon)}{m(E_\epsilon)}=\|g\|_{\infty}-\epsilon.
$$

故对任意 $\epsilon>0$ 有 $\sup_{f\in B_1}F_g(f)\ge\|g\|_{\infty}-\epsilon$, 令 $\epsilon\to0$ 得 $\sup_{f\in B_1}F_g(f)\ge\|g\|_{\infty}$. 综合上下界, $\sup_{f\in B_1}F_g(f)=\|g\|_{\infty}$.

最后说明 $g(x)=x-a$ 时 $\sup$ 不能达到. 此时 $\|g\|_{\infty}=b-a$. 若存在 $f\in B_1$ 使 $F_g(f)=\|g\|_{\infty}=b-a$, 则由 $x-a\le b-a$ 对一切 $x\in[a,b]$ 成立,

$$
b-a=F_g(f)=\int_a^{b}(x-a)f\,\mathrm dm\le\int_a^{b}(b-a)|f|\,\mathrm dm=(b-a)\|f\|_1\le b-a.
$$

上式必须处处取等号, 特别地 $\|f\|_1=1$ 且 $\int_a^{b}(x-a)f\,\mathrm dm=\int_a^{b}(b-a)|f|\,\mathrm dm$. 由 $x-a<b-a$ 在除点 $b$ 外的一切点成立, 最后这个等式迫使 $f$ 几乎处处为零 ($f\neq0$ 的点只能落在单点集 $\{b\}$ 上, 其测度为 $0$), 这与 $\|f\|_1=1$ 矛盾. 故不存在 $f\in B_1$ 使 $F_g(f)=\|g\|_{\infty}$, 即 $\sup$ 不能达到. 证毕.

---

## 1.6-12 (定理 1.6.9 的证明)

证明**定理 1.6.9 (紧度量空间上的性质)**. 即设 $X$ 是紧的度量空间, 证明:

(i) $X$ 上的连续函数是一致连续的;

(ii) $C(X)$ 按范数 $\|f\|=\max_{x\in X}|f(x)|$ 构成巴拿赫空间;

(iii) $A\subset C(X)$ 是相对列紧集当且仅当 $A$ 是有界的且等度连续的.

### 解答 1.6-12

先证 (i). 设 $f\in C(X)$, $\epsilon>0$. 由 $f$ 的连续性, 对每个 $x\in X$ 存在 $\delta_x>0$, 使得 $d(x,x')<\delta_x$ 蕴含 $|f(x)-f(x')|<\frac{\epsilon}{2}$. 开球族 $\left\{U\left(x,\frac{\delta_x}{2}\right):x\in X\right\}$ 覆盖紧空间 $X$, 由**定理 1.6.2 (列紧 $\Leftrightarrow$ 覆盖紧)** 它有有限子覆盖 $\left\{U\left(x_i,\frac{\delta_{x_i}}{2}\right)\right\}_{i=1}^{m}$. 令 $\delta=\min_i\frac{\delta_{x_i}}{2}>0$. 若 $d(x,x')<\delta$, 取 $i$ 使 $x\in U\left(x_i,\frac{\delta_{x_i}}{2}\right)$, 则 $d(x,x_i)<\frac{\delta_{x_i}}{2}<\delta_{x_i}$, 故 $|f(x)-f(x_i)|<\frac{\epsilon}{2}$; 且 $d(x',x_i)\le d(x',x)+d(x,x_i)<\delta+\frac{\delta_{x_i}}{2}\le\frac{\delta_{x_i}}{2}+\frac{\delta_{x_i}}{2}=\delta_{x_i}$, 故 $|f(x')-f(x_i)|<\frac{\epsilon}{2}$. 于是 $|f(x)-f(x')|<\epsilon$. 所以 $f$ 一致连续, (i) 得证.

再证 (ii). 由**推论 1.6.3 (连续函数达到上下确界)**, 连续函数在紧空间上达到上确界, 故 $\|f\|=\max_{x\in X}|f(x)|$ 良定义, 且它满足范数公理 (非负性、齐次性、三角不等式), 故 $C(X)$ 是赋范线性空间. 证其完备: 设 $\{f_n\}\subset C(X)$ 是 Cauchy 列, 则对每个 $x\in X$, $|f_n(x)-f_m(x)|\le\|f_n-f_m\|\to0$, 故 $\{f_n(x)\}$ 是 $\mathbb{R}$ 中的 Cauchy 列, 因 $\mathbb{R}$ 完备而收敛, 记 $f(x)=\lim_nf_n(x)$. 对 $\epsilon>0$, 取 $N$ 使 $\|f_n-f_m\|<\epsilon$ ($n,m\ge N$), 则对一切 $x$ 与 $m\ge N$, $|f_n(x)-f_m(x)|<\epsilon$, 令 $m\to\infty$ 得 $|f_n(x)-f(x)|\le\epsilon$ ($\forall x$), 故 $\|f_n-f\|\le\epsilon$, 即 $f_n\to f$ 于 $C(X)$ 范数. 又因一致极限保持连续性: 对 $\epsilon>0$ 取 $n$ 使 $\|f_n-f\|<\frac{\epsilon}{3}$, 由 $f_n$ 连续取 $\delta$ 使 $d(x,y)<\delta$ 蕴含 $|f_n(x)-f_n(y)|<\frac{\epsilon}{3}$, 则 $|f(x)-f(y)|\le|f(x)-f_n(x)|+|f_n(x)-f_n(y)|+|f_n(y)-f(y)|<\epsilon$, 故 $f$ 连续, $f\in C(X)$. 于是 Cauchy 列收敛, $C(X)$ 完备, 是巴拿赫空间, (ii) 得证.

最后证 (iii). 先证充分性: 设 $A$ 有界且等度连续, 证明 $A$ 相对列紧. 因 $X$ 紧, 由**基础知识: 紧度量空间的性质**, $X$ 完备且完全有界; 由 (ii), $C(X)$ 完备. 故由**定理 1.6.3 (豪斯多夫定理)**, 只须证 $A$ 完全有界. 给定 $\epsilon>0$, 由 $A$ 等度连续, 存在 $\delta>0$ 使 $d(x,y)<\delta$ 蕴含 $|f(x)-f(y)|<\frac{\epsilon}{3}$ ($\forall f\in A$). 因 $X$ 完全有界, $X$ 有有限的 $\delta$-网 $\{x_1,\dots,x_N\}\subset X$. 考虑求值映射 $\Phi:A\to\mathbb{R}^{N}$, $\Phi(f)=(f(x_1),\dots,f(x_N))$. 因 $A$ 有界, $\Phi(A)$ 在 $\mathbb{R}^{N}$ 中有界, 由**例 1.6.3 ($\mathbb{R}^n$ 中有界集完全有界)** 它完全有界, 故有有限的 $\frac{\epsilon}{3}$-网, 即存在有限个 $f_1,\dots,f_K\in A$ 使: 对每个 $f\in A$ 存在 $i$ 满足 $\max_j|f(x_j)-f_i(x_j)|<\frac{\epsilon}{3}$. 对任意 $x\in X$, $x$ 落在某个 $x_j$ 的 $\delta$-邻域内, 故 $d(x,x_j)<\delta$, 由等度连续性 $|f(x)-f(x_j)|<\frac{\epsilon}{3}$、$|f_i(x)-f_i(x_j)|<\frac{\epsilon}{3}$, 于是

$$
|f(x)-f_i(x)|\le|f(x)-f(x_j)|+|f(x_j)-f_i(x_j)|+|f_i(x_j)-f_i(x)|<\epsilon.
$$

对 $x$ 取上确界得 $\|f-f_i\|<\epsilon$, 故 $\{f_1,\dots,f_K\}$ 是 $A$ 的有限 $\epsilon$-网. 故 $A$ 完全有界, 由**定理 1.6.3 (豪斯多夫定理)** 得 $A$ 相对列紧.

再证必要性: 设 $A$ 相对列紧. 由**定理 1.6.3 (豪斯多夫定理)** ($C(X)$ 完备), $A$ 完全有界, 由**推论 1.6.1 (相对列紧集可分且有界)** 得 $A$ 有界. 证等度连续: 对 $\epsilon>0$, 由 $A$ 完全有界, $A$ 有有限的 $\frac{\epsilon}{3}$-网 $\{f_1,\dots,f_N\}$. 由 (i), 每个 $f_i$ 一致连续, 故存在 $\delta>0$ 使 $d(x,y)<\delta$ 蕴含 $|f_i(x)-f_i(y)|<\frac{\epsilon}{3}$ ($\forall i$). 对任意 $f\in A$, 存在 $i$ 使 $\|f-f_i\|<\frac{\epsilon}{3}$, 故 $d(x,y)<\delta$ 时

$$
|f(x)-f(y)|\le|f(x)-f_i(x)|+|f_i(x)-f_i(y)|+|f_i(y)-f(y)|<\epsilon.
$$

故 $A$ 等度连续. 必要性得证. 综上, (iii) 成立. 证毕.

---

## 1.6-16

设 $X$ 是紧的度量空间, $f:X\to Y$ 是度量空间之间的连续映射. 证明 $f$ 是一致连续的.

### 解答 1.6-16

设 $\epsilon>0$. 由 $f$ 的连续性, 对每个 $x\in X$ 存在 $\delta_x>0$, 使得 $d_X(x,x')<\delta_x$ 蕴含 $d_Y(f(x),f(x'))<\frac{\epsilon}{2}$. 开球族 $\left\{U\left(x,\frac{\delta_x}{2}\right):x\in X\right\}$ 覆盖紧空间 $X$, 由**定理 1.6.2 (列紧 $\Leftrightarrow$ 覆盖紧)** 它有有限子覆盖 $\left\{U\left(x_i,\frac{\delta_{x_i}}{2}\right)\right\}_{i=1}^{m}$. 令 $\delta=\min_i\frac{\delta_{x_i}}{2}>0$. 若 $d_X(x,x')<\delta$, 取 $i$ 使 $x\in U\left(x_i,\frac{\delta_{x_i}}{2}\right)$, 则 $d_X(x,x_i)<\frac{\delta_{x_i}}{2}<\delta_{x_i}$, 故 $d_Y(f(x),f(x_i))<\frac{\epsilon}{2}$; 且 $d_X(x',x_i)\le d_X(x',x)+d_X(x,x_i)<\delta+\frac{\delta_{x_i}}{2}\le\delta_{x_i}$, 故 $d_Y(f(x'),f(x_i))<\frac{\epsilon}{2}$. 于是 $d_Y(f(x),f(x'))\le d_Y(f(x),f(x_i))+d_Y(f(x_i),f(x'))<\epsilon$. 所以 $f$ 一致连续. 证毕.

---

## 1.6-17 (迪尼定理)

设 $X$ 是紧的度量空间, $\{f_k\}$ 是 $X$ 上递增的实值连续函数列, 即 $f_k(x)\le f_{k+1}(x)$ ($\forall x\in X$, $k=1,2,\dots$). 若 $\{f_k\}$ 逐点收敛于连续函数 $f$, 则 $f_k\rightrightarrows f$ (即一致收敛于 $f$).

### 解答 1.6-17

记 $g_k=f-f_k$. 因 $f$、$f_k$ 连续且 $f_k\le f_{k+1}\le f$, 故每个 $g_k\in C(X)$、$g_k\ge0$, 且对每个 $x$, $\{g_k(x)\}$ 单调递减趋于 $0$ (因 $f_k(x)\uparrow f(x)$).

给定 $\epsilon>0$. 由 $g_k(x)\to0$, 对每个 $x\in X$ 存在 $k_x$ 使 $g_{k_x}(x)<\frac{\epsilon}{2}$. 由 $g_{k_x}$ 的连续性, 存在 $x$ 的开邻域 $O_x$, 使 $y\in O_x$ 时 $g_{k_x}(y)<\epsilon$. 开集族 $\{O_x:x\in X\}$ 覆盖紧空间 $X$, 由**定理 1.6.2 (列紧 $\Leftrightarrow$ 覆盖紧)** 它有有限子覆盖 $\{O_{x_1},\dots,O_{x_m}\}$. 令 $N=\max\{k_{x_1},\dots,k_{x_m}\}$. 对任意 $k\ge N$ 与 $y\in X$, $y$ 属于某个 $O_{x_j}$, 且 $k\ge k_{x_j}$, 由 $\{g_k(y)\}$ 关于 $k$ 单调递减得

$$
g_k(y)\le g_{k_{x_j}}(y)<\epsilon.
$$

于是 $\|g_k\|=\max_{y\in X}g_k(y)<\epsilon$ 对一切 $k\ge N$ 成立, 故 $\|f_k-f\|=\|g_k\|\to0$, 即 $f_k\rightrightarrows f$. 证毕.
