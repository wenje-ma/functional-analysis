# week2

> **基础知识: 巴塞尔问题**<br>$\sum_{n=1}^{\infty}\frac{1}{n^2}=\frac{\pi^2}{6}$.

> **基础知识: Euclid 范数的三角不等式**<br>$\mathbb R^2$ 上 Euclid 范数 $\left\|(u,v)\right\|=\sqrt{u^2+v^2}$ 满足三角不等式: $\left\|(u_1,v_1)+(u_2,v_2)\right\|\le\left\|(u_1,v_1)\right\|+\left\|(u_2,v_2)\right\|$.

> **基础知识: 稠密的传递性**<br>设 $X$ 是度量空间, $B$ 是 $X$ 的稠密子集. 若对每个 $b\in B$ 与每个 $\epsilon>0$, 存在 $a\in A$ 使 $d(a,b)<\epsilon$, 则 $A$ 在 $X$ 中稠密.

> **基础知识: 非奇异矩阵可逆**<br>数域上的方阵 $A$ 非奇异 (行列式不为零) 当且仅当 $A$ 可逆, 即存在方阵 $A^{-1}$ 使 $AA^{-1}=A^{-1}A=I$.

> **基础知识: 富比尼定理**<br>设 $f$ 在乘积空间 $\mathbb R^m\times\mathbb R^n$ 上 Lebesgue 可积, 则对几乎处处的 $x\in\mathbb R^m$, $f(x,\cdot)$ 关于 $\mathbb R^n$ 可积, 且 $\int_{\mathbb R^m\times\mathbb R^n}f\,\mathrm dm=\int_{\mathbb R^m}\left(\int_{\mathbb R^n}f(x,y)\,\mathrm dn(y)\right)\mathrm dm(x)$.

> **基础知识: 格拉姆-施密特过程不改变张成空间**<br>对内积空间中的向量列 $\{g_n\}$ 施行格拉姆-施密特正交化得到标准正交列 $\{h_n\}$, 则对每个 $N$, $\operatorname{span}\{h_0,h_1,\cdots,h_N\}=\operatorname{span}\{g_0,g_1,\cdots,g_N\}$.

> **基础知识: 积分的线性性**<br>Lebesgue 积分对被积函数是线性的: $\int(\alpha f+\beta g)\,\mathrm dm=\alpha\int f\,\mathrm dm+\beta\int g\,\mathrm dm$.

> **基础知识: 集合论的直接事实**<br>若 $M\subset N\subset H$, 则 $N$ 中元素满足的条件自动对 $M$ 中元素成立, 故 $\{x:x\perp N\}\subset\{x:x\perp M\}$, 即 $N^\perp\subset M^\perp$.

> **基础知识: 可测集的紧-开逼近与卷积磨光**<br>对 $\mathbb R^n$ 中有限测度 Lebesgue 可测集 $E$ 与 $\delta>0$, 存在紧集 $K\subset E$ 与开集 $U\supset E$ 使 $m(U\setminus K)<\delta$, 且存在 $\psi\in C_c^\infty(\mathbb R^n)$ 满足 $0\le\psi\le1$, $\psi\equiv1$ 于 $K$, $\operatorname{supp}\psi\subset U$.

> **基础知识: 勒贝格积分的性质**<br>设 $g\ge0$ 是可测函数, 则 $\int g\,\mathrm dm=0$ 当且仅当 $g=0$ 几乎处处成立.

> **基础知识: 勒贝格控制收敛定理**<br>设 $\{f_n\}$ 是 Lebesgue 可测函数列, 点态收敛于可测函数 $f$, 且存在可积函数 $g$ 使 $\left|f_n(t)\right|\le g(t)$ 对几乎处处的 $t$ 与一切 $n$ 成立, 则 $f$ 可积, 且 $\lim_{n\to\infty}\int f_n\,\mathrm dm=\int f\,\mathrm dm$.

> **基础知识: 实数三角不等式**<br>对任意实数 $a,b$, 有 $\left|a+b\right|\le\left|a\right|+\left|b\right|$.

> **基础知识: 简单函数的单调逼近**<br>对任意 $f\in L^p(\mathbb R^n)$, 存在简单函数列 $\{\Phi_k\}$ 点态收敛于 $f$, 且 $\left|\Phi_k\right|\le\left|f\right|$.

> **基础知识: 平方展开估计**<br>对任意实数 $a,b$, $(\left|a\right|+\left|b\right|)^2\le2\left|a\right|^2+2\left|b\right|^2$.

> **基础知识: 线性无关组的定义**<br>对于线性空间 $X$, $X$ 中的线性无关组是指 $X$ 中的一些元素构成的子集 $A$, 使得 $A$ 中任意一个元素都不能被 $A$ 中其他有限个元素线性表出; 等价地, 若 $\sum_{i=1}^n c_i x_i=0$, 则一切 $c_i=0$.

> **基础知识: 希尔伯特空间的定义**<br>若内积空间 $H$ 所导出的度量是完备的, 则称 $H$ 是一个希尔伯特 (Hilbert) 空间.

> **基础知识: 正交补的定义**<br>设 $H$ 是内积空间, 对于 $x\in H$, $A\subset H$, 若对每个 $y\in A$ 有 $x\perp y$, 则称 $x\perp A$, 并记 $A^\perp=\{x\in H:x\perp A\}$.

> **定义 1.1.2 (极限)**<br>设 $(X,d)$ 是度量空间, $\{x_n\}_{n=1}^\infty$ 是 $X$ 中点列, $x_0\in X$, 若 $\lim_{n\to\infty}d(x_n,x_0)=0$, 则称点列 $\{x_n\}_{n=1}^\infty$ 按照度量 $d$ 收敛于 $x_0$, 记为 $\lim_{n\to\infty}x_n=x_0$.

> **定义 1.2.2 (半范数与范数)**<br>记 $\mathbb K$ 是实数域 $\mathbb R$ 或复数域 $\mathbb C$. 对于 $\mathbb K$ 上的线性空间 $X$, 若每个向量 $x$ 都对应一个实数 $\left\|x\right\|$, 满足: (i) $\left\|x\right\|\ge0$; (ii) $\left\|\alpha x\right\|=\left|\alpha\right|\left\|x\right\|$; (iii) $\left\|x+y\right\|\le\left\|x\right\|+\left\|y\right\|$, 则称 $\left\|\cdot\right\|$ 为半范数. 若还满足 $\left\|x\right\|=0$ 当且仅当 $x=0$, 则称 $\left\|\cdot\right\|$ 为范数, $(X,\left\|\cdot\right\|)$ 称为赋范线性空间. 范数诱导度量 $d(x,y)=\left\|x-y\right\|$.

> **定义 1.2.3 (内积空间)**<br>记 $\mathbb K$ 是实数域 $\mathbb R$ 或复数域 $\mathbb C$. 对于 $\mathbb K$ 上的线性空间 $H$, 如果任何两个向量 $x,y$ 都对应一个数 $\langle x,y\rangle\in\mathbb K$, 满足: (i) 共轭对称性 $\langle x,y\rangle=\overline{\langle y,x\rangle}$; (ii) 对第一变元的线性性 $\langle\alpha x+\beta y,z\rangle=\alpha\langle x,z\rangle+\beta\langle y,z\rangle$; (iii) 正定性 $\langle x,x\rangle\ge0$ 且 $\langle x,x\rangle=0$ 当且仅当 $x=0$, 则称 $\langle\cdot,\cdot\rangle$ 是 $H$ 中的内积, 称 $H$ 是内积空间.

