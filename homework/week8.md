# week8

> **定义 1.2.1 (哈梅尔基)**
> 
> 线性空间 $X$ 上的一个极大线性无关组称为空间 $X$ 的一组哈梅尔基. 若 $X$ 的某个哈梅尔基中只有有限个元素, 则称 $X$ 是有限维线性空间, 否则称其为无限维线性空间.

> **定理 1.4.2 (有限维赋范线性空间完备)**
> 
> 有限维的赋范线性空间是完备的.

> **定义 2.1.2 (算子范数)**
> 
> 设 $T$ 为赋范线性空间 $X$ 到赋范线性空间 $Y$ 的有界算子, 称 $\left\|T\right\|=\sup_{x\neq0}\frac{\left\|Tx\right\|}{\left\|x\right\|}$ 为算子 $T$ 的范数. 对有界线性算子 $T$, 成立 $\left\|Tx\right\|\le\left\|T\right\|\left\|x\right\|,\quad\forall{}x\in{}X$.

> **定理 2.3.1 (哈恩-巴拿赫延拓定理)**
> 
> 设 $L_0$ 是实赋范线性空间 $L$ 的线性子空间. 若 $f_0$ 是 $L_0$ 上的有界线性泛函, 则存在 $L$ 上的有界线性泛函 $f$, $f|_{L_0}=f_0$, 且 $\left\|f\right\|=\left\|f_0\right\|$.

> **推论 2.3.1 (范数可达的泛函)**
> 
> 对赋范线性空间 $X$ 中的非零元素 $x_0$, 存在 $f\in{}X^{*}$ 使得 $\left\|f\right\|=1$ 且 $f\left(x_0\right)=\left\|x_0\right\|$.

> **推论 2.3.4 (闭线性子空间与点的分离)**
> 
> 设 $M$ 是赋范线性空间 $\left(X,\left\|\cdot\right\|\right)$ 的闭线性子空间, $x\notin{}M$, 则存在 $f\in{}X^{*}$ 使得 $\left\|f\right\|=1$, $f\left(M\right)=0$, $f\left(x\right)=d\left(x,M\right)$.

> **定义 2.4.1 (凸集)**
> 
> 设 $V$ 是线性空间, $M$ 是 $V$ 的一个子集. 如果对于任意的 $x,y\in{}M$, 及数 $\alpha\in\left[0,1\right]$, 有 $\alpha{}x+\left(1-\alpha\right)y\in{}M$, 就称 $M$ 是一个凸集.

> **定义 2.4.2 (闵可夫斯基泛函)**
> 
> 设 $M$ 是线性空间 $V$ 中吸收的凸集. 对于任意的 $x\in{}V$, 定义 $p_M\left(x\right)=\inf\left\{\alpha:\alpha>0,\alpha^{-1}x\in{}M\right\}$, 称 $p_M$ 为 $M$ 的闵可夫斯基泛函.

> **命题 2.4.3 (吸收凸集的闵可夫斯基泛函)**
> 
> 设 $M$ 是线性空间 $V$ 中的一个吸收凸子集, 那么 $M$ 的闵可夫斯基泛函 $p_M\left(x\right)$ 是 $V$ 上的一个次线性泛函, 并且 $\left\{x:p_M\left(x\right)<1\right\}\subset{}M\subset\left\{x:p_M\left(x\right)\le1\right\}$. 如果 $M$ 还是均衡的, 那么 $p_M\left(x\right)$ 是 $V$ 上的一个半范数.

## 2.3-1 (有限个给定值的线性泛函与范数估计)

设 $E$ 是赋范线性空间, $x_1,x_2,\cdots,x_k\in{}E$, $\alpha_1,\alpha_2,\cdots,\alpha_k$ 是一组数. 在 $E$ 上存在线性泛函 $f$, 使得 $f\left(x_\nu\right)=\alpha_\nu$, $\nu=1,2,\cdots,k$, 证明: $\left\|f\right\|\le{}M$ 的充要条件是: 对于任意的一组数 $t_1,t_2,\cdots,t_k$, 成立

$$
\left|\sum_{\nu=1}^{k}t_\nu\alpha_\nu\right|\le{}M\left\|\sum_{\nu=1}^{k}t_\nu{}x_\nu\right\|.
$$

### 解答 2.3-1

必要性. 任给一组数 $t_1,\cdots,t_k$. 由 $f$ 的线性, $\sum_{\nu=1}^{k}t_\nu\alpha_\nu=\sum_{\nu=1}^{k}t_\nu{}f\left(x_\nu\right)=f\left(\sum_{\nu=1}^{k}t_\nu{}x_\nu\right)$, 再由**定义 2.1.2 (算子范数)** 中的 $\left|f\left(y\right)\right|\le\left\|f\right\|\left\|y\right\|$,

$$
\left|\sum_{\nu=1}^{k}t_\nu\alpha_\nu\right|=\left|f\left(\sum_{\nu=1}^{k}t_\nu{}x_\nu\right)\right|\le\left\|f\right\|\left\|\sum_{\nu=1}^{k}t_\nu{}x_\nu\right\|\le{}M\left\|\sum_{\nu=1}^{k}t_\nu{}x_\nu\right\|.
$$

$\blacksquare$

充分性. 记 $L_0=\operatorname{span}\left\{x_1,\cdots,x_k\right\}$, $f_0\left(x_\nu\right)=\alpha_\nu$, $x_\nu\in{L_0}$. 对 $y=\sum_{\nu=1}^{k}t_\nu{}x_\nu\in{L_0}$ 与数 $c$, 由不等式可知 $\left|f_0\left(y\right)\right|\le{}M\left\|y\right\|$ ($\forall{}y\in{L_0}$), 故 $f_0$ 是 $L_0$ 上的有界线性泛函, $\left\|f_0\right\|\le{}M$. 由**定理 2.3.1 (哈恩-巴拿赫延拓定理)**, 存在 $E$ 上的有界线性泛函 $f$, 使 $f|_{L_0}=f_0$ 且 $\left\|f\right\|=\left\|f_0\right\|\le{}M$; 特别地 $f\left(x_\nu\right)=f_0\left(x_\nu\right)=\alpha_\nu$ ($\nu=1,\cdots,k$).

$\blacksquare$

## 2.3-2 (对偶族与线性无关性)

设 $\left\{x_\alpha:\alpha\in\Lambda\right\}$, $\left\{f_\alpha:\alpha\in\Lambda\right\}$ 分别是赋范线性空间 $X$ 与 $X^{*}$ 中的两族向量. 若满足 $f_\alpha\left(x_\beta\right)=\delta_{\alpha\beta}$, $\alpha,\beta\in\Lambda$, 则称 $\left\{x_\alpha\right\}$ 和 $\left\{f_\alpha\right\}$ 是对偶族. 证明:

(i) 当 $\left\{x_\alpha\right\}$, $\left\{f_\alpha\right\}$ 是对偶族时, $\left\{x_\alpha\right\}$, $\left\{f_\alpha\right\}$ 必分别是 $X$ 和 $X^{*}$ 中的线性无关组.

(ii) 若 $\left\{x_\alpha\right\}$ 满足: $x_\alpha\notin\operatorname{span}\left\{x_\beta:\beta\neq\alpha,\beta\in\Lambda\right\}$, $\forall\alpha\in\Lambda$, 则必存在 $\left\{f_\alpha\right\}$, 使得 $\left\{x_\alpha\right\}$, $\left\{f_\alpha\right\}$ 是对偶族.

(iii) 在 $X$ 是线性空间的情况下, 对任何一族线性无关向量 $\left\{x_\alpha\right\}$, 必存在一族相应的线性泛函 $\left\{f_\alpha\right\}$, 使得 $f_\alpha\left(x_\beta\right)=\delta_{\alpha\beta}$, 并且 $\left\{f_\alpha\right\}$ 必也是线性无关的.

### 解答 2.3-2

(i) 设 $\alpha_1,\cdots,\alpha_n$ 是 $\Lambda$ 中任意有限个指标, $c_1,\cdots,c_n$ 是一组数, 且 $\sum_{i=1}^{n}c_if_{\alpha_i}=0$. 对每个 $j\in\left\{1,\cdots,n\right\}$, 用 $x_{\alpha_j}$ 作用于该等式两端,

$$
0=\left(\sum_{i=1}^{n}c_if_{\alpha_i}\right)\left(x_{\alpha_j}\right)=\sum_{i=1}^{n}c_i\delta_{\alpha_i\alpha_j}=c_j,
$$

故 $c_1=\cdots=c_n=0$, 即 $\left\{f_\alpha\right\}$ 中任意有限个向量线性无关, $\left\{f_\alpha\right\}$ 是 $X^{*}$ 中的线性无关组; 同理, 设 $\sum_{i=1}^{n}c_ix_{\alpha_i}=0$. 对每个 $j$, 用 $f_{\alpha_j}$ 作用于该等式两端,

$$
0=f_{\alpha_j}\left(\sum_{i=1}^{n}c_ix_{\alpha_i}\right)=\sum_{i=1}^{n}c_if_{\alpha_j}\left(x_{\alpha_i}\right)=\sum_{i=1}^{n}c_i\delta_{\alpha_j\alpha_i}=c_j,
$$

故 $c_1=\cdots=c_n=0$, 即 $\left\{x_\alpha\right\}$ 是 $X$ 中的线性无关组.

$\blacksquare$

(ii) 固定 $\alpha\in\Lambda$, 记 $M_\alpha=\overline{\operatorname{span}\left\{x_\beta:\beta\neq\alpha,\beta\in\Lambda\right\}}$, 它是 $X$ 的闭线性子空间. 由题设 $x_\alpha\notin{}M_\alpha$; 因 $M_\alpha$ 闭, 距离 $d\left(x_\alpha,M_\alpha\right)>0$. 由**推论 2.3.4 (闭线性子空间与点的分离)**, 存在 $g_\alpha\in{}X^{*}$, 使 $\left\|g_\alpha\right\|=1$, $g_\alpha\left(M_\alpha\right)=0$, $g_\alpha\left(x_\alpha\right)=d\left(x_\alpha,M_\alpha\right)$. 令 $f_\alpha=g_\alpha/d\left(x_\alpha,M_\alpha\right)$. 则 $f_\alpha\in{}X^{*}$, $f_\alpha\left(x_\alpha\right)=1$; 而对 $\beta\neq\alpha$, 因 $x_\beta\in{}M_\alpha$, 有 $g_\alpha\left(x_\beta\right)=0$, 故 $f_\alpha\left(x_\beta\right)=0$. 于是 $f_\alpha\left(x_\beta\right)=\delta_{\alpha\beta}$ ($\forall\alpha,\beta\in\Lambda$), $\left\{x_\alpha\right\}$ 与 $\left\{f_\alpha\right\}$ 是对偶族.

$\blacksquare$

(iii) 由**定义 1.2.1 (哈梅尔基)**, 线性无关组 $\left\{x_\alpha:\alpha\in\Lambda\right\}$ 可用扩充为 $X$ 的一组哈梅尔基 $\left\{x_\alpha:\alpha\in\Lambda\right\}\cup\left\{y_\gamma:\gamma\in\Gamma\right\}$. 对每个 $\alpha$, 令 $f_\alpha\left(x_\beta\right)=\delta_{\alpha\beta}$ ($\forall\beta\in\Lambda$), $f_\alpha\left(y_\gamma\right)=0$ ($\forall\gamma\in\Gamma$), 再按线性延拓到 $X$, 仍用符号 $f_a$ 表示. 则 $f_\alpha$ 是 $X$ 上的线性泛函, 且 $f_\alpha\left(x_\beta\right)=\delta_{\alpha\beta}$. 设 $c_1,\cdots,c_n$ 与 $\alpha_1,\cdots,\alpha_n$ 使 $\sum_{i=1}^{n}c_if_{\alpha_i}=0$. 与 (i) 中对 $\left\{f_\alpha\right\}$ 的论证相同, 得出 $\left\{f_\alpha\right\}$ 线性无关.

$\blacksquare$

## 2.3-3 ($X\times{}Y$ 与等价范数下的对偶分解)

(i) 设 $X,Y$ 是两个赋范线性空间, 在 $X\times{}Y$ 上定义 $\left\|\left(x,y\right)\right\|=\max\left(\left\|x\right\|,\left\|y\right\|\right)$. 证明: 对于任意的 $F\in\left(X\times{}Y\right)^{*}$, 必定存在唯一的一对 $f\in{}X^{*}$, $g\in{}Y^{*}$, 使得 $F\left(x,y\right)=f\left(x\right)+g\left(y\right)$. 如果在 $X^{*}\times{}Y^{*}$ 上定义 $\left\|\left(f,g\right)\right\|=\left\|f\right\|+\left\|g\right\|$, 那么 $F\mapsto\left(f,g\right)$ 的映射是 $\left(X\times{}Y\right)^{*}$ 到 $X^{*}\times{}Y^{*}$ 的保范线性同构.

(ii) 设 $\left\|\cdot\right\|_1$, $\left\|\cdot\right\|_2$ 是线性空间 $X$ 上的两个范数, 记 $\left(X,\left\|\cdot\right\|_i\right)$ ($i=1,2$) 的对偶空间为 $X_i^{*}$, 并在 $X$ 上赋范数 $\left\|x\right\|=\left(\left\|x\right\|_1^2+\left\|x\right\|_2^2\right)^{\frac12}$. 证明: $F\in\left(X,\left\|\cdot\right\|\right)^{*}$ 成立的条件是存在 $f_i\in{}X_i^{*}$, 使得 $F=f_1+f_2$.

### 解答 2.3-3

