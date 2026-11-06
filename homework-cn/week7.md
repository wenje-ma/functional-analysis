# week7

> **引理 1.2.3 (柯西-施瓦茨不等式)**
> 
> 对内积空间中任意 $x,y$, 成立 $\left|\left\langle{x},y\right\rangle\right|^2\le\left\langle{x},x\right\rangle\left\langle{y},y\right\rangle$.

> **定理 1.3.2 (标准正交基的等价条件)**
> 
> 设 $\mathfrak{F}=\left\{e_\lambda:\lambda\in\Lambda\right\}$ 是希尔伯特空间 $H$ 中的标准正交系, 下列命题等价:
> 
> (i) 对任意 $x\in{H}$, $x=\sum_{\lambda\in\Lambda}\left\langle{x},e_\lambda\right\rangle{e}_\lambda$;
> 
> (ii) $\overline{\operatorname{span}\left\{e_\lambda:\lambda\in\Lambda\right\}}=H$;
> 
> (iii) $\mathfrak{F}$ 是完全的, 即若 $x\in{H}$ 满足 $x\perp{e}_\lambda$ ($\forall\lambda\in\Lambda$), 则 $x=0$;
> 
> (iv) $\mathfrak{F}$ 是完备的, 即对任意 $x\in{H}$, 帕塞瓦尔等式 $\left\|x\right\|^2=\sum_{\lambda\in\Lambda}\left|\left\langle{x},e_\lambda\right\rangle\right|^2$ 成立.
> 
> 满足上述条件之一的标准正交系称为 $H$ 中的标准正交基.

> **推论 1.3.3 (正交补与稠密性)**
> 
> 设 $H$ 是希尔伯特空间, $M$ 是 $H$ 的线性子空间, 那么 $\overline{M}=\left(M^\perp\right)^\perp$. 特别地, $M^\perp=\left\{0\right\}$ 的充要条件是 $M$ 在 $H$ 中稠密.

> **例 1.3.9 (埃尔米特多项式构成完备正交系)**
> 
> 令 $H_n\left(t\right)=\left(-1\right)^n\mathrm{e}^{t^2}\frac{\mathrm{d}^n}{\mathrm{d}t^n}\mathrm{e}^{-t^2}$ 为埃尔米特多项式, 则 $\psi_n\left(t\right)=\left(2^nn!\sqrt\pi\right)^{-1/2}\mathrm{e}^{-t^2/2}H_n\left(t\right)$ 组成 $L^2\left(\mathbb{R},\mathrm{e}^{-x^2}\mathrm{d}m\left(x\right)\right)$ 中的完备标准正交系.

> **定义 1.4.5 (稠密性)**
> 
> 在度量空间 $\left(X,d\right)$ 中, 对于 $X$ 中一个子集 $A$, 称 $A$ 在 $X$ 中稠密是指 $X\subset\overline{A}$ (即 $\overline{A}=X$).

> **注 1.4.1 ($L^{p}$ 中的稠密子集)**
> 
> (i) $L^p\left(\mathbb{R}^n\right)$ ($1\le{p}<\infty$) 中的简单函数全体, 阶梯函数全体以及 $C_c^\infty\left(\mathbb{R}^n\right)$ 均是稠密子集;
> 
> (ii) 在 $L^\infty\left[a,b\right]$ 中只有简单函数全体稠密.

> **定义 1.4.7 (完备性)**
> 
> (i) 若 $\left\{x_n\right\}$ 满足: 对任意 $\varepsilon>0$, 存在 $N$, 使 $n,m\ge{N}$ 时 $d\left(x_n,x_m\right)<\varepsilon$, 则称 $\left\{x_n\right\}$ 是基本点列 (柯西点列);
> 
> (ii) 若每个基本点列都收敛, 则称 $X$ 完备;
> 
> (iii) 完备赋范线性空间称为巴拿赫空间;
> 
> (iv) 完备内积空间称为希尔伯特空间.

> **例 1.4.13 ($L^{p}\left(E\right)$ 是巴拿赫空间)**
> 
> 设 $E$ 是 $\mathbb{R}^n$ 的勒贝格可测集, 则 $L^p\left(E\right)$ ($1\le{p}<\infty$) 是巴拿赫空间; 特别地, $L^2\left(E\right)$ 是希尔伯特空间.

> **例 2.1.1 (矩阵表示的线性算子)**
> 
> 设 $\mathbb{K}^n$ 是 $n$ 维 (实或复系数) 向量空间, 在 $\mathbb{K}^n$ 中取一组基 $\left\{e_1,e_2,\cdots,e_n\right\}$. 相应于任意一个 $n$ 阶方阵 $\left(t_{ji}\right)$, 作 $\mathbb{K}^n\to\mathbb{K}^n$ 的算子 $T$ 如下: 当 $x=\sum_{i=1}^{n}x_ie_i$ 时, $y=Tx=\sum_{j=1}^{n}y_je_j$, 其中 $y_j=\sum_{i=1}^{n}t_{ji}x_i$ ($j=1,2,\cdots,n$). 这样定义的 $T$ 是一个线性算子, 这个算子在线性代数中称为线性变换. 算子 $T$ 显然由矩阵 $\left(t_{ji}\right)$ 唯一确定, 有时就直接记为 $T=\left(t_{ji}\right)$.

> **例 2.1.6 (傅里叶变换)**
> 
> 对 $f\in{L}^1\left(\mathbb{R}\right)$, 定义它的傅里叶变换 $\mathcal{F}\left(f\right)$ (或记作 $\widehat{f}$) 为
> 
> $$
>\mathcal{F}\left(f\right)\left(t\right)=\int_{\mathbb{R}}f\left(x\right)\mathrm{e}^{-2\pi\mathrm{i}tx}\,\mathrm{d}x,\quad{f}\in{L}^1\left(\mathbb{R}\right).
>$$
> 
> 则 $\widehat{f}$ 是 $\mathbb{R}$ 上的连续函数, 且当 $\left|t\right|\to\infty$ 时 $\widehat{f}\left(t\right)\to0$; 因此 $\mathcal{F}:f\mapsto\widehat{f}$ 是 $L^1\left(\mathbb{R}\right)$ 到 $c_0\left(\mathbb{R}\right)$ 的线性算子.

> **例 2.1.8 (有限维赋范空间上的线性算子连续)**
> 
> 有限维赋范空间中的线性算子是连续算子.

> **例 2.1.9 (微分算子的无界性)**
> 
> 设 $X=C^{\left(1\right)}\left[a,b\right]$, 视 $X$ 为 $C\left[a,b\right]$ 的子空间 (就是说, $X$ 中的范数取为 $C\left[a,b\right]$ 中的范数) 时, $X$ 也成为一个赋范线性空间. 定义算子 $D:X\to{C}\left[a,b\right]$ 如下:
> 
> $$
>\left(Dx\right)\left(t\right)=\frac{\mathrm{d}}{\mathrm{d}t}x\left(t\right),\quad\forall{x}\in{X}.
>$$
> 
> 那么 $D$ 显然是线性算子. $D$ 是无界的: 取 $x_n\left(t\right)=\mathrm{e}^{-n\left(t-a\right)}$, 则 $\left\|x_n\right\|=1$, 但 $\left(Dx_n\right)\left(t\right)=-n\mathrm{e}^{-n\left(t-a\right)}$, 故 $\left\|Dx_n\right\|=n\to\infty$.

> **定理 2.1.1 (线性算子有界与连续的等价条件)**
> 
> 设 $\left(X,\left\|\cdot\right\|\right),\left(Y,\left\|\cdot\right\|\right)$ 是赋范线性空间, $T:X\to{Y}$ 是线性映射, 则下列命题等价:
> 
> (i) $T$ 是连续映射;
> 
> (ii) $T$ 在点 $0$ 连续;
> 
> (iii) 存在 $M>0$, 使得 $\left\|Tx\right\|\le{M}\left\|x\right\|$.
> 
> 如果算子 $T$ 满足定理中任一条件, 就称 $T$ 是有界算子; 否则就称 $T$ 为无界算子.

