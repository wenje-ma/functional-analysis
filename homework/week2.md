# week 2

> **定义 1.1.2** (极限) 设 $\left(X,d\right)$ 是度量空间, $\left\{x_n\right\}_{n=1}^\infty$ 是 $X$ 中点列, $x_0\in X$, 若 $$\lim_{n\to\infty}d\left(x_n,x_0\right)=0,$$ 则称**点列 $\left\{x_n\right\}_{n=1}^\infty$ 按照度量 $d$ 收敛于 $x_0$**, 记为 $\lim_{n\to\infty}x_n=x_0$.

> **定义 1.2.2** (半范数与范数) 记 $\mathbb K$ 是实数域 $\mathbb R$ 或复数域 $\mathbb C$. 对于 $\mathbb K$ 上的线性空间 $X$, 若 $X$ 中的每个向量都对应一个实数 $\left\|x\right\|$, 且满足如下条件:<br>(i) 对任意 $x\in X$, $\left\|x\right\|\ge0$;<br>(ii) 对数 $\alpha$ 与 $x\in X$, $\left\|\alpha x\right\|=\left|\alpha\right|\left\|x\right\|$;<br>(iii) 对任意 $x,y\in X$, $\left\|x+y\right\|\le\left\|x\right\|+\left\|y\right\|$,<br>则称 $\left\|\cdot\right\|$ 为 $X$ 上的**半范数**, $X$ 称为半赋范空间. 若 $\left\|\cdot\right\|$ 还满足 $\left\|x\right\|=0$ 当且仅当 $x=0$, 则称 $\left\|\cdot\right\|$ 为 $X$ 上的**范数**, $\left(X,\left\|\cdot\right\|\right)$ 称为**赋范线性空间**.<br>线性空间上的范数诱导了这个空间上的度量 $d\left(x,y\right)=\left\|x-y\right\|$, 这个度量具有平移不变性, 即 $d\left(x,y\right)=d\left(x+z,y+z\right)$.

> **定义 1.2.3** (内积空间) 记 $\mathbb K$ 是实数域 $\mathbb R$ 或复数域 $\mathbb C$. 对于 $\mathbb K$ 上的线性空间 $H$, 如果 $H$ 中任何两个向量 $x,y$ 都对应着一个数 $\left\langle x,y\right\rangle\in\mathbb K$, 满足条件:<br>(i) **(共轭对称性)** 对任意 $x,y\in H$, $\left\langle x,y\right\rangle=\overline{\left\langle y,x\right\rangle}$;<br>(ii) **(对第一变元的线性性)** 对任意 $x,y,z\in H$, $\alpha,\beta\in\mathbb K$, $\left\langle\alpha x+\beta y,z\right\rangle=\alpha\left\langle x,z\right\rangle+\beta\left\langle y,z\right\rangle$;<br>(iii) **(正定性)** 对任意 $x\in H$, $\left\langle x,x\right\rangle\ge0$, 且 $\left\langle x,x\right\rangle=0$ 的充要条件是 $x=0$,<br>那么称 $\left\langle\cdot,\cdot\right\rangle$ 是 $H$ 中的**内积**, 称 $H$ 是实 (或复) **内积空间**.

> **定义** (线性无关组) 对于线性空间 $X$, $X$ 中的**线性无关组**是指 $X$ 中的一些元素构成的子集 $A$, 使得子集 $A$ 中任意一个元素都不能被 $A$ 中其他有限个元素线性表出.

> **定义** (正交补) 设 $H$ 是内积空间, 对于 $x\in H$, $A\subset H$, 若对每个 $y\in A$ 有 $x\perp y$, 则称 $x\perp A$. 并记 $$A^\perp=\left\{x\in H:x\perp A\right\}.$$

> **定义** (希尔伯特空间) 若内积空间 $H$ 所导出的度量是完备的, 则称 $H$ 是一个 **希尔伯特空间**.

> **引理 1.2.4** (内积的连续性) 设 $H$ 是内积空间, 那么内积关于两个变元是连续的, 即: 当 $x_n\to x$, $y_n\to y$ 时, 有 $\left\langle x_n,y_n\right\rangle\to\left\langle x,y\right\rangle$.

> **定义 1.3.1** (正交系与标准正交系) 设 $\mathcal F$ 是希尔伯特空间 $H$ 中的一族非零向量.<br>(i) 如果 $\mathcal F$ 中任何两个不同的向量都正交, 就称 $\mathcal F$ 是 $H$ 的**正交系**;<br>(ii) 如果正交系 $\mathcal F$ 中每个向量的范数都等于 $1$, 就称 $\mathcal F$ 是**标准正交系** (或规范正交系).

> **定理 1.3.1** (贝塞尔不等式) 设 $\mathcal F=\left\{e_\lambda:\lambda\in\Lambda\right\}$ 是希尔伯特空间 $H$ 中的标准正交系. 那么, 对于每个 $x\in H$, 它的傅里叶系数 $\left\{\left\langle x,e_\lambda\right\rangle:\lambda\in\Lambda\right\}$ 中最多只有可列个不为零, 并且还成立如下的贝塞尔不等式: $$\sum_{\lambda\in\Lambda}\left|\left\langle x,e_\lambda\right\rangle\right|^2\le\left\|x\right\|^2.$$

> **定理 1.3.2** (标准正交基的等价条件) 设 $\mathcal F=\left\{e_\lambda:\lambda\in\Lambda\right\}$ 是希尔伯特空间 $H$ 中的标准正交系, 下列命题等价:<br>(i) 对 $H$ 中任意元素 $x$, 有 $x=\sum\limits_{\lambda\in\Lambda}\left\langle x,e_\lambda\right\rangle e_\lambda$;<br>(ii) $\overline{\operatorname{span}\left\{e_\lambda:\lambda\in\Lambda\right\}}=H$;<br>(iii) $\left\{e_\lambda:\lambda\in\Lambda\right\}$ 是**完全的**, 即: 若 $x\in H$ 满足 $x\perp e_\lambda$ ( $\forall\lambda\in\Lambda$ ), 则 $x=0$;<br>(iv) $\left\{e_\lambda:\lambda\in\Lambda\right\}$ 是**完备的**, 即: 对 $H$ 中任意元素 $x$, 帕塞瓦尔等式 $\left\|x\right\|^2=\sum\limits_{\lambda\in\Lambda}\left|\left\langle x,e_\lambda\right\rangle\right|^2$ 成立.<br>我们称满足上述条件之一的标准正交系为希尔伯特空间 $H$ 中的一组**标准正交基** (或规范正交基).