(i) 存在性. 令 $f\left(x\right)=F\left(x,0\right)$ ($x\in{}X$), $g\left(y\right)=F\left(0,y\right)$ ($y\in{}Y$). 由 $F$ 的线性,

$$
F\left(x,y\right)=F\left(\left(x,0\right)+\left(0,y\right)\right)=F\left(x,0\right)+F\left(0,y\right)=f\left(x\right)+g\left(y\right).
$$

$\blacksquare$

唯一性. 设 $f,f'\in{}X^{*}$, $g,g'\in{}Y^{*}$ 使 $f\left(x\right)+g\left(y\right)=f'\left(x\right)+g'\left(y\right)$ ($\forall\left(x,y\right)$). 取 $y=0$ 得 $f\left(x\right)=f'\left(x\right)$ ($\forall{}x\in{}X$), 故 $f=f'$; 取 $x=0$ 得 $g\left(y\right)=g'\left(y\right)$ ($\forall{}y\in{}Y$), 故 $g=g'$.

$\blacksquare$

保范性. 一方面,

$$
\left|F\left(x,y\right)\right|\le\left|f\left(x\right)\right|+\left|g\left(y\right)\right|\le\left\|f\right\|+\left\|g\right\|,
$$

故 $\left\|F\right\|\le\left\|f\right\|+\left\|g\right\|$. 另一方面任给 $\varepsilon>0$: 若 $f\neq0$, 取向量 $u\in{}X$ 满足 $\left\|u\right\|=1$, 使 $|f\left(u\right)|>\left\|f\right\|-\varepsilon$; 同法取 $v\in{}Y$ 使 $|g\left(v\right)|>\left\|g\right\|-\varepsilon$. 于是

$$
\left\|F\right\|\ge\left|F\left(u,v\right)\right|=\left|f\left(u\right)+g\left(v\right)\right|>\left\|f\right\|+\left\|g\right\|-2\varepsilon,
$$

令 $\varepsilon\to0$ 得 $\left\|F\right\|\ge\left\|f\right\|+\left\|g\right\|$. 故 $\left\|F\right\|=\left\|f\right\|+\left\|g\right\|$.

$\blacksquare$

映射 $F\mapsto\left(f,g\right)$ 的线性性显然. 结合存在唯一性与保范性, 该映射是线性双射且保范, 从而是 $\left(X\times{}Y\right)^{*}$ 到 $X^{*}\times{}Y^{*}$ 的保范线性同构.

$\blacksquare$

(ii) 设 $f_i\in{}X_i^{*}$ ($i=1,2$), $F=f_1+f_2$, 其中 $\left\|f_i\right\|_i$ 表示 $f_i$ 在 $X_i^{*}$ 中的范数. 对任意 $x\in{}X$, 用柯西-施瓦茨不等式,

$$
\begin{aligned}
&\quad\;\left|F\left(x\right)\right|\le\left|f_1\left(x\right)\right|+\left|f_2\left(x\right)\right|\le\left\|f_1\right\|_1\left\|x\right\|_1+\left\|f_2\right\|_2\left\|x\right\|_2\\
&\le\left(\left\|f_1\right\|_1^2+\left\|f_2\right\|_2^2\right)^{\frac12}\left(\left\|x\right\|_1^2+\left\|x\right\|_2^2\right)^{\frac12}=\left(\left\|f_1\right\|_1^2+\left\|f_2\right\|_2^2\right)^{\frac12}\left\|x\right\|,
\end{aligned}
$$

易证 $F$ 线性, 上式知 $F$ 有界, 故 $F\in\left(X,\left\|\cdot\right\|\right)^{*}$.

$\blacksquare$

## 2.3-4 (无穷维空间的对偶空间仍无穷维)

对于赋范线性空间 $X$, 证明: $X$ 是无穷维空间当且仅当 $X^{*}$ 是无穷维空间.

### 解答 2.3-4

由于 $X$ 是有限维空间蕴含 $X^{*}$ 也是有限维空间, 则其逆否命题给出: $X^{*}$ 无穷维蕴含 $X$ 无穷维.

$\blacksquare$

设 $X$ 无穷维, 取 $X$ 中线性无关序列 $x_1,x_2,\cdots$, 令 $M_0=\left\{0\right\}$, $M_n=\operatorname{span}\left\{x_1,\cdots,x_n\right\}$ ($n\ge1$). 由**定理 1.4.2 (有限维赋范线性空间完备)**, $M_n$ 完备; 而完备子集是闭集, 故 $M_n$ 是 $X$ 的闭线性子空间. 因 $x_{n+1}\notin{}M_n$, 由**推论 2.3.4 (闭线性子空间与点的分离)**, 存在 $f_{n+1}\in{}X^{*}$, 使 $\left\|f_{n+1}\right\|=1$, $f_{n+1}\left(M_n\right)=0$, $f_{n+1}\left(x_{n+1}\right)=d\left(x_{n+1},M_n\right)>0$. 特别地 $f_j\left(x_i\right)=0$ ($i<{}j$), $f_j\left(x_j\right)>0$ ($j\ge1$).

任给 $n\ge1$, 设 $\sum_{j=1}^{n}c_jf_j=0$. 依次用 $x_1,\cdots,x_n$ 作用于两端. 由 $f_j\left(x_i\right)=0$ ($i<{}j$) 与 $f_j\left(x_j\right)>0$ ($j\ge1$),

$$
0=\left(\sum_{j=1}^{n}c_jf_j\right)\left(x_1\right)=c_1f_1\left(x_1\right),
$$

故 $c_1=0$; 再用 $x_2$ 作用于两端, 由 $c_1=0$ 与 $f_j\left(x_2\right)=0$ ($j\ge3$) 得 $0=c_2f_2\left(x_2\right)$, 故 $c_2=0$; 如此下去得 $c_1=\cdots=c_n=0$. 因此 $f_1,\cdots,f_n$ 线性无关. 因 $n$ 任意, $X^{*}$ 是无穷维空间.

$\blacksquare$

> 线性空间 $Y$ 无穷维的等价定义: 对任意正整数 $n$, 都能在 $Y$ 里找到至少 $n$ 个线性无关的向量.

## 2.3-5 (算子空间的完备性传递给值域)

设 $X,Y$ 是两个赋范线性空间. 证明: 若 $X\neq\left\{0\right\}$, 并且 $\mathfrak{B}\left(X,Y\right)$ 是巴拿赫空间, 则 $Y$ 必是巴拿赫空间.

### 解答 2.3-5

取 $x_0\in{}X$, $x_0\neq0$. 由**推论 2.3.1 (范数可达的泛函)**, 存在 $f\in{}X^{*}$, $\left\|f\right\|=1$, $f\left(x_0\right)=\left\|x_0\right\|$. 令 $f_1=f/\left\|x_0\right\|$, 则 $f_1\in{}X^{*}$, $f_1\left(x_0\right)=1$, $\left\|f_1\right\|=1/\left\|x_0\right\|$.