> **定义 2.1.2 (算子范数)**
> 
> 设 $T$ 为赋范线性空间 $X$ 到赋范线性空间 $Y$ 的有界算子, 称
> 
> $$
>\left\|T\right\|=\sup_{x\neq0}\frac{\left\|Tx\right\|}{\left\|x\right\|}
>$$
> 
> 为算子 $T$ 的范数. 对有界线性算子 $T$, 成立
> 
> $$
>\left\|Tx\right\|\le\left\|T\right\|\left\|x\right\|,\quad\forall{x}\in{X}.
>$$

> **例 2.2.1 (线性泛函的核 (iv))**
> 
> 设 $1\le{q}\le\infty$, $\frac1q+\frac1p=1$. 对于 $\varphi\in{L}^q\left[a,b\right]$, 令
> 
> $$
>{}F_\varphi\left(\psi\right)=\int_{\left[a,b\right]}\psi\left(t\right)\overline{\varphi\left(t\right)}\,\mathrm{d}t,
>$$
> 
> 由赫尔德不等式, $F_\varphi$ 为 $L^p\left[0,1\right]$ 上的有界线性泛函, 且 $\left\|F_\varphi\right\|=\left\|\varphi\right\|_q$. 它的核
> 
> $$
>\ker{F}_\varphi=\left\{\psi\in{L}^p\left[0,1\right]:\,\int_0^1\psi\left(t\right)\overline{\varphi\left(t\right)}\,\mathrm{d}t=0\right\}.
>$$

> **例 2.2.2 (算子导出的共轭双线性泛函)**
> 
> 设 $T$ 是 $H$ 上的线性算子, 则 $T$ 导出的泛函 $\varphi\left(x,y\right)=\left(Tx,y\right)$ 是共轭双线性泛函. 如果 $T$ 还是有界的, 那么 $\varphi$ 也是有界的共轭双线性泛函且 $\left\|\varphi\right\|=\left\|T\right\|$.

> **定理 2.2.1 (线性泛函有界 $\Leftrightarrow$ 核闭)**
> 
> 设 $f$ 是赋范线性空间 $X$ 上的线性泛函, 则 $f$ 有界的充要条件是 $\ker{f}$ 是闭的.

> **定义 2.2.2 (保范算子与同构)**
> 
> 设 $X,Y$ 是两个赋范线性空间, $U$ 是 $X$ 到 $Y$ 的映射.
> 
> (i) 如果对一切 $x\in{X}$, 有 $\left\|Ux\right\|=\left\|x\right\|$, 那么称 $U$ 是 $X$ 到 $Y$ 的保范算子;
> 
> (ii) 如果 $U$ 不但是保范的, 又是线性的, 而且还实现 $X$ 到 $Y$ 上的一一对应, 那么我们就称 $U$ 是 $X$ 到 $Y$ 上的 (保范) 同构映射;
> 
> (iii) 若空间 $X,Y$ 之间存在一个从 $X$ 到 $Y$ 上的 (保范) 同构映射, 就称 $X$ 和 $Y$ 同构, 记为 $X\cong{Y}$.

> **定理 2.2.2 (里斯表示定理)**
> 
> 设 $H$ 是希尔伯特空间, $F$ 是 $H$ 上的连续线性泛函, 那么存在唯一的向量 $y\in{H}$, 使得
> 
> $$
>{}F\left(x\right)=\left\langle{x},y\right\rangle,\quad\forall{x}\in{H},
>$$
> 
> 并且 $\left\|F\right\|=\left\|y\right\|$.

> **定义 2.2.3 (共轭双线性泛函)**
> 
> 设 $H$ 是内积空间, $\varphi\left(x,y\right)$ 是 $H$ 上的二元泛函.
> 
> (i) 如果对于任何 $x,y,z\in{H}$ 及 $\alpha,\beta\in\mathbb{C}$, 都成立
> 
> $$
>\varphi\left(\alpha{x}+\beta{y},z\right)=\alpha\varphi\left(x,z\right)+\beta\varphi\left(y,z\right),\quad\varphi\left(z,\alpha{x}+\beta{y}\right)=\overline\alpha\varphi\left(z,x\right)+\overline\beta\varphi\left(z,y\right),
>$$
> 
> 那么称 $\varphi\left(\cdot,\cdot\right)$ 是 $H$ 上的共轭双线性泛函.
> 
> (ii) 如果对于任何 $x,y\in{H}$ 成立 $\varphi\left(x,y\right)=\overline{\varphi\left(y,x\right)}$, 那么称 $\varphi\left(x,y\right)$ 是 $H$ 上的埃尔米特泛函.
> 
> (iii) 对共轭双线性泛函 $\varphi$, 如果有正常数 $c$ 使得
> 
> $$
>\left|\varphi\left(x,y\right)\right|\le{c}\left\|x\right\|\left\|y\right\|,\quad\forall{x},y\in{H},
>$$
> 
> 那么称 $\varphi$ 是 $H$ 上有界的共轭双线性泛函, $\left\|\varphi\right\|=\sup_{\left\|x\right\|=\left\|y\right\|=1}\left|\varphi\left(x,y\right)\right|$ 称为泛函 $\varphi$ 的范数.

> **定理 2.2.6 (埃尔米特泛函的有界性)**
> 
> 设 $\varphi\left(\cdot,\cdot\right)$ 是复希尔伯特空间 $H$ 上的共轭双线性埃尔米特泛函, 且存在常数 $c$ 使得
> 
> $$
>\left|\varphi\left(x,x\right)\right|\le{c}\left\|x\right\|^2,\quad\forall{x}\in{H},
>$$
> 
> 那么 $\varphi$ 是有界的, 且 $\left\|\varphi\right\|\le{c}$.

## 2.1-1 (零空间闭并不蕴含算子有界)

设 $T$ 是赋范线性空间 $X$ 到赋范线性空间 $Y$ 的线性算子. 如果零空间 $\ker\left(T\right)=\left\{x:Tx=0\right\}$ 是闭集, 问 $T$ 是否有界?

### 解答 2.1-1

不一定. 反例取自**例 2.1.9 (微分算子的无界性)**: 取 $X=C^{\left(1\right)}\left[a,b\right]$ 按 $C\left[a,b\right]$ 的范数 $\left\|x\right\|=\max_{t\in\left[a,b\right]}\left|x\left(t\right)\right|$, $Y=C\left[a,b\right]$, $T=D$, 其中

$$
\left(Dx\right)\left(t\right)=\frac{\mathrm{d}}{\mathrm{d}t}x\left(t\right),\quad{x}\in{X}.
$$

先证 $\ker{D}$ 是 $X$ 的闭集. 由 $Dx=0$ 当且仅当 $x'$ 在 $\left[a,b\right]$ 上恒为 $0$, 而闭区间上导数恒为 $0$ 的函数是常值函数, 故

$$
\ker{D}=\left\{x\in{X}:\,\exists\,c\in\mathbb{R},x\left(t\right)=c,\forall\,t\in\left[a,b\right]\right\}.
$$

设 $\left\{x_n\right\}\subset\ker{D}$ 且 $x_n\to{x}$ 于 $X$, 则 $x_n\equiv{c}=x$, $\forall\,n\in\mathbb{N}$. 故 $x\in\ker{D}$, 即 $\ker{D}$ 闭. $\blacksquare$



再证 $D$ 无界. 取 $x_n\left(t\right)=\mathrm{e}^{-n\left(t-a\right)}$, 则 $\left\|x_n\right\|=\max_t\mathrm{e}^{-n\left(t-a\right)}=1$, 而 $\left(Dx_n\right)\left(t\right)=-n\mathrm{e}^{-n\left(t-a\right)}$, 故 $\left\|Dx_n\right\|=n$ 无界. $\blacksquare$

## 2.1-2 (稠密子空间上算子范数的双变量表示)

设 $E$ 是希尔伯特空间 $H$ 的一个稠密的线性子空间, $T\in\mathfrak{B}\left(H\right)$. 证明:
$$
\left\|T\right\|=\sup\left\{\left|\left\langle{T}x,y\right\rangle\right|:\,x,y\in{E},\left\|x\right\|=\left\|y\right\|=1\right\}.
$$

### 解答 2.1-2

记右端为 $S$.

第一步: $S\le\left\|T\right\|$. 任取 $x,y\in{E}$ 且 $\left\|x\right\|=\left\|y\right\|=1$. 由**引理 1.2.3 (柯西-施瓦茨不等式)**,