> **注 1.3.1** 在使用定义 1.3.3 时, 注意到 $\left\{e_\lambda:\left\langle x,e_\lambda\right\rangle\neq0\right\}$ 是可数集, 将其排列为一个序列 $\left\{e_{\lambda_1},e_{\lambda_2},\cdots,e_{\lambda_n},\cdots\right\}$. 根据贝塞尔不等式 $\sum_k\left|\left\langle x,e_{\lambda_k}\right\rangle\right|^2<\infty$, 再由 $\left\|\sum_{k=n+1}^m\left\langle x,e_{\lambda_k}\right\rangle e_{\lambda_k}\right\|^2=\sum_{k=n+1}^m\left|\left\langle x,e_{\lambda_k}\right\rangle\right|^2$, 可知 $\sum_{k=1}^n\left\langle x,e_{\lambda_k}\right\rangle e_{\lambda_k}$ 是 $H$ 中的基本点列, 因此其极限存在, 同时也可以说明这个极限与可数集 $\left\{e_\lambda:\left\langle x,e_\lambda\right\rangle\neq0\right\}$ 所取的排列顺序无关 (见习题 1.3 第 8 题).

> **例 1.3.3** 在实 (或复) 周期函数空间 $L^2\left[0,2\pi\right]$ 中, 规定内积为 $$\left\langle f,g\right\rangle=\frac{1}{2\pi}\int_0^{2\pi}f\left(x\right)\overline{g\left(x\right)}\,\mathrm dx,\quad\forall f,g\in L^2\left[0,2\pi\right],$$ 这时 $\left\{1,\sqrt2\cos x,\sqrt2\sin x,\sqrt2\cos2x,\sqrt2\sin2x,\cdots,\sqrt2\cos nx,\sqrt2\sin nx,\cdots\right\}$ 组成 $L^2\left[0,2\pi\right]$ 的标准正交系.

> **例 1.3.7** 在复空间 $L^2\left[0,2\pi\right]$ 中, $\left\{\mathrm{e}^{\mathrm{i}nx}:n\in\mathbb Z\right\}$ 是一组标准正交基.

> **例 1.3.8** (勒让德多项式) 在 $L^2\left[-1,1\right]$ 中, 函数列 $g_k\left(x\right)=x^k\left(k=0,1,2,\cdots\right)$ 是线性无关的. 可以证明勒让德多项式 $$P_0\left(x\right)=1,\quad P_n\left(x\right)=\frac{1}{2^n n!}\frac{\mathrm d^n}{\mathrm dx^n}\left(x^2-1\right)^n,\quad n=1,2,\cdots$$ 是 $L^2\left[-1,1\right]$ 中的正交多项式系. 将勒让德多项式单位化得到 $$h_0\left(x\right)=\frac{1}{\sqrt2},\quad h_n\left(x\right)=\frac{1}{2^n n!}\sqrt{\frac{2n+1}{2}}\frac{\mathrm d^n}{\mathrm dx^n}\left(x^2-1\right)^n,\quad n=1,2,\cdots$$ 就是 $\left\{g_n\right\}$ 经过格拉姆-施密特过程得到的标准正交向量系. 又由于多项式全体在 $L^2\left[-1,1\right]$ 中稠密 (见例 1.4.6), 因此 $\left\{h_n:n=0,1,\cdots\right\}$ 构成了一组标准正交基 (见习题 1.3 第 5 题).

> **定义 1.4.5** (稠密性) 在度量空间 $\left(X,d\right)$ 中, 对于 $X$ 中一个子集 $A$, 我们称 $A$ 在 $X$ 中**稠密**是指 $\overline A=X$.

> **例 1.4.6** 对直线上有界闭区间 $\left[a,b\right]$ 及 $1\le p<\infty$, $L^p\left[a,b\right]$ 中的简单函数全体, 阶梯函数全体, $C_c^\infty\left(a,b\right)$, $C\left[a,b\right]$ 以及多项式全体 $P$ 均是 $L^p\left[a,b\right]$ 的稠密子集.

> **注 1.4.1** (i) 类似地, 可得 $L^p\left(\mathbb R^n\right)$ ( $1\le p<\infty$ ) 中的简单函数全体, 阶梯函数全体以及 $C_c^\infty\left(\mathbb R^n\right)$ 均是稠密子集.

> **例 1.2.8** ( $L^p\left(E\right)$ 的完备性) 设 $E$ 是欧几里得空间 $\mathbb R^k$ 的勒贝格可测集, 对 $1\le p<\infty$, $L^p\left(E\right)$ 按范数 $\left\|f\right\|_p=\left(\int_E\left|f\right|^p\mathrm dm\right)^{1/p}$ 成为赋范线性空间. 若 $\left\{f_n\right\}$ 是 $L^p\left(E\right)$ 中的基本点列, 则 $\left\|f_n-f_m\right\|_p\to0$; 由切比雪夫不等式, 这个函数序列依测度柯西收敛, 由实变函数的理论可取可测函数 $f_0$ 为 $\left\{f_n\right\}$ 的依测度收敛极限; 由法图引理, $\left\|f_n-f_0\right\|_p^p=\int_E\left|f_n-f_0\right|^p\mathrm dm\le\liminf\limits_{m\to\infty}\int_E\left|f_n-f_m\right|^p\mathrm dm\to0$, 从而 $f_0\in L^p\left(E\right)$ 且为 $\left\{f_n\right\}$ 的极限, 即 $L^p\left(E\right)$ 是完备的 (巴拿赫空间).

## 1

证明 $C_c^\infty\left(\mathbb R^n\right)$ 在 $L^p\left(\mathbb R^n\right)$ 中稠密.

### 解答 1

依据**定义 1.4.5 (稠密性)**, 且闭包是极限点的集合, 因此只需证明 $L^p\left(\mathbb R^n\right)$ 中的每一个点都可以是 $C_c^\infty\left(\mathbb R^n\right)$ 的极限点即可, 即证: 对任意 $f\in L^p\left(\mathbb R^n\right)$ 与任意 $\epsilon>0$, 存在 $\varphi\in C_c^\infty\left(\mathbb R^n\right)$ 使得 $\left\|f-\varphi\right\|_p<\epsilon$.

由**例 1.4.6** 及**注 1.4.1 (i)**, $L^p\left(\mathbb R^n\right)$ 中简单函数全体、阶梯函数全体以及 $C_c^\infty\left(\mathbb R^n\right)$ 均是稠密子集, 则:

(1) 由实变函数知识, 对任意 $f\in L^p\left(\mathbb R^n\right)$, 可取简单函数列 $\left\{\Phi_n\right\}$ 点态收敛于 $f$, 且 $\left|\Phi_n\right|\le\left|f\right|$ ($\forall n$), 由勒贝格控制收敛定理得