设 $\left\{y_n\right\}$ 是 $Y$ 中的基本列. 对每个 $n$, 令 $T_nx=f_1\left(x\right)y_n$ ($x\in{}X$). 则 $T_n$ 线性, 且由**定义 2.1.2 (算子范数)** 中的估计,

$$
\left\|T_nx\right\|=\left|f_1\left(x\right)\right|\left\|y_n\right\|\le\left\|f_1\right\|\left\|y_n\right\|\left\|x\right\|,
$$

故 $T_n\in\mathfrak{B}\left(X,Y\right)$, $\left\|T_n\right\|\le\left\|f_1\right\|\left\|y_n\right\|$; 于是 $\left\|T_n-T_m\right\|\le\left\|f_1\right\|\left\|y_n-y_m\right\|$, $\left\{T_n\right\}$ 是 $\mathfrak{B}\left(X,Y\right)$ 中的基本列.

由 $\mathfrak{B}\left(X,Y\right)$ 完备, 存在 $T\in\mathfrak{B}\left(X,Y\right)$ 使 $\left\|T_n-T\right\|\to0$. 由 $f_1\left(x_0\right)=1$ 得 $y_n=T_nx_0$, 故

$$
\left\|y_n-y\right\|:=\left\|y_n-Tx_0\right\|=\left\|T_nx_0-Tx_0\right\|\le\left\|T_n-T\right\|\left\|x_0\right\|\to0,
$$

即 $\left\{y_n\right\}$ 收敛于 $y\in{}Y$. 因此 $Y$ 中每个基本列都收敛, $Y$ 是巴拿赫空间.

$\blacksquare$

## 2.3-6 ($l^{\infty}$ 值算子的保范延拓)

设 $L$ 是赋范线性空间 $X$ 的子空间, $T\in\mathfrak{B}\left(L,l^{\infty}\right)$, 证明: 存在线性延拓 $\widetilde{T}\in\mathfrak{B}\left(X,l^{\infty}\right)$, 使得 $\widetilde{T}|_L=T$ 且 $\left\|\widetilde{T}\right\|=\left\|T\right\|$.

### 解答 2.3-6

将 $l^\infty$ 中每个元 $y$ 中的第 $i$ 个元素看作 $\mathbb{K}$ 中的元素, 则对每个 $L\to\mathbb{K}$ 使用**定理 2.3.1 (哈恩-巴拿赫延拓定理)**, 再拼接得到 $l^\infty$ 中元素, 则的确存在线性延拓 $\widetilde{T}\in\mathfrak{B}\left(X,l^{\infty}\right)$, 使得 $\widetilde{T}|_L=T$ 且 $\left\|\widetilde{T}\right\|=\left\|T\right\|$.

$\blacksquare$

## 2.3-11 ($l^{1}$ 给出的 $l^{\infty}$ 上的泛函及其不可表示性)

对于任意的 $\alpha=\left(\alpha_1,\alpha_2,\cdots\right)\in{}l^1$, 证明:

$$
f\left(x\right)=\sum_{n=1}^{\infty}x_n\alpha_n,\quad\forall{}x=\left(x_1,x_2,\cdots\right)\in{}l^{\infty}
$$

给出了 $l^{\infty}$ 上的一个连续线性泛函. 举例说明 $l^{\infty}$ 上存在连续线性泛函不能表示成上述形式.

### 解答 2.3-11

对每个 $n$, $\left|x_n\alpha_n\right|\le\left\|x\right\|_{l^\infty}\left|\alpha_n\right|$, 而 $\sum_{n=1}^{\infty}\left|\alpha_n\right|=\left\|\alpha\right\|_1<\infty$, 故级数 $\sum_{n=1}^{\infty}x_n\alpha_n$ 绝对收敛. 由级数的线性运算, $f$ 是 $l^{\infty}$ 上的线性泛函; 且

$$
\left|f\left(x\right)\right|\le\sum_{n=1}^{\infty}\left|x_n\right|\left|\alpha_n\right|\le\left\|x\right\|_{l^\infty}\left\|\alpha\right\|_1,
$$

故 $f$ 连续, $\left\|f\right\|\le\left\|\alpha\right\|_1$.

$\blacksquare$

令 $M=\left\{x\in{}l^{\infty}:\lim_{n\to\infty}x_n=0\right\}$, $x_0=\left(1,1,\cdots\right)$, 则 $M$ 是 $l^{\infty}$ 的闭线性子空间. 对任意 $x\in{}M$,

$$
\left\|x_0-x\right\|_{l^\infty}=\sup_{n\ge1}\left|1-x_n\right|\ge\lim_{n\to\infty}\left|1-x_n\right|=1,
$$

而取 $x=0\in{}M$ 得 $\left\|x_0\right\|=1$, 故 $d\left(x_0,M\right)=1$. 由**推论 2.3.4 (闭线性子空间与点的分离)**, 存在 $f\in\left(l^{\infty}\right)^{*}$, 使 $\left\|f\right\|=1$, $f\left(M\right)=0$, $f\left(x_0\right)=1$. 特别地, 对每个 $n$, 因 $e_n\in{}M$, 有 $f\left(e_n\right)=0$.

若存在 $\alpha\in{}l^1$ 使 $f\left(x\right)=\sum_{n=1}^{\infty}x_n\alpha_n$ ($\forall{}x\in{}l^{\infty}$), 则在该式中取 $x=e_n$ 得 $\alpha_n=f\left(e_n\right)=0$ ($\forall{}n$), 故 $\alpha=0$, 从而 $f=0$, 与 $f\left(x_0\right)=1$ 矛盾. 所以这个 $f$ 不能表示成上述形式.

$\blacksquare$

## 2.3-12 (格林函数)

令 $\Delta=\frac{\partial^2}{\partial{}x^2}+\frac{\partial^2}{\partial{}y^2}$. 设 $\Omega$ 是平面上的有界开区域, 它的边界 $\partial\Omega$ 是光滑的. 对于带有狄利克雷边界值条件的拉普拉斯方程

$$
\begin{cases}\Delta{}u\left(x\right)=0,&x\in\Omega,\\u|_{\partial\Omega}=f,\end{cases}
$$

一个重要的解法是寻找 $\overline{\Omega}$ 上的一类格林函数 $G\left(x,y\right)$, 使得

$$
\int_{\Omega}h\left(x\right)G\left(x,y\right)\mathrm{d}m\left(x\right)=h\left(y\right);\quad{}G\left(x,y\right)=0,\quad\forall{}y\in\partial\Omega.
$$

令 $B=C\left(\partial\Omega\right)$ 是 $\partial\Omega$ 上连续函数全体. 设 $B_0=\left\{g\in{}B:\Delta{}u\left(x\right)=0,u|_{\partial\Omega}=g\;\text{有解}\right\}$, 由调和函数的极大模定理容易得到, 对于 $g\in{}B_0$ 解 $u$ 是唯一的. 对于 $P\in\Omega$, 定义 $B_0$ 上的线性泛函 $l_P$ 如下:

$$
l_P\left(g\right)=u\left(P\right),
$$

这里 $u$ 是边值为 $g$ 的调和函数.

(i) 证明: $l_P$ 是一个有界线性泛函, 计算其范数.

(ii) 证明: $l_P$ 可以保范地延拓到整个 $B$ 上.

我们仍然用 $l_P$ 来表示这个延拓. 对任意一点 $\left(a,b\right)\notin\partial\Omega$, 考虑 $B$ 中的函数

$$
\psi_{\left(a,b\right)}\left(x,y\right)=\ln{}d\left(\left(a,b\right),\left(x,y\right)\right).
$$

这里 $d\left(\left(a,b\right),\left(x,y\right)\right)=\sqrt{\left(a-x\right)^2+\left(b-y\right)^2}$ 为欧氏空间度量.

(iii) 证明: $\psi$ 关于变量 $\left(a,b\right)$ 满足拉普拉斯方程 $\frac{\partial^2\psi}{\partial{}a^2}+\frac{\partial^2\psi}{\partial{}b^2}=0$.

(iv) 令 $k_P\left(\left(a,b\right)\right)=\frac{1}{2\pi}l_P\left(\psi_{\left(a,b\right)}\right)$. 证明: $k_P\left(\left(a,b\right)\right)$ 在 $\partial\Omega$ 的补集上是调和函数.

(v) 当 $\left(a,b\right)\notin\overline{\Omega}$ 即在 $\Omega$ 外时, 计算 $k_P\left(\left(a,b\right)\right)$.

对于 $\Omega$ 中离边界足够近的点 $Q=\left(a,b\right)$, 我们承认: $Q$ 关于边界上到它最近的那一点处的切线的对称点 $Q'$ 在 $\Omega$ 外. 并且当 $Q$ 到边界的距离趋于 $0$ 时,