$$
\left|\left\langle{T}x,y\right\rangle\right|\le\left\|Tx\right\|\left\|y\right\|=\left\|Tx\right\|,
$$

再由**定义 2.1.2 (算子范数)** 中的 $\left\|Tx\right\|\le\left\|T\right\|\left\|x\right\|$ 得 $\left|\left\langle{T}x,y\right\rangle\right|\le\left\|T\right\|$. 对这样的 $x,y$ 取上确界即得 $S\le\left\|T\right\|$. $\blacksquare$

第二步: $S\ge\left\|T\right\|$. 任给 $\varepsilon>0$. 由**例 2.2.2 (算子导出的共轭双线性泛函)**, $\left\|T\right\|=\sup_{\left\|x\right\|=\left\|y\right\|=1}\left|\left\langle{T}x,y\right\rangle\right|$, 故存在 $x_0,y_0\in{H}$ 满足 $\left\|x_0\right\|=\left\|y_0\right\|=1$ 且

$$
\left|\left\langle{T}x_0,y_0\right\rangle\right|>\left\|T\right\|-\varepsilon.\tag{1}
$$

由 $E$ 在 $H$ 中稠密, 依据**定义 1.4.5 (稠密性)**, 存在 $\left\{x_n\right\},\left\{y_n\right\}\subset{E}$ 使 $\left\|x_n-x_0\right\|\to0$, $\left\|y_n-y_0\right\|\to0$. 令 $\widetilde{x}_n=x_n/\left\|x_n\right\|$, $\widetilde{y}_n=y_n/\left\|y_n\right\|$; 则 $\widetilde{x}_n,\widetilde{y}_n\in{E}$, $\left\|\widetilde{x}_n\right\|=\left\|\widetilde{y}_n\right\|=1$, 得 $\left\langle{T}\widetilde{x}_n,\widetilde{y}_n\right\rangle\to\left\langle{T}x_0,y_0\right\rangle$. 结合 (1), 当 $n$ 充分大时 $\left|\left\langle{T}\widetilde{x}_n,\widetilde{y}_n\right\rangle\right|>\left\|T\right\|-\varepsilon$. 因 $\widetilde{x}_n,\widetilde{y}_n$ 是 $E$ 中的单位向量, 故左侧取上确界有 $S\ge\left\|T\right\|-\varepsilon$; 令 $\varepsilon\to0$ 得 $S\ge\left\|T\right\|$. $\blacksquare$

## 2.1-3 (矩阵算子在两种范数下的范数)

在**例 2.1.1 (矩阵表示的线性算子)** 中, 如果规定向量 $x=\sum_{i=1}^{n}x_ie_i$ 的范数为 $\left\|x\right\|=\max_{1\le{i}\le{n}}\left|x_i\right|$, 求出其中算子 $T$ 的范数; 如果规定向量 $x$ 的范数为 $\left\|x\right\|=\left(\sum_{i=1}^{n}\left|x_i\right|^2\right)^{\frac12}$, 证明其中算子的范数满足

$$
\max_{1\le{j}\le{n}}\left(\sum_{i=1}^{n}\left|t_{ji}\right|^2\right)^{\frac12}\le\left\|T\right\|\le\left(\sum_{j=1}^{n}\sum_{i=1}^{n}\left|t_{ji}\right|^2\right)^{\frac12}.
$$

### 解答 2.1-3

由**例 2.1.1 (矩阵表示的线性算子)**, $Tx=y$, 其中 $\left(Tx\right)_j=y_j=\sum_{i=1}^{n}t_{ji}x_i$ ($j=1,\cdots,n$).

(1) 范数为 $\left\|x\right\|=\max_i\left|x_i\right|$ 时.

上界: 对任意 $x$ 与任意 $j$,

$$
\left|\left(Tx\right)_j\right|=\left|\sum_{i=1}^{n}t_{ji}x_i\right|\le\sum_{i=1}^{n}\left|t_{ji}\right|\left|x_i\right|\le\left(\max_{1\le{i}\le{n}}\left|x_i\right|\right)\sum_{i=1}^{n}\left|t_{ji}\right|\le\left\|x\right\|\max_{1\le{j}\le{n}}\sum_{i=1}^{n}\left|t_{ji}\right|,
$$

对 $j$ 取最大值得 $\left\|Tx\right\|\le\left\|x\right\|\max_j\sum_i\left|t_{ji}\right|$, 故由**定义 2.1.2 (算子范数)** 有 $\left\|T\right\|\le\max_j\sum_i\left|t_{ji}\right|$. $\blacksquare$

下界: 取指标 $j_0$ 使 $\sum_{i=1}^{n}\left|t_{j_0i}\right|=\max_j\sum_i\left|t_{ji}\right|$, 并令

$$
x_i=\begin{cases}\overline{t_{j_0i}}/\left|t_{j_0i}\right|,&t_{j_0i}\neq0,\\1,&t_{j_0i}=0.\end{cases}
$$

则 $\left|x_i\right|=1$ ($\forall{i}$), 故 $\left\|x\right\|=1$, 且 $t_{j_0i}x_i=\left|t_{j_0i}\right|$, 于是 $\left(Tx\right)_{j_0}=\sum_{i=1}^{n}\left|t_{j_0i}\right|$. 因而

$$
\left\|T\right\|\ge\frac{\left\|Tx\right\|}{\left\|x\right\|}\ge\left|\left(Tx\right)_{j_0}\right|=\sum_{i=1}^{n}\left|t_{j_0i}\right|=\max_{1\le{j}\le{n}}\sum_{i=1}^{n}\left|t_{ji}\right|.
$$

$\blacksquare$

> 依据范数的定义, 先看 $\left\|Tx\right\|$ 最大能放大多少, 分离出 $\left\|x\right\|$ 后得到 $\left\|T\right\|$ 的上界; 再亲自构造一套 $T$ 与 $x$ 证明此上界真的能达到.

(2) 范数为 $\left\|x\right\|=\left(\sum_i\left|x_i\right|^2\right)^{\frac12}$ 时.

上界: 对每个 $j$, 把 $\left(t_{ji}\right)_{i=1}^n$ 与 $\left(x_i\right)_{i=1}^n$ 都看作 $\mathbb{C}^n$ 中的向量, 由**引理 1.2.3 (柯西-施瓦茨不等式)**,

$$
\left|\left(Tx\right)_j\right|^2=\left|\sum_{i=1}^{n}t_{ji}x_i\right|^2\le\left(\sum_{i=1}^{n}\left|t_{ji}\right|^2\right)\left(\sum_{i=1}^{n}\left|x_i\right|^2\right).
$$

对 $j$ 求和得

$$
\left\|Tx\right\|^2=\sum_{j=1}^{n}\left|\left(Tx\right)_j\right|^2\le\left(\sum_{j=1}^{n}\sum_{i=1}^{n}\left|t_{ji}\right|^2\right)\left\|x\right\|^2,
$$

故 $\left\|T\right\|\le\left(\sum_{j}\sum_{i}\left|t_{ji}\right|^2\right)^{\frac12}$. $\blacksquare$

下界: 取指标 $j_0$ 使 $\sum_{i=1}^{n}\left|t_{j_0i}\right|^2=\max_{1\le{j}\le{n}}\sum_{i=1}^{n}\left|t_{ji}\right|^2$, 并令 $x_i=\overline{t_{j_0i}}$. 则

$$
\left\|x\right\|=\left(\sum_{i=1}^{n}\left|t_{j_0i}\right|^2\right)^{\frac12},\quad\left(Tx\right)_{j_0}=\sum_{i=1}^{n}t_{j_0i}\overline{t_{j_0i}}=\sum_{i=1}^{n}\left|t_{j_0i}\right|^2,
$$

于是

$$
\left\|Tx\right\|\ge\left|\left(Tx\right)_{j_0}\right|=\sum_{i=1}^{n}\left|t_{j_0i}\right|^2=\left\|x\right\|\left(\sum_{i=1}^{n}\left|t_{j_0i}\right|^2\right)^{\frac12}.
$$

$\blacksquare$

## 2.1-4 ($l^{p}$ 上由矩阵给定的算子)

作赋范线性空间 $l^p$ ($1<{}p<\infty$) 中算子 $T$ 如下: 当 $x=\left\{x_\nu\right\}\in{l}^p$ 时, $Tx=\left\{y_\mu\right\}$, 其中