$$
\begin{aligned}
&\quad\;\lim_{n\to\infty}\left\|f-\Phi_n\right\|_p\propto\lim_{n\to\infty}\int_{\mathbb R^n}\left|f-\Phi_n\right|^p\,\mathrm dm\\
&=\int_{\mathbb R^n}\lim_{n\to\infty}\left|f-\Phi_n\right|^p\,\mathrm dm=\int_{\mathbb R^n}\lim_{n\to\infty}0\,\mathrm dm=0.
\end{aligned}
$$

故只需说明特征函数可由 $C_c^\infty\left(\mathbb R^n\right)$ 中函数逼近.

(2) 接下来便使用光滑紧支函数 $\psi$ 在 $L^p$ 范数下逼近特征函数 $\chi_E$. 对 $\mathbb R^n$ 中任意勒贝格可测集 $E$ ($m\left(E\right)<\infty$), 存在紧集 $K\subset E$ 与开集 $U\supset E$ 使得 $m\left(U\setminus K\right)<\epsilon$; 利用卷积可构造 $\psi\in C_c^\infty\left(\mathbb R^n\right)$ 满足 $0\le\psi\le1$, $\psi\equiv1$ 于 $K$ 上, $\operatorname{supp}\psi\subset U$, 从而 $\left\|\chi_E-\psi\right\|_p\le m\left(U\setminus K\right)^{1/p}<\epsilon$.

(3) 由线性性, 任意简单函数 $\Phi=\sum_i c_i\chi_{E_i}$ 均可被 $C_c^\infty\left(\mathbb R^n\right)$ 中函数 $\varphi$ 逼近: 对每个 $i$ 取 $\psi_i$ 逼近 $\chi_{E_i}$, 令 $\varphi=\sum_i c_i\psi_i\in C_c^\infty\left(\mathbb R^n\right)$, 则 $\left\|\Phi-\varphi\right\|_p\le\sum_i\left|c_i\right|\left\|\chi_{E_i}-\psi_i\right\|_p$ 可任意小.

综上, 对任意 $f\in L^p\left(\mathbb R^n\right)$ 与 $\epsilon>0$, 存在 $\varphi\in C_c^\infty\left(\mathbb R^n\right)$ 使 $\left\|f-\varphi\right\|_p<\epsilon$, 故 $C_c^\infty\left(\mathbb R^n\right)$ 在 $L^p\left(\mathbb R^n\right)$ 中稠密. $\blacksquare$

---

## 2 (习题 1.2)

3. 设 $L$ 是赋范线性空间, $L\times L$ 按照线性运算:

$$
\alpha\left(x_1,y_1\right)+\beta\left(x_2,y_2\right)=\left(\alpha x_1+\beta x_2,\alpha y_1+\beta y_2\right)
$$

成为线性空间. 在 $L\times L$ 上定义两个范数如下:

$$
\left\|\left(x,y\right)\right\|_1=\sqrt{\left\|x\right\|^2+\left\|y\right\|^2},\quad\left\|\left(x,y\right)\right\|_2=\max\left\{\left\|x\right\|,\left\|y\right\|\right\}.
$$

(i) 证明: $\left(L\times L,\left\|\cdot\right\|_1\right)$ 和 $\left(L\times L,\left\|\cdot\right\|_2\right)$ 都是赋范线性空间.

(ii) 作 $\left(L\times L,\left\|\cdot\right\|_1\right)$ 到 $\left(L\times L,\left\|\cdot\right\|_2\right)$ 的映射:

$$
\varphi\colon\left(x,y\right)\mapsto\left(x',y'\right),\quad\left(x',y'\right)=\left(x,y\right)\begin{bmatrix}a&b\\c&d\end{bmatrix},
$$

其中矩阵 $\begin{bmatrix}a&b\\c&d\end{bmatrix}$ 是非奇异的. 证明: $\varphi$ 是拓扑同胚 (即 $\varphi$ 是到上的一一对应, 且 $\varphi$ 和 $\varphi^{-1}$ 都是连续的).

### 解答 2-3

(i) 依据**定义 1.2.2 (半范数与范数)**, 逐条验证.

**$\left\|\cdot\right\|_1$ 是范数.** 非负性显然. 正定性:

$$
\left\|\left(x,y\right)\right\|_1=0\Leftrightarrow\left\|x\right\|=\left\|y\right\|=0\Leftrightarrow x=y=0.
$$

齐性:

$$
\left\|\alpha\left(x,y\right)\right\|_1=\sqrt{\left\|\alpha x\right\|^2+\left\|\alpha y\right\|^2}=\left|\alpha\right|\sqrt{\left\|x\right\|^2+\left\|y\right\|^2}=\left|\alpha\right|\left\|\left(x,y\right)\right\|_1.
$$

三角不等式:

$$
\begin{aligned}
&\quad\;\left\|\left(x,y\right)+\left(x',y'\right)\right\|_1\\
&=\sqrt{\left\|x+x'\right\|^2+\left\|y+y'\right\|^2}\\
&\le\sqrt{\left(\left\|x\right\|+\left\|x'\right\|\right)^2+\left(\left\|y\right\|+\left\|y'\right\|\right)^2}\\
&\le\sqrt{\left\|x\right\|^2+\left\|y\right\|^2}+\sqrt{\left\|x'\right\|^2+\left\|y'\right\|^2},
\end{aligned}
$$

其中第一个不等号由 $\left\|\cdot\right\|$ 的三角不等式, 第二个不等号为 $\mathbb R^2$ 上 Euclid 范数的三角不等式. 故 $\left\|\cdot\right\|_1$ 是范数.

**$\left\|\cdot\right\|_2$ 是范数.** 非负性显然. 正定性:

$$
\left\|\left(x,y\right)\right\|_2=0\Leftrightarrow\max\left\{\left\|x\right\|,\left\|y\right\|\right\}=0\Leftrightarrow\left\|x\right\|=\left\|y\right\|=0\Leftrightarrow x=y=0.
$$

齐性:

$$
\left\|\alpha\left(x,y\right)\right\|_2=\max\left\{\left|\alpha\right|\left\|x\right\|,\left|\alpha\right|\left\|y\right\|\right\}=\left|\alpha\right|\max\left\{\left\|x\right\|,\left\|y\right\|\right\}=\left|\alpha\right|\left\|\left(x,y\right)\right\|_2.
$$

三角不等式:

$$
\begin{aligned}
&\quad\;\left\|\left(x,y\right)+\left(x',y'\right)\right\|_2\\
&=\max\left\{\left\|x+x'\right\|,\left\|y+y'\right\|\right\}\\
&\le\max\left\{\left\|x\right\|+\left\|x'\right\|,\left\|y\right\|+\left\|y'\right\|\right\}\\
&\le\max\left\{\left\|x\right\|,\left\|y\right\|\right\}+\max\left\{\left\|x'\right\|,\left\|y'\right\|\right\}.
\end{aligned}
$$