$$
\frac{d\left(z,Q\right)}{d\left(z,Q'\right)}
$$

在 $z\in\partial\Omega$ 上是一致趋于 $1$ 的 (这一结论来自边界 $\partial\Omega$ 是光滑的).

(vi) 证明: 当 $Q$ 到边界的距离趋于 $0$ 时, $\left\|\psi_Q-\psi_{Q'}\right\|$ 趋于 $0$, 且 $k_P\left(Q\right)-k_P\left(Q'\right)$ 趋于 $0$.

(vii) 证明: $k_P\left(Q\right)$ 是一个 $\Omega$ 上的调和函数, 并且在 $\overline{\Omega}$ 上连续, 在边界上的值为 $\frac{1}{2\pi}\ln{}d\left(P,Q\right)$.

实际上, 由边界的光滑性我们能得到 $k_P\left(Q\right)$ 在 $\overline{\Omega}$ 上二阶连续可微. 记 $g_0\left(P,Q\right)=k_P\left(Q\right)$, 令

$$
G\left(P,Q\right)=-\frac{1}{2\pi}\ln{}d\left(P,Q\right)+g_0\left(P,Q\right).
$$

(viii) 若 $h$ 在 $\overline{\Omega}$ 上二阶连续可微, 且在 $\Omega$ 内 $\Delta{}h=0$, 证明: $h\left(P\right)=\int_{\partial\Omega}h\left(Q\right)\frac{\partial{}G\left(P,Q\right)}{\partial{}n}\mathrm{d}Q$ ($\forall{}P\in\Omega$), 其中 $\frac{\partial{}G}{\partial{}n}$ 是沿外法线方向的方向导数.

### 解答 2.3-12

按**定义 2.4.1 (凸集)**, (i) 有界性. 由调和函数的极大模原理, $\left|u\left(P\right)\right|\le\max_{z\in\partial\Omega}\left|u\left(z\right)\right|=\left\|g\right\|_{C\left(\partial\Omega\right)}$, 故

$$
\left|l_P\left(g\right)\right|\le\left\|g\right\|,\quad\forall{}g\in{}B_0,
$$

即 $l_P$ 有界, $\left\|l_P\right\|\le1$.

$\blacksquare$

计算范数. 取 $g\equiv1$, 则 $g\in{}B_0$, 其解为 $u\equiv1$. 于是 $\left\|g\right\|=1$, $l_P\left(g\right)=1$, 故 $\left\|l_P\right\|\ge1$. 结合上面的结果得 $\left\|l_P\right\|=1$.

$\blacksquare$

(ii) $B=C\left(\partial\Omega\right)$ 按上确界范数是赋范线性空间, $B_0$ 是它的线性子空间. 由 (i), $l_P$ 是 $B_0$ 上的有界线性泛函. 由**定理 2.3.1 (哈恩-巴拿赫延拓定理)**, 存在 $B$ 上的有界线性泛函 $l_P$ 使 $l_P|_{B_0}$ 等于原来的 $l_P$ 且 $\left\|l_P\right\|=1$, 即 $l_P$ 保范地延拓到整个 $B$ 上.

$\blacksquare$

(iii) 对 $r^2=\left(a-x\right)^2+\left(b-y\right)^2$, 当 $r>0$ 时,

$$
\frac{\partial\psi}{\partial{}a}=\frac{a-x}{r^2},\quad\frac{\partial^2\psi}{\partial{}a^2}=\frac{r^2-2\left(a-x\right)^2}{r^4},
$$

$$
\frac{\partial\psi}{\partial{}b}=\frac{b-y}{r^2},\quad\frac{\partial^2\psi}{\partial{}b^2}=\frac{r^2-2\left(b-y\right)^2}{r^4}.
$$

两式相加, 分子为 $2r^2-2\left[\left(a-x\right)^2+\left(b-y\right)^2\right]=0$, 故

$$
\frac{\partial^2\psi}{\partial{}a^2}+\frac{\partial^2\psi}{\partial{}b^2}=0,\quad\forall\left(a,b\right)\neq\left(x,y\right).
$$

$\blacksquare$

(iv)

$$
\frac{\partial^2k_P}{\partial{}a^2}=\frac{1}{2\pi}l_P\left(\frac{\partial^2\psi_{\left(a,b\right)}}{\partial{}a^2}\right),\quad\frac{\partial^2k_P}{\partial{}b^2}=\frac{1}{2\pi}l_P\left(\frac{\partial^2\psi_{\left(a,b\right)}}{\partial{}b^2}\right).
$$

两式相加, 由 (iii) 与 $l_P$ 的线性,

$$
\Delta_{\left(a,b\right)}k_P=\frac{1}{2\pi}l_P\left(\frac{\partial^2\psi_{\left(a,b\right)}}{\partial{}a^2}+\frac{\partial^2\psi_{\left(a,b\right)}}{\partial{}b^2}\right)=\frac{1}{2\pi}l_P\left(0\right)=0.
$$

$\blacksquare$

(v) 设 $\left(a,b\right)\notin\overline{\Omega}$. 则对 $z\in\overline{\Omega}$ 有 $z\neq\left(a,b\right)$, 由 (iii) $\psi_{\left(a,b\right)}$ 在 $\overline{\Omega}$ 上调和. 于是 $\psi_{\left(a,b\right)}|_{\partial\Omega}\in{}B_0$, 且边值为 $\psi_{\left(a,b\right)}|_{\partial\Omega}$ 的狄利克雷问题的解就是 $\psi_{\left(a,b\right)}$ 本身 (由 $B_0$ 上解的唯一性). 故由延拓后的 $l_P$ 在 $B_0$ 上的取值,

$$
k_P\left(\left(a,b\right)\right)=\frac{1}{2\pi}l_P\left(\psi_{\left(a,b\right)}\right)=\frac{1}{2\pi}\psi_{\left(a,b\right)}\left(P\right)=\frac{1}{2\pi}\ln{}d\left(P,\left(a,b\right)\right).
$$

$\blacksquare$

(vi) 由所承认的一致收敛, 当 $Q$ 到 $\partial\Omega$ 的距离趋于 $0$ 时,

$$
\left\|\psi_Q-\psi_{Q'}\right\|_{C\left(\partial\Omega\right)}=\sup_{z\in\partial\Omega}\left|\ln\frac{d\left(z,Q\right)}{d\left(z,Q'\right)}\right|\to0,
$$

因 $\frac{d\left(z,Q\right)}{d\left(z,Q'\right)}$ 在 $\partial\Omega$ 上一致趋于 $1$, 且 $\ln$ 在 $\left[\frac12,2\right]$ 上一致连续.

$\blacksquare$

又

$$
k_P\left(Q\right)-k_P\left(Q'\right)=\frac{1}{2\pi}l_P\left(\psi_Q-\psi_{Q'}\right),
$$

故 $\left|k_P\left(Q\right)-k_P\left(Q'\right)\right|\le\frac{1}{2\pi}\left\|l_P\right\|\left\|\psi_Q-\psi_{Q'}\right\|=\frac{1}{2\pi}\left\|\psi_Q-\psi_{Q'}\right\|\to0$.

$\blacksquare$

(vii)

连续性与边界值. 设 $Q_n\in\Omega$, $Q_n\to{}Q_0\in\partial\Omega$, 并设 $Q_n$ 按所承认的方式配对称点 $Q_n'\notin\overline{\Omega}$. 当 $Q_n\to{}Q_0$ 时最近点趋于 $Q_0$, 且 $Q_n$ 到边界的距离趋于 $0$, 故 $Q_n'\to{}Q_0$. 由 (v),

$$
k_P\left(Q_n'\right)=\frac{1}{2\pi}\ln{}d\left(P,Q_n'\right)\to\frac{1}{2\pi}\ln{}d\left(P,Q_0\right),
$$

又由 (vi), $k_P\left(Q_n\right)-k_P\left(Q_n'\right)\to0$, 故

$$
\lim_{n\to\infty}k_P\left(Q_n\right)=\frac{1}{2\pi}\ln{}d\left(P,Q_0\right).
$$

该极限只与 $Q_0$ 有关而与 $\left\{Q_n\right\}$ 的取法无关, 故 $k_P$ 在 $\Omega$ 上连续并可连续延拓到 $\overline{\Omega}$, 在 $\partial\Omega$ 上的值为 $\frac{1}{2\pi}\ln{}d\left(P,Q\right)$.

$\blacksquare$

(viii) 记 $\nu$ 为 $\partial\Omega$ 的单位外法向量, 并约定边界上的 $\frac{\partial}{\partial\nu}$ 由 $\Omega$ 内侧取极限; $\mathrm{d}s$ 为边界弧长元. 在边界上由 (vii),

$$
G\left(P,Q\right)=-\frac{1}{2\pi}\ln{}d\left(P,Q\right)+\frac{1}{2\pi}\ln{}d\left(P,Q\right)=0,\quad\forall{}Q\in\partial\Omega.
$$

固定 $P\in\Omega$ 与 $\varepsilon>0$ 使闭球 $\overline{B\left(P,\varepsilon\right)}\subset\Omega$, 记 $\Omega_\varepsilon=\Omega\setminus\overline{B\left(P,\varepsilon\right)}$. 在 $\Omega_\varepsilon$ 上 $h$ 与 $G\left(P,\cdot\right)$ 都二阶连续可微且 $\Delta{}h=0$; 又 $G\left(P,\cdot\right)$ 在 $\Omega_\varepsilon$ 上调和 (由 (vii) $k_P$ 在 $\Omega$ 上调和, 而 $-\frac{1}{2\pi}\ln{}d\left(P,\cdot\right)$ 在 $Q\neq{}P$ 处调和). 对 $h$ 与 $G\left(P,\cdot\right)$ 在 $\Omega_\varepsilon$ 上用格林第二公式,

$$
\int_{\Omega_\varepsilon}\left(h\Delta{}G-G\Delta{}h\right)\mathrm{d}m=\int_{\partial\Omega_\varepsilon}\left(h\frac{\partial{}G}{\partial\nu}-G\frac{\partial{}h}{\partial\nu}\right)\mathrm{d}s,
$$

左端被积函数恒为 $0$, 故左端为 $0$. 而 $\partial\Omega_\varepsilon=\partial\Omega\cup\partial{}B\left(P,\varepsilon\right)$, 在 $\partial\Omega$ 上 $G\left(P,\cdot\right)=0$, 于是

$$
0=\int_{\partial\Omega}h\frac{\partial{}G}{\partial\nu}\mathrm{d}s+\int_{\partial{}B\left(P,\varepsilon\right)}\left(h\frac{\partial{}G}{\partial\nu}-G\frac{\partial{}h}{\partial\nu}\right)\mathrm{d}s.
$$

在 $\partial{}B\left(P,\varepsilon\right)$ 上, $\nu$ 指向球心 $P$, 即 $\nu=-\frac{Q-P}{\left|Q-P\right|}$, 且 $r=\left|Q-P\right|=\varepsilon$. 由 $G\left(P,Q\right)=-\frac{1}{2\pi}\ln{}r+k_P\left(Q\right)$ 与 $k_P$ 二阶连续可微,

$$
\frac{\partial{}G}{\partial\nu}=\frac{1}{2\pi{}r}+\frac{\partial{}k_P}{\partial\nu},\quad\left|G\left(P,Q\right)\right|\le\frac{1}{2\pi}\left|\ln{}r\right|+C,
$$

其中 $C=\sup_{\overline{\Omega}}\left|k_P\right|$. 于是

$$
\int_{\partial{}B\left(P,\varepsilon\right)}h\frac{\partial{}G}{\partial\nu}\mathrm{d}s=\frac{1}{2\pi\varepsilon}\int_{\partial{}B\left(P,\varepsilon\right)}h\,\mathrm{d}s+\int_{\partial{}B\left(P,\varepsilon\right)}h\frac{\partial{}k_P}{\partial\nu}\mathrm{d}s.
$$

因 $h$ 在 $P$ 连续, 圆周平均值 $\frac{1}{2\pi\varepsilon}\int_{\partial{}B\left(P,\varepsilon\right)}h\,\mathrm{d}s\to{}h\left(P\right)$; 而 $\left|\frac{\partial{}k_P}{\partial\nu}\right|\le{}M_1$, 故第二项满足 $\left|\int_{\partial{}B\left(P,\varepsilon\right)}h\frac{\partial{}k_P}{\partial\nu}\mathrm{d}s\right|\le2\pi\varepsilon\max_{\overline{\Omega}}\left|h\right|{M}_1\to0$. 又

$$
\left|\int_{\partial{}B\left(P,\varepsilon\right)}G\frac{\partial{}h}{\partial\nu}\mathrm{d}s\right|\le2\pi\varepsilon\left(\frac{\left|\ln\varepsilon\right|}{2\pi}+C\right)\max_{\overline{\Omega}}\left|\nabla{}h\right|\to0.
$$

于是 $0=\int_{\partial\Omega}h\frac{\partial{}G}{\partial\nu}\mathrm{d}s+h\left(P\right)$, 即

$$
h\left(P\right)=-\int_{\partial\Omega}h\left(Q\right)\frac{\partial{}G\left(P,Q\right)}{\partial\nu}\mathrm{d}s,\quad\forall{}P\in\Omega.
$$

$\blacksquare$

## 2.4-1 (闭集的凸包与凸集的凸包)

在欧氏空间 $\mathbb{R}^{n}$ 中, 闭集的凸包是否一定是闭集? 凸集的凸包是否一定是凸集?

### 解答 2.4-1

闭集的凸包不一定是闭集. 在 $\mathbb{R}^2$ 中取

$$
A=\left\{\left(x,y\right):x>0,y\ge\frac1x\right\}\cup\left\{\left(0,0\right)\right\}.
$$

易证 $A$ 闭.

下证 $\left(0,1\right)\in\overline{\operatorname{co}\left(A\right)}$, 但 $\left(0,1\right)\not\in\operatorname{co}\left(A\right)$. 对 $t\in\left(0,1\right]$, $t\left(t,\frac1t\right)+\left(1-t\right)\left(0,0\right)=\left(t^2,1\right)\in\operatorname{co}\left(A\right)$, 令 $t\to0^+$ 得 $\left(0,1\right)$ 是 $\operatorname{co}\left(A\right)$ 的聚点, 故 $\left(0,1\right)\in\overline{\operatorname{co}\left(A\right)}$; 若 $x=0$, 则 $y=0\ne1$. 故 $\left(0,1\right)\notin\operatorname{co}\left(A\right)$, $\operatorname{co}\left(A\right)$ 不是闭集.

$\blacksquare$

凸集的凸包就是它自己, 所以一定是凸集.

$\blacksquare$

## 2.4-2 (超平面与半空间的凸性, 闭性与开性)

设 $f$ 是实赋范线性空间 $V$ 上的线性泛函, $c$ 为实数. 证明:

(i) 超平面 $V_c\left(f\right)=\left\{x:f\left(x\right)=c\right\}$ 和它决定的半空间 $\left\{x:f\left(x\right)\ge{}c\right\}$, $\left\{x:f\left(x\right)\le{}c\right\}$, $\left\{x:f\left(x\right)>c\right\}$, $\left\{x:f\left(x\right)<{}c\right\}$ 都是凸集.

(ii) 当 $f$ 连续时, $\left\{x:f\left(x\right)\ge{}c\right\}$, $\left\{x:f\left(x\right)\le{}c\right\}$ 是闭的, $\left\{x:f\left(x\right)>c\right\}$, $\left\{x:f\left(x\right)<{}c\right\}$ 是开的.

(iii) $V_c\left(f\right)$ 和半空间中任一个具有内点时, $f$ 是连续的.

### 解答 2.4-2

按**定义 2.4.2 (闵可夫斯基泛函)**, (i) 设 $x,y$ 属于 $V_c\left(f\right)$, $t\in\left[0,1\right]$. 由 $f$ 的线性, $f\left(tx+\left(1-t\right)y\right)=tf\left(x\right)+\left(1-t\right)f\left(y\right)=tc+\left(1-t\right)c=c$, 故 $tx+\left(1-t\right)y\in{}V_c\left(f\right)$, 即 $V_c\left(f\right)$ 凸; 同法, 把 $=$ 换成不等号时, 由 $tf\left(x\right)+\left(1-t\right)f\left(y\right)$ 的相应不等式仍得结论. 故四个半空间都是凸集.

$\blacksquare$

(ii) 设 $f$ 连续. 则 $\left\{x:f\left(x\right)\ge{}c\right\}=f^{-1}\left(\left[c,+\infty\right)\right)$, $\left\{x:f\left(x\right)\le{}c\right\}=f^{-1}\left(\left(-\infty,c\right]\right)$ 是闭区间的原像, 故闭; $\left\{x:f\left(x\right)>c\right\}=f^{-1}\left(\left(c,+\infty\right)\right)$, $\left\{x:f\left(x\right)<{}c\right\}=f^{-1}\left(\left(-\infty,c\right)\right)$ 是开区间的原像, 故开.

$\blacksquare$

(iii) 先设半空间 $\left\{x:f\left(x\right)\ge{}c\right\}$ 有内点 $x_0$, 即存在 $\rho>0$ 使 $B\left(x_0,\rho\right)\subset\left\{x:f\left(x\right)\ge{}c\right\}$. 任给 $u\in{}V$, $\left\|u\right\|<\rho$, 则 $x_0+u$ 与 $x_0-u$ 都属于该半空间, 故 $f\left(x_0\right)+f\left(u\right)\ge{}c$ 且 $f\left(x_0\right)-f\left(u\right)\ge{}c$, 即

$$
\left|f\left(u\right)\right|\le{}f\left(x_0\right)-c,\quad\forall{}u\in{}B\left(0,\rho\right).
$$

故 $f$ 在原点邻域内有界, 从而 $f$ 连续.

$\blacksquare$

对 $\left\{x:f\left(x\right)\le{}c\right\}$ 有内点的情形, 把 $f$ 换成 $-f$ 即可; 对 $\left\{x:f\left(x\right)>c\right\}$ 有内点的情形, 由 $x_0\pm{}u$ 属于该半空间得 $f\left(x_0\right)+f\left(u\right)>c$ 与 $f\left(x_0\right)-f\left(u\right)>c$, 同样得 $\left|f\left(u\right)\right|\le{}f\left(x_0\right)-c$ ($\left\|u\right\|<\rho$), 故 $f$ 连续; 对 $\left\{x:f\left(x\right)<{}c\right\}$ 有内点的情形再用 $-f$ 归结.

$\blacksquare$

最后设 $V_c\left(f\right)$ 有内点 $x_0$, 即存在 $\rho>0$ 使 $B\left(x_0,\rho\right)\subset{}V_c\left(f\right)$. 则对 $\left\|u\right\|<\rho$, $f\left(x_0+u\right)=f\left(x_0-u\right)=c$, 相减得 $f\left(u\right)=0$. 于是 $f$ 在 $B\left(0,\rho\right)$ 上恒为 $0$, 故 $f$ 连续.

$\blacksquare$

## 2.4-3 (吸收闭凸集的闵可夫斯基泛函)

设 $V$ 是实赋范线性空间, $M$ 是 $V$ 的吸收闭凸集, 那么 $0\in{}M$. 如果 $p\left(x\right)$ 是 $M$ 的闵可夫斯基泛函, 那么 $p\left(x\right)$ 是下半连续的, 且有 $M=\left\{x\in{}X:p\left(x\right)\le1\right\}$. 此外, 如果 $M$ 还是有界的, 那么 $p\left(x\right)$ 满足 $p\left(x\right)=0\Leftrightarrow{}x=0$.

### 解答 2.4-3

由 $M$ 吸收, 对 $x=0$ 存在 $\alpha>0$ 使 $\alpha^{-1}0=0\in{}M$, 故 $0\in{}M$.

$\blacksquare$

由**命题 2.4.3 (吸收凸集的闵可夫斯基泛函)**, $p$ 是 $V$ 上的次线性泛函, 且

$$
\left\{x:p\left(x\right)<1\right\}\subset{}M\subset\left\{x:p\left(x\right)\le1\right\}.
$$

$\blacksquare$

再证引理 $\left\{x:p\left(x\right)\le\lambda\right\}=\lambda{}M$ ($\lambda>0$). 若 $x\in\lambda{}M$, 即 $x=\lambda{}y$, $y\in{}M$, 由 $p$ 的正齐次性与 $M\subset\left\{x:p\left(x\right)\le1\right\}$,

$$
p\left(x\right)=p\left(\lambda{}y\right)=\lambda{}p\left(y\right)\le\lambda.
$$

反之设 $p\left(x\right)\le\lambda$. 由 $p$ 的定义, 对每个 $n$ 存在 $\alpha_n>p\left(x\right)$ 使 $\alpha_n^{-1}x\in{}M$, 且可取 $\alpha_n<\lambda+1/n$ (因 $p\left(x\right)\le\lambda$). 于 $n\to\infty$, $\frac{x}{\lambda+1/n}\to\frac{x}{\lambda}$, 由 $M$ 闭得 $\frac{x}{\lambda}\in{}M$, 即 $x\in\lambda{}M$.

$\blacksquare$

下水平集闭. 对 $\lambda>0$, 上面的等式给出 $\left\{x:p\left(x\right)\le\lambda\right\}=\lambda{}M$, 而 $\lambda{}M$ 是闭集 $M$ 的伸缩, 故闭. 对 $\lambda=0$, $\left\{x:p\left(x\right)=0\right\}=\bigcap_{k=1}^{\infty}\left\{x:p\left(x\right)\le\frac1k\right\}=\bigcap_{k=1}^{\infty}\frac1k{M}$ 是闭集之交, 故闭. 由下半连续的定义, $p$ 下半连续当且仅当对每个实数 $\lambda$, $\left\{x:p\left(x\right)\le\lambda\right\}$ 闭; 故 $p$ 下半连续.

$\blacksquare$

$M=\left\{x:p\left(x\right)\le1\right\}$. 由 $\left\{x:p\left(x\right)\le\lambda\right\}=\lambda{}M$ 取 $\lambda=1$.

$\blacksquare$

设 $M$ 有界, 则存在 $R>0$ 使 $M\subset{}B\left(0,R\right)$. 若 $p\left(x\right)=0$, 则 $\inf\left\{\alpha:\alpha>0,\alpha^{-1}x\in{}M\right\}=0$, 说明对任意的 $\alpha$, $\alpha^{-1}x\in{}M$ 均成立, 故 $x=0$; 反之 $p\left(0\right)=0$ 显然. 于是 $p\left(x\right)=0\Leftrightarrow{}x=0$.

$\blacksquare$

## 2.4-4 (闵可夫斯基泛函与内点, 闭包的关系)

设 $V$ 是实赋范线性空间, $M$ 是 $V$ 的真凸子集, $0\in{}M^{\circ}$, $p\left(x\right)$ 是 $M$ 的闵可夫斯基泛函, 证明:

(i) $x\in{}M^{\circ}\Leftrightarrow{}p\left(x\right)<1$;

(ii) $\overline{M^{\circ}}=\overline{M}$.

### 解答 2.4-4

(i) 设 $x\in{}M^{\circ}$. 若 $x=0$, 则 $p\left(x\right)=p\left(0\right)=0<1$. 若 $x\neq0$, 则存在 $\rho>0$ 使 $B\left(x,\rho\right)\subset{}M$. 取 $\delta=\frac{\rho}{2\left\|x\right\|}>0$, 则 $\left\|\delta{}x\right\|\le\frac\rho2<\rho$, 故 $\left(1+\delta\right)x=x+\delta{}x\in{}M$, 从而由**命题 2.4.3 (吸收凸集的闵可夫斯基泛函)** 中 $M\subset\left\{x:p\left(x\right)\le1\right\}$ 得 $p\left(\left(1+\delta\right)x\right)\le1$; 由 $p$ 的正齐次性, $\left(1+\delta\right)p\left(x\right)\le1$, 即 $p\left(x\right)\le\frac{1}{1+\delta}<1$.

$\blacksquare$

反之设 $p\left(x\right)=\lambda<1$. 取 $\mu$ 使 $\lambda<\mu<1$. 由 $p\left(x/\mu\right)\le\lambda/\mu<1$ 与**命题 2.4.3 (吸收凸集的闵可夫斯基泛函)** 中 $\left\{x:p\left(x\right)<1\right\}\subset{}M$, 得 $x/\mu\in{}M$. 由于 $x$ 放大了还在 $M$ 中, 故 $x\in{}M^{\circ}$.

$\blacksquare$

(ii) 由 $M^{\circ}\subset{}M$ 得 $\overline{M^{\circ}}\subset\overline{M}$. 反之设 $x\in{}M$. 由 (i), 对 $n\ge2$, 取 $x_n=\left(1-\frac1n\right)x$, 则

$$
p\left(x_n\right)\le\left(1-\frac1n\right)p\left(x\right)\le1-\frac1n<1,
$$

故 $x_n\in{}M^{\circ}$; 又 $x_n\to{}x$, 故 $x\in\overline{M^{\circ}}$. 于是 $\overline{M}\subset\overline{M^{\circ}}$, 结合上面的结果得 $\overline{M^{\circ}}=\overline{M}$.

$\blacksquare$