$$
y_\mu=\sum_{\nu=1}^{\infty}t_{\mu\nu}x_\nu,\quad\mu=1,2,\cdots,
$$

且

$$
\sum_{\mu=1}^{\infty}\left(\sum_{\nu=1}^{\infty}\left|t_{\mu\nu}\right|^q\right)^{\frac{p}q}<\infty,\quad\frac1p+\frac1q=1.
$$

证明 $T$ 是 $l^p$ 上有界线性算子. 又问 $l^p$ 上有界线性算子是否都是这种形式?

### 解答 2.1-4

记

$$
C=\sum_{\mu=1}^{\infty}\left(\sum_{\nu=1}^{\infty}\left|t_{\mu\nu}\right|^q\right)^{\frac{p}q}<\infty.
$$

第一步: $T$ 良定义且线性. 由 $C$ 有限可知, 对每个固定的 $\mu$, $\left(\left|t_{\mu\nu}\right|\right)_\nu$ 与 $\left(\left|x_\nu\right|\right)_\nu$ 正是 $l^q$ 与 $l^p$ 中的元素, 由赫尔德不等式,

$$
\left|y_\mu\right|\le\sum_{\nu=1}^{\infty}\left|t_{\mu\nu}\right|\left|x_\nu\right|\le\left(\sum_{\nu=1}^{\infty}\left|t_{\mu\nu}\right|^q\right)^{\frac1q}\left(\sum_{\nu=1}^{\infty}\left|x_\nu\right|^p\right)^{\frac1p}<\infty,
$$

故每个 $y_\mu$ 都是有限数, $Tx$ 有意义. 线性性由数项级数逐项相加与数乘的运算律直接得到. $\blacksquare$

第二步: $T$ 有界. 记 $c_\mu=\left(\sum_{\nu}\left|t_{\mu\nu}\right|^q\right)^{\frac1q}$, 由上一步 $\left|y_\mu\right|\le{c}_\mu\left\|x\right\|_p$. 于是

$$
\left\|Tx\right\|_p^p=\sum_{\mu=1}^{\infty}\left|y_\mu\right|^p\le\sum_{\mu=1}^{\infty}c_\mu^p\left\|x\right\|_p^p=C\left\|x\right\|_p^p,
$$

即 $\left\|Tx\right\|_p\le{C}^{\frac1p}\left\|x\right\|_p$; 由**定义 2.1.2 (算子范数)** 得 $\left\|T\right\|\le{C}^{\frac1p}<\infty$. $\blacksquare$

第三步: 每个 $l^p$ 上的有界线性算子都有矩阵形式. 设 $T\in\mathfrak{B}\left(l^p\right)$, 记 $e_\nu$ 为第 $\nu$ 个标准单位向量, $t_{\mu\nu}=\left(Te_\nu\right)_\mu$. 因 $\sum_{\nu>{}N}\left|x_\nu\right|^p\to0$, 有 $x^{\left(N\right)}=\sum_{\nu\le{N}}x_\nu{e}_\nu\to{x}$ ($N\to\infty$); 由**定理 2.1.1 (线性算子有界与连续的等价条件)** $T$ 连续, 故

$$
Tx=\lim_{N\to\infty}Tx^{\left(N\right)}=\lim_{N\to\infty}\sum_{\nu=1}^{N}x_\nu{T}e_\nu.
$$

于是

$$
y_\mu=\left(Tx\right)_\mu=\lim_{N\to\infty}\sum_{\nu=1}^{N}x_\nu\left(Te_\nu\right)_\mu=\sum_{\nu=1}^{\infty}t_{\mu\nu}x_\nu,
$$

$\blacksquare$

第四步: 求和条件不一定都满足. 取恒等算子 $T=I$, 其矩阵为 $t_{\mu\nu}=\delta_{\mu\nu}$, 此时 $\sum_{\nu}\left|t_{\mu\nu}\right|^q=1$, 从而 $\sum_{\mu}\left(\sum_{\nu}\left|t_{\mu\nu}\right|^q\right)^{\frac{p}q}=\sum_{\mu}1=\infty$. $\blacksquare$

## 2.1-5 (积分算子的范数)

$T$ 是 $C\left[a,b\right]$ 到自身的积分算子:

$$
\left(T\varphi\right)\left(s\right)=\int_a^bK\left(s,t\right)\varphi\left(t\right)\mathrm{d}t,\quad\varphi\in{C}\left[a,b\right],
$$

其中 $K\left(s,t\right)$ 是 $\left[a,b\right]\times\left[a,b\right]$ 上二元连续函数. 证明

$$
\left\|T\right\|=\max_{a\le{s}\le{b}}\int_a^b\left|K\left(s,t\right)\right|\mathrm{d}t.
$$

### 解答 2.1-5

记 $M=\max_{a\le{s}\le{b}}\int_a^b\left|K\left(s,t\right)\right|\mathrm{d}t$; 因 $K$ 在紧集 $\left[a,b\right]\times\left[a,b\right]$ 上连续, 故对 $t$ 积分所得的 $\int_a^b\left|K\left(s,t\right)\right|\mathrm{d}t$ 关于 $s$ 连续, 从而该最大值存在.

上界. 对任意 $\varphi\in{C}\left[a,b\right]$ 与 $s\in\left[a,b\right]$,

$$
\left|\left(T\varphi\right)\left(s\right)\right|\le\int_a^b\left|K\left(s,t\right)\right|\left|\varphi\left(t\right)\right|\mathrm{d}t\le\left\|\varphi\right\|\int_a^b\left|K\left(s,t\right)\right|\mathrm{d}t\le{M}\left\|\varphi\right\|,
$$

对 $s$ 取最大值得 $\left\|T\varphi\right\|\le{M}\left\|\varphi\right\|$, 故 $\left\|T\right\|\le{M}$. $\blacksquare$

下界. 取 $s_0\in\left[a,b\right]$ 使 $\int_a^b\left|K\left(s_0,t\right)\right|\mathrm{d}t=M$. 由**注 1.4.1 ($L^{p}$ 中的稠密子集)(i)** (取 $n=1$, $p=1$), 存在 $g_n\in{C}_c^\infty\left(\mathbb{R}\right)$ 使

$$
g_n\to\chi_{\left[a,b\right]}\left(t\right)\operatorname{sign}\left(K\left(s_0,t\right)\right)\quad\text{于~}L^1\left(\mathbb{R}\right).
$$

令 $\varphi_n=g_n|_{\left[a,b\right]}$, 则 $\varphi_n\in{C}\left[a,b\right]$ 且 $\left\|\varphi_n\right\|\le1$.

由于被积函数被可积函数 $\left|K\left(s_0,t\right)\right|$ 控制, 由控制收敛定理,

$$
\left(T\varphi_n\right)\left(s_0\right)=\int_a^bK\left(s_0,t\right)\varphi_n\left(t\right)\mathrm{d}t\to\int_a^b\left|K\left(s_0,t\right)\right|\mathrm{d}t=M.
$$

由**定义 2.1.2 (算子范数)**

$$
\left\|T\right\|\ge\frac{\left\|T\varphi_n\right\|}{\left\|\varphi_n\right\|}\ge\left|\left(T\varphi_n\right)\left(s_0\right)\right|,
$$

令 $n\to\infty$ 得 $\left\|T\right\|\ge{M}$. $\blacksquare$

## 2.1-6 (微分算子的范数)

证明 $\frac{\mathrm{d}}{\mathrm{d}x}$ 是 $C^{\left(k\right)}\left[a,b\right]$ ($k\ge1$) 到 $C\left[a,b\right]$ 的连续线性算子, 并求出它的范数. 其中 $C^{\left(k\right)}\left[a,b\right]$ 是区间 $\left[a,b\right]$ 中具有连续的 $k$ 阶导函数的函数全体, 以

$$
\left\|x\right\|=\max_{0\le{j}\le{k}}\max_{t\in\left[a,b\right]}\left|x^{\left(j\right)}\left(t\right)\right|
$$

为范数.

### 解答 2.1-6

线性. 记 $T=\frac{\mathrm{d}}{\mathrm{d}x}$, 即 $\left(Tx\right)\left(t\right)=x'\left(t\right)$. 因求导是线性运算, 故 $T$ 是从 $C^{\left(k\right)}\left[a,b\right]$ 到 $C\left[a,b\right]$ 的线性算子.

