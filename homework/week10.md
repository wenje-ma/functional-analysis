# week10

> **定理 1.3.1 (贝塞尔不等式)**
> 
> 设 $\left\{e_\lambda:\lambda\in\Lambda\right\}$ 是希尔伯特空间 $H$ 中的标准正交系, 则对任意 $x\in{}H$ 有 $\sum_{\lambda\in\Lambda}\left|\langle{}x,e_\lambda\rangle\right|^2\le\left\|x\right\|^2$.

> **注 1.4.1 (简单函数在 $L^\infty[a,b]$ 中稠密)**
> 
> 在 $L^\infty[a,b]$ 中, 简单函数全体是稠密子集.

> **定理 1.4.2 (有限维赋范线性空间完备)**
> 
> 有限维的赋范线性空间是完备的; 若 $e_1,\ldots,e_n$ 是它的一组基, $x=\sum_{i=1}^nx_ie_i$, 则存在 $c_1,c_2>0$ 使 $c_1\sqrt{\sum_{i=1}^n\left|x_i\right|^2}\le\left\|x\right\|\le{}c_2\sqrt{\sum_{i=1}^n\left|x_i\right|^2}$.

> **例 1.4.6 ($L^p[a,b]$ 的稠密子集)**
> 
> 对 $[a,b]$ 及 $1\le{}p<\infty$, $L^p[a,b]$ 中的简单函数全体, 阶梯函数全体, $C_c^{\infty}\left(a,b\right)$, $C[a,b]$ 以及多项式全体都是稠密子集.

> **例 1.4.14 (商空间)**
> 
> 设 $M$ 是赋范线性空间 $X$ 的闭线性子空间, 对 $[x]\in{}X/M$ 定义 $\left\|[x]\right\|=d(x,M)=\inf_{y\in{}M}\left\|x+y\right\|$, 则 $X/M$ 是赋范线性空间, 商映射 $\pi$ 把 $X$ 的开单位球映成 $X/M$ 的开单位球; 当 $X$ 是巴拿赫空间时 $X/M$ 也是巴拿赫空间.

> **定理 1.6.9 (连续函数空间 $C(X)$ 的完备性)**
> 
> 设 $X$ 是紧度量空间, 对 $f\in{}C(X)$ 定义 $\left\|f\right\|=\max_{x\in{}X}\left|f(x)\right|$, 则 $C(X)$ 是巴拿赫空间.

> **定理 1.6.11 (魏尔斯特拉斯第二逼近定理)**
> 
> 三角多项式全体在 $C(T)$ 中稠密, 这里 $T$ 是单位圆周.

> **例 2.1.8 (有限维赋范空间中的线性算子)**
> 
> 有限维赋范空间中的线性算子都是连续算子; 有限维赋范线性空间中依范数收敛等价于按坐标收敛.

> **定理 2.2.2 (希尔伯特空间上的里斯表示定理)**
> 
> 设 $H$ 是希尔伯特空间, $F$ 是 $H$ 上的连续线性泛函, 则存在唯一的 $y\in{}H$ 使 $F(x)=\langle{}x,y\rangle$ 对一切 $x\in{}H$ 成立, 且 $\left\|F\right\|=\left\|y\right\|$.

> **定理 2.2.3 ($l^p$ 空间上的里斯表示定理)**
> 
> 设 $1\le{}p<\infty$, $\frac1p+\frac1q=1$. 若 $f$ 是 $l^p$ 上的连续线性泛函, 则存在唯一的 $\eta\in{}l^q$ 使 $f(x)=\sum_{\nu=1}^\infty{}x_\nu\eta_\nu$ 对一切 $x\in{}l^p$ 成立, 且 $\left\|f\right\|=\left\|\eta\right\|_q$; 特别地 $\left(l^1\right)^*=l^\infty$.

> **定理 2.3.1 (哈恩-巴拿赫延拓定理)**
> 
> 设 $L_0$ 是实赋范线性空间 $L$ 的线性子空间. 若 $f_0$ 是 $L_0$ 上的有界线性泛函, 则存在 $L$ 上的有界线性泛函 $f$, $f|_{L_0}=f_0$, 且 $\left\|f\right\|=\left\|f_0\right\|$.

> **定义 2.3.2 (零化子与预零化子)**
> 
> 对赋范线性空间 $X$ 的子集 $M$, 定义 $M^\perp=\left\{f\in{}X^*:f(x)=0,\forall{}x\in{}M\right\}$; 对对偶空间 $X^*$ 的子集 $N$, 定义 ${}^{\perp}N=\left\{x\in{}X:f(x)=0,\forall{}f\in{}N\right\}$. $M^\perp$ 是 $X^*$ 的闭线性子空间, ${}^{\perp}N$ 是 $X$ 的闭线性子空间.

> **推论 2.3.4 (闭线性子空间与点的分离)**
> 
> 设 $M$ 是赋范线性空间 $\left(X,\left\|\cdot\right\|\right)$ 的闭线性子空间, $x\notin{}M$, 则存在 $f\in{}X^*$ 使得 $\left\|f\right\|=1$, $f(M)=0$, $f(x)=d(x,M)$.

> **定义 2.5.1 (自反空间)**
> 
> 设 $X$ 是赋范线性空间, $J$ 是典则映射. 如果 $J:X\to{}X^{**}$ 是同构, 就称 $X$ 是自反的.