> **引理 1.2.3 (柯西-施瓦茨不等式)**<br>设 $H$ 是内积空间, $x,y\in H$, 则 $\left|\langle x,y\rangle\right|^2\le\langle x,x\rangle\langle y,y\rangle$.

> **定理 1.2.2 (勾股定理, 毕达哥拉斯定理)**<br>对内积空间 $H$ 中两个元素 $x,y$, 若 $x\perp y$, 则 $\left\|x+y\right\|^2=\left\|x\right\|^2+\left\|y\right\|^2$.

> **引理 1.2.4 (内积的连续性)**<br>设 $H$ 是内积空间, 则内积关于两个变元是连续的: 当 $x_n\to x$, $y_n\to y$ 时, 有 $\langle x_n,y_n\rangle\to\langle x,y\rangle$.

> **例 1.2.8 ($L^p(E)$ 是巴拿赫空间)**<br>设 $E$ 是 Euclid 空间 $\mathbb R^k$ 的 Lebesgue 可测集, $1\le p<\infty$, 则 $L^p(E)$ 按范数 $\left\|f\right\|_p=\left(\int_E\left|f\right|^p\,\mathrm dm\right)^{1/p}$ 是赋范线性空间, 且该范数诱导的度量是完备的, 即 $L^p(E)$ 是巴拿赫空间.

> **定义 1.3.1 (正交系与标准正交系)**<br>设 $\mathfrak F$ 是内积空间 $H$ 中的一族非零向量. (i) 如果 $\mathfrak F$ 中任何两个不同的向量都正交, 就称 $\mathfrak F$ 是 $H$ 的正交系; (ii) 如果正交系 $\mathfrak F$ 中每个向量的范数都等于 $1$, 就称 $\mathfrak F$ 是标准正交系 (规范正交系).

> **定理 1.3.1 (贝塞尔不等式)**<br>设 $\mathfrak F=\{e_\lambda:\lambda\in\Lambda\}$ 是 Hilbert 空间 $H$ 中的标准正交系. 对每个 $x\in H$, 其 Fourier 系数 $\{\langle x,e_\lambda\rangle:\lambda\in\Lambda\}$ 中最多只有可列个不为零, 且 $\sum_{\lambda\in\Lambda}\left|\langle x,e_\lambda\rangle\right|^2\le\left\|x\right\|^2$.

> **定理 1.3.2 (标准正交基的等价条件)**<br>设 $\mathfrak F=\{e_\lambda:\lambda\in\Lambda\}$ 是 Hilbert 空间 $H$ 中的标准正交系, 下列命题等价: (i) 对任意 $x\in H$, $x=\sum_{\lambda\in\Lambda}\langle x,e_\lambda\rangle e_\lambda$; (ii) $\overline{\operatorname{span}\{e_\lambda:\lambda\in\Lambda\}}=H$; (iii) $\mathfrak F$ 是完全的, 即若 $x\in H$ 满足 $x\perp e_\lambda$ ($\forall\lambda\in\Lambda$), 则 $x=0$; (iv) $\mathfrak F$ 是完备的, 即对任意 $x\in H$, 帕塞瓦尔等式 $\left\|x\right\|^2=\sum_{\lambda\in\Lambda}\left|\langle x,e_\lambda\rangle\right|^2$ 成立. 满足上述条件之一的标准正交系称为 $H$ 中的标准正交基.

> **例 1.3.3 (三角多项式标准正交系)**<br>在实 (或复) 周期函数空间 $L^2[0,2\pi]$ 中, 规定内积 $\langle f,g\rangle=\frac{1}{2\pi}\int_0^{2\pi}f(x)\overline{g(x)}\,\mathrm dx$, 则 $\{1,\sqrt2\cos x,\sqrt2\sin x,\sqrt2\cos2x,\sqrt2\sin2x,\cdots,\sqrt2\cos nx,\sqrt2\sin nx,\cdots\}$ 组成 $L^2[0,2\pi]$ 的标准正交系.

> **例 1.3.7 ($e^{inx}$ 构成标准正交基)**<br>在复空间 $L^2[0,2\pi]$ 中, $\{e^{inx}:n\in\mathbb Z\}$ 是一组标准正交基.

> **例 1.3.8 (勒让德多项式)**<br>在 $L^2[-1,1]$ 中, 函数列 $g_k(x)=x^k$ ($k=0,1,2,\cdots$) 是线性无关的. 勒让德多项式 $P_0(x)=1$, $P_n(x)=\frac{1}{2^n n!}\frac{\mathrm d^n}{\mathrm dx^n}(x^2-1)^n$ ($n=1,2,\cdots$) 是 $L^2[-1,1]$ 中的正交多项式系; 单位化后 $h_0(x)=\frac{1}{\sqrt2}$, $h_n(x)=\frac{1}{2^n n!}\sqrt{\frac{2n+1}{2}}\frac{\mathrm d^n}{\mathrm dx^n}(x^2-1)^n$ 是 $\{g_k\}$ 经过格拉姆-施密特过程得到的标准正交向量系.

> **定义 1.4.5 (稠密性)**<br>在度量空间 $(X,d)$ 中, 对于 $X$ 中一个子集 $A$, 称 $A$ 在 $X$ 中稠密是指 $X\subset\overline A$ (即 $\overline A=X$).

> **例 1.4.6 ($L^p$ 中的稠密子集)**<br>对直线上有界闭区间 $[a,b]$ 及 $1\le p<\infty$, $L^p[a,b]$ 中的简单函数全体、阶梯函数全体、$C_c^\infty(a,b)$、$C[a,b]$ 以及多项式全体 $P$ 均是 $L^p[a,b]$ 的稠密子集.

> **注 1.4.1 ($L^p(\mathbb R^n)$ 中的稠密子集)**<br>类似地, 可得 $L^p(\mathbb R^n)$ ($1\le p<\infty$) 中的简单函数全体、阶梯函数全体以及 $C_c^\infty(\mathbb R^n)$ 均是稠密子集.

---

## 1.4-8 ($C_c^\infty$ 在 $L^p$ 中稠密)

在直线 $\mathbb R$ 上, 证明:

(i) $C_c^\infty(\mathbb R)$ 在 $L^p(\mathbb R)$ ($1\le p<\infty$) 中稠密.

(ii) $C_c^\infty(\mathbb R)$ 不在 $L^\infty(\mathbb R)$ 中稠密.

(iii) 多项式全体不在 $L^p(\mathbb R)$ ($1\le p<\infty$) 中稠密.

本题作业要求作答第 (i) 问.

### 解答 1.4-8

教材为 $\mathbb R$ 情形, 下面证明更强的 $\mathbb R^n$ 情形 (令 $n=1$ 即得本题).

