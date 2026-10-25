# week5

> **基础知识: 紧度量空间的性质**<br>紧的度量空间是完备的且完全有界的.

> **基础知识: 闵可夫斯基不等式**<br>设 $1\le p< \infty$, $f,g\in L^{p}$, 则 $\left\|f+g\right\|_{p}\le\left\|f\right\|_{p}+\left\|g\right\|_{p}$.

> **基础知识: 凸包**<br>对于线性空间 $X$, 存在一个 $A\subset X$, 则 $A$ 的凸包 $\mathrm{co}\left(A\right)$ 是包含 $A$ 的最小凸集.

> **基础知识: 单 (纯) 形**<br>欧氏空间里, 由 $m+1$ 个 "不在同一个 $m-1$ 维超平面上" 的点（仿射无关点）张出来的凸集, 是三角形, 四面体的高维推广.

> **例 1.2.8 ($L^{p}$ 是巴拿赫空间)**<br>设 $1\le p< \infty$, 则 $L^{p}\left(\mathbb{R}\right)$ 按范数 $\left\|f\right\|_{p}=\left(\int_{\mathbb{R}}\left|f\right|^{p}\,\mathrm dm\right)^{1/p}$ 是巴拿赫空间.

> **例 1.2.12 ($C\left[a,b\right]$ 是巴拿赫空间)**<br>设 $\left[a,b\right]$ 是有限闭区间, 则 $C\left[a,b\right]$ 按范数 $\left\|f\right\|=\max_{x\in\left[a,b\right]}\left|f\left(x\right)\right|$ 是巴拿赫空间.

> **引理 1.4.1 (基本点列与完备性)**<br>设 $X$ 是度量空间, 则:<br>(i) 基本点列是有界的;<br>(ii) 若 $X$ 完备, 则点列收敛当且仅当它是基本点列;<br>(iii) 完备度量空间的闭子集是完备的.

> **习题 1.4-15 (平均连续性)**<br>设 $f\in L^{p}\left(\mathbb{R}\right)$, $1\le p< \infty$, 则 $\lim_{h\to0}\left(\int_{\mathbb{R}}\left|f\left(x+h\right)-f\left(x\right)\right|^{p}\,\mathrm dm\right)^{1/p}=0$.

> **定义 1.5.1 (不动点)**<br>设 $T$ 是集合 $X$ 到自身的映射. 若存在 $x\in X$ 使得 $Tx=x$, 则称 $x$ 是 $T$ 的不动点.

> **定理 1.5.1 (巴拿赫不动点定理)**<br>设 $X$ 是完备的度量空间, $T:X\to X$ 是压缩映射, 则 $T$ 在 $X$ 中存在唯一的不动点 $x$; 且对任意的 $x_0\in X$, 迭代序列 $x_n=T^{n}x_0$ 收敛于 $x$, 误差估计 $d\left(x_n,x\right)\le \frac{\theta^{n}}{1-\theta}d\left(x_0,Tx_0\right)$.

> **定义 1.5.2 (压缩映射)**<br>设 $X$ 是度量空间, $T:X\to X$. 若存在 $0< \theta< 1$, 使得 $d\left(Tx,Ty\right)\le \theta d\left(x,y\right)$ ($\forall x,y\in X$), 则称 $T$ 是 $X$ 上的压缩映射, $\theta$ 称为压缩系数.

> **定义 1.6.1 (相对列紧集)**<br>设 $A$ 是度量空间 $X$ 的子集. 若 $A$ 的闭包 $\overline{A}$ 是紧集, 则称 $A$ 是相对列紧集.

> **推论 1.6.1 (相对列紧集可分且有界)**<br>相对列紧集是可分的有界集.

> **例 1.6.1 (有限维空间中相对列紧 $\Leftrightarrow$ 有界)**<br>在有限维赋范线性空间 (特别地 $\mathbb{R}^n$) 中, $A$ 是相对列紧集当且仅当 $A$ 是有界集.

> **注 1.6.1 (网中的点不必属于集合本身)**<br>$\varepsilon$-网中的点可以不必属于 $A$ 本身.

> **定理 1.6.2 (列紧 $\Leftrightarrow$ 覆盖紧)**<br>度量空间 $X$ 是紧集当且仅当它是列紧集 (即 $X$ 中任意点列都有收敛子列).

> **定义 1.6.3 ($\varepsilon$-网与完全有界集)**<br>设 $A$ 是度量空间 $X$ 的子集, $\varepsilon> 0$. 若存在 $X$ 的有限子集 $\left\{x_1,\dots,x_N\right\}$, 使得 $A\subset \bigcup_{i=1}^{N}U\left(x_i,\varepsilon\right)$, 则称 $\left\{x_1,\dots,x_N\right\}$ 是 $A$ 的一个 $\varepsilon$-网. 若对每个 $\varepsilon> 0$, $A$ 都有有限的 $\varepsilon$-网, 则称 $A$ 是完全有界集.

> **定理 1.6.3 (豪斯多夫定理)**<br>设 $X$ 是完备的度量空间, $A\subset X$, 则 $A$ 是相对列紧集当且仅当 $A$ 是完全有界集.

> **推论 1.6.3 (连续函数达到上下确界)**<br>设 $X$ 是紧度量空间, $f\in C\left(X\right)$, 则 $f$ 在 $X$ 上达到上确界与下确界.

> **例 1.6.3 ($\mathbb{R}^n$ 中有界集完全有界)**<br>设 $A$ 是 $\mathbb{R}^n$ 中的有界集, 则 $A$ 是完全有界集.

> **定义 1.6.5 (一致连续与等度连续)**<br>(i) 设 $f:X\to Y$ 是度量空间之间的映射. 若对每个 $\varepsilon> 0$ 存在 $\delta> 0$, 使得 $d_X\left(x_1,x_2\right)< \delta$ 蕴含 $d_Y\left(f\left(x_1\right),f\left(x_2\right)\right)< \varepsilon$, 则称 $f$ 一致连续.<br>(ii) 设 $X$ 是紧度量空间, $\mathscr{F}\subset C\left(X\right)$. 若对每个 $\varepsilon> 0$ 存在 $\delta> 0$, 使得对一切 $f\in\mathscr{F}$ 及 $x_1,x_2\in X$, 由 $d\left(x_1,x_2\right)< \delta$ 可推出 $\left|f\left(x_1\right)-f\left(x_2\right)\right|< \varepsilon$, 则称 $\mathscr{F}$ 是等度连续的.

> **定理 1.6.5 (阿泽拉-阿斯卡里定理)**<br>设 $A\subset C\left[a,b\right]$, 则 $A$ 是相对列紧集当且仅当 $A$ 是有界的且等度连续的.

> **定理 1.6.7 (科尔莫戈罗夫-里斯-弗雷歇定理)**<br>设 $A\subset L^{p}\left(\mathbb{R}\right)$, $1\le p< \infty$. 则 $A$ 是完全有界集当且仅当下列三条件同时成立:<br>(i) $A$ 是有界集;<br>(ii) (等度 $L^{p}$-胎紧) 对每个 $\varepsilon> 0$, 存在 $M> 0$, 使得 $\int_{\left\{\left|x\right|> M\right\}}\left|f\left(x\right)\right|^{p}\,\mathrm dm< \varepsilon^{p}$, $\forall f\in A$;<br>(iii) (等度 $L^{p}$-范数连续) 对每个 $\varepsilon> 0$, 存在 $\delta> 0$, 使得 $\left\|f\left(x+h\right)-f\left(x\right)\right\|_{p}\le\varepsilon$, $\forall f\in A$, $\forall \left|h\right|< \delta$.

> **定理 1.6.9 (紧度量空间上的性质)**<br>设 $X$ 是紧的度量空间, 则:<br>(i) $X$ 上的连续函数是一致连续的;<br>(ii) $C\left(X\right)$ 按范数 $\left\|f\right\|=\max_{x\in X}\left|f\left(x\right)\right|$ 构成巴拿赫空间;<br>(iii) (阿泽拉-阿斯卡里定理) $A\subset C\left(X\right)$ 是相对列紧集当且仅当 $A$ 是有界的且等度连续的.

---

## 1.5-8 (隐函数存在定理)

设函数 $F:U\times V\to\mathbb{R}^{m}$, 其中 $U$ 和 $V$ 分别是 $\mathbb{R}^{n}$ 和 $\mathbb{R}^{m}$ 中的开区域, $\left(x_0,y_0\right)\in U\times V$. 如果 $F$ 在 $U\times V$ 中连续, 并且对于任意的 $x\in U$, $F\left(x,\cdot\right)$ 在 $V$ 中是连续可微的, 同时满足

$$
F\left(x_0,y_0\right)=0,\quad \det\left(\frac{\partial F}{\partial y}\right)\left(x_0,y_0\right)\neq 0,
$$

其中 $\frac{\partial F}{\partial y}$ 是 $F$ 关于 $y$ 的雅可比矩阵. 对于 $r> 0$, 令 $C\left(B\left(x_0,r\right),\mathbb{R}^{m}\right)$ 表示定义在闭球 $B\left(x_0,r\right)$ 上, 取值在 $\mathbb{R}^{m}$ 中的向量值连续函数空间, 它按范数

$$
\left\|\varphi\right\|=\max_{x\in B\left(x_0,r\right),\,1\le i\le m}\left|\varphi_i\left(x\right)\right|,\quad \varphi=\left(\varphi_1,\dots,\varphi_m\right),
$$