连续性与 $\left\|T\right\|\le1$. 对任意 $x\in{C}^{\left(k\right)}\left[a,b\right]$,

$$
\left\|Tx\right\|=\max_{t\in\left[a,b\right]}\left|x'\left(t\right)\right|\le\max_{0\le{j}\le{k}}\max_{t\in\left[a,b\right]}\left|x^{\left(j\right)}\left(t\right)\right|=\left\|x\right\|,
$$

故由**定理 2.1.1 (线性算子有界与连续的等价条件)** ($\left(\mathrm{iii}\right)\Rightarrow\left(\mathrm{i}\right)$), $T$ 连续, 且由**定义 2.1.2 (算子范数)** 有 $\left\|T\right\|\le1$.

$\left\|T\right\|=1$. 取 $x\left(t\right)=\sin\left(t-a\right)$, 则 $\left\|x\right\|=1$. 且

$$
\left\|Tx\right\|=\max_{t\in\left[a,b\right]}\left|\cos\left(t-a\right)\right|=1,
$$

故 $\left\|T\right\|\ge1$. 结合得 $\left\|T\right\|=1$. $\blacksquare$

## 2.1-7 (一致有界算子列在稠密子空间上收敛则可延拓)

令 $X$ 是赋范线性空间, $L$ 是 $X$ 的稠密线性子空间, $Y$ 是巴拿赫空间. 设 $\left\{T_n\right\}$ 是 $\mathfrak{B}\left(X,Y\right)$ 中的一致有界算子列: 即存在 $M>0$ 使得 $\left\|T_n\right\|\le{M}$. 且对每个 $x\in{L}$, $T_nx$ 都在 $Y$ 中收敛. 那么, 存在 $T\in\mathfrak{B}\left(X,Y\right)$, 使得对 $x\in{X}$, 都有 $\lim_{n\to\infty}\left\|T_nx-Tx\right\|=0$.

### 解答 2.1-7

若 $M=0$, 则 $\left\|T_n\right\|=0$, 由**定义 2.1.2 (算子范数)** 得 $T_n=0$, 取 $T=0$ 即可; 以下设 $M>0$.

第一步: $\left\{T_nx\right\}$ 对每个 $x\in{X}$ 都是 $Y$ 中的基本点列. 对 $x\in{X}$ 与 $z\in{L}$,

$$
\left\|T_nx-T_mx\right\|\le\left\|T_n\left(x-z\right)\right\|+\left\|T_nz-T_mz\right\|+\left\|T_m\left(z-x\right)\right\|\le2M\left\|x-z\right\|+\left\|T_nz-T_mz\right\|.\tag{1}
$$

任给 $\varepsilon>0$. 由 $L$ 在 $X$ 中稠密 (**定义 1.4.5 (稠密性)**), 故 $2M\|x-z\|<\frac{\varepsilon}{2}$. 对 $z\in{L}$, $\left\{T_nz\right\}$ 收敛故 $\left\|T_nz-T_mz\right\|<\frac{\varepsilon}{2}$. 代入 (1) 得 $\left\|T_nx-T_mx\right\|<\varepsilon$, 即 $\left\{T_nx\right\}$ 是基本点列.

由 $Y$ 是巴拿赫空间 (**定义 1.4.7 (完备性)**), $\left\{T_nx\right\}$ 收敛; 定义

$$
Tx=\lim_{n\to\infty}T_nx,\quad{x}\in{X}.
$$

$\blacksquare$

第二步: $T$ 线性且 $T\in\mathfrak{B}\left(X,Y\right)$. 线性由极限的线性性成立; 在 $\left\|T_nx\right\|\le{M}\left\|x\right\|$ 中令 $n\to\infty$ 得 $\left\|Tx\right\|\le{M}\left\|x\right\|$. 故 $T$ 有界, 且 $\left\|T\right\|\le{M}$. $\blacksquare$

第三步: $T_nx\to{T}x$ 对一切 $x\in{X}$ 成立. 对 $x\in{X}$ 与 $z\in{L}$,

$$
\left\|T_nx-Tx\right\|\le\left\|T_n\left(x-z\right)\right\|+\left\|T_nz-Tz\right\|+\left\|T\left(z-x\right)\right\|\le2M\left\|x-z\right\|+\left\|T_nz-Tz\right\|.\tag{2}
$$

任给 $\varepsilon>0$. 由 $L$ 在 $X$ 中稠密 (**定义 1.4.5 (稠密性)**), 故 $2M\|x-z\|<\frac{\varepsilon}{2}$. 对 $z\in{L}$, 由 (1) 知 $\left\|T_nz-Tz\right\|<\frac{\varepsilon}{2}$. 代入 (2) 得 $\left\|T_nx-Tx\right\|<\varepsilon$. 故 $\lim_{n\to\infty}\left\|T_nx-Tx\right\|=0$. $\blacksquare$

## 2.1-8 (阶梯函数的傅里叶变换与 $L^{2}$ 上的等距延拓)

令 $A$ 为 $L^2\left(\mathbb{R}\right)$ 中阶梯函数全体, 那么 $A$ 中的函数也是 $L^1\left(\mathbb{R}\right)$ 的, 它们的傅里叶变换可以使用**例 2.1.6 (傅里叶变换)** 中给出的定义.

(i) 证明: 存在有界线性算子 $T:L^2\left(\mathbb{R}\right)\to{L}^2\left(\mathbb{R}\right)$, 使得 $T$ 是等距的: 即 $\left\|Tf\right\|=\left\|f\right\|$, 且对于 $f\in{A}$ 有 $T\left(f\right)=\widehat{f}$.

(ii) 对 $L^2\left(\mathbb{R}\right)$ 中函数 $f$, 如何合理定义 $\widehat{f}$?

### 解答 2.1-8

预备. 阶梯函数有界且支在有限区间上, 故 $A\subset{L}^1\left(\mathbb{R}\right)\cap{L}^2\left(\mathbb{R}\right)$; 由**例 2.1.6 (傅里叶变换)**, 对 $f\in{A}$ 可定义

$$
\widehat{f}\left(t\right)=\int_{\mathbb{R}}f\left(x\right)\mathrm{e}^{-2\pi\mathrm{i}tx}\,\mathrm{d}x,
$$

(i) 第一步: $A$ 在 $L^2\left(\mathbb{R}\right)$ 中稠密. 由**注 1.4.1 ($L^{p}$ 中的稠密子集)(i)** (取 $n=1$, $p=2$), 阶梯函数全体在 $L^2\left(\mathbb{R}\right)$ 中稠密. $\blacksquare$

(i) 第二步: $f\mapsto\widehat{f}$ 在 $A$ 上线性且保范. 线性由积分对 $f$ 的线性性得到. 因 $A$ 中每个函数是有限个区间指示函数的线性组合, 因此保范性只需对 $f=\chi_{\left[\alpha,\beta\right]}$ 验证. 对 $t\neq0$,

$$
\widehat{f}\left(t\right)=\int_\alpha^\beta\mathrm{e}^{-2\pi\mathrm{i}tx}\,\mathrm{d}x=\mathrm{e}^{-\pi\mathrm{i}t\left(\alpha+\beta\right)}\frac{\sin\left(\pi{t}\left(\beta-\alpha\right)\right)}{\pi{t}},
$$

故

$$
\left|\widehat{f}\left(t\right)\right|^2=\frac{\sin^2\left(\pi{t}L\right)}{\pi^2t^2},\quad{L}=\beta-\alpha>0.
$$

令 $u=\pi{t}L$, 则 $\mathrm{d}t=\mathrm{d}u/\left(\pi{L}\right)$, $\pi^2t^2=u^2/L^2$, 于是

$$
\int_{\mathbb{R}}\left|\widehat{f}\left(t\right)\right|^2\mathrm{d}t=\int_{\mathbb{R}}\frac{L\sin^2u}{\pi{u}^2}\,\mathrm{d}u=\frac{L}{\pi}\cdot\pi=L=\left\|f\right\|_2^2.
$$

其中用了 $\int_{\mathbb{R}}\frac{\sin^2u}{u^2}\,\mathrm{d}u=\pi$ 与 $\left\|f\right\|_2^2=m\left(\left[\alpha,\beta\right]\right)=L$. $\blacksquare$