第一步: 化归为逼近简单函数. 由**定义 1.4.5 (稠密性)**, 只需证明: 对任意 $f\in L^p(\mathbb R^n)$ 与任意 $\epsilon>0$, 存在 $\varphi\in C_c^\infty(\mathbb R^n)$ 使 $\left\|f-\varphi\right\|_p<\epsilon$. 由**注 1.4.1 ($L^p(\mathbb R^n)$ 中的稠密子集)**, 简单函数全体在 $L^p(\mathbb R^n)$ 中稠密. 于是由**基础知识: 稠密的传递性**, 只需证明每个简单函数都能被 $C_c^\infty(\mathbb R^n)$ 中函数以任意 $L^p$ 精度逼近.

第二步: 用简单函数逼近 $f$. 由**基础知识: 简单函数的单调逼近**, 存在简单函数列 $\{\Phi_k\}$ 点态收敛于 $f$, 且 $\left|\Phi_k\right|\le\left|f\right|$. 于是 $\left|f-\Phi_k\right|^p\le(2\left|f\right|)^p\in L^1$, 由**基础知识: 勒贝格控制收敛定理**,

$$
\lim_{k\to\infty}\left\|f-\Phi_k\right\|_p^p=\lim_{k\to\infty}\int_{\mathbb R^n}\left|f-\Phi_k\right|^p\,\mathrm dm=\int_{\mathbb R^n}\lim_{k\to\infty}\left|f-\Phi_k\right|^p\,\mathrm dm=0.
$$

故对给定的 $\epsilon>0$, 存在简单函数 $\Phi$ 使 $\left\|f-\Phi\right\|_p<\frac{\epsilon}{2}$. 余下只需证明 $\Phi$ 可被 $C_c^\infty$ 函数逼近到任意精度.

第三步: 用卷积磨光逼近特征函数. 设 $E\subset\mathbb R^n$ 是有限测度 Lebesgue 可测集. 由**基础知识: 可测集的紧-开逼近与卷积磨光**, 存在紧集 $K\subset E$, 开集 $U\supset E$ 以及 $\psi\in C_c^\infty(\mathbb R^n)$, 使 $m(U\setminus K)<\left(\frac{\epsilon}{2}\right)^p$, 且 $0\le\psi\le1$, $\psi\equiv1$ 于 $K$, $\operatorname{supp}\psi\subset U$. 于是 $\chi_E-\psi$ 只可能在 $U\setminus K$ 上非零, 且 $\left|\chi_E-\psi\right|\le1$, 故

$$
\left\|\chi_E-\psi\right\|_p^p=\int_{U\setminus K}\left|\chi_E-\psi\right|^p\,\mathrm dm\le m(U\setminus K)<\left(\frac{\epsilon}{2}\right)^p,
$$

即 $\left\|\chi_E-\psi\right\|_p<\frac{\epsilon}{2}$. 故特征函数可被 $C_c^\infty$ 函数逼近.

第四步: 用线性性逼近一般简单函数. 设 $\Phi=\sum_{i=1}^s c_i\chi_{E_i}$ 是简单函数, 其中每个 $E_i$ 有限测度. 对每个 $i$, 由第三步取 $\psi_i\in C_c^\infty(\mathbb R^n)$ 使 $\left\|\chi_{E_i}-\psi_i\right\|_p<\frac{\epsilon}{2s(\left|c_i\right|+1)}$. 令 $\varphi=\sum_{i=1}^s c_i\psi_i$, 则 $\varphi\in C_c^\infty(\mathbb R^n)$ (有限个紧支集光滑函数的线性组合仍紧支光滑). 由**定义 1.2.2 (半范数与范数)** (iii) 范数的三角不等式,

$$
\left\|\Phi-\varphi\right\|_p=\left\|\sum_{i=1}^s c_i(\chi_{E_i}-\psi_i)\right\|_p\le\sum_{i=1}^s\left|c_i\right|\left\|\chi_{E_i}-\psi_i\right\|_p<\frac{\epsilon}{2}.
$$

故每个简单函数都可被 $C_c^\infty$ 函数以任意精度逼近.

第五步: 合拢. 对给定的 $f$ 与 $\epsilon>0$, 由第二步取简单函数 $\Phi$ 使 $\left\|f-\Phi\right\|_p<\frac{\epsilon}{2}$, 由第四步取 $\varphi\in C_c^\infty(\mathbb R^n)$ 使 $\left\|\Phi-\varphi\right\|_p<\frac{\epsilon}{2}$. 再由**定义 1.2.2 (半范数与范数)** (iii) 的三角不等式,

$$
\left\|f-\varphi\right\|_p\le\left\|f-\Phi\right\|_p+\left\|\Phi-\varphi\right\|_p<\epsilon.
$$

由**定义 1.4.5 (稠密性)**, $C_c^\infty(\mathbb R^n)$ 在 $L^p(\mathbb R^n)$ 中稠密, 特别地 $C_c^\infty(\mathbb R)$ 在 $L^p(\mathbb R)$ 中稠密. $\blacksquare$

---

## 1.2-3 (乘积空间上两范数与非奇异矩阵映射的拓扑同胚)

设 $L$ 是赋范线性空间, $L\times L$ 按照线性运算

$$
\alpha(x_1,y_1)+\beta(x_2,y_2)=(\alpha x_1+\beta x_2,\alpha y_1+\beta y_2)
$$

成为线性空间. 在 $L\times L$ 上定义两个范数如下:

$$
\left\|(x,y)\right\|_1=\sqrt{\left\|x\right\|^2+\left\|y\right\|^2},\quad\left\|(x,y)\right\|_2=\max\{\left\|x\right\|,\left\|y\right\|\}.
$$

(i) 证明: $(L\times L,\left\|\cdot\right\|_1)$ 和 $(L\times L,\left\|\cdot\right\|_2)$ 都是赋范线性空间.

(ii) 作 $(L\times L,\left\|\cdot\right\|_1)$ 到 $(L\times L,\left\|\cdot\right\|_2)$ 的映射:

$$
\varphi:(x,y)\mapsto(x',y'),\quad(x',y')=(x,y)\begin{pmatrix}a&b\\c&d\end{pmatrix},
$$

其中矩阵 $\begin{pmatrix}a&b\\c&d\end{pmatrix}$ 是非奇异的. 证明: $\varphi$ 是拓扑同胚 (即 $\varphi$ 是到上的一一对应, 且 $\varphi$ 和 $\varphi^{-1}$ 都是连续的).

### 解答 1.2-3

(i) 先验证 $\left\|\cdot\right\|_1$. 由**定义 1.2.2 (半范数与范数)** 逐条验证. 非负性: 由 $L$ 的范数非负, $\left\|\left(x,y\right)\right\|_1=\sqrt{\left\|x\right\|^2+\left\|y\right\|^2}\ge0$. 正定性: $\left\|\left(x,y\right)\right\|_1=0$ 当且仅当 $\left\|x\right\|=\left\|y\right\|=0$, 当且仅当 $x=0$ 且 $y=0$, 当且仅当 $(x,y)=(0,0)$. 齐次性: 由 $L$ 中范数的齐次性 (**定义 1.2.2 (半范数与范数)** (ii)),