故 $\left\|\cdot\right\|_2$ 是范数. 因此 $\left(L\times L,\left\|\cdot\right\|_1\right)$ 与 $\left(L\times L,\left\|\cdot\right\|_2\right)$ 都是赋范线性空间. $\blacksquare$

(ii) 先证 **$\varphi$ 是到上的一一对应**. 矩阵 $\begin{bmatrix}a&b\\c&d\end{bmatrix}$ 非奇异, 故其逆矩阵存在, 记 $\begin{bmatrix}a&b\\c&d\end{bmatrix}^{-1}=\begin{bmatrix}a'&b'\\c'&d'\end{bmatrix}$.

对任意 $\left(x',y'\right)\in L\times L$, 令 $\left(x,y\right)=\left(x',y'\right)\begin{bmatrix}a'&b'\\c'&d'\end{bmatrix}$, 则 $\varphi\left(x,y\right)=\left(x',y'\right)$, 且 $\left(x,y\right)$ 由 $\left(x',y'\right)$ 唯一确定. 故 $\varphi$ 是到上的一一对应.

再证 **$\varphi$ 连续**. 设 $\left(x_n,y_n\right)\to\left(x,y\right)$ 按 $\left\|\cdot\right\|_1$, 即 $\left\|x_n-x\right\|\to0$, $\left\|y_n-y\right\|\to0$. 由**定义 1.2.2 (半范数与范数)** 的三角不等式与齐性,

$$
\begin{aligned}
&\quad\;\left\|\varphi\left(x_n,y_n\right)-\varphi\left(x,y\right)\right\|_2\\
&=\max\left\{\left\|a\left(x_n-x\right)+b\left(y_n-y\right)\right\|,\left\|c\left(x_n-x\right)+d\left(y_n-y\right)\right\|\right\}\\
&\le\max\left\{\left(\left|a\right|+\left|b\right|\right)\delta_n,\left(\left|c\right|+\left|d\right|\right)\delta_n\right\}\to0,
\end{aligned}
$$

其中 $\delta_n=\max\left\{\left\|x_n-x\right\|,\left\|y_n-y\right\|\right\}\to0$. 依据**定义 1.1.2 (极限)**, $\varphi$ 连续.

$\varphi^{-1}$ 由逆矩阵给出: $\varphi^{-1}\left(x',y'\right)=\left(x',y'\right)\begin{bmatrix}a'&b'\\c'&d'\end{bmatrix}$, 同理可知 $\varphi^{-1}$ 也连续. 故 $\varphi$ 是拓扑同胚. $\blacksquare$

---

6. 设 $C_b\left(0,1\right]$ 表示在半开半闭区间 $\left(0,1\right]$ 上处处连续且有界的函数全体. 对于每个 $x\in C_b\left(0,1\right]$, 令

$$
\left\|x\right\|=\sup_{0<t\le 1}\left|x\left(t\right)\right|.
$$

证明:

(i) $\left\|x\right\|$ 是空间 $C_b\left(0,1\right]$ 上的范数；$C_b\left(0,1\right]$ 按 $\left\|\cdot\right\|$ 成为赋范线性空间；

(ii) 在 $C_b\left(0,1\right]$ 中点列 $\left\{x_n\right\}$ 按范数 $\left\|\cdot\right\|$ 收敛于 $x_0$ 的充要条件是 $\left\{x_n\right\}$ 在 $\left(0,1\right]$ 上一致收敛于 $x_0$.

### 解答 2-6

(i) 首先, $C_b\left(0,1\right]$ 按通常函数的线性运算成为线性空间: 有界连续函数的线性组合仍有界且连续. 依据**定义 1.2.2 (半范数与范数)**, 只需验证 $\left\|\cdot\right\|$ 是范数.

非负性:

$$
\left\|x\right\|=\sup\limits_{0<t\le1}\left|x\left(t\right)\right|\ge0.
$$

正定性:

$$
\left\|x\right\|=0\Leftrightarrow\sup\limits_{0<t\le1}\left|x\left(t\right)\right|=0\Leftrightarrow x\left(t\right)=0\left(\forall 0<t\le1\right)\Leftrightarrow x=0.
$$

齐性:

$$
\left\|\alpha x\right\|=\sup\left|\alpha x\left(t\right)\right|=\left|\alpha\right|\sup\left|x\left(t\right)\right|=\left|\alpha\right|\left\|x\right\|.
$$

三角不等式: 对任意 $x,y\in C_b\left(0,1\right]$ 与 $t\in\left(0,1\right]$,

$$
\left|x\left(t\right)+y\left(t\right)\right|\le\left|x\left(t\right)\right|+\left|y\left(t\right)\right|\le\left\|x\right\|+\left\|y\right\|,
$$

对 $t$ 取上确界得 $\left\|x+y\right\|\le\left\|x\right\|+\left\|y\right\|$. 故 $\left\|\cdot\right\|$ 是 $C_b\left(0,1\right]$ 上的范数, $C_b\left(0,1\right]$ 按 $\left\|\cdot\right\|$ 成为赋范线性空间. $\blacksquare$

(ii) 依据**定义 1.1.2 (极限)**, $\left\{x_n\right\}$ 按范数 $\left\|\cdot\right\|$ 收敛于 $x_0$ 当且仅当

$$
\left\|x_n-x_0\right\|=\sup_{0<t\le1}\left|x_n\left(t\right)-x_0\left(t\right)\right|\to0.
$$

而 $\sup\limits_{0<t\le1}\left|x_n\left(t\right)-x_0\left(t\right)\right|\to0$ 正是 $\left\{x_n\right\}$ 在 $\left(0,1\right]$ 上一致收敛于 $x_0$ 的定义. 故两者等价. $\blacksquare$

---

10. 设 $H$ 是内积空间. 如果 $x_1,x_2,\cdots,x_n$ 是 $H$ 中的向量, 它们满足条件 $\left\langle x_i,x_j\right\rangle=\delta_{ij}$, 证明:

$$
x_1,x_2,\cdots,x_n\text{ 是一组线性无关的向量}.
$$

### 解答 2-10

设 $\sum_{i=1}^n c_i x_i=0$, 其中 $c_i\in\mathbb K$. 对任意 $j\in\left\{1,2,\cdots,n\right\}$, 取内积并依据**定义 1.2.3 (内积空间)** 中对第一变元的线性性:

$$
0=\left\langle\sum_{i=1}^n c_i x_i,x_j\right\rangle=\sum_{i=1}^n c_i\left\langle x_i,x_j\right\rangle=\sum_{i=1}^n c_i\delta_{ij}=c_j.
$$

故 $c_j=0$ 对一切 $j$ 成立, 即 $x_1,x_2,\cdots,x_n$ 中任意有限组合为零只能系数全为零. 依据**定义 (线性无关组)**, $x_1,x_2,\cdots,x_n$ 是一组线性无关的向量. $\blacksquare$