> **注 2.5.1 (一般可测空间上 $L^p$ 的对偶)**
> 
> 设 $\left(X,\mathcal{R}\right)$ 是可测空间, $\mu$ 是它的一个 $\sigma$-有限测度. 对 $L^p(X,\mu)$ ($1\le{}p<\infty$) 上的连续线性泛函 $\psi$, 存在唯一的 $g\in{}L^q(X,\mu)$ ($\frac1p+\frac1q=1$), 使 $\psi(f)=\int_Xfg\,\mathrm{d}\mu$ 对一切 $f\in{}L^p(X,\mu)$ 成立, 且 $\left\|\psi\right\|=\left\|g\right\|_q$; 特别地 $\left(L^1\right)^*=L^\infty$.

> **定义 2.5.2 (弱收敛与弱*收敛)**
> 
> 称 $X$ 中的点列 $\left\{x_n\right\}$ 弱收敛于 $x$ (记作 $x_n\rightharpoonup{x}$) 是指对任意 $f\in{}X^*$ 有 $f(x_n)\to{}f(x)$; 称 $X^*$ 中的点列 $\left\{f_n\right\}$ 弱*收敛于 $f$ (记作 $f_n\overset{w^*}{\longrightarrow}f$) 是指对任意 $x\in{}X$ 有 $f_n(x)\to{}f(x)$.

> **定理 2.5.2 (连续函数空间上的里斯表示定理)**
> 
> 设 $X$ 是紧度量空间, 对 $C(X)$ 上的连续线性泛函 $f$, 存在 $X$ 上唯一的全有限广义测度 (复测度) $\mu$ 使得 $f(x)=\int_Xx(t)\,\mathrm{d}\mu(t)$ 对一切 $x\in{}C(X)$ 成立, 并且 $\left\|f\right\|=\left|\mu\right|(X)$.

> **定义 2.5.3 (弱拓扑与弱*拓扑)**
> 
> 固定 $x_0\in{}X$, 对 $f_1,\ldots,f_n\in{}X^*$ 与 $\varepsilon_1,\ldots,\varepsilon_n>0$ 令 $U_{f_1,\ldots,f_n}^{\varepsilon_1,\ldots,\varepsilon_n}(x_0)=\left\{x\in{}X:\left|f_i(x-x_0)\right|<\varepsilon_i,i=1,\ldots,n\right\}$, 这些集合构成 $x_0$ 的拓扑基, 由此得到的拓扑称为 $X$ 上的弱拓扑.

> **定理 2.5.3 (典则映射的保范性)**
> 
> 设 $X$ 是赋范线性空间, 则典则映射 $J:x\mapsto{}x^{**}$ 是从 $X$ 到 $X^{**}$ 的保范线性算子, 即 $\left(\alpha{}x+\beta{}y\right)^{**}=\alpha{}x^{**}+\beta{}y^{**}$, $\left\|x^{**}\right\|=\left\|x\right\|$.

> **定义 3.2.1 (可逆算子)**
> 
> 设 $X,Y$ 是赋范线性空间, $T\in{}B(X,Y)$. 如果 $T$ 既是单射又是满射, 并且 $T^{-1}\in{}B(Y,X)$, 就称 $T$ 是可逆算子.

> **定义 3.2.2 (范数的强弱与等价)**
> 
> 设 $X$ 是线性空间, 其上赋有两个范数 $\left\|\cdot\right\|_1,\left\|\cdot\right\|_2$. 如果存在正数 $c$ 使 $\left\|x\right\|_1\le{}c\left\|x\right\|_2$ 对一切 $x\in{}X$ 成立, 就称 $\left\|\cdot\right\|_1$ 弱于 $\left\|\cdot\right\|_2$; 如果 $\left\|\cdot\right\|_1$ 既弱于 $\left\|\cdot\right\|_2$ 又强于 $\left\|\cdot\right\|_2$, 就称两个范数等价.

> **定理 3.2.3 (范数等价定理)**
> 
> 设 $\left\|\cdot\right\|_1,\left\|\cdot\right\|_2$ 是线性空间 $X$ 上的两个范数. 如果 $X$ 按这两个范数都成为巴拿赫空间, 并且 $\left\|\cdot\right\|_1$ 弱于 $\left\|\cdot\right\|_2$, 那么 $\left\|\cdot\right\|_1,\left\|\cdot\right\|_2$ 等价.

> **定理 3.2.4 (单射算子的值域闭性与下有界性)**
> 
> 设 $X,Y$ 是巴拿赫空间, $T\in{}B(X,Y)$. 若 $T$ 为单射, 则 $T$ 的值域 $R(T)$ 是闭的, 当且仅当 $T$ 是下有界的, 即存在 $c>0$ 使得对任意 $x\in{}X$ 有 $\left\|Tx\right\|\ge{}c\left\|x\right\|$.

## 2.5-10 (零化子与预零化子的对合)

设 $X$ 是赋范线性空间, $M$ 是 $X$ 中的线性子空间. 证明:

$$
{}^{\perp}\left(M^{\perp}\right)=\overline{M}.
$$

### 解答 2.5-10

按**定义 2.3.2 (零化子与预零化子)**, $M^{\perp}=\left\{f\in{}X^*:f(M)=0\right\}$, 且

$$
{}^{\perp}\left(M^{\perp}\right)=\left\{x\in{}X:f(x)=0,\forall{}f\in{}M^{\perp}\right\}.
$$