$$
\left\|\alpha(x,y)\right\|_1=\sqrt{\left\|\alpha x\right\|^2+\left\|\alpha y\right\|^2}=\sqrt{\left|\alpha\right|^2\left\|x\right\|^2+\left|\alpha\right|^2\left\|y\right\|^2}=\left|\alpha\right|\left\|\left(x,y\right)\right\|_1.
$$

三角不等式: 由 $L$ 中范数的三角不等式 (**定义 1.2.2 (半范数与范数)** (iii)), $\left\|x+x'\right\|\le\left\|x\right\|+\left\|x'\right\|$, $\left\|y+y'\right\|\le\left\|y\right\|+\left\|y'\right\|$. 由**基础知识: Euclid 范数的三角不等式**,

$$
\begin{aligned}
\left\|\left(x,y\right)+\left(x',y'\right)\right\|_1&=\sqrt{\left\|x+x'\right\|^2+\left\|y+y'\right\|^2}\\
&\le\sqrt{(\left\|x\right\|+\left\|x'\right\|)^2+(\left\|y\right\|+\left\|y'\right\|)^2}\\
&\le\sqrt{\left\|x\right\|^2+\left\|y\right\|^2}+\sqrt{\left\|x'\right\|^2+\left\|y'\right\|^2}.
\end{aligned}
$$

故 $\left\|\cdot\right\|_1$ 满足**定义 1.2.2 (半范数与范数)** 的全部条件, 是范数.

再验证 $\left\|\cdot\right\|_2$. 非负性与正定性: $\left\|\left(x,y\right)\right\|_2=\max\{\left\|x\right\|,\left\|y\right\|\}\ge0$, 且它为零当且仅当 $\left\|x\right\|=\left\|y\right\|=0$, 当且仅当 $(x,y)=(0,0)$. 齐次性:

$$
\left\|\alpha(x,y)\right\|_2=\max\{\left\|\alpha x\right\|,\left\|\alpha y\right\|\}=\left|\alpha\right|\max\{\left\|x\right\|,\left\|y\right\|\}=\left|\alpha\right|\left\|\left(x,y\right)\right\|_2.
$$

三角不等式: 由 $L$ 中范数的三角不等式 (**定义 1.2.2 (半范数与范数)** (iii)), $\left\|x+x'\right\|\le\left\|x\right\|+\left\|x'\right\|$, $\left\|y+y'\right\|\le\left\|y\right\|+\left\|y'\right\|$, 故

$$
\begin{aligned}
\left\|\left(x,y\right)+\left(x',y'\right)\right\|_2&=\max\{\left\|x+x'\right\|,\left\|y+y'\right\|\}\\
&\le\max\{\left\|x\right\|+\left\|x'\right\|,\left\|y\right\|+\left\|y'\right\|\}\\
&\le\max\{\left\|x\right\|,\left\|y\right\|\}+\max\{\left\|x'\right\|,\left\|y'\right\|\}.
\end{aligned}
$$

故 $\left\|\cdot\right\|_2$ 也是范数. 因此 $(L\times L,\left\|\cdot\right\|_1)$ 与 $(L\times L,\left\|\cdot\right\|_2)$ 都是赋范线性空间.

(ii) 先证 $\varphi$ 是到上的一一对应. 记 $A=\begin{pmatrix}a&b\\c&d\end{pmatrix}$. 由**基础知识: 非奇异矩阵可逆**, $A$ 非奇异蕴含 $A^{-1}$ 存在. 对任意 $(x',y')\in L\times L$, 令 $(x,y)=(x',y')A^{-1}$, 则 $\varphi(x,y)=(x,y)A=(x',y')A^{-1}A=(x',y')$, 故 $\varphi$ 是到上的. 又若 $\varphi(x,y)=\varphi(u,v)$, 则 $(x,y)A=(u,v)A$, 两边右乘 $A^{-1}$ 得 $(x,y)=(u,v)$, 故 $\varphi$ 是一一的.

再证 $\varphi$ 连续. 由**定义 1.1.2 (极限)**, 只需证明: 若 $(x_n,y_n)\to(x,y)$ 按 $\left\|\cdot\right\|_1$, 则 $\varphi(x_n,y_n)\to\varphi(x,y)$ 按 $\left\|\cdot\right\|_2$. 由 $\left\|\cdot\right\|_1$ 的定义, $\left\|x_n-x\right\|\to0$ 且 $\left\|y_n-y\right\|\to0$, 故 $\delta_n=\max\{\left\|x_n-x\right\|,\left\|y_n-y\right\|\}\to0$. 由 $L$ 中范数的三角不等式与齐次性 (**定义 1.2.2 (半范数与范数)** (ii)(iii)),

$$
\begin{aligned}
\left\|\varphi(x_n,y_n)-\varphi(x,y)\right\|_2&=\max\{\left\|a(x_n-x)+b(y_n-y)\right\|,\left\|c(x_n-x)+d(y_n-y)\right\|\}\\
&\le\max\{(\left|a\right|+\left|b\right|)\delta_n,(\left|c\right|+\left|d\right|)\delta_n\}\to0.
\end{aligned}
$$

故 $\varphi$ 连续. 最后证 $\varphi^{-1}$ 连续: $\varphi^{-1}(x',y')=(x',y')A^{-1}$, 而 $A^{-1}$ 也是非奇异矩阵, 对 $\varphi^{-1}$ 重复上面 $\varphi$ 的论证即得 $\varphi^{-1}$ 连续. 综上, $\varphi$ 是到上的一一对应且 $\varphi,\varphi^{-1}$ 均连续, 故 $\varphi$ 是拓扑同胚. $\blacksquare$

---

## 1.2-6 ($C_b(0,1]$ 上的上确界范数)

设 $C_b(0,1]$ 表示在半开半闭区间 $(0,1]$ 上处处连续且有界的函数全体. 对于每个 $x\in C_b(0,1]$, 令

$$
\left\|x\right\|=\sup_{0<t\le1}\left|x(t)\right|.
$$

证明:

(i) $\left\|x\right\|$ 是空间 $C_b(0,1]$ 上的范数; $C_b(0,1]$ 按 $\left\|\cdot\right\|$ 成为赋范线性空间;

(ii) 在 $C_b(0,1]$ 中点列 $\{x_n\}$ 按范数 $\left\|\cdot\right\|$ 收敛于 $x_0$ 的充要条件是 $\{x_n\}$ 在 $(0,1]$ 上一致收敛于 $x_0$.

### 解答 1.2-6

(i) $C_b(0,1]$ 按通常函数的线性运算成为线性空间, 因为两个有界连续函数的线性组合仍是有界连续函数. 由**定义 1.2.2 (半范数与范数)** 逐条验证范数公理. 非负性: $\left\|x\right\|=\sup_{0<t\le1}\left|x(t)\right|\ge0$. 正定性: $\left\|x\right\|=0$ 当且仅当 $\left|x(t)\right|=0$ 对一切 $0<t\le1$ 成立, 当且仅当 $x\equiv0$. 齐次性: 由**定义 1.2.2 (半范数与范数)** (ii),