---

12. 设 $H$ 是一个希尔伯特空间.

(i) 对于 $x\in H$, $x\perp H$ 的充要条件是 $x=0$.

(ii) 对 $H$ 中的子集 $A$, $A^\perp$ 是闭的线性子空间.

(iii) 若子集 $M\subset N\subset H$, 则 $M^\perp\supset N^\perp$.

(iv) 对线性空间 $M\subset H$, $M\cap M^\perp=\left\{0\right\}$.

(v) 设 $L$ 是由 $H$ 的两个子集 $M$ 和 $N$ 张成的线性子空间, 证明 $L^\perp=M^\perp\cap N^\perp$.

### 解答 2-12

依据**定义 (正交补)**, 以下用 $x\perp A$ 表示 $x$ 与 $A$ 中每个元素正交.

(i) **$\Leftarrow$**: 若 $x=0$, 则对任意 $y\in H$, $\left\langle0,y\right\rangle=0$ (内积对第一变元线性), 故 $x\perp H$.

**$\Rightarrow$**: 若 $x\perp H$, 特别地 $x\perp x$, 即 $\left\langle x,x\right\rangle=0$. 依据**定义 1.2.3 (内积空间)** 的正定性, $x=0$. 故 $x\perp H\Leftrightarrow x=0$. $\blacksquare$

(ii) **线性**: 设 $x_1,x_2\in A^\perp$, $\alpha,\beta\in\mathbb K$. 对任意 $y\in A$, 由内积对第一变元的线性性,

$$
\left\langle\alpha x_1+\beta x_2,y\right\rangle=\alpha\left\langle x_1,y\right\rangle+\beta\left\langle x_2,y\right\rangle=0,
$$

故 $\alpha x_1+\beta x_2\in A^\perp$, $A^\perp$ 是线性子空间.

**闭性**: 设 $x_n\in A^\perp$ 且 $x_n\to x$ (按内积诱导的范数). 对任意 $y\in A$, 依据**引理 1.2.4 (内积的连续性)**, $\left\langle x,y\right\rangle=\lim\limits_{n\to\infty}\left\langle x_n,y\right\rangle=0$, 故 $x\in A^\perp$. 因此 $A^\perp$ 是闭的线性子空间. $\blacksquare$

(iii) 设 $x\in N^\perp$, 则 $x\perp y$ 对一切 $y\in N$ 成立. 因 $M\subset N$, 特别地 $x\perp y$ 对一切 $y\in M$ 成立, 即 $x\in M^\perp$. 故 $N^\perp\subset M^\perp$, 即 $M^\perp\supset N^\perp$. $\blacksquare$

(iv) 设 $x\in M\cap M^\perp$, 则 $x\in M$ 且 $x\perp M$, 特别地 $x\perp x$, 即 $\left\langle x,x\right\rangle=0$. 由**定义 1.2.3** 的正定性, $x=0$. 故 $M\cap M^\perp=\left\{0\right\}$. $\blacksquare$

(v) $L=\operatorname{span}\left(M\cup N\right)$ 由 $M,N$ 中元素的有限线性组合构成. 由内积对第一变元的线性性, 对任意 $z\in H$,

$$
\begin{aligned}
&\quad\;z\in L^\perp\Leftrightarrow\left\langle z,w\right\rangle=0,\quad\forall w\in L\\
&\Leftrightarrow\left\langle z,m\right\rangle=0,\quad\forall m\in M\text{ 且 }\left\langle z,n\right\rangle=0,\quad\forall n\in N\\
&\Leftrightarrow z\in M^\perp\text{ 且 }z\in N^\perp.
\end{aligned}
$$

故 $L^\perp=M^\perp\cap N^\perp$. $\blacksquare$

---

## 3 (习题 1.3)

1. 设 $\mathfrak{F}=\left\{e_\lambda:\lambda\in\Lambda\right\}$ 是希尔伯特空间 $H$ 的标准正交基. 证明: 对任何 $x,y\in H$,

$$
\left\langle x,y\right\rangle=\sum_{\lambda\in\Lambda}\left\langle x,e_\lambda\right\rangle\overline{\left\langle y,e_\lambda\right\rangle}.
$$

### 解答 3-1

由**定理 1.3.2 (标准正交基的等价条件)** (i), 对任何 $x,y\in H$ 有傅里叶展开

$$
x=\sum_{\lambda\in\Lambda}\left\langle x,e_\lambda\right\rangle e_\lambda,\quad y=\sum_{\mu\in\Lambda}\left\langle y,e_\mu\right\rangle e_\mu.
$$

依据**引理 1.2.4 (内积的连续性)** 与**定义 1.2.3** 中对第一变元的线性性、共轭对称性,

$$
\left\langle x,y\right\rangle=\left\langle\sum_{\lambda\in\Lambda}\left\langle x,e_\lambda\right\rangle e_\lambda,\sum_{\mu\in\Lambda}\left\langle y,e_\mu\right\rangle e_\mu\right\rangle=\sum_{\lambda,\mu\in\Lambda}\left\langle x,e_\lambda\right\rangle\overline{\left\langle y,e_\mu\right\rangle}\left\langle e_\lambda,e_\mu\right\rangle=\sum_{\lambda\in\Lambda}\left\langle x,e_\lambda\right\rangle\overline{\left\langle y,e_\lambda\right\rangle},
$$

其中最后一个等号用到 $\left\langle e_\lambda,e_\mu\right\rangle=\delta_{\lambda\mu}$ ( $\mathcal F$ 是标准正交系, **定义 1.3.1**). 证毕. $\blacksquare$

---

3. 令 $L^2\left(\left[0,2\pi\right]\times\left[0,2\pi\right]\right)$ 上的内积为

$$
\left\langle f,g\right\rangle=\iint\limits_{\left[0,2\pi\right]\times\left[0,2\pi\right]} f\left(x,y\right)\overline{g\left(x,y\right)}\frac{\mathrm dx\mathrm dy}{4\pi^2}.
$$

证明: $\left\{\mathrm{e}^{\mathrm{i}mx}\mathrm{e}^{\mathrm{i}ny}:m,n\in\mathbb Z\right\}$ 构成 $L^2\left(\left[0,2\pi\right]\times\left[0,2\pi\right]\right)$ 的一组标准正交基.

### 解答 3-3

**标准正交性.** 对任意 $m,n,m',n'\in\mathbb Z$, 乘积测度下，若二重积分的被积函数绝对值可积, 则可使用富比尼定理:

$$
\begin{aligned}
&\quad\;\left\langle \mathrm{e}^{\mathrm{i}mx}\mathrm{e}^{\mathrm{i}ny},\mathrm{e}^{\mathrm{i}m'x}\mathrm{e}^{\mathrm{i}n'y}\right\rangle\\
&=\frac{1}{4\pi^2}\iint \mathrm{e}^{\mathrm{i}\left(m-m'\right)x}\mathrm{e}^{\mathrm{i}\left(n-n'\right)y}\,\mathrm dx\mathrm dy\\
&=\left(\frac{1}{2\pi}\int_0^{2\pi}\mathrm{e}^{\mathrm{i}\left(m-m'\right)x}\,\mathrm dx\right)\left(\frac{1}{2\pi}\int_0^{2\pi}\mathrm{e}^{\mathrm{i}\left(n-n'\right)y}\mathrm dy\right)=\delta_{mm'}\delta_{nn'},
\end{aligned}
$$

其中用到**例 1.3.7**: $\left\{\mathrm{e}^{\mathrm{i}kx}\right\}$ 是 $L^2\left[0,2\pi\right]$ 的标准正交系. 故 $\left\{\mathrm{e}^{\mathrm{i}mx}\mathrm{e}^{\mathrm{i}ny}\right\}$ 是标准正交系 (依据**定义 1.3.1**).

**完全性.** 设 $f\in L^2\left(\left[0,2\pi\right]\times\left[0,2\pi\right]\right)$ 且 $f\perp \mathrm{e}^{\mathrm{i}mx}\mathrm{e}^{\mathrm{i}ny}$ ( $\forall m,n\in\mathbb Z$ ), 即 $\left\langle f,\mathrm{e}^{\mathrm{i}mx}\mathrm{e}^{\mathrm{i}ny}\right\rangle=0$. 由富比尼定理,

$$
0=\left\langle f,\mathrm{e}^{\mathrm{i}mx}\mathrm{e}^{\mathrm{i}ny}\right\rangle=\frac{1}{2\pi}\int_0^{2\pi}\left(\frac{1}{2\pi}\int_0^{2\pi}f\left(x,y\right)\mathrm{e}^{-\mathrm{i}mx}\,\mathrm dx\right)\mathrm{e}^{-\mathrm{i}ny}\mathrm dy.
$$

记 $c_m\left(y\right)=\frac{1}{2\pi}\int_0^{2\pi}f\left(x,y\right)\mathrm{e}^{-\mathrm{i}mx}\,\mathrm dx$, 即 $f\left(\cdot,y\right)$ 关于 $\left\{\mathrm{e}^{\mathrm{i}mx}\right\}$ 的傅里叶系数. 由富比尼定理, 可得 $c_m\in L^2\left[0,2\pi\right]$, 且 $\left\langle f,\mathrm{e}^{\mathrm{i}mx}\mathrm{e}^{\mathrm{i}ny}\right\rangle=0$ 说明 $c_m\perp \mathrm{e}^{\mathrm{i}ny}$ ( $\forall n\in\mathbb Z$ ) 于 $L^2\left[0,2\pi\right]$. 依据**例 1.3.7** ($\left\{\mathrm{e}^{\mathrm{i}ny}\right\}$ 是 $L^2\left[0,2\pi\right]$ 的标准正交基, 从而完全) 及**定理 1.3.2** (iii), $c_m\left(y\right)=0$ a.e. 对每个 $m$ 成立; 再由**例 1.3.7** 在 $x$ 变量的完全性, $f\left(x,y\right)=0$ a.e. 于 $\left[0,2\pi\right]\times\left[0,2\pi\right]$. 故 $\left\{\mathrm{e}^{\mathrm{i}mx}\mathrm{e}^{\mathrm{i}ny}\right\}$ 是完全的.

由**定理 1.3.2**, 完全的标准正交系即标准正交基, 因此 $\left\{\mathrm{e}^{\mathrm{i}mx}\mathrm{e}^{\mathrm{i}ny}:m,n\in\mathbb Z\right\}$ 构成 $L^2\left(\left[0,2\pi\right]\times\left[0,2\pi\right]\right)$ 的一组标准正交基. $\blacksquare$

---

5. 在 $L^2\left[-1,1\right]$ 中, 函数列 $g_k\left(x\right)=x^k\left(k=0,1,2,\cdots\right)$ 是线性无关的. 因此可以用格拉姆–施密特方法将 $\left\{g_k\right\}$ 化成标准正交的:

$$
h_0=\frac{g_0}{\left\|g_0\right\|},\quad h_1=\frac{g_1-\left\langle g_1,h_0\right\rangle h_0}{\left\|g_1-\left\langle g_1,h_0\right\rangle h_0\right\|},\cdots.
$$

显然 $h_k$ 依旧是 $k$ 次的多项式. 可是要用直接计算的方法算出函数 $h_k$ 是比较麻烦的, 因此对许多具体问题往往还要用一些特殊的方法.

实际上, 可以证明勒让德多项式

$$
P_0\left(x\right)=1,\quad P_n\left(x\right)=\frac{1}{2^n n!}\frac{\mathrm d^n}{\mathrm dx^n}\left(x^2-1\right)^n,\quad n=1,2,\cdots
$$

是 $L^2\left[-1,1\right]$ 中的正交多项式系. 将勒让德多项式单位化得到

$$
h_0\left(x\right)=\frac{1}{\sqrt{2}},\quad h_n\left(x\right)=\frac{1}{2^n n!}\sqrt{\frac{2n+1}{2}}\frac{\mathrm d^n}{\mathrm dx^n}\left(x^2-1\right)^n,\quad n=1,2,\cdots
$$

就是 $\left\{g_n\right\}$ 经过格拉姆–施密特过程得到的标准正交向量系. 又由于多项式全体在 $L^2\left[-1,1\right]$ 中稠密, 因此 $\left\{h_n:n=0,1,\cdots\right\}$ 构成了一组标准正交基. 证明:

(i) $\left\{h_n:n=0,1,\cdots,n\right\}$ 是一组标准正交系;

(ii) $\left\{h_n:n=0,1,\cdots,n\right\}$ 是一组标准正交基.

### 解答 3-5

(i) 依据**例 1.3.8 (勒让德多项式)**: 勒让德多项式 $P_n$ 是 $L^2\left[-1,1\right]$ 中的正交多项式系, 单位化后的 $h_n$ 正是 $\left\{g_k\right\}$ 经过格拉姆–施密特过程得到的标准正交向量系. 而格拉姆–施密特过程保正两两正交且范数为 $1$, 因此对任意 $i\neq j$, $\left\langle h_i,h_j\right\rangle=0$, 且 $\left\|h_i\right\|=1$. 故 $\left\{h_n:n=0,1,\cdots,N\right\}$ 是 $L^2\left[-1,1\right]$ 中的标准正交系 (依据**定义 1.3.1**).