构成了一个巴拿赫空间. 证明:

(i) 存在 $r> 0$ 与 $\delta> 0$, 使得在 $C\left(B\left(x_0,r\right),\mathbb{R}^{m}\right)$ 的子集

$$
E=\left\{\varphi\in C\left(B\left(x_0,r\right),\mathbb{R}^{m}\right):\ \varphi\left(x_0\right)=y_0,\ \left|\varphi\left(x\right)-y_0\right|\le\delta,\ \forall x\in B\left(x_0,r\right)\right\}
$$

中, $\left(T\varphi\right)\left(x\right)=\varphi\left(x\right)-\left(\frac{\partial F}{\partial y}\left(x_0,y_0\right)\right)^{-1}F\left(x,\varphi\left(x\right)\right)$ 是良定义的压缩映射;

(ii) 存在 $x_0$ 的邻域 $U_0\subset U$ 以及唯一的连续函数 $\varphi:U_0\to\mathbb{R}^{m}$, 满足

$$
F\left(x,\varphi\left(x\right)\right)=0,\ \forall x\in U_0,\quad \varphi\left(x_0\right)=y_0.
$$

### 解答 1.5-8

(i) 记 $A=\left(\frac{\partial F}{\partial y}\right)\left(x_0,y_0\right)$. 由线性代数知识, $\det A\neq0$ 蕴含 $A$ 是可逆矩阵; 于是 $A^{-1}$ 存在且按算子范数有界, 记其范数为 $\left\|A^{-1}\right\|$.

由于 $F\left(x_0,y_0\right)=0$ 且 $F$ 在 $U\times V$ 中连续, 故对任意 $\varepsilon> 0$, 存在 $r_1> 0$, $\delta_1> 0$, 使得 $B\left(x_0,r_1\right)\subset U$, $B\left(y_0,\delta_1\right)\subset V$, 并且当 $\left|x-x_0\right|\le r_1$, $\left|y-y_0\right|\le\delta_1$ 时有 $\left|F\left(x,y\right)\right|< \varepsilon$. 取 $\varepsilon=\frac{\delta_1}{2\left\|A^{-1}\right\|}$, 可找到 $r_1,\delta_1> 0$ 使

$$
\left\|A^{-1}\right\|\cdot\left|F\left(x,y\right)\right|< \frac{\delta_1}{2},\quad \left|x-x_0\right|\le r_1,\ \left|y-y_0\right|\le\delta_1. \tag{1}
$$

另一方面, 由于 $F\left(x,\cdot\right)$ 对每个 $x\in U$ 连续可微, $\frac{\partial F}{\partial y}$ 在 $U\times V$ 上连续, 且 $\frac{\partial F}{\partial y}\left(x_0,y_0\right)=A$, 故存在 $0< r\le r_1$, $0< \delta\le\delta_1$, 使得当 $\left|x-x_0\right|\le r$, $\left|y-y_0\right|\le\delta$ 时有

$$
\left\|A^{-1}\frac{\partial F}{\partial y}\left(x,y\right)-I\right\|< \theta< 1 \tag{2}
$$

对某个 $0< \theta< 1$ 成立 (例如取 $\theta=\frac12$).

现在验证 $T$ 良定义. 取 $\varphi\in E$. 因 $F$ 连续, $\varphi$ 连续, 故 $T\varphi=\varphi-A^{-1}F\left(\cdot,\varphi\left(\cdot\right)\right)$ 是 $B\left(x_0,r\right)$ 上的连续函数, 即 $T\varphi\in C\left(B\left(x_0,r\right),\mathbb{R}^{m}\right)$. 又因 $F\left(x_0,y_0\right)=0$, 故

$$
\left(T\varphi\right)\left(x_0\right)=\varphi\left(x_0\right)-A^{-1}F\left(x_0,\varphi\left(x_0\right)\right)=y_0-A^{-1}F\left(x_0,y_0\right)=y_0.
$$

再由 (1), 对一切 $x\in B\left(x_0,r\right)$ 有 $\left|\left(T\varphi\right)\left(x\right)-y_0\right|=\left|A^{-1}F\left(x,\varphi\left(x\right)\right)\right|\le\left\|A^{-1}\right\|\cdot\left|F\left(x,\varphi\left(x\right)\right)\right|< \delta$. 于是 $T\varphi\in E$, 即 $T:E\to E$ 良定义.

下证 $T$ 是压缩映射. 设 $\varphi_1,\varphi_2\in E$, $x\in B\left(x_0,r\right)$. 由于 $F\left(x,\cdot\right)$ 在包含线段 $\left[\varphi_2\left(x\right),\varphi_1\left(x\right)\right]$ 的开集 $V$ 上连续可微, 由向量值函数的微分中值定理,

$$
F\left(x,\varphi_1\left(x\right)\right)-F\left(x,\varphi_2\left(x\right)\right)=\left(\int_0^{1}\frac{\partial F}{\partial y}\left(x,\varphi_2\left(x\right)+t\left(\varphi_1\left(x\right)-\varphi_2\left(x\right)\right)\right)\,\mathrm dt\right)\left(\varphi_1\left(x\right)-\varphi_2\left(x\right)\right).
$$

因为 $\varphi_1,\varphi_2\in E$, 故 $\varphi_2\left(x\right)+t\left(\varphi_1\left(x\right)-\varphi_2\left(x\right)\right)\in B\left(y_0,\delta\right)$, 故由 (2),

$$
\begin{aligned}
\left|\left(T\varphi_1\right)\left(x\right)-\left(T\varphi_2\right)\left(x\right)\right|&=\left|\left(I-A^{-1}\int_0^{1}\frac{\partial F}{\partial y}\left(x,\varphi_2\left(x\right)t\left(\varphi_1\left(x\right)-\varphi_2\left(x\right)\right)\right)\,\mathrm dt\right)\left(\varphi_1\left(x\right)-\varphi_2\left(x\right)\right)\right|\\
&\le\theta\left|\varphi_1\left(x\right)-\varphi_2\left(x\right)\right|.
\end{aligned}
$$

对 $x$ 取最大值, 得到 $\left\|T\varphi_1-T\varphi_2\right\|\le\theta\left\|\varphi_1-\varphi_2\right\|$, 其中 $0< \theta< 1$. 故 $T$ 是 $E$ 上的压缩映射.

(ii) 已知 $E$ 关于条件 $\varphi\left(x_0\right)=y_0$, $\left|\varphi\left(x\right)-y_0\right|\le\delta$ ($\forall x$) 是闭集, 故 $E$ 是巴拿赫空间 $C\left(B\left(x_0,r\right),\mathbb{R}^{m}\right)$ 的闭子集, 由**引理 1.4.1 (基本点列与完备性)(iii)**, $E$ 是完备的. 由**定理 1.5.1 (巴拿赫不动点定理)**, $T$ 在 $E$ 中存在唯一的不动点 $\varphi$, 即 $T\varphi=\varphi$. 于是对一切 $x\in B\left(x_0,r\right)$,

$$
\varphi\left(x\right)-A^{-1}F\left(x,\varphi\left(x\right)\right)=\varphi\left(x\right)\ \Rightarrow\ A^{-1}F\left(x,\varphi\left(x\right)\right)=0\ \Rightarrow\ F\left(x,\varphi\left(x\right)\right)=0.
$$

其中, 最后一步用到 $A^{-1}$ 可逆, 故 $A^{-1}F=0$ 蕴含 $F=0$, 且 $\varphi\left(x_0\right)=y_0$. 

取 $U_0=B\left(x_0,r\right)\cap U$, 则 $U_0$ 是 $x_0$ 在 $U$ 中的邻域, $\varphi|_{U_0}$ 连续, 满足 $F\left(x,\varphi\left(x\right)\right)=0$ ($\forall x\in U_0$) 且 $\varphi\left(x_0\right)=y_0$. 唯一性: 若在 $U_0'\subset U$ 上还有连续解 $\psi$, 满足 $F\left(x,\psi\left(x\right)\right)=0$, $\psi\left(x_0\right)=y_0$, 则由 $\psi$ 的连续性和 $\psi\left(x_0\right)=y_0$, 适当缩小邻域可设 $B\left(x_0,r\right)\subset U_0\cap U_0'$ 且 $\left|\psi\left(x\right)-y_0\right|\le\delta$ 对 $x\in B\left(x_0,r\right)$ 成立, 于是 $\psi|_{B\left(x_0,r\right)}\in E$ 且 $T\psi=\psi$, 由不动点的唯一性得 $\psi=\varphi$ 于 $B\left(x_0,r\right)$, 进而于 $U_0\cap U_0'$. $\blacksquare$

---

## 1.6-1 (紧度量空间的有限交性质)

设 $A$ 是紧的度量空间, $\left\{F_\lambda\right\}$ 是 $A$ 的一族闭子集, 如果 $\left\{F_\lambda\right\}$ 中任意有限个 $F_{\lambda_1},\dots,F_{\lambda_n}$ 的交集都不空, 那么 $\bigcap_\lambda F_\lambda$ 也不空. 反之, 如果度量空间 $A$ 具有如下性质: 对于 $A$ 中任意的闭子集族 $\left\{F_\lambda\right\}$, 从任意有限交集不空可推出 $\bigcap_\lambda F_\lambda$ 不空, 那么 $A$ 是紧的度量空间.

### 解答 1.6-1