$$
\left\|\alpha x\right\|=\sup_{0<t\le1}\left|\alpha x(t)\right|=\left|\alpha\right|\sup_{0<t\le1}\left|x(t)\right|=\left|\alpha\right|\left\|x\right\|.
$$

三角不等式: 对任意 $x,y\in C_b(0,1]$ 与 $t\in(0,1]$, 由**基础知识: 实数三角不等式**,

$$
\left|x(t)+y(t)\right|\le\left|x(t)\right|+\left|y(t)\right|\le\left\|x\right\|+\left\|y\right\|.
$$

右端与 $t$ 无关, 对 $t$ 取上确界即得 $\left\|x+y\right\|\le\left\|x\right\|+\left\|y\right\|$. 故 $\left\|\cdot\right\|$ 是 $C_b(0,1]$ 上的范数, $C_b(0,1]$ 按 $\left\|\cdot\right\|$ 成为赋范线性空间.

(ii) 由**定义 1.1.2 (极限)**, $\{x_n\}$ 按范数 $\left\|\cdot\right\|$ 收敛于 $x_0$ 当且仅当

$$
\left\|x_n-x_0\right\|=\sup_{0<t\le1}\left|x_n(t)-x_0(t)\right|\to0.
$$

而该式正是 $\{x_n\}$ 在 $(0,1]$ 上一致收敛于 $x_0$ 的定义. 故按范数收敛与一致收敛等价. $\blacksquare$

---

## 1.2-10 (标准正交向量组线性无关)

设 $H$ 是内积空间. 如果 $x_1,x_2,\cdots,x_n$ 是 $H$ 中的向量, 它们满足条件 $\langle x_i,x_j\rangle=\delta_{ij}$, 证明: $x_1,x_2,\cdots,x_n$ 是一组线性无关的向量.

### 解答 1.2-10

设 $\sum_{i=1}^n c_i x_i=0$, 其中 $c_i\in\mathbb K$. 对任意固定的 $j\in\{1,2,\cdots,n\}$, 两边与 $x_j$ 取内积. 由**定义 1.2.3 (内积空间)** (ii) 内积对第一变元的线性性,

$$
0=\left\langle\sum_{i=1}^n c_i x_i,x_j\right\rangle=\sum_{i=1}^n c_i\left\langle x_i,x_j\right\rangle=\sum_{i=1}^n c_i\delta_{ij}=c_j.
$$

因 $j$ 任意, 故 $\sum_{i=1}^n c_i x_i=0$ 蕴含一切 $c_j=0$. 由**基础知识: 线性无关组的定义**, $x_1,x_2,\cdots,x_n$ 是一组线性无关的向量. $\blacksquare$

---

## 1.2-12 (正交补的性质)

设 $H$ 是一个 Hilbert 空间.

(i) 对于 $x\in H$, $x\perp H$ 的充要条件是 $x=0$.

(ii) 对 $H$ 中的子集 $A$, $A^\perp$ 是闭的线性子空间.

(iii) 若子集 $M\subset N\subset H$, 则 $M^\perp\supset N^\perp$.

(iv) 对线性空间 $M\subset H$, $M\cap M^\perp=\{0\}$.

(v) 设 $L$ 是由 $H$ 的两个子集 $M$ 和 $N$ 张成的线性子空间, 证明 $L^\perp=M^\perp\cap N^\perp$.

### 解答 1.2-12

由**基础知识: 正交补的定义**, 以下记 $x\perp A$ 为 $x$ 与 $A$ 中每个元素正交, 并记 $A^\perp=\{x\in H:x\perp A\}$.

(i) 先证充分性: 若 $x=0$, 则对任意 $y\in H$, 由内积对第一变元的线性性 (**定义 1.2.3 (内积空间)** (ii)), $\langle0,y\rangle=0$, 故 $x\perp H$. 再证必要性: 若 $x\perp H$, 特别地 $x\perp x$, 即 $\langle x,x\rangle=0$. 由**定义 1.2.3 (内积空间)** (iii) 的正定性, $x=0$. 故 $x\perp H$ 当且仅当 $x=0$.

(ii) 先证 $A^\perp$ 是线性子空间: 设 $x_1,x_2\in A^\perp$, $\alpha,\beta\in\mathbb K$. 对任意 $y\in A$, 由内积对第一变元的线性性,

$$
\langle\alpha x_1+\beta x_2,y\rangle=\alpha\langle x_1,y\rangle+\beta\langle x_2,y\rangle=\alpha\cdot0+\beta\cdot0=0,
$$

故 $\alpha x_1+\beta x_2\in A^\perp$, 即 $A^\perp$ 对线性组合封闭. 再证 $A^\perp$ 是闭的: 设 $x_n\in A^\perp$ 且 $x_n\to x$ (按内积诱导的范数). 对任意 $y\in A$, 由**引理 1.2.4 (内积的连续性)**, $\langle x,y\rangle=\lim_{n\to\infty}\langle x_n,y\rangle=0$, 故 $x\in A^\perp$. 故 $A^\perp$ 是闭的线性子空间.

(iii) 设 $x\in N^\perp$, 则 $x\perp y$ 对一切 $y\in N$ 成立. 由 $M\subset N$, $N$ 中每个元素都属于 $M$ 这一条件自动成立 (**基础知识: 集合论的直接事实**), 故 $x\perp y$ 对一切 $y\in M$ 也成立, 即 $x\in M^\perp$. 故 $N^\perp\subset M^\perp$, 即 $M^\perp\supset N^\perp$.

(iv) 设 $x\in M\cap M^\perp$. 则 $x\in M$ 且 $x\perp M$, 特别地 $x\perp x$, 即 $\langle x,x\rangle=0$. 由**定义 1.2.3 (内积空间)** (iii) 的正定性, $x=0$. 故 $M\cap M^\perp=\{0\}$.

(v) 由题设 $L=\operatorname{span}(M\cup N)$ 是 $M\cup N$ 中元素的有限线性组合全体. 对任意 $z\in H$, 由内积对第一变元的线性性 (**定义 1.2.3 (内积空间)** (ii)), $\langle z,\cdot\rangle$ 在有限线性组合上为零当且仅当它在每个基元上为零, 故

$$
\begin{aligned}
z\in L^\perp&\Leftrightarrow\langle z,w\rangle=0\quad(\forall w\in L)\\
&\Leftrightarrow\langle z,m\rangle=0\ (\forall m\in M)\ \text{且}\ \langle z,n\rangle=0\ (\forall n\in N)\\
&\Leftrightarrow z\in M^\perp\ \text{且}\ z\in N^\perp\Leftrightarrow z\in M^\perp\cap N^\perp.
\end{aligned}
$$

故 $L^\perp=M^\perp\cap N^\perp$. $\blacksquare$

---

## 1.3-1 (标准正交基下内积的展开式)

设 $\mathfrak F=\{e_\lambda:\lambda\in\Lambda\}$ 是 Hilbert 空间 $H$ 的标准正交基. 证明: 对任何 $x,y\in H$,