(ii) 首先, $h_n$ 是 $n$ 次多项式, 且 $\left\{h_0,h_1,\cdots,h_N\right\}$ 与 $\left\{g_0,g_1,\cdots,g_N\right\}=\left\{1,x,\cdots,x^N\right\}$ 张成同一线性空间 (格拉姆–施密特过程不改变张成空间), 故

$$
\operatorname{span}\left\{h_n:n=0,1,\cdots\right\}=\text{多项式全体 }P.
$$

由**例 1.4.6** (4), 多项式全体 $P$ 在 $L^2\left[-1,1\right]$ 中稠密, 即 $\overline{\operatorname{span}\left\{h_n\right\}}=L^2\left[-1,1\right]$. 依据**定理 1.3.2 (标准正交基的等价条件)** (ii), $\left\{h_n:n=0,1,\cdots\right\}$ 是 $L^2\left[-1,1\right]$ 的标准正交基. $\blacksquare$

---

7. 设 $\omega\left(t\right)$ 是 $\mathbb R$ 上勒贝格可积的非负函数. 令

$$
H=\left\{f \text{ 是 }\mathbb R\text{ 上勒贝格可测函数: }\int_{\mathbb R}\left|f\left(t\right)\right|^2\omega\left(t\right)dt<\infty\right\}
$$

证明: $H$ 按通常函数的线性运算以及内积

$$
\left\langle f,g\right\rangle=\int_{\mathbb R}f\left(t\right)\overline{g\left(t\right)}\omega\left(t\right)dt,\quad \forall f,g\in H
$$

成为希尔伯特空间.

### 解答 3-7

按几乎处处相等的等价类取商, 与 $L^2\left(\mathbb R\right)$ 的处理方式一致; 以下在等价类意义下讨论.

**$H$ 是线性空间.** 对 $f,g\in H$ 与数 $\alpha,\beta$, 由 $\left|f\right|^2\omega$, $\left|g\right|^2\omega$ 可积及由不等式 $\left(a+b\right)^2\le2a^2+2b^2$,

$$
\left|\alpha f+\beta g\right|^2\omega\le2\left|\alpha\right|^2\left|f\right|^2\omega+2\left|\beta\right|^2\left|g\right|^2\omega
$$

得 $\alpha f+\beta g\in H$, 故 $H$ 是线性空间.

**$\left\langle\cdot,\cdot\right\rangle$ 是内积.** 依据**定义 1.2.3 (内积空间)**, 逐条验证. (i) 共轭对称性:

$$
\left\langle f,g\right\rangle=\int f\overline g\omega=\overline{\int g\overline f\omega}=\overline{\left\langle g,f\right\rangle}.
$$

(ii) 对第一变元的线性性: 由积分线性性,

$$
\left\langle\alpha f+\beta g,h\right\rangle=\alpha\left\langle f,h\right\rangle+\beta\left\langle g,h\right\rangle.
$$

(iii) 正定性: $\left\langle f,f\right\rangle=\int\left|f\right|^2\omega\ge0$, 且

$$
\begin{aligned}
&\quad\;\left\langle f,f\right\rangle=0\\
&\Leftrightarrow\int\left|f\right|^2\omega=0\\
&\Leftrightarrow \left|f\right|^2\omega=0\text{ a.e.}\\
&\Leftrightarrow f=0\text{ a.e.}\\
&\Leftrightarrow f=0\text{ \left(在等价类意义下\right)}.
\end{aligned}
$$

故 $\left\langle\cdot,\cdot\right\rangle$ 是 $H$ 上的内积.

**完备性.** 设 $\left\{f_n\right\}$ 是 $H$ 中的基本点列, 即 $\left\|f_n-f_m\right\|_H^2=\int\left|f_n-f_m\right|^2\omega\mathrm dt\to0$. 由于 $L^p\left(E\right)$ 已知完备 (**例 1.2.8**), 故考虑构造保范映射 $f\mapsto f\sqrt{\omega}: H \to L^2\left(\mathbb R\right)$ 将 $H$ 放到 $L^p\left(E\right)$ 中再拉回即可: 则 $f_n\sqrt{\omega}\in L^2\left(\mathbb R,\mathrm dm\right)$ 且

$$
\left\|f_n\sqrt{\omega}-f_m\sqrt{\omega}\right\|_{L^2\left(\mathbb R\right)}^2=\int\left|f_n-f_m\right|^2\omega\mathrm dt=\left\|f_n-f_m\right\|_H^2\to0,
$$

故 $\left\{f_n\sqrt{\omega}\right\}$ 是 $L^2\left(\mathbb R\right)$ 中的基本点列. 由**例 1.2.8** ($L^p\left(E\right)$ 的完备性), 存在 $g\in L^2\left(\mathbb R\right)$ 使 $\left\|f_n\sqrt{\omega}-g\right\|_{L^2\left(\mathbb R\right)}\to0$. 令

$$
f\left(t\right)=\begin{cases}g\left(t\right)/\sqrt{\omega\left(t\right)},&\omega\left(t\right)>0,\\0,&\omega\left(t\right)=0,\end{cases}
$$

则 $f$ 可测, 且 $\int\left|f\right|^2\omega\mathrm dt=\int\left|g\right|^2\mathrm dt<\infty$, 故 $f\in H$; 并且 $\left\|f_n-f\right\|_H=\left\|f_n\sqrt{\omega}-g\right\|_{L^2\left(\mathbb R\right)}\to0$, 即 $\left\{f_n\right\}$ 在 $H$ 中收敛于 $f$. 故 $H$ 按内积诱导的度量完备.

由**定义 (希尔伯特空间)**, $H$ 是希尔伯特空间. $\blacksquare$

---