设 $x\in{}M$. 对任意 $f\in{}M^{\perp}$ 有 $f(x)=0$, 故 $x\in{}^{\perp}\left(M^{\perp}\right)$, 即 $M\subset{}^{\perp}\left(M^{\perp}\right)$. 每个 $f\in{}X^*$ 连续, 故 $f^{-1}(0)$ 是闭集, 从而

$$
{}^{\perp}\left(M^{\perp}\right)=\bigcap_{f\in{}M^{\perp}}f^{-1}(0)
$$

是闭集. 于是 $\overline{M}\subset{}^{\perp}\left(M^{\perp}\right)$.

反之设 $x_0\notin\overline{M}$. $M$ 是线性子空间, 故 $\overline{M}$ 是 $X$ 的闭线性子空间. 距离函数 $\rho(x)=d(x,M)$ 连续, 故 $d\left(x_0,\overline{M}\right)=d\left(x_0,M\right)>0$. 由**推论 2.3.4 (闭线性子空间与点的分离)** (用于闭子空间 $\overline{M}$), 存在 $f\in{}X^*$ 使得 $\left\|f\right\|=1$, $f\left(\overline{M}\right)=0$, $f(x_0)=d\left(x_0,\overline{M}\right)>0$. 因 $M\subset\overline{M}$, 有 $f(M)=0$, 即 $f\in{}M^{\perp}$; 而 $f(x_0)\ne0$, 故 $x_0\notin{}^{\perp}\left(M^{\perp}\right)$. 于是

$$
{}^{\perp}\left(M^{\perp}\right)\subset\overline{M}.
$$

两式合并即得 ${}^{\perp}\left(M^{\perp}\right)=\overline{M}$.

$\blacksquare$

## 2.5-11 (商空间的自反性)

设 $X$ 是自反空间, $M$ 是 $X$ 的闭子空间. 证明: 商空间 $X/M$ 也是自反的.

### 解答 2.5-11

按**定义 2.5.1 (自反空间)**, 只需证明典则映射 $J_{X/M}:X/M\to\left(X/M\right)^{**}$ 是满射; 按**定理 2.5.3 (典则映射的保范性)**, 它已是保范线性的.

记 $\pi:X\to{}X/M$ 为商映射, $\pi^*:\left(X/M\right)^*\to{}X^*$ 为它的共轭, 即 $\pi^*h=h\circ\pi$.

先说明 $\pi^*$ 是 $\left(X/M\right)^*$ 到 $M^{\perp}$ 的等距同构. 由**例 1.4.14 (商空间)**, $\pi$ 把 $X$ 的开单位球映成 $X/M$ 的开单位球, 故

$$
\left\|\pi^*h\right\|=\sup_{\left\|x\right\|<1}\left|h\left(\pi{}x\right)\right|=\sup_{\left\|\left[x\right]\right\|<1}\left|h\left(\left[x\right]\right)\right|=\left\|h\right\|.
$$