$$
\langle x,y\rangle=\sum_{\lambda\in\Lambda}\langle x,e_\lambda\rangle\overline{\langle y,e_\lambda\rangle}.
$$

### 解答 1.3-1

由**定理 1.3.2 (标准正交基的等价条件)** (i), 对任何 $x,y\in H$ 有 Fourier 展开

$$
x=\sum_{\lambda\in\Lambda}\langle x,e_\lambda\rangle e_\lambda,\qquad y=\sum_{\mu\in\Lambda}\langle y,e_\mu\rangle e_\mu.
$$

由**引理 1.2.4 (内积的连续性)**, 内积可换入级数. 再由**定义 1.2.3 (内积空间)** (ii) 对第一变元的线性性与 (i) 共轭对称性,

$$
\langle x,y\rangle=\left\langle\sum_{\lambda}\langle x,e_\lambda\rangle e_\lambda,\sum_{\mu}\langle y,e_\mu\rangle e_\mu\right\rangle=\sum_{\lambda,\mu}\langle x,e_\lambda\rangle\overline{\langle y,e_\mu\rangle}\langle e_\lambda,e_\mu\rangle.
$$

由 $\mathfrak F$ 是标准正交系 (**定义 1.3.1 (正交系与标准正交系)**), $\langle e_\lambda,e_\mu\rangle=\delta_{\lambda\mu}$, 故上式中仅 $\lambda=\mu$ 的项保留, 得

$$
\langle x,y\rangle=\sum_{\lambda\in\Lambda}\langle x,e_\lambda\rangle\overline{\langle y,e_\lambda\rangle}.
$$

$\blacksquare$

---

## 1.3-3 (二元三角标准正交基)

令 $L^2([0,2\pi]\times[0,2\pi])$ 上的内积为

$$
\langle f,g\rangle=\iint_{[0,2\pi]\times[0,2\pi]}f(x,y)\overline{g(x,y)}\frac{\mathrm dx\mathrm dy}{4\pi^2}.
$$

证明: $\{e^{imx}e^{iny}:m,n\in\mathbb Z\}$ 构成 $L^2([0,2\pi]\times[0,2\pi])$ 的一组标准正交基.

### 解答 1.3-3

第一步: 证标准正交性. 对任意 $m,n,m',n'\in\mathbb Z$, 被积函数在乘积测度下绝对可积, 由**基础知识: 富比尼定理**,

$$
\begin{aligned}
\langle e^{imx}e^{iny},e^{im'x}e^{in'y}\rangle&=\frac{1}{4\pi^2}\int_0^{2\pi}\int_0^{2\pi}e^{i(m-m')x}e^{i(n-n')y}\,\mathrm dx\mathrm dy\\
&=\left(\frac{1}{2\pi}\int_0^{2\pi}e^{i(m-m')x}\,\mathrm dx\right)\left(\frac{1}{2\pi}\int_0^{2\pi}e^{i(n-n')y}\,\mathrm dy\right).
\end{aligned}
$$

由**例 1.3.7 ($e^{inx}$ 构成标准正交基)**, $\{e^{ikx}\}_{k\in\mathbb Z}$ 是 $L^2[0,2\pi]$ 的标准正交系, 即 $\frac{1}{2\pi}\int_0^{2\pi}e^{ikx}\,\mathrm dx=\delta_{k0}$. 故上式 $=\delta_{mm'}\delta_{nn'}$. 由**定义 1.3.1 (正交系与标准正交系)**, $\{e^{imx}e^{iny}:m,n\in\mathbb Z\}$ 是 $L^2([0,2\pi]\times[0,2\pi])$ 的标准正交系.

第二步: 证完全性. 设 $f\in L^2([0,2\pi]\times[0,2\pi])$ 且 $f\perp e^{imx}e^{iny}$ 对一切 $m,n\in\mathbb Z$ 成立. 由**基础知识: 富比尼定理**,

$$
0=\langle f,e^{imx}e^{iny}\rangle=\frac{1}{2\pi}\int_0^{2\pi}\left(\frac{1}{2\pi}\int_0^{2\pi}f(x,y)e^{-imx}\,\mathrm dx\right)e^{-iny}\,\mathrm dy.
$$

记 $c_m(y)=\frac{1}{2\pi}\int_0^{2\pi}f(x,y)e^{-imx}\,\mathrm dx$, 即 $f(\cdot,y)$ 关于 $\{e^{imx}\}$ 的 Fourier 系数. 由**引理 1.2.3 (柯西-施瓦茨不等式)**, $\left|c_m(y)\right|^2\le\frac{1}{2\pi}\int_0^{2\pi}\left|f(x,y)\right|^2\,\mathrm dx$, 对 $y$ 积分并再次用**基础知识: 富比尼定理** 得

$$
\int_0^{2\pi}\left|c_m(y)\right|^2\,\mathrm dy\le\frac{1}{2\pi}\int_0^{2\pi}\int_0^{2\pi}\left|f(x,y)\right|^2\,\mathrm dx\mathrm dy<\infty,
$$

故 $c_m\in L^2[0,2\pi]$. 而上面的等式说明 $c_m\perp e^{iny}$ 于 $L^2[0,2\pi]$ 对一切 $n$ 成立. 由**例 1.3.7 ($e^{inx}$ 构成标准正交基)**, $\{e^{iny}\}$ 是 $L^2[0,2\pi]$ 的标准正交基, 由**定理 1.3.2 (标准正交基的等价条件)** (iii), 它完全, 故 $c_m=0$ 几乎处处成立. 此对每个 $m$ 成立. 再由**例 1.3.7 ($e^{inx}$ 构成标准正交基)** 在 $x$ 变量上的完全性 (即**定理 1.3.2 (标准正交基的等价条件)** (iii)), 对几乎处处每个 $y$, $f(\cdot,y)$ 的所有 Fourier 系数为零蕴含 $f(\cdot,y)=0$ 几乎处处于 $x$, 即 $f=0$ 几乎处处于 $[0,2\pi]\times[0,2\pi]$. 故该标准正交系完全, 由**定理 1.3.2 (标准正交基的等价条件)** 它是 $L^2([0,2\pi]\times[0,2\pi])$ 的一组标准正交基. $\blacksquare$

---

## 1.3-5 (勒让德多项式构成标准正交基)

基本假设如**例 1.3.8 (勒让德多项式)**, 证明:

(i) $\{h_n:n=0,1,\cdots,n\}$ 是一组标准正交系;

(ii) $\{h_n:n=0,1,\cdots,n\}$ 是一组标准正交基.

### 解答 1.3-5

(i) 由**例 1.3.8 (勒让德多项式)**, 勒让德多项式 $P_n$ 是 $L^2[-1,1]$ 中的正交多项式系, 而单位化后的 $h_n$ 正是 $\{g_k\}$ 经过格拉姆-施密特过程得到的标准正交向量系. 故对 $i\neq j$, $\langle h_i,h_j\rangle=0$, 且 $\left\|h_i\right\|=1$. 由**定义 1.3.1 (正交系与标准正交系)**, $\{h_n:n=0,1,\cdots,N\}$ 是 $L^2[-1,1]$ 中的标准正交系.