(i) 第三步: 延拓到 $L^2\left(\mathbb{R}\right)$. 任取 $f\in{L}^2\left(\mathbb{R}\right)$, 由第一步取 $\left\{f_n\right\}\subset{A}$ 使 $\left\|f_n-f\right\|_2\to0$. 由第二步,

$$
\left\|\widehat{f}_n-\widehat{f}_m\right\|_2=\left\|\widehat{f_n-f_m}\right\|_2=\left\|f_n-f_m\right\|_2\le\left\|f_n-f\right\|_2+\left\|f-f_m\right\|_2,
$$

故 $\left\{\widehat{f}_n\right\}$ 是 $L^2\left(\mathbb{R}\right)$ 中的基本点列; 由**例 1.4.13 ($L^{p}\left(E\right)$ 是巴拿赫空间)**, $L^2\left(\mathbb{R}\right)$ 完备, 故它收敛. 定义

$$
Tf=\lim_{n\to\infty}\widehat{f}_n\quad\text{于~}L^2\left(\mathbb{R}\right).
$$

这个极限与 $\left\{f_n\right\}$ 的取法无关: 对于任意的 $n$, 都有

$$
\left\|\widehat{f}_n-\widehat{f}\right\|_2=\left\|\widehat{f_n-f}\right\|_2=\left\|f_n-f\right\|_2\le\left\|f_n-f\right\|_2+\left\|f-f\right\|_2.
$$

由极限的线性性可知 $T$ 线性; 又

$$
\left\|Tf\right\|_2=\lim_n\left\|\widehat{f}_n\right\|_2=\lim_n\left\|f_n\right\|_2=\left\|f\right\|_2,
$$

故 $T$ 是等距的 $\blacksquare$

(ii) 定义方式. 对 $f\in{L}^2\left(\mathbb{R}\right)$, 定义 $\widehat{f}:=Tf$, 即取 $\left\{f_n\right\}\subset{A}$ 使 $\left\|f_n-f\right\|_2\to0$ 后令 $\widehat{f}$ 为 $\widehat{f}_n$ 在 $L^2\left(\mathbb{R}\right)$ 中的极限. $\blacksquare$

## 2.2-1 ($L^{q}$ 诱导的有界线性泛函的范数)

对**例 2.2.1 (线性泛函的核 (iv))**, 证明 $\left\|F_\varphi\right\|=\left\|\varphi\right\|_q$.

### 解答 2.2-1

记 $F=F_\varphi$, 即 $F\left(\psi\right)=\int_a^b\psi\left(t\right)\overline{\varphi\left(t\right)}\,\mathrm{d}t$.

情形 $1<{}q<\infty$ (此时 $p=\frac{q}{q-1}$): 上界: 对任意 $\psi\in{L}^p\left[a,b\right]$, 由赫尔德不等式,

$$
\left|F\left(\psi\right)\right|\le\int_a^b\left|\psi\left(t\right)\right|\left|\varphi\left(t\right)\right|\mathrm{d}t\le\left\|\psi\right\|_p\left\|\varphi\right\|_q,
$$

故 $\left\|F\right\|\le\left\|\varphi\right\|_q$. $\blacksquare$

下界: 若 $\left\|\varphi\right\|_q=0$, 则 $\varphi=0$ a.e., $F=0$, 等式平凡; 以下设 $\left\|\varphi\right\|_q>0$. 令

$$
g\left(t\right)=\left|\varphi\left(t\right)\right|^{q-2}\varphi\left(t\right)\quad\left(\text{在~}\varphi\left(t\right)=0\text{~处取~}0\right).
$$

则 $\left|g\right|=\left|\varphi\right|^{q-1}$, $g\overline\varphi=\left|\varphi\right|^{q-2}\varphi\overline\varphi=\left|\varphi\right|^{q}$. 由 $\left(q-1\right)p=q$ 得

$$
\left\|g\right\|_p^p=\int_a^b\left|\varphi\right|^{\left(q-1\right)p}\mathrm{d}t=\int_a^b\left|\varphi\right|^q\mathrm{d}t=\left\|\varphi\right\|_q^q,\quad{F}\left(g\right)=\int_a^b\left|\varphi\right|^q\mathrm{d}t=\left\|\varphi\right\|_q^q.
$$

由 $\left(q-1\right)p=q$ 得 $\left\|g\right\|_p=\left\|\varphi\right\|_q^{\frac{q}p}=\left\|\varphi\right\|_q^{q-1}$, 依据**定义 2.1.2 (算子范数)**,

$$
\left\|F\right\|\ge\frac{\left|F\left(g\right)\right|}{\left\|g\right\|_p}=\frac{\left\|\varphi\right\|_q^q}{\left\|\varphi\right\|_q^{q-1}}=\left\|\varphi\right\|_q.
$$

结合上界得 $\left\|F\right\|=\left\|\varphi\right\|_q$. $\blacksquare$

情形 $q=1$ (此时 $p=\infty$): 上界: $\left|F\left(\psi\right)\right|\le\left\|\varphi\right\|_1\left\|\psi\right\|_\infty$, 故 $\left\|F\right\|\le\left\|\varphi\right\|_1$. $\blacksquare$

下界: 令

$$
\psi\left(t\right)=\begin{cases}\overline{\varphi\left(t\right)}/\left|\varphi\left(t\right)\right|,&\varphi\left(t\right)\neq0,\\0,&\varphi\left(t\right)=0,\end{cases}
$$

则 $\left|\psi\right|\le1$, 故 $\left\|\psi\right\|_\infty\le1$, 且 $\psi\overline\varphi=\left|\varphi\right|$, 于是 $F\left(\psi\right)=\int_a^b\left|\varphi\right|\mathrm{d}t=\left\|\varphi\right\|_1$, 从而 $\left\|F\right\|\ge\left\|\varphi\right\|_1$. $\blacksquare$

情形 $q=\infty$ (此时 $p=1$): 上界: $\left|F\left(\psi\right)\right|\le\left\|\varphi\right\|_\infty\left\|\psi\right\|_1$, 故 $\left\|F\right\|\le\left\|\varphi\right\|_\infty$. $\blacksquare$

下界: 对 $\varepsilon>0$, 由 $\left\|\varphi\right\|_\infty$ 是本质上确界, 集合 $E_\varepsilon=\left\{t\in\left[a,b\right]:\left|\varphi\left(t\right)\right|>\left\|\varphi\right\|_\infty-\varepsilon\right\}$ 有正测度. 令

$$
\psi\left(t\right)=\frac{1}{m\left(E_\varepsilon\right)}\chi_{E_\varepsilon}\left(t\right)\frac{\overline{\varphi\left(t\right)}}{\left|\varphi\left(t\right)\right|},
$$

则 $\left\|\psi\right\|_1=1$, 且

$$
F\left(\psi\right)=\frac{1}{m\left(E_\varepsilon\right)}\int_{E_\varepsilon}\left|\varphi\left(t\right)\right|\mathrm{d}t\ge\left\|\varphi\right\|_\infty-\varepsilon,
$$

于是 $\left\|F\right\|\ge\left\|\varphi\right\|_\infty-\varepsilon$; 令 $\varepsilon\to0$ 得 $\left\|F\right\|\ge\left\|\varphi\right\|_\infty$. $\blacksquare$

## 2.2-3 (零集包含关系给出线性泛函的线性组合)

对线性空间 $L$ 上的线性泛函 $f,f_1,f_2,\cdots,f_n$, 假设由 $f_1\left(x\right)=0,f_2\left(x\right)=0,\cdots,f_n\left(x\right)=0$ 可推得 $f\left(x\right)=0$. 证明: 存在常数 $a_1,a_2,\cdots,a_n$, 使得 $f=\sum_{k=1}^na_kf_k$.

### 解答 2.2-3

定义线性映射

$$
\Lambda:L\to\mathbb{K}^n,\quad\Lambda{x}=\left(f_1\left(x\right),f_2\left(x\right),\cdots,f_n\left(x\right)\right),
$$

其线性性由各 $f_k$ 的线性性得到; 记 $M=\Lambda\left(L\right)\subset\mathbb{K}^n$, 它是 $\mathbb{K}^n$ 的线性子空间.