又 $\pi^*h$ 在 $M$ 上为 $0$, 故 $R\left(\pi^*\right)\subset{}M^{\perp}$. 反之设 $f\in{}X^*$ 且 $f(M)=0$. 令 $h\left(\left[x\right]\right)=f(x)$; 若 $\left[x\right]=\left[x'\right]$, 则 $x-x'\in{}M$, $f(x)=f(x')$, 故 $h$ 良定义. 对 $y\in{}M$ 有 $f(x)=f(x+y)$, 取 $y$ 使 $\left\|x+y\right\|$ 接近 $d(x,M)$, 得

$$
\left|h\left(\left[x\right]\right)\right|=\left|f(x)\right|\le\left\|f\right\|d(x,M)=\left\|f\right\|\left\|\left[x\right]\right\|,
$$

故 $h\in\left(X/M\right)^*$ 且 $\pi^*h=f$. 于是 $R\left(\pi^*\right)=M^{\perp}$.

再说明 $\left(\pi^*\right)^*:X^{**}\to\left(X/M\right)^{**}$ 是满射. 一般地, 设 $T\in{}B(Y,Z)$ 满足 $\left\|Ty\right\|=\left\|y\right\|$, 则 $T^*:Z^*\to{}Y^*$ 是满射: 任给 $g\in{}Y^*$, 在子空间 $T(Y)$ 上令 $\varphi(Ty)=g(y)$, 由等距性 $\varphi$ 良定义且 $\left|\varphi(Ty)\right|\le\left\|g\right\|\left\|Ty\right\|$, 即 $\varphi$ 是 $T(Y)$ 上的有界线性泛函; 由**定理 2.3.1 (哈恩-巴拿赫延拓定理)** (复情形对其实部应用), 把 $\varphi$ 保范延拓为 $\psi\in{}Z^*$, 则 $T^*\psi=g$. 取 $Y=X/M$, $Z=X$, $T=\pi^*$, 即得 $\left(\pi^*\right)^*$ 满射.

任取 $\Lambda\in\left(X/M\right)^{**}$. 由上一段, 存在 $x^{**}\in{}X^{**}$ 使 $\left(\pi^*\right)^*\left(x^{**}\right)=\Lambda$. 由 $X$ 自反, 存在 $x\in{}X$ 使 $x^{**}=J_Xx$. 于是对任意 $h\in\left(X/M\right)^*$,

$$
\Lambda(h)=\left(\pi^*\right)^*\left(x^{**}\right)(h)=x^{**}\left(\pi^*h\right)=\left(\pi^*h\right)(x)=h\left(\left[x\right]\right)=J_{X/M}\left(\left[x\right]\right)(h).
$$

故 $\Lambda=J_{X/M}\left(\left[x\right]\right)$, 即 $J_{X/M}$ 满射. 结合保范性, $J_{X/M}$ 是 $X/M$ 到 $\left(X/M\right)^{**}$ 的同构, 按**定义 2.5.1 (自反空间)**, $X/M$ 自反.

$\blacksquare$

## 2.5-12 (连续函数列弱收敛的逐点刻画)

对 $C[a,b]$ 中一致有界点列 $\left\{x_n\right\}$, 证明: $x_n$ 弱收敛于 $x_0$ 的充要条件是对任意的 $t\in[a,b]$,

$$
\lim_{n\to\infty}x_n(t)=x_0(t).
$$

### 解答 2.5-12

设 $\sup_n\left\|x_n\right\|\le{}M$.

必要性. 固定 $t\in[a,b]$, 令 $\delta_t(x)=x(t)$. 则 $\left|\delta_t(x)\right|\le\left\|x\right\|$, 故 $\delta_t\in{}C[a,b]^*$. 由**定义 2.5.2 (弱收敛与弱*收敛)**, $x_n\rightharpoonup{x}_0$ 给出 $\delta_t(x_n)\to\delta_t(x_0)$, 即 $x_n(t)\to{}x_0(t)$.

充分性. 设 $x_n(t)\to{}x_0(t)$ 对一切 $t\in[a,b]$ 成立. 任给 $f\in{}C[a,b]^*$, 由**定理 2.5.2 (连续函数空间上的里斯表示定理)**, 存在 $[a,b]$ 上唯一的全有限广义测度 $\mu$ 使得

$$
f(x)=\int_a^bx(t)\,\mathrm{d}\mu(t),\quad\forall{}x\in{}C[a,b],
$$

且 $\left\|f\right\|=\left|\mu\right|\left([a,b]\right)$. 因 $\left|x_n\right|\le{}M$ 且 $x_n(t)\to{}x_0(t)$ 逐点, 由控制收敛定理,

$$
\left|f(x_n)-f(x_0)\right|\le\int_a^b\left|x_n(t)-x_0(t)\right|\,\mathrm{d}\left|\mu\right|(t)\to0.
$$

故 $f(x_n)\to{}f(x_0)$ 对一切 $f\in{}C[a,b]^*$ 成立, 即 $x_n\rightharpoonup{x}_0$.

$\blacksquare$

## 2.5-13 ($L^1$ 中弱收敛的测度刻画)

设 $\left\{f_n\right\}$ 是 $L^1[0,1]$ 中的一致有界点列. 证明: $f_n$ 弱收敛于一个可积函数 $f$, 当且仅当对任意 $[0,1]$ 中勒贝格可测集 $E$ 成立

$$
\lim_{n\to\infty}\int_Ef_n\,\mathrm{d}m=\int_Ef\,\mathrm{d}m.
$$

### 解答 2.5-13

设 $\sup_n\left\|f_n\right\|_1\le{}M<\infty$.

必要性. 设 $f_n\rightharpoonup{f}$. 对可测集 $E$, $\chi_E\in{}L^{\infty}[0,1]$. 由**注 2.5.1 (一般可测空间上 $L^p$ 的对偶)** (取 $p=1$), $L^{\infty}[0,1]=\left(L^1[0,1]\right)^*$, 故 $\chi_E$ 是 $L^1[0,1]$ 上的连续线性泛函, 由**定义 2.5.2 (弱收敛与弱*收敛)** 得 $\int_Ef_n\,\mathrm{d}m\to\int_Ef\,\mathrm{d}m$.

充分性. 设对一切可测集 $E$ 有 $\int_Ef_n\,\mathrm{d}m\to\int_Ef\,\mathrm{d}m$. 取 $E=[0,1]$, $E_+=\left\{f>0\right\}$, $E_-=\left\{f<0\right\}$, 则

$$
\left\|f\right\|_1=\int_{E_+}f\,\mathrm{d}m-\int_{E_-}f\,\mathrm{d}m=\lim_{n\to\infty}\left(\int_{E_+}f_n\,\mathrm{d}m-\int_{E_-}f_n\,\mathrm{d}m\right)\le2M,
$$

故 $\left\|f_n-f\right\|_1\le3M$ 对一切 $n$ 成立.

任给 $g\in{}L^{\infty}[0,1]$. 由**注 1.4.1 (简单函数在 $L^\infty[a,b]$ 中稠密)**, 存在简单函数 $\varphi$ 使 $\left\|g-\varphi\right\|_\infty<\varepsilon$. 简单函数是示性函数的有限线性组合, 故由假设 $\int{}f_n\varphi\,\mathrm{d}m\to\int{}f\varphi\,\mathrm{d}m$. 于是

$$
\limsup_{n\to\infty}\left|\int\left(f_n-f\right)g\,\mathrm{d}m\right|\le\limsup_{n\to\infty}\left|\int\left(f_n-f\right)\varphi\,\mathrm{d}m\right|+\left\|f_n-f\right\|_1\left\|g-\varphi\right\|_\infty\le3M\varepsilon.
$$

令 $\varepsilon\to0$, 得 $\int{}f_ng\,\mathrm{d}m\to\int{}fg\,\mathrm{d}m$ 对一切 $g\in{}L^{\infty}[0,1]$ 成立; 由**注 2.5.1 (一般可测空间上 $L^p$ 的对偶)** (取 $p=1$), 这正是 $f_n\rightharpoonup{f}$.

$\blacksquare$

## 2.5-14 ($l^\infty$ 中元素由 $c_0$ 弱*逼近)

对 $l^\infty$ 中元素 $x$, 给出 $l^\infty$ 中的一个点列 $\left\{x_n\right\}$, 使得 $x_n\in{}c_0$ 且 $x_n$ 弱*收敛于 $x$.

### 解答 2.5-14

对 $x=\left(x_1,x_2,\ldots\right)\in{}l^\infty$, 令

$$
x_n=\left(x_1,\ldots,x_n,0,0,\ldots\right),\quad{}n=1,2,\ldots.
$$

每个 $x_n$ 只有有限个非零分量, 故 $x_n\in{}c_0$.

由**定理 2.2.3 ($l^p$ 空间上的里斯表示定理)** (取 $p=1$), $\left(l^1\right)^*=l^\infty$, 即 $l^\infty$ 是 $l^1$ 的对偶, 其上弱*收敛就是与一切 $\eta\in{}l^1$ 配对后收敛. 对 $\eta=\left(\eta_k\right)\in{}l^1$,

$$
\left|\left\langle{}x_n-x,\eta\right\rangle\right|=\left|\sum_{k=n+1}^\infty{}x_k\eta_k\right|\le\left\|x\right\|_\infty\sum_{k=n+1}^\infty\left|\eta_k\right|\to0,
$$

最后一步因为 $\sum_k\left|\eta_k\right|$ 收敛, 其余项趋于 $0$. 按**定义 2.5.2 (弱收敛与弱*收敛)**, $x_n$ 弱*收敛于 $x$.

$\blacksquare$

## 2.5-15 ($L^\infty$ 的弱*逼近与傅里叶系数的唯一性)

(i) 对一个 $L^\infty[a,b]$ 函数 $f$, 给出一个 $C[a,b]$ 中的函数列 $\left\{f_n\right\}$, 使得 $\left\{f_n\right\}$ 在 $L^\infty[a,b]$ 弱*收敛于 $f$.

(ii) 在第 6 题中, 我们证明了: 若一个 $L^1[0,2\pi]$ 函数 $f$ 的傅里叶系数全为零, 则 $f$ 是零函数. 使用 (i) 给出这个结果的直接证明.

### 解答 2.5-15

(i) 记 $M=\left\|f\right\|_\infty$. 对每个 $n$, 由**例 1.4.6 ($L^p[a,b]$ 的稠密子集)** (取 $p=1$), $C[a,b]$ 在 $L^1[a,b]$ 中稠密, 故存在 $g_n\in{}C[a,b]$ 使 $\left\|g_n-f\right\|_1<\frac1n$. 令

$$
f_n=g_n\min\left\{1,\frac{M}{\left|g_n\right|}\right\}
$$

($g_n=0$ 处取值 $0$), 即把 $g_n$ 径向截断到闭圆盘 $\left|z\right|\le{}M$. 圆盘上的度量投影是 $1$-利普希茨的, 故 $\left|f_n-f\right|\le\left|g_n-f\right|$ 逐点; 又 $f_n\in{}C[a,b]$ 且 $\left\|f_n\right\|_\infty\le{}M$, 于是 $\left\|f_n-f\right\|_1<\frac1n$.

任给 $h\in{}L^1[a,b]$ 与 $K>0$, 记 $h_K=h\chi_{\left\{\left|h\right|\le{}K\right\}}$. 则

$$
\left|\int_a^b\left(f_n-f\right)h\,\mathrm{d}m\right|\le\int\left|f_n-f\right|\left|h_K\right|\,\mathrm{d}m+\int\left|f_n-f\right|\left|h-h_K\right|\,\mathrm{d}m\le{}K\left\|f_n-f\right\|_1+2M\left\|h-h_K\right\|_1.
$$

先令 $n\to\infty$, 得 $\limsup\le2M\left\|h-h_K\right\|_1$; 再令 $K\to\infty$, 由 $\left|h\right|\in{}L^1$ 得右端趋于 $0$. 故 $\int{}f_nh\,\mathrm{d}m\to\int{}fh\,\mathrm{d}m$ 对一切 $h\in{}L^1[a,b]$ 成立. 由**注 2.5.1 (一般可测空间上 $L^p$ 的对偶)** (取 $p=1$), $L^\infty[a,b]=\left(L^1[a,b]\right)^*$, 故 $\left\{f_n\right\}$ 在 $L^\infty[a,b]$ 中弱*收敛于 $f$.

$\blacksquare$

(ii) 把 $[0,2\pi]$ 上的 $f$ 按 $2\pi$ 周期延拓, 看作 $T$ 上的可积函数, 于是 $\hat{f}(n)$ 就是它在 $T$ 上的傅里叶系数, 且题设即

$$
\frac1{2\pi}\int_0^{2\pi}f(t)\mathrm{e}^{-\mathrm{i}nt}\,\mathrm{d}t=0,\quad\forall{}n\in\mathbb{Z}.
$$

对三角多项式 $p(t)=\sum_{k=-N}^Na_k\mathrm{e}^{\mathrm{i}kt}$,

$$
\frac1{2\pi}\int_0^{2\pi}f(t)\overline{p(t)}\,\mathrm{d}t=\sum_{k=-N}^N\overline{a_k}\hat{f}(k)=0.
$$

由**定理 1.6.11 (魏尔斯特拉斯第二逼近定理)**, 三角多项式在 $C(T)$ 中稠密, 故对任意 $g\in{}C(T)$, 取 $p$ 使 $\left\|g-p\right\|_\infty<\varepsilon$, 得

$$
\left|\frac1{2\pi}\int_0^{2\pi}f(t)\overline{g(t)}\,\mathrm{d}t\right|\le\left\|f\right\|_1\left\|g-p\right\|_\infty\to0,
$$

即 $\frac1{2\pi}\int{}f\overline{g}=0$ 对一切 $g\in{}C(T)$ 成立.

任给 $g\in{}L^\infty(T)$. 连续函数在 $L^1(T)$ 中稠密 (由**例 1.4.6 ($L^p[a,b]$ 的稠密子集)** 与 $T$ 上函数的周期延拓得到), 与 (i) 的论证相同 (把 $[a,b]$ 换成 $T$), 存在 $g_n\in{}C(T)$ 使 $\left\|g_n\right\|_\infty\le\left\|g\right\|_\infty$, $\left\|g_n-g\right\|_1\to0$, 且对一切 $h\in{}L^1(T)$ 有 $\frac1{2\pi}\int\left(g_n-g\right)\overline{h}\to0$. 取 $h=f$ 得

$$
\frac1{2\pi}\int_0^{2\pi}f(t)\overline{g_n(t)}\,\mathrm{d}t\to\frac1{2\pi}\int_0^{2\pi}f(t)\overline{g(t)}\,\mathrm{d}t.
$$

而 $g_n\in{}C(T)$, 由上一段 $\frac1{2\pi}\int{}f\overline{g_n}=0$, 故 $\frac1{2\pi}\int{}f\overline{g}=0$ 对一切 $g\in{}L^\infty(T)$ 成立.

取 $g=\operatorname{sgn}f$ ($f(t)\ne0$ 时取值 $f(t)/\left|f(t)\right|$, 否则取值 $0$), 则 $g\in{}L^\infty(T)$ 且 $\frac1{2\pi}\int{}f\overline{g}=\left\|f\right\|_1$. 于是 $\left\|f\right\|_1=0$, 即 $f=0$ 几乎处处.

$\blacksquare$

## 2.5-16 (希尔伯特空间弱拓扑与范数拓扑一致的条件)

对希尔伯特空间 $H$, 证明: $H$ 上的范数拓扑和弱拓扑是一致的, 当且仅当 $H$ 是有限维空间.

### 解答 2.5-16

先设 $\dim{}H=n<\infty$. 取 $H$ 的一组基 $e_1,\ldots,e_n$, 记 $f_i$ 为相应的坐标泛函, 即 $x=\sum_{i=1}^nf_i(x)e_i$. 由**例 2.1.8 (有限维赋范空间中的线性算子)**, $f_1,\ldots,f_n\in{}H^*$; 由**定理 1.4.2 (有限维赋范线性空间完备)** 中的范数估计, 存在 $c>0$ 使

$$
\left\|x\right\|\le{}c\max_{1\le{}i\le{}n}\left|f_i(x)\right|.
$$

按**定义 2.5.3 (弱拓扑与弱*拓扑)**, 弱拓扑由形如 $U_{g_1,\ldots,g_m}^{\varepsilon_1,\ldots,\varepsilon_m}(x_0)$ 的集合生成. 每个 $g\in{}H^*$ 连续, 故每个弱开集是范数开集. 反之, 对 $\varepsilon>0$, 集合 $U=\left\{x:\max_i\left|f_i(x)\right|<\frac{\varepsilon}{c}\right\}$ 是 $0$ 的弱邻域且 $U\subset\left\{\left\|x\right\|<\varepsilon\right\}$; 平移后每个范数开球都含一个弱邻域, 故每个范数开集是弱开集. 两种拓扑一致.

$\blacksquare$

再设 $\dim{}H=\infty$. 取 $H$ 中线性无关点列, 经格拉姆-施密特正交化得标准正交列 $\left\{e_n\right\}$. 由**定理 1.3.1 (贝塞尔不等式)**, 对任意 $y\in{}H$,

$$
\sum_{n=1}^\infty\left|\langle{}e_n,y\rangle\right|^2\le\left\|y\right\|^2,
$$

故 $\langle{}e_n,y\rangle\to0$. 由**定理 2.2.2 (希尔伯特空间上的里斯表示定理)**, 每个 $f\in{}H^*$ 形如 $f=\langle\cdot,y\rangle$, 故 $f(e_n)\to0=f(0)$, 即 $e_n\rightharpoonup0$. 但 $\left\|e_n\right\|=1$, 故 $\left\{e_n\right\}$ 不依范数收敛于 $0$.

若两种拓扑一致, 则依弱拓扑收敛的点列必依范数拓扑收敛到同一极限; $\left\{e_n\right\}$ 给出矛盾. 故两种拓扑不一致.

$\blacksquare$

## 2.5-17 (弱*极限的范数下半连续)

若赋范线性空间 $X$ 上的有界线性泛函序列 $f_n$ 弱*收敛于 $f$, 证明:

$$
\liminf_{n\to\infty}\left\|f_n\right\|\ge\left\|f\right\|.
$$

### 解答 2.5-17

若 $\left\|f\right\|=0$ 则结论显然, 故设 $\left\|f\right\|>0$. 任给 $\varepsilon>0$, 由 $\left\|f\right\|=\sup_{\left\|x\right\|\le1}\left|f(x)\right|$, 存在 $x\in{}X$, $\left\|x\right\|\le1$, 使 $\left|f(x)\right|>\left\|f\right\|-\varepsilon$. 由**定义 2.5.2 (弱收敛与弱*收敛)**, $f_n(x)\to{}f(x)$, 故

$$
\liminf_{n\to\infty}\left\|f_n\right\|\ge\liminf_{n\to\infty}\left|f_n(x)\right|=\left|f(x)\right|>\left\|f\right\|-\varepsilon.
$$

令 $\varepsilon\to0$ 即得 $\liminf_{n\to\infty}\left\|f_n\right\|\ge\left\|f\right\|$.

$\blacksquare$

## 2.5-18 (希尔伯特空间中范数收敛的弱收敛刻画)

对希尔伯特空间 $X$ 中点列 $\left\{x_n\right\}$, 证明: $\left\{x_n\right\}$ 按范数收敛于 $x$, 当且仅当 $\left\{x_n\right\}$ 弱收敛于 $x$ 且

$$
\lim_{n\to\infty}\left\|x_n\right\|=\left\|x\right\|.
$$

### 解答 2.5-18

必要性. 若 $\left\|x_n-x\right\|\to0$, 则对任意 $f\in{}X^*$,

$$
\left|f(x_n)-f(x)\right|\le\left\|f\right\|\left\|x_n-x\right\|\to0,
$$

即 $x_n\rightharpoonup{x}$; 又 $\left|\left\|x_n\right\|-\left\|x\right\|\right|\le\left\|x_n-x\right\|\to0$.

$\blacksquare$

充分性. 设 $x_n\rightharpoonup{x}$ 且 $\left\|x_n\right\|\to\left\|x\right\|$. 由**定理 2.2.2 (希尔伯特空间上的里斯表示定理)**, $y\mapsto\langle{}y,x\rangle$ 是 $X$ 上的连续线性泛函, 故 $\langle{}x_n,x\rangle\to\langle{}x,x\rangle=\left\|x\right\|^2$. 于是

$$
\left\|x_n-x\right\|^2=\left\|x_n\right\|^2-2\operatorname{Re}\langle{}x_n,x\rangle+\left\|x\right\|^2\to\left\|x\right\|^2-2\left\|x\right\|^2+\left\|x\right\|^2=0.
$$

故 $x_n$ 按范数收敛于 $x$.

$\blacksquare$

## 3.2-1 (值域闭的商空间刻画)

设 $X,Y$ 是巴拿赫空间, $T\in{}B(X,Y)$. 证明: $R(T)$ 是闭的当且仅当存在 $c>0$, 使得对任意 $x\in{}X$ 有

$$
c\left\|Tx\right\|\ge{}d\left(x,\ker{}T\right).
$$

### 解答 3.2-1

$\ker{}T=T^{-1}(0)$ 是 $X$ 的闭线性子空间. 按**例 1.4.14 (商空间)**, $X/\ker{}T$ 是巴拿赫空间, 且 $\left\|\left[x\right]\right\|=d\left(x,\ker{}T\right)$.

令 $\widetilde{T}\left(\left[x\right]\right)=Tx$. 若 $\left[x\right]=\left[x'\right]$, 则 $x-x'\in\ker{}T$, $Tx=Tx'$, 故 $\widetilde{T}$ 良定义; 它显然线性, 且 $\left\|\widetilde{T}\left(\left[x\right]\right)\right\|=\left\|Tx\right\|$. 又 $T$ 在 $\ker{}T$ 上为零, 故 $\left\|Tx\right\|=\left\|T(x+y)\right\|\le\left\|T\right\|\left\|x+y\right\|$ 对一切 $y\in\ker{}T$ 成立, 取 $y$ 使 $\left\|x+y\right\|$ 接近 $d\left(x,\ker{}T\right)$, 得 $\left\|Tx\right\|\le\left\|T\right\|d\left(x,\ker{}T\right)=\left\|T\right\|\left\|\left[x\right]\right\|$, 故 $\widetilde{T}$ 有界. 于是 $\widetilde{T}\in{}B\left(X/\ker{}T,Y\right)$, $R\left(\widetilde{T}\right)=R(T)$. 又 $\widetilde{T}\left(\left[x\right]\right)=0$ 蕴含 $Tx=0$, 即 $x\in\ker{}T$, $\left[x\right]=0$, 故 $\widetilde{T}$ 是单射.

由**定理 3.2.4 (单射算子的值域闭性与下有界性)**, $R\left(\widetilde{T}\right)$ 闭当且仅当存在 $c_0>0$ 使 $\left\|\widetilde{T}\left(\left[x\right]\right)\right\|\ge{}c_0\left\|\left[x\right]\right\|$ 对一切 $\left[x\right]$ 成立, 即

$$
\left\|Tx\right\|\ge{}c_0d\left(x,\ker{}T\right),\quad\forall{}x\in{}X.
$$

因 $R\left(\widetilde{T}\right)=R(T)$, 上式等价于 $R(T)$ 闭; 取 $c=\frac1{c_0}$ 即得所证形式.

$\blacksquare$

## 3.2-2 ($C[0,1]$ 按 $L^1$ 范数不完备)

用范数等价定理证明: $C[0,1]$ 按范数

$$
\left\|f\right\|_1=\int_{[0,1]}\left|f(t)\right|\,\mathrm{d}m(t)
$$

不是巴拿赫空间.

### 解答 3.2-2

记 $\left\|f\right\|_\infty=\max_{t\in[0,1]}\left|f(t)\right|$. 因 $\int_0^1\left|f\right|\,\mathrm{d}m\le\left\|f\right\|_\infty$, 按**定义 3.2.2 (范数的强弱与等价)**, 范数 $\left\|\cdot\right\|_1$ 弱于 $\left\|\cdot\right\|_\infty$. 由**定理 1.6.9 (连续函数空间 $C(X)$ 的完备性)** (取 $X=[0,1]$), $\left(C[0,1],\left\|\cdot\right\|_\infty\right)$ 是巴拿赫空间.

若 $\left(C[0,1],\left\|\cdot\right\|_1\right)$ 也是巴拿赫空间, 则由**定理 3.2.3 (范数等价定理)**, 两个范数等价, 特别存在 $C>0$ 使

$$
\left\|f\right\|_\infty\le{}C\left\|f\right\|_1,\quad\forall{}f\in{}C[0,1].
$$

取 $f_n(t)=\max\left\{0,1-nt\right\}$, 则 $f_n\in{}C[0,1]$, $\left\|f_n\right\|_\infty=1$, 而

$$
\left\|f_n\right\|_1=\int_0^{1/n}\left(1-nt\right)\,\mathrm{d}t=\frac1{2n}.
$$

于是 $1=\left\|f_n\right\|_\infty\le\frac{C}{2n}\to0$, 矛盾. 故 $\left(C[0,1],\left\|\cdot\right\|_1\right)$ 不是巴拿赫空间.

$\blacksquare$

## 3.2-3 (乘子算子的范数与可逆性)

对勒贝格可测函数 $\varphi\in{}L^\infty[0,1]$, 定义 $L^2[0,1]$ 上的有界线性算子 $M_\varphi$ 为

$$
M_\varphi(f)=\varphi{}f,\quad\forall{}f\in{}L^2[0,1].
$$

证明: $\left\|M_\varphi\right\|=\left\|\varphi\right\|_\infty$, 并且 $M_\varphi$ 是可逆算子当且仅当存在正数 $c>0$, 使得对几乎处处的 $x\in[0,1]$ 成立不等式 $\left|\varphi(x)\right|>c$.

### 解答 3.2-3

先证范数等式. 因 $\left|\varphi(x)f(x)\right|\le\left\|\varphi\right\|_\infty\left|f(x)\right|$ 几乎处处, $\left\|M_\varphi{}f\right\|_2\le\left\|\varphi\right\|_\infty\left\|f\right\|_2$, 故 $\left\|M_\varphi\right\|\le\left\|\varphi\right\|_\infty$.

反之设 $\varepsilon>0$, 令 $E_\varepsilon=\left\{x\in[0,1]:\left|\varphi(x)\right|>\left\|\varphi\right\|_\infty-\varepsilon\right\}$. 由 $\left\|\varphi\right\|_\infty=\inf\left\{M:m\left(\left|\varphi\right|>M\right)=0\right\}$ 知 $m\left(E_\varepsilon\right)>0$. 取 $f=\chi_{E_\varepsilon}/\sqrt{m\left(E_\varepsilon\right)}$, 则 $\left\|f\right\|_2=1$ 且

$$
\left\|M_\varphi{}f\right\|_2\ge\left\|\varphi\right\|_\infty-\varepsilon.
$$

故 $\left\|M_\varphi\right\|\ge\left\|\varphi\right\|_\infty$, 结合上一段得 $\left\|M_\varphi\right\|=\left\|\varphi\right\|_\infty$.

$\blacksquare$

再证可逆性的等价.

充分性. 设存在 $c>0$ 使 $\left|\varphi(x)\right|>c$ 几乎处处成立. 则 $1/\varphi$ 可测且 $\left\|1/\varphi\right\|_\infty\le\frac1c$, 故 $M_{1/\varphi}\in{}B\left(L^2[0,1]\right)$, 且

$$
M_{1/\varphi}M_\varphi{}f=f,\quad{}M_\varphi{}M_{1/\varphi}f=f,\quad\forall{}f\in{}L^2[0,1].
$$

按**定义 3.2.1 (可逆算子)**, $M_\varphi$ 可逆.

$\blacksquare$

必要性. 设 $M_\varphi$ 可逆, 记 $S$ 为其有界逆. 则对一切 $f\in{}L^2[0,1]$,

$$
\left\|f\right\|_2=\left\|SM_\varphi{}f\right\|_2\le\left\|S\right\|\left\|\varphi{}f\right\|_2.
$$

令 $E=\left\{\left|\varphi\right|<\frac1{\left\|S\right\|}\right\}$. 若 $m(E)>0$, 取 $f=\chi_E/\sqrt{m(E)}$, 则 $\left\|\varphi{}f\right\|_2<\frac1{\left\|S\right\|}\left\|f\right\|_2$, 与上式矛盾. 故 $\left|\varphi\right|\ge\frac1{\left\|S\right\|}$ 几乎处处; 取 $c=\frac1{2\left\|S\right\|}>0$, 即得 $\left|\varphi(x)\right|>c$ 对几乎处处的 $x$ 成立.

$\blacksquare$