(ii) 由**例 1.3.8 (勒让德多项式)**, $h_n$ 是 $n$ 次多项式. 由**基础知识: 格拉姆-施密特过程不改变张成空间**, $\operatorname{span}\{h_0,\cdots,h_N\}=\operatorname{span}\{g_0,\cdots,g_N\}=\operatorname{span}\{1,x,\cdots,x^N\}$. 令 $N\to\infty$ 得

$$
\overline{\operatorname{span}\{h_n:n=0,1,\cdots\}}=\overline{\operatorname{span}\{1,x,x^2,\cdots\}}=\overline{P},
$$

其中 $P$ 是多项式全体. 由**例 1.4.6 ($L^p$ 中的稠密子集)**, 多项式全体 $P$ 在 $L^2[-1,1]$ 中稠密, 故 $\overline{\operatorname{span}\{h_n\}}=L^2[-1,1]$. 由**定理 1.3.2 (标准正交基的等价条件)** (ii), $\{h_n:n=0,1,\cdots\}$ 是 $L^2[-1,1]$ 的一组标准正交基. $\blacksquare$

---

## 1.3-7 (带权 $L^2$ 空间是希尔伯特空间)

设 $\omega(t)$ 是 $\mathbb R$ 上 Lebesgue 可积的非负函数. 令

$$
H=\{f\text{ 是 }\mathbb R\text{ 上 Lebesgue 可测函数: }\int_{\mathbb R}\left|f(t)\right|^2\omega(t)\,\mathrm dt<\infty\}.
$$

证明: $H$ 按通常函数的线性运算以及内积

$$
\langle f,g\rangle=\int_{\mathbb R}f(t)\overline{g(t)}\omega(t)\,\mathrm dt,\quad\forall f,g\in H
$$

成为 Hilbert 空间.

### 解答 1.3-7

以下按几乎处处相等的等价类讨论.

第一步: $H$ 是线性空间. 对 $f,g\in H$ 与 $\alpha,\beta\in\mathbb K$, 由**基础知识: 平方展开估计** $(\left|a\right|+\left|b\right|)^2\le2\left|a\right|^2+2\left|b\right|^2$,

$$
\left|\alpha f+\beta g\right|^2\omega\le2\left|\alpha\right|^2\left|f\right|^2\omega+2\left|\beta\right|^2\left|g\right|^2\omega\in L^1(\mathbb R),
$$

故 $\int_{\mathbb R}\left|\alpha f+\beta g\right|^2\omega\,\mathrm dt<\infty$, 即 $\alpha f+\beta g\in H$. 故 $H$ 是线性空间.

第二步: $\langle\cdot,\cdot\rangle$ 是内积. 由**定义 1.2.3 (内积空间)** 逐条验证. (i) 共轭对称性:

$$
\langle f,g\rangle=\int_{\mathbb R}f\overline g\,\omega=\overline{\int_{\mathbb R}g\overline f\,\omega}=\overline{\langle g,f\rangle}.
$$

(ii) 对第一变元的线性性: 由**基础知识: 积分的线性性**, $\langle\alpha f+\beta g,h\rangle=\alpha\langle f,h\rangle+\beta\langle g,h\rangle$. (iii) 正定性: $\langle f,f\rangle=\int_{\mathbb R}\left|f\right|^2\omega\,\mathrm dt\ge0$, 且

$$
\langle f,f\rangle=0\Leftrightarrow\int_{\mathbb R}\left|f\right|^2\omega\,\mathrm dt=0\Leftrightarrow\left|f\right|^2\omega=0\ \text{a.e.}\Leftrightarrow f=0\ \text{a.e.},
$$

其中倒数第二步用**基础知识: 勒贝格积分的性质**. 故 $\langle\cdot,\cdot\rangle$ 是 $H$ 上的内积.

第三步: 完备性. 设 $\{f_n\}$ 是 $H$ 中的基本点列, 即 $\left\|f_n-f_m\right\|_H^2=\int_{\mathbb R}\left|f_n-f_m\right|^2\omega\,\mathrm dt\to0$. 定义映射 $T:H\to L^2(\mathbb R)$, $Tf=f\sqrt{\omega}$. 则

$$
\left\|Tf_n-Tf_m\right\|_{L^2}^2=\int_{\mathbb R}\left|f_n-f_m\right|^2\omega\,\mathrm dt=\left\|f_n-f_m\right\|_H^2\to0,
$$

故 $\{Tf_n\}$ 是 $L^2(\mathbb R)$ 中的基本点列. 由**例 1.2.8 ($L^p(E)$ 是巴拿赫空间)**, $L^2(\mathbb R)$ 完备, 故存在 $g\in L^2(\mathbb R)$ 使 $\left\|Tf_n-g\right\|_{L^2}\to0$. 令

$$
f(t)=\begin{cases}g(t)/\sqrt{\omega(t)},&\omega(t)>0,\\0,&\omega(t)=0.\end{cases}
$$

则 $f$ 可测, 且 $\int_{\mathbb R}\left|f\right|^2\omega\,\mathrm dt=\int_{\mathbb R}\left|g\right|^2\,\mathrm dt<\infty$, 故 $f\in H$. 又 $\left\|f_n-f\right\|_H=\left\|Tf_n-g\right\|_{L^2}\to0$, 即 $\{f_n\}$ 在 $H$ 中收敛于 $f$. 故 $H$ 按内积诱导的度量完备. 由**基础知识: 希尔伯特空间的定义**, $H$ 是希尔伯特空间. $\blacksquare$

---

## 1.3-8 (标准正交系重排后 Fourier 级数极限不变)