在 $M$ 上定义泛函 $g$ 为

$$
g\left(\Lambda{x}\right)=f\left(x\right),\quad{x}\in{L}.
$$

验证 $g$ 良定义: 若 $\Lambda{x}=\Lambda{y}$, 则 $f_k\left(x-y\right)=0$ ($k=1,\cdots,n$), 由假设 $f\left(x-y\right)=0$, 即 $f\left(x\right)=f\left(y\right)$. $g$ 的线性性: 对 $x,y\in{L}$ 与 $\alpha,\beta\in\mathbb{K}$,

$$
g\left(\Lambda\left(\alpha{x}+\beta{y}\right)\right)=f\left(\alpha{x}+\beta{y}\right)=\alpha{f}\left(x\right)+\beta{f}\left(y\right)=\alpha{g}\left(\Lambda{x}\right)+\beta{g}\left(\Lambda{y}\right).
$$

把 $g$ 延拓为 $\mathbb{K}^n$ 上的线性泛函 $\widetilde{g}$, 则有 $\widetilde{g}|_M=g$. 由于 $\mathbb{K}^n$ 上每个线性泛函都有 $\widetilde{g}\left(y\right)=\sum_{k=1}^{n}a_ky_k$ 的形式, 于是对一切 $x\in{L}$,

$$
f\left(x\right)=g\left(\Lambda{x}\right)=\widetilde{g}\left(\Lambda{x}\right)=\sum_{k=1}^{n}a_k\left(\Lambda{x}\right)_k=\sum_{k=1}^{n}a_kf_k\left(x\right),
$$

$\blacksquare$

## 2.2-4 ($\left(l^{1}\right)^{*}=l^{\infty}$)

证明 $\left(l^1\right)^*=l^\infty$.

### 解答 2.2-4

记 $l^1$ 上的范数为 $\left\|x\right\|_1=\sum_{n=1}^{\infty}\left|x_n\right|$, $l^\infty$ 上的范数为 $\left\|\eta\right\|_\infty=\sup_n\left|\eta_n\right|$.

第一步: 由 $l^\infty$ 中的元素作出 $\left(l^1\right)^*$ 中的元素. 对 $\eta=\left(\eta_n\right)\in{l}^\infty$, 令

$$
f_\eta\left(x\right)=\sum_{n=1}^{\infty}x_n\eta_n,\quad{x}=\left(x_n\right)\in{l}^1.
$$

该级数绝对收敛, 且

$$
\left|f_\eta\left(x\right)\right|\le\sum_{n=1}^{\infty}\left|x_n\right|\left|\eta_n\right|\le\left\|\eta\right\|_\infty\left\|x\right\|_1,
$$

故 $f_\eta\in\left(l^1\right)^*$ 且 $\left\|f_\eta\right\|\le\left\|\eta\right\|_\infty$. $\blacksquare$

另一方面, 取 $x=e_m$ (第 $m$ 个标准单位向量), 则 $\left\|e_m\right\|_1=1$ 且 $f_\eta\left(e_m\right)=\eta_m$, 故 $\left\|f_\eta\right\|\ge\left|\eta_m\right|$; 对 $m$ 取上确界得 $\left\|f_\eta\right\|\ge\left\|\eta\right\|_\infty$. 于是

$$
\left\|f_\eta\right\|=\left\|\eta\right\|_\infty.
$$

$\blacksquare$

第二步: 每个 $f\in\left(l^1\right)^*$ 都如此得到. 设 $f\in\left(l^1\right)^*$, 令 $\eta_n=f\left(e_n\right)$. 由 $\left|f\left(e_n\right)\right|\le\left\|f\right\|\left\|e_n\right\|_1=\left\|f\right\|$ 得 $\eta=\left(\eta_n\right)\in{l}^\infty$ 且 $\left\|\eta\right\|_\infty\le\left\|f\right\|$.

又因 $\left\|x-\sum_{n=1}^{N}x_ne_n\right\|_1=\sum_{n>{}N}\left|x_n\right|\to0$ ($N\to\infty$), 由 $f$ 连续 (**定理 2.1.1 (线性算子有界与连续的等价条件)**) 得

$$
f\left(x\right)=\lim_{N\to\infty}\sum_{n=1}^{N}x_nf\left(e_n\right)=\sum_{n=1}^{\infty}x_n\eta_n=f_\eta\left(x\right),
$$

$\blacksquare$

第三步: 得到同构. 记 $\Phi:l^\infty\to\left(l^1\right)^*$, $\Phi\left(\eta\right)=f_\eta$. 由第一, 二步, $\Phi$ 是线性双射且保范, 由**定义 2.2.2 (保范算子与同构)** 它是 $l^\infty$ 到 $\left(l^1\right)^*$ 上的保范同构映射, 故 $\left(l^1\right)^*=l^\infty$. $\blacksquare$

## 2.2-7 (多项式在加权 $L^{2}$ 空间中稠密)

令 $L^2\left(\mathbb{R},\mathrm{e}^{-t^2}\mathrm{d}t\right)$ 为希尔伯特空间:

$$
L^2\left(\mathbb{R},\mathrm{e}^{-t^2}\mathrm{d}t\right)\overset{\text{def}}{=}\left\{f\;\text{在}\;\mathbb{R}\;\text{上勒贝格可测}:\,\left\|f\right\|_2=\left(\int_{\mathbb{R}}\left|f\left(t\right)\right|^2\mathrm{e}^{-t^2}\mathrm{d}t\right)^{\frac12}<+\infty\right\}.
$$

证明: 多项式全体在 $L^2\left(\mathbb{R},\mathrm{e}^{-t^2}\mathrm{d}t\right)$ 中稠密.

### 解答 2.2-7

记 $H=L^2\left(\mathbb{R},\mathrm{e}^{-t^2}\mathrm{d}t\right)$, $P$ 为多项式全体. **推论 1.3.3 (正交补与稠密性)**, 只需证明对任意 $f\in{H}$, 若 $f\perp{P}$ 则 $f=0$. 由**例 1.3.9 (埃尔米特多项式构成完备正交系)**, $\left\{\psi_n\right\}$ 关于勒贝格测度标准正交, 且是完备的. 由**定理 1.3.2 (标准正交基的等价条件)(iii)**, $f\perp{P}$ 推出 $f=0$ 于 $H$. $\blacksquare$

## 2.2-9 (共轭双线性泛函有界 $\Leftrightarrow$ 二元连续)

证明: 希尔伯特空间 $H$ 上共轭双线性泛函 $\varphi\left(\cdot,\cdot\right)$ 有界的充要条件是 $\varphi$ 是 $H$ 上二元连续函数 (即当 $x_n\to0$, $y_n\to0$ 时, $\varphi\left(x_n,y_n\right)\to0$).

### 解答 2.2-9

必要性. 设 $\varphi$ 有界, 即存在 $C>0$ 使 $\left|\varphi\left(x,y\right)\right|\le{C}\left\|x\right\|\left\|y\right\|$ (**定义 2.2.3 (共轭双线性泛函)(iii)**). 若 $x_n\to0$, $y_n\to0$, 则

$$
\left|\varphi\left(x_n,y_n\right)\right|\le{C}\left\|x_n\right\|\left\|y_n\right\|\to0,
$$

即 $\varphi\left(x_n,y_n\right)\to0$. $\blacksquare$

充分性. 用反证法. 若 $\varphi$ 无界. 则

$$
\sup_{\left\|x\right\|=\left\|y\right\|=1}\left|\varphi\left(x,y\right)\right|=\infty,
$$

故存在 $\left\{x_n\right\},\left\{y_n\right\}\subset{H}$ 满足 $\left\|x_n\right\|=\left\|y_n\right\|=1$ 且 $\left|\varphi\left(x_n,y_n\right)\right|\ge{n}$. 令

$$
u_n=\frac{x_n}{\sqrt{n}},\quad{v}_n=\frac{y_n}{\sqrt{n}},
$$

则 $\left\|u_n\right\|=\left\|v_n\right\|=\frac{1}{\sqrt{n}}\to0$; 又 $\varphi$ 关于第一变元线性, 关于第二变元共轭线性, 而 $\frac1{\sqrt{n}}$ 是实数, 故

$$
\left|\varphi\left(u_n,v_n\right)\right|=\frac{1}{n}\left|\varphi\left(x_n,y_n\right)\right|\ge1,
$$