8. 设 $\mathcal F=\left\{e_1,e_2,\cdots,e_n,\cdots\right\}$ 是希尔伯特空间 $\left(H,\left\langle\cdot,\cdot\right\rangle\right)$ 的一组标准正交系, 将 $\mathcal F$ 重排成另一个序列 $\left\{e_1',e_2',\cdots,e_n',\cdots\right\}$. 证明: 对于 $x\in H$,

$$
\lim_{n\to\infty}\sum_{k=1}^n \left\langle x,e_k\right\rangle e_k=\lim_{n\to\infty}\sum_{k=1}^n \left\langle x,e_k'\right\rangle e_k'.
$$

### 解答 3-8

记 $S_n=\sum_{k=1}^n\left\langle x,e_k\right\rangle e_k$, $S_n'=\sum_{k=1}^n\left\langle x,e_k'\right\rangle e_k'$. 先说明两个极限都存在.

由**定理 1.3.1 (贝塞尔不等式)**, $\sum_k\left|\left\langle x,e_k\right\rangle\right|^2\le\left\|x\right\|^2<\infty$. 对 $m<n$, 由标准正交性 (**定义 1.3.1**) 与勾股定理,

$$
\left\|S_n-S_m\right\|^2=\left\|\sum_{k=m+1}^n\left\langle x,e_k\right\rangle e_k\right\|^2=\sum_{k=m+1}^n\left|\left\langle x,e_k\right\rangle\right|^2\to0\left(m,n\to\infty\right),
$$

故 $\left\{S_n\right\}$ 是 $H$ 中的基本点列. 依据 $H$ 的完备性, $S_n$ 收敛, 记 $S=\lim S_n$; 同理 $S_n'$ 收敛, 记 $S'=\lim S_n'$.

下证 $S=S'$. 显然 $S,S'\in\overline{\operatorname{span}\left\{e_k\right\}}$. 对任意固定的 $j$, 依据**引理 1.2.4 (内积的连续性)** 与标准正交性,

$$
\left\langle S,e_j\right\rangle=\lim_{n\to\infty}\sum_{k=1}^n\left\langle x,e_k\right\rangle\left\langle e_k,e_j\right\rangle=\left\langle x,e_j\right\rangle,
$$

$$
\left\langle S',e_j\right\rangle=\lim_{n\to\infty}\sum_{k=1}^n\left\langle x,e_k'\right\rangle\left\langle e_k',e_j\right\rangle=\left\langle x,e_j\right\rangle,
$$

第二个等式成立是因为 $\left\{e_k'\right\}$ 是 $\left\{e_k\right\}$ 的重排: 序列中恰有一个 $e_{k_0}'=e_j$, 其余各项与 $e_j$ 正交. 因此 $S-S'\perp e_j$ 对一切 $j$ 成立, 由**引理 1.2.4 (内积的连续性)** 得 $S-S'\perp\overline{\operatorname{span}\left\{e_k\right\}}$; 而 $S-S'\in\overline{\operatorname{span}\left\{e_k\right\}}$, 故 $\left\langle S-S',S-S'\right\rangle=0$, 由**定义 1.2.3** 的正定性得 $S-S'=0$, 即 $S=S'$. 证毕. $\blacksquare$

---

10. 令 $f_{0}=1+\sum_{n=1}^{\infty}\frac{1}{n}\left(\cos nx+\sin nx\right)$. 设 $H$ 是 $L^2\left[0,2\pi\right]$ 中由

$$
\left\{f_{0},\cos x,\sin x,\cdots,\cos nx,\sin nx,\cdots\right\}
$$

张成的线性子空间. 给出 $H$ 中的一组完全标准正交系, 但不是完备的.

### 解答 3-10

取

$$
\mathcal E=\left\{e_n:=\sqrt2\cos nx,\tilde e_n:=\sqrt2\sin nx:n=1,2,\cdots\right\}.
$$

**$\mathcal E$ 是 $H$ 中的标准正交系.** 由**例 1.3.3**, $\left\{1,\sqrt2\cos nx,\sqrt2\sin nx:n\ge1\right\}$ 是 $L^2\left[0,2\pi\right]$ 的标准正交系, 故其子集 $\mathcal E$ 也是标准正交系 (依据**定义 1.3.1**); 且 $e_n,\tilde e_n\in H$ ($\cos nx,\sin nx\in H$ 且 $H$ 是线性子空间).

**$\mathcal E$ 在 $H$ 中是完全的.** 设 $x\in H$ 且 $x\perp\mathcal E$. 因 $H=\operatorname{span}\left\{f_0,\cos nx,\sin nx:n\ge1\right\}$, 存在 $c_0,c_k,d_k$ 使得 (有限和)

$$
x=c_0f_0+\sum_{k=1}^{N}\left(c_k\cos kx+d_k\sin kx\right).
$$

对 $k\ge1$, 由 $x\perp\cos kx$ ( $x\perp e_k$ 与 $x\perp\tilde e_k$ 等价于 $x\perp\cos kx,\sin kx$ ) 及标准正交性,

$$
0=\left\langle x,\cos kx\right\rangle=c_0\left\langle f_0,\cos kx\right\rangle+c_k\left\langle\cos kx,\cos kx\right\rangle.
$$

计算傅里叶系数:

$$
\begin{aligned}
\left\langle f_0,\cos kx\right\rangle=\frac{1}{k}\left\langle\cos kx,\cos kx\right\rangle&=\frac{1}{2k},\\
\left\langle\cos kx,\cos kx\right\rangle&=\frac12,
\end{aligned}
$$

故 $0=\frac{c_0}{2k}+\frac{c_k}{2}$, 即 $c_k=-\frac{c_0}{k}$; 同理 $d_k=-\frac{c_0}{k}$. 由于 $x$ 是有限线性组合, 当 $k>N$ 时 $c_k=d_k=0$, 代入 $c_k=-c_0/k$ 得 $c_0=0$, 从而所有 $c_k=d_k=0$, 即 $x=0$. 依据**定理 1.3.2** (iii), $\mathcal E$ 在 $H$ 中完全.

**$\mathcal E$ 不是完备的.** 取 $x=f_0\in H$. 计算得 $\left\|1\right\|^2=1$, $\left\|\cos nx\right\|^2=\left\|\sin nx\right\|^2=\frac12$, 故

$$
\left\|f_0\right\|^2=\left\|1\right\|^2+\sum_{n=1}^{\infty}\frac{1}{n^2}\left(\left\|\cos nx\right\|^2+\left\|\sin nx\right\|^2\right)=1+\sum_{n=1}^{\infty}\frac{1}{n^2}=1+\frac{\pi^2}{6}.
$$

而 $\left\langle f_0,\sqrt2\cos nx\right\rangle=\sqrt2\cdot\frac{1}{2n}=\frac{1}{\sqrt2n}$, $\left\langle f_0,\sqrt2\sin nx\right\rangle=\frac{1}{\sqrt2n}$, 故

$$
\sum_{e\in\mathcal E}\left|\left\langle f_0,e\right\rangle\right|^2=\sum_{n=1}^{\infty}\left(\frac{1}{2n^2}+\frac{1}{2n^2}\right)=\sum_{n=1}^{\infty}\frac{1}{n^2}=\frac{\pi^2}{6}<1+\frac{\pi^2}{6}=\left\|f_0\right\|^2,
$$

即帕塞瓦尔等式不成立. 依据**定理 1.3.2** (iv), $\mathcal E$ 不是完备的.

因此 $\mathcal E=\left\{\sqrt2\cos nx,\sqrt2\sin nx:n=1,2,\cdots\right\}$ 是 $H$ 中的一组完全标准正交系, 但不是完备的. $\blacksquare$

> **为什么选取 $f_0$ 作为反例**: 正交系 $\mathcal E$ 不含常数方向的基向量, 无法捕获常数分量. 而 $f_0\in H$, 其展开式中恰好含有常数项 $1$, 这就导致了帕塞瓦尔等式不能取等.