设 $\mathfrak F=\{e_1,e_2,\cdots,e_n,\cdots\}$ 是 Hilbert 空间 $(H,\langle\cdot,\cdot\rangle)$ 的一组标准正交系, 将 $\mathfrak F$ 重排成另一个序列 $\{e_1',e_2',\cdots,e_n',\cdots\}$. 证明: 对于 $x\in H$,

$$
\lim_{n\to\infty}\sum_{k=1}^n\langle x,e_k\rangle e_k=\lim_{n\to\infty}\sum_{k=1}^n\langle x,e_k'\rangle e_k'.
$$

### 解答 1.3-8

记 $S_n=\sum_{k=1}^n\langle x,e_k\rangle e_k$, $S_n'=\sum_{k=1}^n\langle x,e_k'\rangle e_k'$.

第一步: 证两个极限都存在. 由**定理 1.3.1 (贝塞尔不等式)**, $\sum_{k=1}^{\infty}\left|\langle x,e_k\rangle\right|^2\le\left\|x\right\|^2<\infty$. 对 $m<n$, 由标准正交性 (**定义 1.3.1 (正交系与标准正交系)**) 与**定理 1.2.2 (勾股定理, 毕达哥拉斯定理)**,

$$
\left\|S_n-S_m\right\|^2=\left\|\sum_{k=m+1}^n\langle x,e_k\rangle e_k\right\|^2=\sum_{k=m+1}^n\left|\langle x,e_k\rangle\right|^2\to0\quad(m,n\to\infty).
$$

故 $\{S_n\}$ 是 $H$ 中的基本点列. 由**基础知识: 希尔伯特空间的定义** ($H$ 完备), $S_n$ 收敛, 记 $S=\lim_{n\to\infty}S_n$; 同理 $S_n'$ 收敛, 记 $S'=\lim_{n\to\infty}S_n'$.

第二步: 证 $S=S'$. 对任意固定的 $j$, 由**引理 1.2.4 (内积的连续性)** 与标准正交性,

$$
\langle S,e_j\rangle=\lim_{n\to\infty}\sum_{k=1}^n\langle x,e_k\rangle\langle e_k,e_j\rangle=\langle x,e_j\rangle.
$$

同理, 因 $\{e_k'\}$ 是 $\{e_k\}$ 的重排, 序列 $\{e_k'\}$ 中恰有一项等于 $e_j$, 其余各项均与 $e_j$ 正交, 故

$$
\langle S',e_j\rangle=\lim_{n\to\infty}\sum_{k=1}^n\langle x,e_k'\rangle\langle e_k',e_j\rangle=\langle x,e_j\rangle.
$$

两式相减得 $\langle S-S',e_j\rangle=0$ 对一切 $j$ 成立. 由**引理 1.2.4 (内积的连续性)**, $\langle S-S',z\rangle=0$ 对一切 $z\in\overline{\operatorname{span}\{e_k\}}$ 成立. 而每个 $S_n\in\operatorname{span}\{e_k\}$, 故 $S\in\overline{\operatorname{span}\{e_k\}}$; 同理 $S'\in\overline{\operatorname{span}\{e_k\}}$. 于是 $S-S'\in\overline{\operatorname{span}\{e_k\}}$, 特别地 $\langle S-S',S-S'\rangle=0$. 由**定义 1.2.3 (内积空间)** (iii) 的正定性, $S-S'=0$, 即 $S=S'$. $\blacksquare$

---

## 1.3-10 (完全但不完备的标准正交系)

令 $f_0=1+\sum_{n=1}^{\infty}\frac{1}{n}(\cos nx+\sin nx)$. 设 $H$ 是 $L^2[0,2\pi]$ 中由

$$
\{f_0,\cos x,\sin x,\cdots,\cos nx,\sin nx,\cdots\}
$$

张成的线性子空间. 给出 $H$ 中的一组完全标准正交系, 但不是完备的.

### 解答 1.3-10

取 $\mathcal E=\{\sqrt2\cos nx,\sqrt2\sin nx:n=1,2,\cdots\}$.

第一步: $\mathcal E$ 是 $H$ 中的标准正交系. 由**例 1.3.3 (三角多项式标准正交系)**, $\{1,\sqrt2\cos nx,\sqrt2\sin nx:n\ge1\}$ 是 $L^2[0,2\pi]$ 的标准正交系. 由**定义 1.3.1 (正交系与标准正交系)**, 标准正交系的子集仍是标准正交系, 故 $\mathcal E$ 是 $L^2[0,2\pi]$ 的标准正交系. 又 $\sqrt2\cos nx,\sqrt2\sin nx\in H$ (因为 $\cos nx,\sin nx\in H$ 且 $H$ 是线性子空间), 故 $\mathcal E$ 是 $H$ 中的标准正交系.

第二步: $\mathcal E$ 在 $H$ 中完全. 设 $x\in H$ 且 $x\perp\mathcal E$. 由 $H=\operatorname{span}\{f_0,\cos nx,\sin nx:n\ge1\}$ 是有限线性组合全体, 存在 $c_0\in\mathbb K$ 与有限个 $c_k,d_k$ 使

$$
x=c_0f_0+\sum_{k=1}^{N}(c_k\cos kx+d_k\sin kx).
$$

对 $k\ge1$, 由 $x\perp\mathcal E$ 与 $\mathcal E$ 中元素分别与 $\cos kx,\sin kx$ 只相差常数倍, 故 $x\perp\cos kx$ 且 $x\perp\sin kx$. 由**例 1.3.3 (三角多项式标准正交系)** 计算得 $\langle\cos kx,\cos kx\rangle=\frac12$, 且 $f_0$ 展开式中 $\cos kx$ 的系数为 $\frac{1}{k}$, 故 $\langle f_0,\cos kx\rangle=\frac{1}{k}\cdot\frac{1}{2}=\frac{1}{2k}$. 于是

$$
0=\langle x,\cos kx\rangle=c_0\langle f_0,\cos kx\rangle+c_k\langle\cos kx,\cos kx\rangle=\frac{c_0}{2k}+\frac{c_k}{2},
$$

即 $c_k=-\frac{c_0}{k}$. 同理, $0=\langle x,\sin kx\rangle$ 给出 $d_k=-\frac{c_0}{k}$. 由于 $x$ 是有限线性组合, 当 $k>N$ 时 $c_k=d_k=0$, 代入 $c_k=-c_0/k$ 得 $c_0=0$, 从而一切 $c_k=d_k=0$, 即 $x=0$. 由**定理 1.3.2 (标准正交基的等价条件)** (iii), $\mathcal E$ 在 $H$ 中完全.

第三步: $\mathcal E$ 不完备. 取 $x=f_0\in H$. 由**例 1.3.3 (三角多项式标准正交系)** 计算得 $\langle1,1\rangle=1$, $\langle\cos nx,\cos nx\rangle=\langle\sin nx,\sin nx\rangle=\frac12$, 且不同项互相正交, 故

$$
\left\|f_0\right\|^2=\langle1,1\rangle+\sum_{n=1}^{\infty}\frac{1}{n^2}(\langle\cos nx,\cos nx\rangle+\langle\sin nx,\sin nx\rangle)=1+\sum_{n=1}^{\infty}\frac{1}{n^2}.
$$

由**基础知识: 巴塞尔问题**, $\sum_{n=1}^{\infty}\frac{1}{n^2}=\frac{\pi^2}{6}$, 故 $\left\|f_0\right\|^2=1+\frac{\pi^2}{6}$. 另一方面, $\langle f_0,\sqrt2\cos nx\rangle=\frac{1}{n}\langle\cos nx,\sqrt2\cos nx\rangle=\frac{\sqrt2}{2n}=\frac{1}{\sqrt2\,n}$, 同理 $\langle f_0,\sqrt2\sin nx\rangle=\frac{1}{\sqrt2\,n}$, 故

$$
\sum_{e\in\mathcal E}\left|\langle f_0,e\rangle\right|^2=\sum_{n=1}^{\infty}\left(\frac{1}{2n^2}+\frac{1}{2n^2}\right)=\sum_{n=1}^{\infty}\frac{1}{n^2}=\frac{\pi^2}{6}<1+\frac{\pi^2}{6}=\left\|f_0\right\|^2.
$$

即帕塞瓦尔等式不成立. 由**定理 1.3.2 (标准正交基的等价条件)** (iv), $\mathcal E$ 不完备.

综上, $\mathcal E=\{\sqrt2\cos nx,\sqrt2\sin nx:n=1,2,\cdots\}$ 是 $H$ 中的一组完全但不完备的标准正交系. $\blacksquare$