先证第一句. 用反证法, 假设 $\bigcap_\lambda F_\lambda=\emptyset$. 由德摩根律, $\left\{A\setminus F_\lambda\right\}$ 是 $A$ 的开覆盖: 每个 $A\setminus F_\lambda$ 都是开集 (因 $F_\lambda$ 是闭集), 且 $\bigcup_\lambda\left(A\setminus F_\lambda\right)=A\setminus\bigcap_\lambda F_\lambda=A$. 由**定理 1.6.2 (列紧 $\Leftrightarrow$ 覆盖紧)**, 紧的度量空间 $A$ 的每个开覆盖都有有限子覆盖, 故存在有限个指标 $\lambda_1,\dots,\lambda_n$ 使

$$
A=\bigcup_{i=1}^{n}\left(A\setminus F_{\lambda_i}\right)=A\setminus\bigcap_{i=1}^{n}F_{\lambda_i},
$$

从而 $\bigcap_{i=1}^{n}F_{\lambda_i}=\emptyset$, 这与 $\left\{F_\lambda\right\}$ 的任意有限交集不空矛盾. 故 $\bigcap_\lambda F_\lambda\neq\emptyset$.

再证第二句. 设度量空间 $A$ 具有所述有限交性质, 证明 $A$ 是紧的. 由**定理 1.6.2 (列紧 $\Leftrightarrow$ 覆盖紧)**, 只须证明 $A$ 是列紧的, 即 $A$ 中任意点列都有收敛子列. 用反证法, 设存在点列 $\left\{x_n\right\}\subset A$ 没有收敛子列. 令 $F_n=\overline{\left\{x_k:k\ge n\right\}}$ ($A$ 中从第 $n$ 项起的尾集的闭包). 则每个 $F_n$ 是闭集, 且 $F_1\supset F_2\supset\cdots$, 故任意有限个 $F_{n_1},\dots,F_{n_m}$ (设 $n=\max\left\{n_i\right\}$) 的交 $\bigcap_{i=1}^{m}F_{n_i}=F_n\neq\emptyset$ (因为 $x_n\in F_n$). 由有限交性质, $\bigcap_{n=1}^{\infty}F_n\neq\emptyset$. 取 $x\in\bigcap_{n=1}^{\infty}F_n$. 由 $x\in F_n=\overline{\left\{x_k:k\ge n\right\}}$, 对每个 $n$ 与 $\varepsilon=\frac1m$, 存在 $k_m\ge n$ 使 $d\left(x_{k_m},x\right)< \frac1m$, 于是取子列 $k_1< k_2< \cdots$ 即得 $x_{k_m}\to x$, 这与 $\left\{x_n\right\}$ 没有收敛子列矛盾. 故 $A$ 列紧, 由**定理 1.6.2 (列紧 $\Leftrightarrow$ 覆盖紧)**, $A$ 是紧的. $\blacksquare$

---

## 1.6-3 ($\mathbb{R}^{n}$ 有界子集的有限 $\varepsilon$-网)

对 $\mathbb{R}^{n}$ 的有界子集 $E$ 及数 $\varepsilon> 0$, 给出它的一个有限 $\varepsilon$-网.

### 解答 1.6-3

因 $E$ 有界, 故存在 $M> 0$ 使 $E\subset\left[-M,M\right]^{n}$. 把 $\mathbb{R}^{n}$ 按平行于坐标轴的方向分割成边长为 $a=\frac{\varepsilon}{\sqrt{n}}$ 的小方体

$$
\left\{\prod_{i=1}^{n}\left[k_i a,\ \left(k_i+1\right)a\right]:\ k_i\in\mathbb{Z},\ i=1,\dots,n\right\}.
$$

每个小方体的 (外接球的) 直径不超过 $\sqrt{n}\,a=\varepsilon$. 因为 $E\subset\left[-M,M\right]^{n}$, 故与 $E$ 相交的小方体只有有限多个 (事实上至多 $\left(\left\lfloor\frac{2M}{a}\right\rfloor+2\right)^{n}$ 个). 对这有限多个小方体, 每个与 $E$ 相交的方体 $Q_j$ 中取一个点 $x_j\in E\cap Q_j$, 得到有限集 $\left\{x_1,\dots,x_N\right\}$. 对任意 $x\in E$, $x$ 属于某个与 $E$ 相交的方体 $Q_j$, 故 $\left|x-x_j\right|\le\operatorname{diam}Q_j\le\varepsilon$, 即 $x\in U\left(x_j,\varepsilon\right)$. 所以 $\left\{x_1,\dots,x_N\right\}$ 是 $E$ 的有限 $\varepsilon$-网. $\blacksquare$

---

## 1.6-5 (完全有界等价于有限维子空间逼近)

设 $L$ 是赋范线性空间, $A$ 是 $L$ 的有界子集. 证明: $A$ 是完全有界集的充要条件是: 对任何 $\varepsilon> 0$, 存在 $L$ 的有限维子空间 $M$, 使 $A$ 中每个点与 $M$ 的距离都小于 $\varepsilon$.

### 解答 1.6-5

先证充分性. 设 $A$ 完全有界. 由**定义 1.6.3 ($\varepsilon$-网与完全有界集)**, 对 $\varepsilon> 0$, $A$ 有有限的 $\varepsilon$-网 $\left\{a_1,\dots,a_N\right\}\subset A$. 令 $M=\operatorname{span}\left\{a_1,\dots,a_N\right\}$, 则 $M$ 是 $L$ 的有限维子空间. 对任意 $a\in A$, 存在 $a_i$ 使 $\left\|a-a_i\right\|< \varepsilon$, 而 $a_i\in M$, 故 $d\left(a,M\right)=\inf_{m\in M}\left\|a-m\right\|\le\left\|a-a_i\right\|< \varepsilon$. 故 $A$ 中每个点与 $M$ 的距离小于 $\varepsilon$.

再证必要性. 设对任何 $\varepsilon> 0$ 存在有限维子空间 $M$, 使 $A$ 中每个点与 $M$ 的距离小于 $\varepsilon$. 给定 $\varepsilon> 0$, 取 $M$ 使 $d\left(a,M\right)< \frac{\varepsilon}{2}$ 对一切 $a\in A$ 成立. 对每个 $a\in A$, 由 $d\left(a,M\right)< \frac{\varepsilon}{2}$ 可取 $m\left(a\right)\in M$ 使 $\left\|a-m\left(a\right)\right\|< \frac{\varepsilon}{2}$. 因 $A$ 有界且 $\left\|m\left(a\right)\right\|\le\left\|m\left(a\right)-a\right\|+\left\|a\right\|$, 故集合 $\left\{m\left(a\right):a\in A\right\}\subset M$ 有界. 由**例 1.6.3 ($\mathbb{R}^n$ 中有界集完全有界)**, 有限维赋范线性空间 $M$ 中的有界集是完全有界集, 故存在有限集 $\left\{m_1,\dots,m_N\right\}\subset M$ 使 $\left\{m\left(a\right):a\in A\right\}\subset\bigcup_{i=1}^{N}U\left(m_i,\varepsilon/2\right)$. 于是对任意 $a\in A$, 存在 $i$ 使 $\left\|m\left(a\right)-m_i\right\|< \frac{\varepsilon}{2}$, 故

$$
\left\|a-m_i\right\|\le\left\|a-m\left(a\right)\right\|+\left\|m\left(a\right)-m_i\right\|< \frac{\varepsilon}{2}+\frac{\varepsilon}{2}=\varepsilon.
$$

所以 $\left\{m_1,\dots,m_N\right\}$ 是 $A$ 的有限 $\varepsilon$-网 (由**注 1.6.1 (网中的点不必属于集合本身)**, 网点不必属于 $A$). 由 $\varepsilon$ 的任意性, $A$ 完全有界. $\blacksquare$

---

## 1.6-6 (赫尔德空间 $C_\alpha$ 中完全有界集的充分条件)