这与 "$x_n\to0$, $y_n\to0$ 时 $\varphi\left(x_n,y_n\right)\to0$" 矛盾. 故 $\varphi$ 有界. $\blacksquare$

## 2.2-10 (实空间上仅控制对角项不足以得到有界性)

设 $\varphi\left(\cdot,\cdot\right)$ 是实希尔伯特空间 $H$ 上的共轭双线性泛函. 如果

$$
\sup_{\left\|x\right\|=1}\left|\varphi\left(x,x\right)\right|<\infty,
$$

问 $\varphi$ 是否为有界的? 并说明理由.

### 解答 2.2-10

不一定有界. 反例只在 $H$ 无限维时存在; 若 $H$ 有限维, 则由**例 2.1.8 (有限维赋范空间上的线性算子连续)**, $H$ 上的线性泛函都连续, 从而一切双线性泛函都有界. 以下设 $H$ 无限维, 且取 $H$ 的一组哈梅尔基, 并把基向量单位化, 记为 $\mathfrak{B}$; 从中取出一列互不相同的向量 $b_1,b_2,\cdots$.

第一步: 构造无界线性泛函 $f$. 规定

$$
k_\lambda=\begin{cases}n,&\lambda=\lambda_n\,\left(b_{\lambda_n}=b_n\right),\\0,&\text{其他},\end{cases}\quad{f}\left(x\right)=\sum_{\lambda\in{F}}c_\lambda\left(x\right)k_\lambda.
$$

则 $f$ 是 $H$ 上的线性泛函 (有限和, 且表示唯一), 而 $f\left(b_n\right)=n$, $\left\|b_n\right\|=1$, 故 $\sup_{\left\|x\right\|=1}\left|f\left(x\right)\right|=\infty$, 即 $f$ 无界. $\blacksquare$

第二步: 令 $\varphi\left(x,y\right)=f\left(x\right)-f\left(y\right)$, 验证题设条件成立. 由 $f$ 线性, $\varphi$ 对第一个变元线性, 且对第二个变元也是线性的 (实空间中共轭线性即线性), 故 $\varphi\left(x,y\right)=f\left(x\right)-f\left(y\right)$ 是双线性泛函; 且

$$
\varphi\left(x,x\right)=f\left(x\right)-f\left(x\right)=0,\quad\forall{x}\in{H},
$$

故 $\sup_{\left\|x\right\|=1}\left|\varphi\left(x,x\right)\right|=0<\infty$. $\blacksquare$

第三步: $\varphi$ 无界. 对每个 $n$, 由 $f$ 线性,

$$
\left|\varphi\left(b_n,-b_n\right)\right|=\left|f\left(b_n\right)-f\left(-b_n\right)\right|=\left|n-\left(-n\right)\right|=2n,
$$

而 $\left\|b_n\right\|=\left\|-b_n\right\|=1$, 故 $\left\|\varphi\right\|\ge2n$ 对一切 $n$ 成立, 即 $\varphi$ 无界.

所以题设条件不能保证 $\varphi$ 有界. $\blacksquare$

> 实际上, 依据**定理 2.2.6 (埃尔米特泛函的有界性)**, 只有加上对称性 $\varphi(x,y)=\varphi(y,x)$ 后, 通过极化恒等式推出非对角线项可由对角线项控制, 此时才能推出有界性.

## 2.2-12 (拉克斯-米尔格拉姆定理)

设 $\varphi\left(x,y\right)$ 是希尔伯特空间 $H$ 上的一个共轭双线性泛函, 且满足下面两个条件:

(1) 连续性: 存在 $M>0$, 使得 $\left|\varphi\left(x,y\right)\right|\le{M}\left\|x\right\|\left\|y\right\|$, $\forall{x},y\in{H}$;

(2) 强制性: 存在 $c>0$, 使得 $\left|\varphi\left(x,x\right)\right|\ge{c}\left\|x\right\|^2$,

则对任意 $f\in{H}^*$, 存在唯一 $y_f\in{H}$, 使得 $\varphi\left(x,y_f\right)=f\left(x\right)$.

### 解答 2.2-12

第一步: 定义算子 $C:H\to{H}$. 固定 $y\in{H}$, 映射 $x\mapsto\varphi\left(x,y\right)$ 是 $H$ 上的线性泛函 (由**定义 2.2.3 (共轭双线性泛函)(i)**, $\varphi$ 对第一个变元线性), 且由条件 (1) 有 $\left|\varphi\left(x,y\right)\right|\le\left(M\left\|y\right\|\right)\left\|x\right\|$, 故它连续. 由**定理 2.2.2 (里斯表示定理)**, 存在唯一的 $v\in{H}$ 使

$$
\varphi\left(x,y\right)=\left\langle{x},v\right\rangle,\quad\forall{x}\in{H}.
$$

令 $Cy=v$; 由 $v$ 的唯一性, $C$ 是 $H$ 到自身的映射, 且 $\left\|Cy\right\|=\sup_{\left\|x\right\|=1}\left|\varphi\left(x,y\right)\right|$, 从而

$$
\left\|Cy\right\|\le{M}\left\|y\right\|.
$$

$\blacksquare$

第二步: $C$ 线性. $C$ 继承了 $\varphi$ 的线性且满足 $\left\|C\right\|\le{M}$. $\blacksquare$

第三步: $C$ 是单射. 对 $y\in{H}$, 条件 (2) 与 (1) 前的表示式给出

$$
c\left\|y\right\|^2\le\left|\varphi\left(y,y\right)\right|=\left|\left\langle{y},Cy\right\rangle\right|\le\left\|y\right\|\left\|Cy\right\|,
$$

故当 $y\neq0$ 时 $\left\|Cy\right\|\ge{c}\left\|y\right\|$ (对 $y=0$ 显然成立). 特别地 $C$ 是单射. $\blacksquare$

第四步: $C$ 的值域是闭的. 设 $Cy_n\to{z}$ ($n\to\infty$). 则

$$
\left\|y_n-y_m\right\|\le\frac1c\left\|C\left(y_n-y_m\right)\right\|=\frac1c\left\|Cy_n-Cy_m\right\|\to0\quad\left(n,m\to\infty\right),
$$

故 $C\left(H\right)$ 是闭集. $\blacksquare$

第五步: $C$ 的值域在 $H$ 中稠密. 设 $z\perp{C}\left(H\right)$, 即 $\left\langle{z},Cy\right\rangle=0$ 对一切 $y$ 成立, 则 $\varphi\left(z,y\right)=0$ 对一切 $y$ 成立. 取 $y=z$ 并用条件 (2):

$$
c\left\|z\right\|^2\le\left|\varphi\left(z,z\right)\right|=0,
$$

故 $z=0$. 于是 $\left(C\left(H\right)\right)^\perp=\left\{0\right\}$, 由**推论 1.3.3 (正交补与稠密性)** 得 $C\left(H\right)$ 在 $H$ 中稠密. $\blacksquare$

第六步: $C$ 是双射. 由第四, 五步, $C\left(H\right)$ 既闭又稠密, 故 $C\left(H\right)=H$; 结合 $C$ 单射, $C$ 是双射.

现在设 $f\in{H}^*$. 由**定理 2.2.2 (里斯表示定理)**, 存在唯一的 $w\in{H}$ 使 $f\left(x\right)=\left\langle{x},w\right\rangle$ 对一切 $x$ 成立. 因 $C$ 是双射, 存在唯一的 $y_f\in{H}$ 使 $Cy_f=w$; 于是对一切 $x\in{H}$,

$$
\varphi\left(x,y_f\right)=\left\langle{x},Cy_f\right\rangle=\left\langle{x},w\right\rangle=f\left(x\right).
$$

$\blacksquare$

唯一性: 若 $y,y'$ 都满足 $\varphi\left(x,y\right)=f\left(x\right)=\varphi\left(x,y'\right)$ 对一切 $x$ 成立, 则 $\left\langle{x},C\left(y-y'\right)\right\rangle=0$ 对一切 $x$ 成立, 故 $C\left(y-y'\right)=0$, 由第三步得 $\left\|y-y'\right\|\le\frac1c\left\|C\left(y-y'\right)\right\|=0$, 即 $y=y'$. $\blacksquare$