设 $0< \alpha\le1$. $C_\alpha\left[a,b\right]$ 是由在 $\left[a,b\right]$ 上满足赫尔德条件 $\left|f\left(x\right)-f\left(x'\right)\right|\le M_f\left|x-x'\right|^{\alpha}$, 并且 $f\left(a\right)=0$ 的函数组成的线性空间, 其范数定义为

$$
\left\|f\right\|=\sup_{x,x'\in\left[a,b\right],\,x\neq x'}\frac{\left|f\left(x\right)-f\left(x'\right)\right|}{\left|x-x'\right|^{\alpha}}.
$$

试写出 $C_\alpha\left[a,b\right]$ 中的点集是完全有界集的一些条件.

### 解答 1.6-6

我给出如下的充分条件: 若 $A\subset C_\alpha\left[a,b\right]$ 满足:

(i) $A$ 在 $C_\alpha\left[a,b\right]$ 中有界, 即存在 $M> 0$ 使 $\left\|f\right\|\le M$ ($\forall f\in A$) ;

(ii) 对每个 $\varepsilon> 0$, 存在 $\delta> 0$, 使得

$$
\sup_{f\in A}\ \sup_{0< \left|x-x'\right|< \delta}\frac{\left|f\left(x\right)-f\left(x'\right)\right|}{\left|x-x'\right|^{\alpha}}< \varepsilon,
$$

则 $A$ 是完全有界集.

先由 (i) 推出 $A$ 在 $C\left[a,b\right]$ 中一致有界且等度连续. 事实上, 对 $f\in A$ 与 $x\in\left[a,b\right]$, 由 $f\left(a\right)=0$ 得 $\left|f\left(x\right)\right|=\left|f\left(x\right)-f\left(a\right)\right|\le\left\|f\right\|\left|x-a\right|^{\alpha}\le M\left(b-a\right)^{\alpha}$, 故 $A$ 在 $C\left[a,b\right]$ 中一致有界; 且 $\left|f\left(x\right)-f\left(x'\right)\right|\le\left\|f\right\|\left|x-x'\right|^{\alpha}\le M\left|x-x'\right|^{\alpha}$, 故 $A$ 在 $C\left[a,b\right]$ 中等度连续. 由**定理 1.6.5 (阿泽拉-阿斯卡里定理)**, $A$ 在 $C\left[a,b\right]$ 中相对列紧. 由**定理 1.6.3 (豪斯多夫定理)**, 因 $C\left[a,b\right]$ 完备, 故其是完全有界的.

下面用 $\varepsilon$-网直接证明 $A$ 在 $C_\alpha\left[a,b\right]$ 中完全有界. 给定 $\varepsilon> 0$, 由条件 (ii) 取 $\delta> 0$ 使

$$
\sup_{f\in A}\ \sup_{0< \left|x-x'\right|< \delta}\frac{\left|f\left(x\right)-f\left(x'\right)\right|}{\left|x-x'\right|^{\alpha}}< \frac{\varepsilon}{4}. \tag{1}
$$

取 $\left[a,b\right]$ 的一个分划 $a=t_0< t_1< \cdots< t_N=b$, 使网格长 $h=\max_j\left(t_{j+1}-t_j\right)< \delta$, 且 $h$ 小到

$$
\frac{\varepsilon h^{\alpha}}{\delta^{\alpha}}< \frac{\varepsilon}{4}. \tag{2}
$$

由 (i) 得到的一致有界性, 求值向量集 $\left\{\left(f\left(t_0\right),\dots,f\left(t_N\right)\right):f\in A\right\}\subset\mathbb{R}^{N+1}$ 有界, 由**例 1.6.3 ($\mathbb{R}^n$ 中有界集完全有界)** 它在 $\mathbb{R}^{N+1}$ (按最大坐标范数) 中完全有界, 故存在有限集 $\left\{f_1,\dots,f_K\right\}\subset A$ 使: 对每个 $f\in A$, 存在 $i$ 满足

$$
\max_{0\le j\le N}\left|f\left(t_j\right)-f_i\left(t_j\right)\right|< \frac{\varepsilon\delta^{\alpha}}{8}. \tag{3}
$$

下证 $\left\{f_1,\dots,f_K\right\}$ 是 $A$ 在 $C_\alpha\left[a,b\right]$ 中的有限 $\varepsilon$-网. 任取 $f\in A$, 取 $i$ 使 (3) 成立, 对任意 $x\neq x'\in\left[a,b\right]$ 估计 $\frac{\left|\left(f-f_i\right)\left(x\right)-\left(f-f_i\right)\left(x'\right)\right|}{\left|x-x'\right|^{\alpha}}$.

若 $\left|x-x'\right|< \delta$, 则由 (1) 分别用于 $f$ 与 $f_i$ (均属于 $A$):

$$
\left|\left(f-f_i\right)\left(x\right)-\left(f-f_i\right)\left(x'\right)\right|\le\left|f\left(x\right)-f\left(x'\right)\right|+\left|f_i\left(x\right)-f_i\left(x'\right)\right|< \frac{\varepsilon}{4}\left|x-x'\right|^{\alpha}+\frac{\varepsilon}{4}\left|x-x'\right|^{\alpha}=\frac{\varepsilon}{2}\left|x-x'\right|^{\alpha}.
$$

若 $\left|x-x'\right|\ge\delta$, 先估计 $\left|\left(f-f_i\right)\left(z\right)\right|$ ($z\in\left[a,b\right]$). 设 $z\in\left[t_j,t_{j+1}\right]$, 则 $\left|z-t_j\right|\le h< \delta$, 由 (1) 得 $\left|f\left(z\right)-f\left(t_j\right)\right|< \frac{\varepsilon}{4}\left|z-t_j\right|^{\alpha}\le\frac{\varepsilon}{4}h^{\alpha}$, 同理 $\left|f_i\left(z\right)-f_i\left(t_j\right)\right|< \frac{\varepsilon}{4}h^{\alpha}$; 再由 (3) 得 $\left|f\left(t_j\right)-f_i\left(t_j\right)\right|< \frac{\varepsilon\delta^{\alpha}}{8}$. 故

$$
\left|\left(f-f_i\right)\left(z\right)\right|\le\left|f\left(z\right)-f\left(t_j\right)\right|+\left|f\left(t_j\right)-f_i\left(t_j\right)\right|+\left|f_i\left(t_j\right)-f_i\left(z\right)\right|< \frac{\varepsilon}{2}h^{\alpha}+\frac{\varepsilon\delta^{\alpha}}{8}.
$$

于是由 (2),

$$
\frac{\left|\left(f-f_i\right)\left(x\right)-\left(f-f_i\right)\left(x'\right)\right|}{\left|x-x'\right|^{\alpha}}\le\frac{\left|\left(f-f_i\right)\left(x\right)\right|+\left|\left(f-f_i\right)\left(x'\right)\right|}{\delta^{\alpha}}\le\frac{2\left(\frac{\varepsilon}{2}h^{\alpha}+\frac{\varepsilon\delta^{\alpha}}{8}\right)}{\delta^{\alpha}}=\frac{\varepsilon h^{\alpha}}{\delta^{\alpha}}+\frac{\varepsilon}{4}< \frac{\varepsilon}{2}.
$$

综合两情形, $\left\|f-f_i\right\|_{C_\alpha\left[a,b\right]}< \varepsilon$, 故 $\left\{f_1,\dots,f_K\right\}$ 是 $A$ 的有限 $\varepsilon$-网. 由 $\varepsilon$ 的任意性, $A$ 完全有界. $\blacksquare$

---

## 1.6-7 (科尔莫戈罗夫-里斯-弗雷歇定理的必要性)

证明**定理 1.6.7 (科尔莫戈罗夫-里斯-弗雷歇定理)** 中的必要性, 即若 $A\subset L^{p}\left(\mathbb{R}\right)$ ($1\le p< \infty$) 是完全有界集, 则:

(i) $A$ 是有界集;

(ii) 对每个 $\varepsilon> 0$, 存在 $M> 0$, 使得 $\int_{\left\{\left|x\right|> M\right\}}\left|f\left(x\right)\right|^{p}\,\mathrm dm< \varepsilon^{p}$, $\forall f\in A$;

(iii) 对每个 $\varepsilon> 0$, 存在 $\delta> 0$, 使得 $\left\|f\left(x+h\right)-f\left(x\right)\right\|_{p}\le\varepsilon$, $\forall f\in A$, $\forall \left|h\right|< \delta$.

### 解答 1.6-7

先证 (i). 由**定理 1.6.3 (豪斯多夫定理)**, $L^{p}\left(\mathbb{R}\right)$ 完备且 $A$ 完全有界, 故 $A$ 相对列紧; 由**推论 1.6.1 (相对列紧集可分且有界)**, 相对列紧集是有界的, 故 $A$ 有界.

再证 (ii). 由**定义 1.6.3 ($\varepsilon$-网与完全有界集)**, $A$ 完全有界, 故对给定的 $\varepsilon> 0$, $A$ 有有限的 $\frac{\varepsilon}{2}$-网 $\left\{f_1,\dots,f_N\right\}\subset A$. 因为每个 $f_i\in L^{p}\left(\mathbb{R}\right)$ 满足 $\int_{\left\{\left|x\right|> M\right\}}\left|f_i\left(x\right)\right|^{p}\,\mathrm dm\to0$ ($M\to\infty$), 故存在 $M> 0$ 使对一切 $i$ 有

$$
\left(\int_{\left\{\left|x\right|> M\right\}}\left|f_i\left(x\right)\right|^{p}\,\mathrm dm\right)^{1/p}< \frac{\varepsilon}{2}.
$$

对任意 $f\in A$, 存在 $i$ 使 $\left\|f-f_i\right\|_{p}< \frac{\varepsilon}{2}$. 由**闵可夫斯基不等式**,

$$
\begin{aligned}
&\quad\;\left(\int_{\left\{\left|x\right|> M\right\}}\left|f\left(x\right)\right|^{p}\,\mathrm dm\right)^{1/p}\le\left(\int_{\left\{\left|x\right|> M\right\}}\left|f\left(x\right)-f_i\left(x\right)\right|^{p}\,\mathrm dm\right)^{1/p}\\
&+\left(\int_{\left\{\left|x\right|> M\right\}}\left|f_i\left(x\right)\right|^{p}\,\mathrm dm\right)^{1/p}\le\left\|f-f_i\right\|_{p}+\frac{\varepsilon}{2}< \varepsilon.
\end{aligned}
$$

于是 $\int_{\left\{\left|x\right|> M\right\}}\left|f\left(x\right)\right|^{p}\,\mathrm dm< \varepsilon^{p}$ ($\forall f\in A$), (ii) 得证.

最后证 (iii). 对给定的 $\varepsilon> 0$, 由**定义 1.6.3 ($\varepsilon$-网与完全有界集)**, $A$ 有有限的 $\frac{\varepsilon}{3}$-网 $\left\{f_1,\dots,f_N\right\}\subset A$. 由**习题 1.4-15 (平均连续性)**, 每个 $f_i$ 满足 $\left\|f_i\left(x+h\right)-f_i\left(x\right)\right\|_{p}\to0$ ($h\to0$), 故存在 $\delta> 0$ 使 $\left|h\right|< \delta$ 时对一切 $i$ 有 $\left\|f_i\left(x+h\right)-f_i\left(x\right)\right\|_{p}< \frac{\varepsilon}{3}$. 对任意 $f\in A$, 存在 $i$ 使 $\left\|f-f_i\right\|_{p}< \frac{\varepsilon}{3}$; 由 $L^{p}$ 范数的平移不变性和**闵可夫斯基不等式**,

$$
\left\|f\left(x+h\right)-f\left(x\right)\right\|_{p}\le\left\|f\left(x+h\right)-f_i\left(x+h\right)\right\|_{p}+\left\|f_i\left(x+h\right)-f_i\left(x\right)\right\|_{p}+\left\|f_i\left(x\right)-f\left(x\right)\right\|_{p}< \frac{\varepsilon}{3}+\frac{\varepsilon}{3}+\frac{\varepsilon}{3}=\varepsilon
$$

对一切 $\left|h\right|< \delta$ 成立. 故 (iii) 得证. 综上, 必要性成立. $\blacksquare$

---

## 1.6-8 ($C_0\left(\mathbb R\right)$ 中相对列紧的充要条件)

设

$$
C_0\left(\mathbb{R}\right)=\left\{f:\ f\ \text{在}\ \mathbb{R}\ \text{上连续且}\ \lim_{\left|x\right|\to\infty}f\left(x\right)=0\right\}
$$

按范数 $\left\|f\right\|=\sup_{x\in\mathbb{R}}\left|f\left(x\right)\right|$ 构成巴拿赫空间. 证明 $A\subset C_0\left(\mathbb{R}\right)$ 是相对列紧集的充要条件是 $A$ 有界, 等度连续, 且对任意 $\varepsilon> 0$ 存在 $N> 0$, 使得 $\left|f\left(x\right)\right|\le\varepsilon$ ($\forall \left|x\right|> N$, $f\in A$).

### 解答 1.6-8

先证必要性. 设 $A\subset C_0\left(\mathbb{R}\right)$ 相对列紧. 由**定理 1.6.3 (豪斯多夫定理)** ($C_0\left(\mathbb{R}\right)$ 完备), $A$ 完全有界, 故由**推论 1.6.1 (相对列紧集可分且有界)**, $A$ 有界.

由**定义 1.6.3 ($\varepsilon$-网与完全有界集)**, 对 $\varepsilon> 0$, $A$ 有有限的 $\frac{\varepsilon}{2}$-网 $\left\{f_1,\dots,f_N\right\}\subset A$. 每个 $f_i\in C_0\left(\mathbb{R}\right)$ 连续且 $\lim_{\left|x\right|\to\infty}f_i\left(x\right)=0$, 故存在 $M_i> 0$ 使 $\left|f_i\left(x\right)\right|< \frac{\varepsilon}{2}$ 当 $\left|x\right|> M_i$. 令 $M=\max_iM_i$, 则 $\left|f_i\left(x\right)\right|< \frac{\varepsilon}{2}$ 对 $\left|x\right|> M$ 及一切 $i$ 成立. 对任意 $f\in A$, 存在 $i$ 使 $\left\|f-f_i\right\|< \frac{\varepsilon}{2}$, 于是当 $\left|x\right|> M$ 时

$$
\left|f\left(x\right)\right|\le\left|f\left(x\right)-f_i\left(x\right)\right|+\left|f_i\left(x\right)\right|< \frac{\varepsilon}{2}+\frac{\varepsilon}{2}=\varepsilon.
$$

故对任意 $\varepsilon> 0$ 存在 $N=M$ 使 $\left|f\left(x\right)\right|\le\varepsilon$ ($\forall\left|x\right|> N$, $f\in A$).

再证 $A$ 等度连续. 每个 $f_i\in C_0\left(\mathbb{R}\right)$ 在 $\mathbb{R}$ 上一致连续 (见**习题 1.6-16**: 紧区间外函数趋于 $0$, 紧区间上连续则一致连续), 故存在 $\delta> 0$ 使 $\left|x-x'\right|< \delta$ 时 $\left|f_i\left(x\right)-f_i\left(x'\right)\right|< \frac{\varepsilon}{3}$ 对一切 $i$ 成立. 对任意 $f\in A$, 存在 $i$ 使 $\left\|f-f_i\right\|< \frac{\varepsilon}{3}$, 故 $\left|x-x'\right|< \delta$ 时

$$
\left|f\left(x\right)-f\left(x'\right)\right|\le\left|f\left(x\right)-f_i\left(x\right)\right|+\left|f_i\left(x\right)-f_i\left(x'\right)\right|+\left|f_i\left(x'\right)-f\left(x'\right)\right|< \frac{\varepsilon}{3}+\frac{\varepsilon}{3}+\frac{\varepsilon}{3}=\varepsilon.
$$

故 $A$ 等度连续. 必要性得证.

再证充分性. 设 $A$ 有界, 等度连续, 且对任意 $\varepsilon> 0$ 存在 $N$ 使 $\left|f\left(x\right)\right|\le\varepsilon$ 对 $\left|x\right|> N$, $f\in A$. 证明 $A$ 完全有界, 再由**定理 1.6.3 (豪斯多夫定理)** ($C_0\left(\mathbb{R}\right)$ 完备) 得 $A$ 相对列紧.

给定 $\varepsilon> 0$, 由假设取 $N> 0$ 使 $\left|f\left(x\right)\right|\le\frac{\varepsilon}{3}$ 对 $\left|x\right|> N$, $f\in A$. 在紧区间 $\left[-N,N\right]$ 上, $A$ 作为 $C\left[-N,N\right]$ 的子集有界且等度连续, 由**定理 1.6.5 (阿泽拉-阿斯卡里定理)**, $A|_{\left[-N,N\right]}$ 在 $C\left[-N,N\right]$ 中相对列紧, 从而是完全有界的, 故存在有限个函数 $g_1,\dots,g_K$ 使: 对每个 $f\in A|_{\left[-N,N\right]}$, 存在 $k$ 满足

$$
\max_{\left|x\right|\le N}\left|f\left(x\right)-g_k\left(x\right)\right|< \frac{\varepsilon}{3}.
$$

把每个 $g_k$ 线性延拓为 $\widetilde g_k\in C_0\left(\mathbb{R}\right)$: $\widetilde g_k=g_k$ 于 $\left[-N,N\right]$, 在 $\left[N,N+1\right]$ 与 $\left[-N-1,-N\right]$ 上从 $g_k\left(\pm N\right)$ 线性过渡到 $0$, 在 $\left|x\right|\ge N+1$ 上取 $0$. 则 $\left\{\widetilde g_1,\dots,\widetilde g_K\right\}\subset C_0\left(\mathbb{R}\right)$. 当 $\left|x\right|\le N$ 时 $\left|f\left(x\right)-\widetilde g_k\left(x\right)\right|=\left|f\left(x\right)-g_k\left(x\right)\right|< \frac{\varepsilon}{3}$; 当 $\left|x\right|> N$ 时 $\left|f\left(x\right)\right|\le\frac{\varepsilon}{3}$, 且 $\left|\widetilde g_k\left(x\right)\right|\le\max\left\{\left|g_k\left(N\right)\right|,\left|g_k\left(-N\right)\right|\right\}$, 而 $\left|g_k\left(\pm N\right)\right|\le\left|f\left(\pm N\right)-g_k\left(\pm N\right)\right|+\left|f\left(\pm N\right)\right|< \frac{\varepsilon}{3}+\frac{\varepsilon}{3}=\frac{2\varepsilon}{3}$, 故 $\left|f\left(x\right)-\widetilde g_k\left(x\right)\right|\le\left|f\left(x\right)\right|+\left|\widetilde g_k\left(x\right)\right|< \frac{\varepsilon}{3}+\frac{2\varepsilon}{3}=\varepsilon$. 于是 $\left\|f-\widetilde g_k\right\|< \varepsilon$, 故 $\left\{\widetilde g_1,\dots,\widetilde g_K\right\}$ 是 $A$ 的有限 $\varepsilon$-网. 由 $\varepsilon$ 的任意性, $A$ 完全有界, 从而相对列紧. $\blacksquare$

---

## 1.6-9 (相对列紧集的凸包仍相对列紧)

设 $X$ 是巴拿赫空间, $A$ 是 $X$ 中的相对列紧集, 证明它的凸包 $\operatorname{co}\left(A\right)$ 也是相对列紧集.

### 解答 1.6-9

因 $X$ 完备且 $A$ 相对列紧, 由**定理 1.6.3 (豪斯多夫定理)**, $A$ 完全有界. 故对 $\varepsilon> 0$, $A$ 有有限的 $\varepsilon$-网 $\left\{a_1,\dots,a_N\right\}\subset A$.

下证 $\operatorname{co}\left(A\right)\subset\operatorname{co}\left\{a_1,\dots,a_N\right\}+B\left(0,\varepsilon\right)$. 由**基础知识: 凸包**, 任取 $z\in\operatorname{co}\left(A\right)$, 则存在 $x_1,\dots,x_m\in A$ 与非负实数 $\lambda_1,\dots,\lambda_m$ ($\sum_{j=1}^{m}\lambda_j=1$) 使 $z=\sum_{j=1}^{m}\lambda_jx_j$. 对每个 $j$, 由 $\left\{a_1,\dots,a_N\right\}$ 是 $A$ 的 $\varepsilon$-网, 存在 $i_j\in\left\{1,\dots,N\right\}$ 使 $\left\|x_j-a_{i_j}\right\|< \varepsilon$. 于是

$$
z=\sum_{j=1}^{m}\lambda_ja_{i_j}+\sum_{j=1}^{m}\lambda_j\left(x_j-a_{i_j}\right),
$$

其中 $\sum_{j=1}^{m}\lambda_ja_{i_j}\in\operatorname{co}\left\{a_1,\dots,a_N\right\}$, 且

$$
\left\|\sum_{j=1}^{m}\lambda_j\left(x_j-a_{i_j}\right)\right\|\le\sum_{j=1}^{m}\lambda_j\left\|x_j-a_{i_j}\right\|< \sum_{j=1}^{m}\lambda_j\varepsilon=\varepsilon.
$$

故 $z\in\operatorname{co}\left\{a_1,\dots,a_N\right\}+B\left(0,\varepsilon\right)$.

记 $K=\operatorname{co}\left\{a_1,\dots,a_N\right\}=\left\{\sum_{i=1}^{N}\lambda_ia_i:\lambda_i\ge0,\ \sum_{i=1}^{N}\lambda_i=1\right\}$. 依据**基础知识: 单 (纯) 形**, 它是 $\mathbb{R}^{N}$ 中的单形 $\Delta_{N-1}=\left\{\lambda_i\ge0,\ \sum\lambda_i=1\right\}$ 在连续映射 $\left(\lambda_1,\dots,\lambda_N\right)\mapsto\sum\lambda_ia_i$ 下的像, 故 $K$ 是紧集, 由**例 1.6.3 ($\mathbb{R}^n$ 中有界集完全有界)** 知 $K$ 完全有界, 故对 $\varepsilon> 0$, $K$ 有有限的 $\varepsilon$-网 $\left\{y_1,\dots,y_M\right\}\subset K$. 于是对任意 $z\in\operatorname{co}\left(A\right)$, 存在 $u\in K$ 使 $\left\|z-u\right\|< \varepsilon$, 且存在 $l$ 使 $\left\|u-y_l\right\|< \varepsilon$, 故 $\left\|z-y_l\right\|< 2\varepsilon$. 所以 $\left\{y_1,\dots,y_M\right\}$ 是 $\operatorname{co}\left(A\right)$ 的有限 $2\varepsilon$-网. 由 $\varepsilon$ 的任意性, $\operatorname{co}\left(A\right)$ 完全有界, 再由**定理 1.6.3 (豪斯多夫定理)** ($X$ 完备) 得 $\operatorname{co}\left(A\right)$ 相对列紧. $\blacksquare$

---

## 1.6-10 (格罗滕迪克定理)

设 $X$ 是巴拿赫空间, $K$ 是 $X$ 中的相对列紧集. 证明存在 $X$ 中的点列 $\left\{x_n\right\}$, 使得 $\lim_{n\to\infty}x_n=0$, 且

$$
K\subset\left\{\sum_{n=1}^{\infty}a_nx_n:\ \sum_{n=1}^{\infty}\left|a_n\right|\le1\right\}.
$$

### 解答 1.6-10

因 $K$ 相对列紧, 由**定理 1.6.3 (豪斯多夫定理)** ($X$ 完备) $K$ 完全有界, 故由**定义 1.6.3 ($\varepsilon$-网与完全有界集)**, 对每个 $n$, $K$ 有有限的 $\frac{1}{n}$-网, 记作 $\left\{y_{n,1},\dots,y_{n,m_n}\right\}\subset K$. 令

$$
B=\bigcup_{n=1}^{\infty}\left\{y_{n,1},\dots,y_{n,m_n}\right\},
$$

则 $B$ 是可数集, 且 $B$ 在 $K$ 中稠密 (因 $B$ 以任意精度逼近 $K$ 中每个点). 把 $B$ 依序排列成点列 $\left\{z_1,z_2,\dots\right\}$, 使先排 $\frac{1}{n}$-网, 再排 $\frac{1}{n+1}$-网……由于后加入的点属于更细的网, 与已有点的距离至多约 $\frac{1}{n}+\frac{1}{n-1}$, 故可排得相邻点距离递减且满足

$$
\left\|z_k-z_{k-1}\right\|\to0,\quad \sum_{k=2}^{\infty}\left\|z_k-z_{k-1}\right\|< \infty. \tag{1}
$$

若有必要, 在每层网间插入更细的有限点使 (1) 成立, 这不改变 $B$ 的稠密性. 因 $B$ 在 $K$ 中稠密, 故 $B$ 在 $\overline{K}$ 中稠密, 于是

$$
\overline{K}\subset\overline{B}\subset\overline{\operatorname{co}}\left(B\right)=\overline{\operatorname{co}}\left\{z_k\right\}. \tag{2}
$$

定义点列 $\left\{x_n\right\}$:

$$
x_1=z_1,\quad x_n=z_n-z_{n-1}\ \ \left(n\ge2\right).
$$

由 (1), $\left\|x_n\right\|=\left\|z_n-z_{n-1}\right\|\to0$, 故 $\lim_{n\to\infty}x_n=0$; 且 $\sum_{n=1}^{\infty}\left\|x_n\right\|\le\left\|z_1\right\|+\sum_{n=2}^{\infty}\left\|z_n-z_{n-1}\right\|< \infty$, 即 $\left\{x_n\right\}$ 绝对可和.

下面证明 $K\subset\overline{\operatorname{co}}\left\{\pm x_n\right\}$. 任取 $w\in\overline{K}$, 由 (2), 存在 $w^{\left(m\right)}\in\operatorname{co}\left\{z_k\right\}$ 使 $w^{\left(m\right)}\to w$. 每个 $w^{\left(m\right)}$ 形如有限凸组合 $w^{\left(m\right)}=\sum_{k=1}^{p_m}\lambda_k^{\left(m\right)}z_k$, 其中 $\lambda_k^{\left(m\right)}\ge0$, $\sum_k\lambda_k^{\left(m\right)}=1$. 由于 $z_k=\sum_{i=1}^{k}x_i$ (望远镜求和), 故

$$
w^{\left(m\right)}=\sum_{k=1}^{p_m}\lambda_k^{\left(m\right)}\sum_{i=1}^{k}x_i=\sum_{i=1}^{p_m}\left(\sum_{k=i}^{p_m}\lambda_k^{\left(m\right)}\right)x_i.
$$

记 $c_i^{\left(m\right)}=\sum_{k=i}^{p_m}\lambda_k^{\left(m\right)}$, 则 $0\le c_i^{\left(m\right)}\le\sum_k\lambda_k^{\left(m\right)}=1$, 故 $c_i^{\left(m\right)}\in\left[0,1\right]$. 于是每个 $w^{\left(m\right)}$ 是 $\left\{\pm x_i\right\}$ 的有限凸组合 (系数在 $\left[-1,1\right]$ 内), 即

$$
w^{\left(m\right)}\in\operatorname{co}\left\{\pm x_1,\dots,\pm x_{p_m}\right\}\subset\overline{\operatorname{co}}\left\{\pm x_n\right\}.
$$

因 $w^{\left(m\right)}\to w$ 且 $\overline{\operatorname{co}}\left\{\pm x_n\right\}$ 是闭集, 故 $w\in\overline{\operatorname{co}}\left\{\pm x_n\right\}$. 所以 $\overline{K}\subset\overline{\operatorname{co}}\left\{\pm x_n\right\}$, 特别地 $K\subset\overline{\operatorname{co}}\left\{\pm x_n\right\}$.

最后说明 $\overline{\operatorname{co}}\left\{\pm x_n\right\}=\left\{\sum_{n=1}^{\infty}a_nx_n:\ \left|a_n\right|\le1\right\}$. 一方面, $\left\{\pm x_n\right\}$ 的每个有限凸组合 $\sum\varepsilon_i\lambda_ix_i$ ($\lambda_i\ge0,\sum\lambda_i=1,\varepsilon_i\in\left\{\pm1\right\}$) 满足 $\left|\varepsilon_i\lambda_i\right|\le1$, 且由于 $\sum\left\|x_n\right\|< \infty$ 级数绝对收敛, 故 $\overline{\operatorname{co}}\left\{\pm x_n\right\}\subset\left\{\sum a_nx_n:\left|a_n\right|\le1\right\}$. 另一方面, $\left\{\sum a_nx_n:\left|a_n\right|\le1\right\}$ 是闭集 (若 $u^{\left(m\right)}=\sum a_n^{\left(m\right)}x_n\to u$, $\left|a_n^{\left(m\right)}\right|\le1$, 则由对角线抽取与控制收敛可得子列 $a_n^{\left(m_k\right)}\to a_n$ (逐 $n$) 且 $u=\sum a_nx_n$, $\left|a_n\right|\le1$), 且含 $\left\{\pm x_n\right\}$ 的凸包, 故 $\overline{\operatorname{co}}\left\{\pm x_n\right\}\supset\left\{\sum a_nx_n:\left|a_n\right|\le1\right\}$. 两方向合起来得等号. 于是

$$
K\subset\overline{\operatorname{co}}\left\{\pm x_n\right\}=\left\{\sum_{n=1}^{\infty}a_nx_n:\ \left|a_n\right|\le1,\ n=1,2,\dots\right\},\quad \lim_{n\to\infty}x_n=0.
$$

$\blacksquare$

---

## 1.6-11 ($L^1$ 单位球上的线性泛函与上确界不可达)

设 $B_1=\left\{f\in L^{1}\left[a,b\right]:\ \left\|f\right\|_1\le1\right\}$ 是实 $L^{1}\left[a,b\right]$ 的闭单位球, $g\in L^{\infty}\left[a,b\right]$ 是实值函数. 对 $f\in B_1$, 定义 $F_g\left(f\right)=\int_a^{b}fg\,\mathrm dm$. 证明 $F_g$ 在 $B_1$ 上是连续的, 并且

$$
\sup_{f\in B_1}F_g\left(f\right)=\left\|g\right\|_{\infty};
$$

又说明当 $g\left(x\right)=x-a$ 时, $\sup$ 不能达到.

### 解答 1.6-11

先证 $F_g$ 连续. 对 $f,h\in B_1$, 由 $L^{1}$-范数定义与 $\left|g\right|\le\left\|g\right\|_{\infty}$ (a.e.),

$$
\left|F_g\left(f\right)-F_g\left(h\right)\right|=\left|\int_a^{b}\left(f-h\right)g\,\mathrm dm\right|\le\int_a^{b}\left|f-h\right|\left|g\right|\,\mathrm dm\le\left\|g\right\|_{\infty}\int_a^{b}\left|f-h\right|\,\mathrm dm=\left\|g\right\|_{\infty}\left\|f-h\right\|_1.
$$

由于 $\left\|g\right\|_\infty$ 与 $f$, $h$ 无关, 故认为是常数. 即 $F_g$ 是 $B_1$ 上的利普希茨映射, 从而是连续的.

再证 $\sup_{f\in B_1}F_g\left(f\right)=\left\|g\right\|_{\infty}$. 先看上界: 对任意 $f\in B_1$, 同样有

$$
F_g\left(f\right)=\int_a^{b}fg\,\mathrm dm\le\int_a^{b}\left|f\right|\left|g\right|\,\mathrm dm\le\left\|g\right\|_{\infty}\left\|f\right\|_1\le\left\|g\right\|_{\infty},
$$

故 $\sup_{f\in B_1}F_g\left(f\right)\le\left\|g\right\|_{\infty}$.

再看下界. 对 $\varepsilon> 0$, 因 $\left\|g\right\|_{\infty}$ 是 $g$ 的本质上确界, 集合 $E_\varepsilon=\left\{x\in\left[a,b\right]:\ \left|g\left(x\right)\right|> \left\|g\right\|_{\infty}-\varepsilon\right\}$ 具有正测度 $m\left(E_\varepsilon\right)> 0$. 取

$$
f_\varepsilon\left(x\right)=\frac{\operatorname{sign}\left(g\left(x\right)\right)}{m\left(E_\varepsilon\right)}\chi_{E_\varepsilon}\left(x\right),
$$

其中 $\operatorname{sign}\left(g\right)$ 是 $g$ 的符号函数 (可测). 则 $\left\|f_\varepsilon\right\|_1=\int_{E_\varepsilon}\frac{\left|\operatorname{sign}\left(g\right)\right|}{m\left(E_\varepsilon\right)}\,\mathrm dm=\frac{m\left(E_\varepsilon\right)}{m\left(E_\varepsilon\right)}=1$, 故 $f_\varepsilon\in B_1$. 于是

$$
F_g\left(f_\varepsilon\right)=\int_{E_\varepsilon}\frac{g\left(x\right)\operatorname{sign}\left(g\left(x\right)\right)}{m\left(E_\varepsilon\right)}\,\mathrm dm=\frac{1}{m\left(E_\varepsilon\right)}\int_{E_\varepsilon}\left|g\left(x\right)\right|\,\mathrm dm\ge\frac{\left(\left\|g\right\|_{\infty}-\varepsilon\right)\,m\left(E_\varepsilon\right)}{m\left(E_\varepsilon\right)}=\left\|g\right\|_{\infty}-\varepsilon.
$$

故对任意 $\varepsilon> 0$ 有 $\sup_{f\in B_1}F_g\left(f\right)\ge\left\|g\right\|_{\infty}-\varepsilon$, 令 $\varepsilon\to0$ 得 $\sup_{f\in B_1}F_g\left(f\right)\ge\left\|g\right\|_{\infty}$. 综合上下界, $\sup_{f\in B_1}F_g\left(f\right)=\left\|g\right\|_{\infty}$.

最后说明 $g\left(x\right)=x-a$ 时 $\sup$ 不能达到. 此时 $\left\|g\right\|_{\infty}=b-a$. 若存在 $f\in B_1$ 使 $F_g\left(f\right)=\left\|g\right\|_{\infty}=b-a$, 则由 $x-a\le b-a$ 对一切 $x\in\left[a,b\right]$ 成立,

$$
b-a=F_g\left(f\right)=\int_a^{b}\left(x-a\right)f\,\mathrm dm\le\int_a^{b}\left(b-a\right)\left|f\right|\,\mathrm dm=\left(b-a\right)\left\|f\right\|_1\le b-a.
$$

上式必须处处取等号, 特别地 $\left\|f\right\|_1=1$ 且 $\int_a^{b}\left(x-a\right)f\,\mathrm dm=\int_a^{b}\left(b-a\right)\left|f\right|\,\mathrm dm$. 由 $x-a< b-a$ 在除点 $b$ 外的一切点成立, 最后这个等式迫使 $f$ 几乎处处为零 ($f\neq0$ 的点只能落在单点集 $\left\{b\right\}$ 上, 其测度为 $0$), 这与 $\left\|f\right\|_1=1$ 矛盾. 故不存在 $f\in B_1$ 使 $F_g\left(f\right)=\left\|g\right\|_{\infty}$, 即 $\sup$ 不能达到. $\blacksquare$

> 直观理解 $\sup$ 不能达到的原因是, 一次函数 $x-a$ 取到上确界当且仅当 $x=b$, 而单点集测度为 $0$, 因此其本性上确界必然达不到 $b-a$.

---

## 1.6-12 (定理 1.6.9 的证明)

证明**定理 1.6.9 (紧度量空间上的性质)**. 即设 $X$ 是紧的度量空间, 证明:

(i) $X$ 上的连续函数是一致连续的;

(ii) $C\left(X\right)$ 按范数 $\left\|f\right\|=\max_{x\in X}\left|f\left(x\right)\right|$ 构成巴拿赫空间;

(iii) $A\subset C\left(X\right)$ 是相对列紧集当且仅当 $A$ 是有界的且等度连续的.

### 解答 1.6-12

先证 (i). 设 $f\in C\left(X\right)$, $\varepsilon> 0$. 由 $f$ 的连续性, 对每个 $x\in X$ 存在 $\delta_x> 0$, 使得 $d\left(x,x'\right)< \delta_x$ 蕴含 $\left|f\left(x\right)-f\left(x'\right)\right|< \frac{\varepsilon}{2}$. 开球族 $\left\{U\left(x,\frac{\delta_x}{2}\right):x\in X\right\}$ 覆盖紧空间 $X$, 由**定理 1.6.2 (列紧 $\Leftrightarrow$ 覆盖紧)** 它有有限子覆盖 $\left\{U\left(x_i,\frac{\delta_{x_i}}{2}\right)\right\}_{i=1}^{m}$. 令 $\delta=\min_i\frac{\delta_{x_i}}{2}> 0$. 若 $d\left(x,x'\right)< \delta$, 取 $i$ 使 $x\in U\left(x_i,\frac{\delta_{x_i}}{2}\right)$, 则 $d\left(x,x_i\right)< \frac{\delta_{x_i}}{2}< \delta_{x_i}$, 故 $\left|f\left(x\right)-f\left(x_i\right)\right|< \frac{\varepsilon}{2}$; 且 $d\left(x',x_i\right)\le d\left(x',x\right)+d\left(x,x_i\right)< \delta+\frac{\delta_{x_i}}{2}\le\frac{\delta_{x_i}}{2}+\frac{\delta_{x_i}}{2}=\delta_{x_i}$, 故 $\left|f\left(x'\right)-f\left(x_i\right)\right|< \frac{\varepsilon}{2}$. 于是 $\left|f\left(x\right)-f\left(x'\right)\right|< \varepsilon$. 所以 $f$ 一致连续, (i) 得证.

再证 (ii). 由**推论 1.6.3 (连续函数达到上下确界)**, 连续函数在紧空间上达到上确界, 故 $\left\|f\right\|=\max_{x\in X}\left|f\left(x\right)\right|$ 良定义, 且它满足范数公理 (非负性, 齐次性, 三角不等式), 故 $C\left(X\right)$ 是赋范线性空间. 证其完备: 设 $\left\{f_n\right\}\subset C\left(X\right)$ 是柯西列, 则对每个 $x\in X$, $\left|f_n\left(x\right)-f_m\left(x\right)\right|\le\left\|f_n-f_m\right\|\to0$, 故 $\left\{f_n\left(x\right)\right\}$ 是 $\mathbb{R}$ 中的柯西列, 因 $\mathbb{R}$ 完备而收敛, 记 $f\left(x\right)=\lim_nf_n\left(x\right)$. 对 $\varepsilon> 0$, 取 $N$ 使 $\left\|f_n-f_m\right\|< \varepsilon$ ($n,m\ge N$), 则对一切 $x$ 与 $m\ge N$, $\left|f_n\left(x\right)-f_m\left(x\right)\right|< \varepsilon$, 令 $m\to\infty$ 得 $\left|f_n\left(x\right)-f\left(x\right)\right|\le\varepsilon$ ($\forall x$), 故 $\left\|f_n-f\right\|\le\varepsilon$, 即 $f_n\to f$ 于 $C\left(X\right)$ 范数. 又因一致极限保持连续性: 对 $\varepsilon> 0$ 取 $n$ 使 $\left\|f_n-f\right\|< \frac{\varepsilon}{3}$, 由 $f_n$ 连续取 $\delta$ 使 $d\left(x,y\right)< \delta$ 蕴含 $\left|f_n\left(x\right)-f_n\left(y\right)\right|< \frac{\varepsilon}{3}$, 则 $\left|f\left(x\right)-f\left(y\right)\right|\le\left|f\left(x\right)-f_n\left(x\right)\right|+\left|f_n\left(x\right)-f_n\left(y\right)\right|+\left|f_n\left(y\right)-f\left(y\right)\right|< \varepsilon$, 故 $f$ 连续, $f\in C\left(X\right)$. 于是柯西列收敛, $C\left(X\right)$ 完备, 是巴拿赫空间, (ii) 得证.

最后证 (iii). 先证充分性: 设 $A$ 有界且等度连续, 证明 $A$ 相对列紧. 因 $X$ 紧, 由**基础知识: 紧度量空间的性质**, $X$ 完备且完全有界; 由 (ii), $C\left(X\right)$ 完备. 故由**定理 1.6.3 (豪斯多夫定理)**, 只须证 $A$ 完全有界. 给定 $\varepsilon> 0$, 由 $A$ 等度连续, 存在 $\delta> 0$ 使 $d\left(x,y\right)< \delta$ 蕴含 $\left|f\left(x\right)-f\left(y\right)\right|< \frac{\varepsilon}{3}$ ($\forall f\in A$). 因 $X$ 完全有界, $X$ 有有限的 $\delta$-网 $\left\{x_1,\dots,x_N\right\}\subset X$. 考虑求值映射 $\Phi:A\to\mathbb{R}^{N}$, $\Phi\left(f\right)=\left(f\left(x_1\right),\dots,f\left(x_N\right)\right)$. 因 $A$ 有界, $\Phi\left(A\right)$ 在 $\mathbb{R}^{N}$ 中有界, 由**例 1.6.3 ($\mathbb{R}^n$ 中有界集完全有界)** 它完全有界, 故有有限的 $\frac{\varepsilon}{3}$-网, 即存在有限个 $f_1,\dots,f_K\in A$ 使: 对每个 $f\in A$ 存在 $i$ 满足 $\max_j\left|f\left(x_j\right)-f_i\left(x_j\right)\right|< \frac{\varepsilon}{3}$. 对任意 $x\in X$, $x$ 落在某个 $x_j$ 的 $\delta$-邻域内, 故 $d\left(x,x_j\right)< \delta$, 由等度连续性 $\left|f\left(x\right)-f\left(x_j\right)\right|< \frac{\varepsilon}{3}$, $\left|f_i\left(x\right)-f_i\left(x_j\right)\right|< \frac{\varepsilon}{3}$, 于是

$$
\left|f\left(x\right)-f_i\left(x\right)\right|\le\left|f\left(x\right)-f\left(x_j\right)\right|+\left|f\left(x_j\right)-f_i\left(x_j\right)\right|+\left|f_i\left(x_j\right)-f_i\left(x\right)\right|< \varepsilon.
$$

对 $x$ 取上确界得 $\left\|f-f_i\right\|< \varepsilon$, 故 $\left\{f_1,\dots,f_K\right\}$ 是 $A$ 的有限 $\varepsilon$-网. 故 $A$ 完全有界, 由**定理 1.6.3 (豪斯多夫定理)** 得 $A$ 相对列紧.

再证必要性: 设 $A$ 相对列紧. 由**定理 1.6.3 (豪斯多夫定理)** ($C\left(X\right)$ 完备), $A$ 完全有界, 由**推论 1.6.1 (相对列紧集可分且有界)** 得 $A$ 有界. 证等度连续: 对 $\varepsilon> 0$, 由 $A$ 完全有界, $A$ 有有限的 $\frac{\varepsilon}{3}$-网 $\left\{f_1,\dots,f_N\right\}$. 由 (i), 每个 $f_i$ 一致连续, 故存在 $\delta> 0$ 使 $d\left(x,y\right)< \delta$ 蕴含 $\left|f_i\left(x\right)-f_i\left(y\right)\right|< \frac{\varepsilon}{3}$ ($\forall i$). 对任意 $f\in A$, 存在 $i$ 使 $\left\|f-f_i\right\|< \frac{\varepsilon}{3}$, 故 $d\left(x,y\right)< \delta$ 时

$$
\left|f\left(x\right)-f\left(y\right)\right|\le\left|f\left(x\right)-f_i\left(x\right)\right|+\left|f_i\left(x\right)-f_i\left(y\right)\right|+\left|f_i\left(y\right)-f\left(y\right)\right|< \varepsilon.
$$

故 $A$ 等度连续. 必要性得证. 综上, (iii) 成立. $\blacksquare$

---

## 1.6-16 (紧度量空间上连续映射一致连续)

设 $X$ 是紧的度量空间, $f:X\to Y$ 是度量空间之间的连续映射. 证明 $f$ 是一致连续的.

### 解答 1.6-16

设 $\varepsilon> 0$. 由 $f$ 的连续性, 对每个 $x\in X$ 存在 $\delta_x> 0$, 使得 $d_X\left(x,x'\right)< \delta_x$ 蕴含 $d_Y\left(f\left(x\right),f\left(x'\right)\right)< \frac{\varepsilon}{2}$. 开球族 $\left\{U\left(x,\frac{\delta_x}{2}\right):x\in X\right\}$ 覆盖紧空间 $X$, 由**定理 1.6.2 (列紧 $\Leftrightarrow$ 覆盖紧)** 它有有限子覆盖 $\left\{U\left(x_i,\frac{\delta_{x_i}}{2}\right)\right\}_{i=1}^{m}$. 令 $\delta=\min_i\frac{\delta_{x_i}}{2}> 0$. 若 $d_X\left(x,x'\right)< \delta$, 取 $i$ 使 $x\in U\left(x_i,\frac{\delta_{x_i}}{2}\right)$, 则 $d_X\left(x,x_i\right)< \frac{\delta_{x_i}}{2}< \delta_{x_i}$, 故 $d_Y\left(f\left(x\right),f\left(x_i\right)\right)< \frac{\varepsilon}{2}$; 且 $d_X\left(x',x_i\right)\le d_X\left(x',x\right)+d_X\left(x,x_i\right)< \delta+\frac{\delta_{x_i}}{2}\le\delta_{x_i}$, 故 $d_Y\left(f\left(x'\right),f\left(x_i\right)\right)< \frac{\varepsilon}{2}$. 于是 $d_Y\left(f\left(x\right),f\left(x'\right)\right)\le d_Y\left(f\left(x\right),f\left(x_i\right)\right)+d_Y\left(f\left(x_i\right),f\left(x'\right)\right)< \varepsilon$. 所以 $f$ 一致连续. $\blacksquare$

---

## 1.6-17 (迪尼定理)

设 $X$ 是紧的度量空间, $\left\{f_k\right\}$ 是 $X$ 上递增的实值连续函数列, 即 $f_k\left(x\right)\le f_{k+1}\left(x\right)$ ($\forall x\in X$, $k=1,2,\dots$). 若 $\left\{f_k\right\}$ 逐点收敛于连续函数 $f$, 则 $f_k\rightrightarrows f$ (即一致收敛于 $f$).

### 解答 1.6-17

记 $g_k=f-f_k$. 因 $f$, $f_k$ 连续且 $f_k\le f_{k+1}\le f$, 故每个 $g_k\in C\left(X\right)$, $g_k\ge0$, 且对每个 $x$, $\left\{g_k\left(x\right)\right\}$ 单调递减趋于 $0$ (因 $f_k\left(x\right)\uparrow f\left(x\right)$).

给定 $\varepsilon> 0$. 由 $g_k\left(x\right)\to0$, 对每个 $x\in X$ 存在 $k_x$ 使 $g_{k_x}\left(x\right)< \frac{\varepsilon}{2}$. 由 $g_{k_x}$ 的连续性, 存在 $x$ 的开邻域 $O_x$, 使 $y\in O_x$ 时 $g_{k_x}\left(y\right)< \varepsilon$. 开集族 $\left\{O_x:x\in X\right\}$ 覆盖紧空间 $X$, 由**定理 1.6.2 (列紧 $\Leftrightarrow$ 覆盖紧)** 它有有限子覆盖 $\left\{O_{x_1},\dots,O_{x_m}\right\}$. 令 $N=\max\left\{k_{x_1},\dots,k_{x_m}\right\}$. 对任意 $k\ge N$ 与 $y\in X$, $y$ 属于某个 $O_{x_j}$, 且 $k\ge k_{x_j}$, 由 $\left\{g_k\left(y\right)\right\}$ 关于 $k$ 单调递减得

$$
g_k\left(y\right)\le g_{k_{x_j}}\left(y\right)< \varepsilon.
$$

于是 $\left\|g_k\right\|=\max_{y\in X}g_k\left(y\right)< \varepsilon$ 对一切 $k\ge N$ 成立, 故 $\left\|f_k-f\right\|=\left\|g_k\right\|\to0$, 即 $f_k\rightrightarrows f$. $\blacksquare$
