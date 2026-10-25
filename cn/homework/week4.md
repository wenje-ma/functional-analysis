# week4

> **基础知识: 闵可夫斯基不等式**<br>设 $1\le p< \infty$, $f,g\in L^p$, 则 $\left\|f+g\right\|_p\le\left\|f\right\|_p+\left\|g\right\|_p$.

> **基础知识: 闭集与补集开集**<br>度量空间中集合 $A$ 是闭集当且仅当它的补集 $X\setminus A$ 是开集.

> **基础知识: 有理数在实数中稠密**<br>有理数集 $\mathbb Q$ 在 $\mathbb R$ 中稠密, 即对任意实数 $a< b$ 存在有理数 $r$ 使 $a< r< b$.

> **基础知识: 可积函数尾积分趋于零**<br>若 $g\in L^1\left(\mathbb R\right)$ 非负可积, 则 $\int_{\left|t\right|> N}g\left(t\right)\mathrm dt\to0$ ($N\to\infty$).

> **基础知识: 稠密关系的传递性**<br>若 $D$ 在 $E$ 中稠密且 $E$ 在 $X$ 中稠密, 则 $D$ 在 $X$ 中稠密.

> **基础知识: 分片线性延拓保最大模**<br>对定义在整数点 $\mathbb Z$ 上的有界实数列 $\left(a_n\right)_{n\in\mathbb Z}$, 在每个区间 $\left[n,n+1\right]$ 上线性连接 $\left(n,a_n\right)$ 与 $\left(n+1,a_{n+1}\right)$ 所得的分片连续函数 $f$ 满足 $\sup_{t\in\mathbb R}\left|f\left(t\right)\right|=\sup_{n\in\mathbb Z}\left|a_n\right|$.

> **基础知识: 积分三角不等式**<br>对可积复值函数 $g$, $\left|\int_E g\left(t\right)\mathrm dt\right|\le\int_E\left|g\left(t\right)\right|\mathrm dt$.

> **基础知识: 勒贝格测度平移不变性**<br>对任意可积函数 $g$ 与实数 $h$, $\int_{\mathbb R}\left|g\left(t+h\right)\right|^p\mathrm dt=\int_{\mathbb R}\left|g\left(t\right)\right|^p\mathrm dt$.

> **基础知识: 紧区间上连续函数一致连续**<br>有限闭区间上的连续函数必一致连续.

> **基础知识: 弱导数定义**<br>设 $g,h\in L_{\mathrm{loc}}^2\left(\mathbb R\right)$. 若对一切 $\varphi\in C_c^\infty\left(\mathbb R\right)$ 成立 $\int_{\mathbb R}g\varphi'\mathrm dt=-\int_{\mathbb R}h\varphi\mathrm dt$, 则称 $h$ 是 $g$ 的弱导数, 记 $g'=h$.

> **基础知识: 弱导数绝对连续**<br>若 $g\in L_{\mathrm{loc}}^2\left(\mathbb R\right)$ 有弱导数 $h\in L^2\left(\mathbb R\right)$, 则 $g$ 绝对连续, 且 $g'=h$ 几乎处处成立.

> **基础知识: 微分中值定理**<br>若一元实函数 $F$ 在 $\left[a,b\right]$ 上连续、在 $\left(a,b\right)$ 内可导, 则存在 $\xi\in\left(a,b\right)$ 使 $F\left(b\right)-F\left(a\right)=F'\left(\xi\right)\left(b-a\right)$.

> **基础知识: 微积分基本定理**<br>对可微函数 $F$ 及 $a< b$ 有 $\int_a^bF'\left(t\right)\,\mathrm dt=F\left(b\right)-F\left(a\right)$; 特别地, 初值问题 $y'=f\left(x,y\right)$, $y\left(x_0\right)=y_0$ 等价于积分方程 $y\left(x\right)=y_0+\int_{x_0}^xf\left(t,y\left(t\right)\right)\,\mathrm dt$.

> **基础知识: 绝对连续函数的常数性**<br>若绝对连续函数 $f$ 的导数几乎处处为零, 则 $f$ 几乎处处为常数.

> **定义 1.1.1 (度量空间)**<br>设 $X$ 是一个非空集合, 若对于 $X$ 中任意两个元素 $x,y$, 有一个实数 $d\left(x,y\right)$ 与它们对应, 而且满足: (i) $d\left(x,y\right)\ge0$, $d\left(x,y\right)=0$ 当且仅当 $x=y$; (ii) $d\left(x,y\right)=d\left(y,x\right)$; (iii) $d\left(x,y\right)\le d\left(x,z\right)+d\left(z,y\right)$, 则称 $\left(X,d\right)$ 是度量空间.

> **定义 1.1.2 (极限)**<br>设 $\left(X,d\right)$ 是度量空间, $\left\{x_n\right\}\subset X$, $x_0\in X$. 若 $\lim_{n\to\infty}d\left(x_n,x_0\right)=0$, 则称点列 $\left\{x_n\right\}$ 按度量 $d$ 收敛于 $x_0$.

> **定义 1.2.1 (哈梅尔基与维数)**<br>线性空间 $X$ 上的一个极大线性无关组称为 $X$ 的一组哈梅尔基; 若哈梅尔基中只有有限个元素, 则称 $X$ 是有限维线性空间.

> **定义 1.2.2 (半范数与范数)**<br>设 $X$ 是 $\mathbb K$ 上的线性空间. 若每个 $x\in X$ 对应实数 $\left\|x\right\|$, 满足<br>(i) $\left\|x\right\|\ge0$;<br>(ii) $\left\|\alpha x\right\|=\left|\alpha\right|\left\|x\right\|$;<br>(iii) $\left\|x+y\right\|\le\left\|x\right\|+\left\|y\right\|$,<br>则称 $\left\|\cdot\right\|$ 为半范数. 若还满足 $\left\|x\right\|=0\Leftrightarrow x=0$, 则称 $\left\|\cdot\right\|$ 为范数, $\left(X,\left\|\cdot\right\|\right)$ 称为赋范线性空间. 范数诱导度量 $d\left(x,y\right)=\left\|x-y\right\|$, 且 $\left\|\cdot\right\|$ 在该度量拓扑下连续.

> **定理 1.2.2 (勾股定理, 毕达哥拉斯定理)**<br>对内积空间 $H$ 中两个元素 $x,y$, 若 $x\perp y$, 则 $\left\|x+y\right\|^2=\left\|x\right\|^2+\left\|y\right\|^2$.

> **定义 1.2.3 (内积空间)**<br>记 $\mathbb K$ 是实数域 $\mathbb R$ 或复数域 $\mathbb C$. 对于 $\mathbb K$ 上的线性空间 $H$, 如果任何两个向量 $x,y$ 都对应一个数 $\left\langle x,y\right\rangle\in\mathbb K$, 满足:<br>(i) 共轭对称性 $\left\langle x,y\right\rangle=\overline{\left\langle y,x\right\rangle}$;<br>(ii) 对第一变元的线性性 $\left\langle\alpha x+\beta y,z\right\rangle=\alpha\left\langle x,z\right\rangle+\beta\left\langle y,z\right\rangle$;<br>(iii) 正定性 $\left\langle x,x\right\rangle\ge0$ 且 $\left\langle x,x\right\rangle=0$ 当且仅当 $x=0$,<br>则称 $\left\langle\cdot,\cdot\right\rangle$ 是 $H$ 中的内积, 称 $H$ 是内积空间.

> **引理 1.2.3 (柯西-施瓦茨不等式)**<br>对内积空间中任意 $x,y$, 成立 $\left|\left\langle x,y\right\rangle\right|^2\le\left\langle x,x\right\rangle\left\langle y,y\right\rangle$.

> **例 1.2.12 ($C\left[a,b\right]$ 是巴拿赫空间)**<br>有限闭区间 $\left[a,b\right]$ 上的连续函数空间 $C\left[a,b\right]$ 按范数 $\left\|f\right\|=\max_{x\in\left[a,b\right]}\left|f\left(x\right)\right|$ 是巴拿赫空间.

> **习题 1.2-13 (内积空间的可数直和)**<br>设 $R_n$ 都是内积空间, $R=\left\{\left\{x_n\right\}:x_n\in R_n,\ \sum_n\left\|x_n\right\|^2< \infty\right\}$ 按 $\left\langle\left\{x_n\right\},\left\{y_n\right\}\right\rangle=\sum_n\left\langle x_n,y_n\right\rangle$ 成为内积空间; 若每个 $R_n$ 是希尔伯特空间, 则 $R$ 也是希尔伯特空间.

> **定理 1.3.2 (标准正交基的等价条件)**<br>设 $\mathfrak F=\left\{e_\lambda:\lambda\in\Lambda\right\}$ 是希尔伯特空间 $H$ 中的标准正交系, 下列命题等价:<br>(i) 对任意 $x\in H$, $x=\sum_{\lambda\in\Lambda}\left\langle x,e_\lambda\right\rangle e_\lambda$;<br>(ii) $\overline{\operatorname{span}\left\{e_\lambda:\lambda\in\Lambda\right\}}=H$;<br>(iii) $\mathfrak F$ 是完全的, 即若 $x\in H$ 满足 $x\perp e_\lambda$ ($\forall\lambda\in\Lambda$), 则 $x=0$;<br>(iv) $\mathfrak F$ 是完备的, 即对任意 $x\in H$, 帕塞瓦尔等式 $\left\|x\right\|^2=\sum_{\lambda\in\Lambda}\left|\left\langle x,e_\lambda\right\rangle\right|^2$ 成立.<br>满足上述条件之一的标准正交系称为 $H$ 中的标准正交基.

> **定理 1.3.3 (标准正交系可扩张为标准正交基)**<br>希尔伯特空间 $H$ 中的任意标准正交系都可扩张为 $H$ 的一组标准正交基.

> **例 1.3.9 (埃尔米特多项式构成完备正交系)**<br>令 $H_n\left(t\right)=\left(-1\right)^n\mathrm e^{t^2}\frac{\mathrm d^n}{\mathrm dt^n}\mathrm e^{-t^2}$ 为埃尔米特多项式, 则加权多项式族 $\psi_n\left(t\right)=\left(2^n n!\sqrt\pi\right)^{-1/2}\mathrm e^{-t^2/2}H_n\left(t\right)$ 组成 $L^2\left(\mathbb R,\mathrm e^{-t^2}\mathrm dt\right)$ 中的完备标准正交系; 特别地, 多项式族关于权 $\mathrm e^{-t^2}$ 正交且完备.

> **定义 1.4.1 (内点、内部与开集)**<br>设 $A$ 是度量空间 $\left(X,d\right)$ 的点集, $x_0\in A$. 若存在 $r> 0$ 使 $\left\{x:d\left(x,x_0\right)< r\right\}\subset A$, 则称 $x_0$ 是 $A$ 的内点; $A$ 的内点全体称为 $A$ 的内部; 若 $A$ 中每点都是内点, 则称 $A$ 是开集.

> **引理 1.4.1 (基本点列与完备性)**<br>设 $X$ 是度量空间, 则:<br>(i) 基本点列是有界的;<br>(ii) 若 $X$ 完备, 则点列收敛当且仅当它是基本点列;<br>(iii) 完备度量空间的闭子集是完备的.

> **命题 1.4.1 (可分空间的子空间可分)**<br>设 $\left(X,d\right)$ 可分, $A\subset X$, 则 $\left(A,d\right)$ 也是可分的.

> **定理 1.4.1 (连续映射的等价条件)**<br>设 $f:X\to Y$ 是度量空间之间的映射, 下列条件等价:<br>(i) $f$ 连续;<br>(ii) $Y$ 中任一开集 $O$ 的原像 $f^{-1}\left(O\right)$ 是 $X$ 中的开集;<br>(iii) $Y$ 中任一闭集 $F$ 的原像 $f^{-1}\left(F\right)$ 是 $X$ 中的闭集.

> **例 1.4.1 (开球是开集)**<br>度量空间中开球 $O\left(x_0,r\right)=\left\{x:d\left(x,x_0\right)< r\right\}$ 是开集.

> **注 1.4.1 ($L^{p}$ 中的稠密子集)**<br>(i) $L^p\left(\mathbb R^n\right)$ ($1\le p< \infty$) 中的简单函数全体、阶梯函数全体以及 $C_c^\infty\left(\mathbb R^n\right)$ 均是稠密子集;<br>(ii) 在 $L^\infty\left[a,b\right]$ 中只有简单函数全体稠密.

> **例 1.4.2 (闭球是闭集)**<br>度量空间中闭球 $B\left(x_0,r\right)=\left\{x:d\left(x,x_0\right)\le r\right\}$ 是闭集.

> **定义 1.4.3 (极限点、导集、闭包与闭集)**<br>(i) 若存在异于 $x_0$ 的点列 $x_n\to x_0$, 则 $x_0$ 是 $A$ 的极限点;<br>(ii) 极限点全体记为导集 $A'$, 闭包 $\overline A=A\cup A'$;<br>(iii) 若 $A'\subset A$, 则称 $A$ 是闭集.

> **例 1.4.3 (距离函数连续)**<br>设 $F$ 是度量空间 $\left(X,d\right)$ 的非空子集, $d\left(x,F\right)=\inf_{z\in F}d\left(x,z\right)$. 由三角不等式得 $\left|d\left(x_1,F\right)-d\left(x_2,F\right)\right|\le d\left(x_1,x_2\right)$, 故 $x\mapsto d\left(x,F\right)$ 连续且一致连续.

> **定义 1.4.5 (稠密性)**<br>在度量空间 $\left(X,d\right)$ 中, 对于 $X$ 中一个子集 $A$, 称 $A$ 在 $X$ 中稠密是指 $X\subset\overline A$ (即 $\overline A=X$).

> **例 1.4.5 (魏尔斯特拉斯第一逼近定理)**<br>有界闭区间 $\left[a,b\right]$ 上, 多项式全体 $P$ 在 $C\left[a,b\right]$ 中稠密.

> **定义 1.4.6 (可分性)**<br>若度量空间 $X$ 中存在可数稠密子集, 则称 $X$ 是可分空间.

> **定义 1.4.7 (完备性)**<br>(i) 若 $\left\{x_n\right\}$ 满足: 对任意 $\varepsilon> 0$, 存在 $N$, 使 $n,m\ge N$ 时 $d\left(x_n,x_m\right)< \varepsilon$, 则称 $\left\{x_n\right\}$ 是基本点列 (柯西点列);<br>(ii) 若每个基本点列都收敛, 则称 $X$ 完备;<br>(iii) 完备赋范线性空间称为巴拿赫空间;<br>(iv) 完备内积空间称为希尔伯特空间.

> **例 1.4.9 ($C$ 与 $L^{p}$ 的可分性)**<br>$C\left[a,b\right]$ 和 $L^p\left[a,b\right]$ ($1\le p< \infty$) 是可分空间.

> **例 1.4.10 ($l^{\infty}$ 不可分)**<br>有界数列空间 $l^\infty$ 是不可分的.

> **例 1.4.11 ($L^{\infty}$ 不可分)**<br>$L^\infty\left[a,b\right]$ 是不可分的.

> **例 1.4.13 ($L^{p}\left(E\right)$ 是巴拿赫空间)**<br>设 $E$ 是 $\mathbb R^n$ 的勒贝格可测集, 则 $L^p\left(E\right)$ ($1\le p< \infty$) 是巴拿赫空间; 特别地, $L^2\left(E\right)$ 是希尔伯特空间.

> **定义 1.5.1 (不动点)**<br>设 $X$ 为集合, $\varphi:X\to X$. 若 $x^*\in X$ 使 $\varphi\left(x^*\right)=x^*$, 则称 $x^*$ 是 $\varphi$ 的不动点.

> **定理 1.5.1 (巴拿赫不动点定理)**<br>设 $X$ 是完备度量空间, $\varphi:X\to X$ 是压缩映射, 则 $\varphi$ 在 $X$ 中有唯一不动点 $x^*$; 对任意初值 $x_0$, 迭代 $x_n=\varphi^n\left(x_0\right)$ 收敛于 $x^*$, 且 $d\left(x^*,x_n\right)\le\frac{\alpha^n}{1-\alpha}d\left(x_1,x_0\right)$.

> **注 1.5.1 (迭代法的误差估计)**<br>在**定理 1.5.1 (巴拿赫不动点定理)** 的证明中, 令误差不等式两端取极限可得 $d\left(x^*,x_n\right)\le\frac{\alpha^n}{1-\alpha}d\left(x_1,x_0\right)$.

> **定义 1.5.2 (压缩映射)**<br>设 $\left(X,d\right)$ 是度量空间, $\varphi:X\to X$. 若存在 $0\le\alpha< 1$, 使对一切 $x,y\in X$ 有 $d\left(\varphi\left(x\right),\varphi\left(y\right)\right)\le\alpha d\left(x,y\right)$, 则称 $\varphi$ 是 $X$ 上的压缩映射, $\alpha$ 称为压缩系数.

> **定理 1.5.2 ($\varphi^{n}$ 压缩蕴含唯一不动点)**<br>设完备度量空间 $X$ 上的映射 $\varphi$ 存在自然数 $n$, 使 $\varphi^n$ 是压缩映射, 则 $\varphi$ 在 $X$ 中有唯一不动点.

> **定理 1.5.3 (初值问题解的存在唯一性)**<br>设 $f\left(x,y\right)$ 在区域 $D$ 上连续且关于 $y$ 满足利普希茨条件 $\left|f\left(x,y_1\right)-f\left(x,y_2\right)\right|\le L\left|y_1-y_2\right|$, 则当 $h< \min\left\{a,\frac{\lambda}{M},\frac{1}{L}\right\}$ 时, 初值问题 $y'=f\left(x,y\right)$, $y\left(x_0\right)=y_0$ 在 $\left[x_0-h,x_0+h\right]$ 上有唯一解.

> **例 1.6.1 (有限维空间中相对列紧等价于有界)**<br>在 $\mathbb R^n$ (及任意有限维赋范线性空间) 中, 子集 $A$ 是相对列紧集当且仅当 $A$ 是有界集; 有界闭集因此是紧集.

> **推论 1.6.3 (连续函数达到上下确界)**<br>度量空间 $X$ 的紧子集 $K$ 上的连续函数 $f$ 有界, 且上、下确界在 $K$ 上达到.

---

## 1.4.2 (定理: 有限维赋范线性空间与 $\mathbb R^{n}$ 的等价)

设 $X$ 是 $n$ 维赋范线性空间 (数域为 $\mathbb R$), 证明 $X$ 与 $\mathbb R^n$ 在范数意义下等价.

### 解答 1.4.2

欲证明 $X$ 与 $\mathbb R^n$ 在范数意义下等价, 即要证明存在正实数 $c_1,c_2$, 使得对 $X$ 中每个 $x=\sum_{i=1}^n x_i e_i$ 成立

$$
c_1\sqrt{\sum_{i=1}^n\left|x_i\right|^2}\le\left\|x\right\|\le c_2\sqrt{\sum_{i=1}^n\left|x_i\right|^2}.
$$

**第一步: 建立坐标同构.** 因 $X$ 是 $n$ 维线性空间, 依据**定义 1.2.1 (哈梅尔基与维数)**, 可取 $X$ 的一组基 $e_1,e_2,\cdots,e_n$. 定义线性映射

$$
T\colon\mathbb R^n\to X,\quad T\left(\left(x_1,x_2,\cdots,x_n\right)\right)=\sum_{i=1}^n x_i e_i.
$$

由于 $\left\{e_i\right\}$ 是基, $T$ 是 $\mathbb R^n$ 到 $X$ 上的一一对应, 即线性同构.

**第二步: 证明范数 $\left\|T\left(\cdot\right)\right\|$ 在 $\mathbb R^n$ 的单位球面上连续且恒正.** 在 $\mathbb R^n$ 的单位球面 $S^{n-1}=\left\{\left(x_i\right):\sum_{i=1}^n x_i^2=1\right\}$ 上定义函数

$$
f\left(\left(x_i\right)\right)=\left\|T\left(\left(x_i\right)\right)\right\|=\left\|\sum_{i=1}^n x_i e_i\right\|.
$$

依据**定义 1.2.2 (半范数与范数)** 的说明, 范数 $\left\|\cdot\right\|$ 在所诱导的度量拓扑下连续. 下证 $T$ 连续: 对任意 $u,v\in\mathbb R^n$, 由**定义 1.2.2 (半范数与范数)** (iii) 的三角不等式与 (ii) 的齐次性,

$$
\left\|T\left(u-v\right)\right\|=\left\|\sum_{i=1}^n\left(u_i-v_i\right)e_i\right\|\le\sum_{i=1}^n\left|u_i-v_i\right|\left\|e_i\right\|.
$$

再由**引理 1.2.3 (柯西-施瓦茨不等式)** 应用于向量 $\left(\left|u_i-v_i\right|\right)$ 与 $\left(\left\|e_i\right\|\right)$, 右端不超过 $\sqrt{\sum_i\left\|e_i\right\|^2}\cdot\left\|u-v\right\|_2$, 故 $T$ 是 $\mathbb R^n$ 到 $X$ 的利普希茨映射, 从而连续. 于是复合函数 $f=\left\|\cdot\right\|\circ T$ 是 $\mathbb R^n$ 上的连续函数. 又因 $\left\{e_i\right\}$ 线性无关, 对一切 $\left(x_i\right)\ne0$ 有 $\sum_i x_i e_i\ne0$, 故在 $S^{n-1}$ 上 $f> 0$.

**第三步: 用紧性取上下确界.** 由**例 1.6.1 (有限维空间中相对列紧等价于有界)**, $\mathbb R^n$ 中有界集相对列紧, 而 $S^{n-1}$ 是有界闭集, 故 $S^{n-1}$ 是紧集. 依据**推论 1.6.3 (连续函数达到上下确界)**, 连续函数 $f$ 在 $S^{n-1}$ 上同时达到下确界与上确界: 存在 $\left(x_i^0\right),\left(x_i^1\right)\in S^{n-1}$ 使

$$
c_1:=f\left(\left(x_i^0\right)\right)=\min_{\left(x_i\right)\in S^{n-1}}f\left(\left(x_i\right)\right)> 0,\quad
c_2:=f\left(\left(x_i^1\right)\right)=\max_{\left(x_i\right)\in S^{n-1}}f\left(\left(x_i\right)\right).
$$

于是对一切 $\left(x_i\right)\in S^{n-1}$ 有 $c_1\le f\left(\left(x_i\right)\right)\le c_2$.

**第四步: 由齐性推广到全空间.** 对任意 $\left(x_i\right)\ne0$, 记 $r=\sqrt{\sum_i x_i^2}$, 则 $\left(x_i\right)/r\in S^{n-1}$. 依据**定义 1.2.2 (半范数与范数)** 中的齐次性 $\left\|\alpha x\right\|=\left|\alpha\right|\left\|x\right\|$, 有

$$
\left\|T\left(\left(x_i\right)\right)\right\|=r\left\|T\left(\left(x_i\right)/r\right)\right\|,\quad c_1\le\left\|T\left(\left(x_i\right)/r\right)\right\|\le c_2,
$$

故 $c_1 r\le\left\|T\left(\left(x_i\right)\right)\right\|\le c_2 r$, 即

$$
c_1\sqrt{\sum_{i=1}^n\left|x_i\right|^2}\le\left\|\sum_{i=1}^n x_i e_i\right\|\le c_2\sqrt{\sum_{i=1}^n\left|x_i\right|^2}.
$$

该不等式对 $\left(x_i\right)=0$ 也平凡成立. 故 $X$ 上的范数与 $\mathbb R^n$ 上的欧几里得范数互相控制, 即二者在范数意义下等价. $\blacksquare$

---

## 1.4-2 (闭集的递减开集邻域列)

设 $B$ 是度量空间中的闭集, 证明存在一个递减开集列 $\left\{O_1,O_2,\cdots,O_n,\cdots\right\}$, 使得每个 $O_n$ 包含 $B$ 且 $\bigcap_{n=1}^{\infty}O_n=B$.

### 解答 1.4-2

对每个正整数 $n$, 令

$$
O_n=\left\{x\in X:d\left(x,B\right)< \frac1n\right\}.
$$

**第一步: 每个 $O_n$ 是开集.** 依据**例 1.4.3 (距离函数连续)**, 函数 $x\mapsto d\left(x,B\right)$ 是 $X$ 上的连续函数. 而区间 $\left(-\infty,\frac1n\right)$ 是 $\mathbb R$ 中的开集, 依据**定理 1.4.1 (连续映射的等价条件)**, 开集的原像 $O_n=\left(d\left(\cdot,B\right)\right)^{-1}\left(\left(-\infty,\frac1n\right)\right)$ 是 $X$ 中的开集.

**第二步: $\left\{O_n\right\}$ 递减且每个 $O_n$ 包含 $B$.** 因 $\frac1{n+1}< \frac1n$, 故 $d\left(x,B\right)< \frac1{n+1}$ 蕴含 $d\left(x,B\right)< \frac1n$, 即 $O_{n+1}\subset O_n$, 故 $\left\{O_n\right\}$ 是递减开集列. 又对任意 $x\in B$, 由下确界定义 $d\left(x,B\right)=\inf_{z\in B}d\left(x,z\right)\le d\left(x,x\right)=0$, 故 $d\left(x,B\right)=0< \frac1n$, 从而 $x\in O_n$, 即 $B\subset O_n$ 对一切 $n$ 成立.

**第三步: 证明 $\bigcap_n O_n\subset B$.** 设 $x\in\bigcap_{n=1}^{\infty}O_n$, 则 $d\left(x,B\right)< \frac1n$ 对一切 $n$ 成立, 令 $n\to\infty$ 得 $d\left(x,B\right)=0$. 由下确界定义, 对每个 $n$ 存在 $z_n\in B$ 使 $d\left(x,z_n\right)< \frac1n$, 故 $z_n\to x$. 依据**定义 1.4.3 (极限点、导集、闭包与闭集)**, $x$ 是 $B$ 的极限点, 故 $x\in B'$. 又 $B$ 是闭集, 依据**定义 1.4.3 (极限点、导集、闭包与闭集)** (iii), 闭集满足 $B'\subset B$, 故 $x\in B$. 于是 $\bigcap_n O_n\subset B$.

综合第二步与第三步, $B\subset\bigcap_n O_n\subset B$, 故 $\bigcap_{n=1}^{\infty}O_n=B$. $\blacksquare$

---

## 1.4-4 (两不相交集合的分离开集)

设 $E,F$ 是度量空间 $X$ 中的两个子集并且 $d\left(E,F\right)\stackrel{\mathrm{def}}{=}\inf_{x\in E,y\in F}d\left(x,y\right)> 0$. 证明: 存在两个互不相交的开集 $O,G$ 分别包含 $E$ 和 $F$.

### 解答 1.4-4

记 $\delta=d\left(E,F\right)> 0$, 令

$$
O=\left\{x\in X:d\left(x,E\right)< \frac{\delta}{2}\right\},\quad
G=\left\{x\in X:d\left(x,F\right)< \frac{\delta}{2}\right\}.
$$

**第一步: $O,G$ 是开集且分别包含 $E,F$.** 依据**例 1.4.3 (距离函数连续)**, $x\mapsto d\left(x,E\right)$ 与 $x\mapsto d\left(x,F\right)$ 都是连续函数. 依据**定理 1.4.1 (连续映射的等价条件)**, 开区间 $\left(-\infty,\frac{\delta}{2}\right)$ 在这两个连续函数下的原像 $O,G$ 都是 $X$ 中的开集. 对任意 $x\in E$, 由下确界定义 $d\left(x,E\right)=\inf_{z\in E}d\left(x,z\right)\le d\left(x,x\right)=0$, 故 $d\left(x,E\right)=0< \frac{\delta}{2}$, 即 $x\in O$, 从而 $E\subset O$; 同理 $F\subset G$.

**第二步: 证明 $O\cap G=\varnothing$.** 反设存在 $x\in O\cap G$, 则 $d\left(x,E\right)< \frac{\delta}{2}$ 且 $d\left(x,F\right)< \frac{\delta}{2}$. 由下确界定义, 存在 $y\in E$ 与 $z\in F$ 使 $d\left(x,y\right)< \frac{\delta}{2}$ 与 $d\left(x,z\right)< \frac{\delta}{2}$. 依据**定义 1.1.1 (度量空间)** (iii) 中的三角不等式,

$$
d\left(y,z\right)\le d\left(y,x\right)+d\left(x,z\right)< \frac{\delta}{2}+\frac{\delta}{2}=\delta.
$$

但 $y\in E$, $z\in F$, 故 $\delta=\inf_{u\in E,v\in F}d\left(u,v\right)\le d\left(y,z\right)$, 这与 $d\left(y,z\right)< \delta$ 矛盾. 故 $O\cap G=\varnothing$.

于是 $O,G$ 是分别包含 $E,F$ 的两个互不相交的开集. $\blacksquare$

---

## 1.4-5 (上半连续与水平集闭)

设 $f\left(x\right)$ 是度量空间 $X$ 上的实函数. 如果对于任意点 $x_0\in X$, 有

$$
\lim_{r\to0}\sup_{x\in O\left(x_0,r\right)}f\left(x\right)\le f\left(x_0\right),
$$

就称 $f\left(x\right)$ 在 $X$ 上是上半连续的. 证明: 当 $f\left(x\right)$ 是 $X$ 上的上半连续函数时, 对任何常数 $a$, 集合 $X\left(f\ge a\right)\stackrel{\mathrm{def}}{=}\left\{x:f\left(x\right)\ge a\right\}$ 是闭集. 反之也真.

### 解答 1.4-5

**先证 $\Rightarrow$ (上半连续蕴含 $X\left(f\ge a\right)$ 闭).** 固定常数 $a$. 依据**基础知识: 闭集与补集开集**, 要证 $X\left(f\ge a\right)$ 闭, 只须证其补集 $X\setminus X\left(f\ge a\right)$ 是开集. 任取 $x_0\notin X\left(f\ge a\right)$, 即 $f\left(x_0\right)< a$. 由上半连续定义,

$$
\lim_{r\to0}\sup_{x\in O\left(x_0,r\right)}f\left(x\right)\le f\left(x_0\right)< a.
$$

由上式左端的极限严格小于 $a$, 存在 $r_0> 0$ 使 $\sup_{x\in O\left(x_0,r_0\right)}f\left(x\right)< a$, 即对一切 $x\in O\left(x_0,r_0\right)$ 有 $f\left(x\right)< a$, 故 $O\left(x_0,r_0\right)\subset X\setminus X\left(f\ge a\right)$. 依据**例 1.4.1 (开球是开集)**, $O\left(x_0,r_0\right)$ 是开集, 故 $x_0$ 是其内点 (依据**定义 1.4.1 (内点、内部与开集)**). 由于 $x_0$ 任取, $X\setminus X\left(f\ge a\right)$ 是开集, 故 $X\left(f\ge a\right)$ 是闭集.

**再证 $\Leftarrow$ (水平集对一切 $a$ 闭蕴含上半连续).** 固定 $x_0\in X$. 对任意实数 $a> f\left(x_0\right)$, 因 $f\left(x_0\right)< a$, 故 $x_0\notin X\left(f\ge a\right)$. 由假设 $X\left(f\ge a\right)$ 是闭集, 依据**基础知识: 闭集与补集开集**, 其补集 $X\setminus X\left(f\ge a\right)$ 是开集; 而 $x_0$ 属于该开集, 依据**定义 1.4.1 (内点、内部与开集)**, 存在 $r_0> 0$ 使 $O\left(x_0,r_0\right)\subset X\setminus X\left(f\ge a\right)$, 即对一切 $x\in O\left(x_0,r_0\right)$ 有 $f\left(x\right)< a$, 从而

$$
\sup_{x\in O\left(x_0,r_0\right)}f\left(x\right)\le a.
$$

注意 $\lim_{r\to0}\sup_{x\in O\left(x_0,r\right)}f\left(x\right)=\inf_{r> 0}\sup_{x\in O\left(x_0,r\right)}f\left(x\right)$, 它关于 $r_0$ 是递减的, 故

$$
\lim_{r\to0}\sup_{x\in O\left(x_0,r\right)}f\left(x\right)\le\sup_{x\in O\left(x_0,r_0\right)}f\left(x\right)\le a.
$$

上式对一切 $a> f\left(x_0\right)$ 成立, 令 $a\downarrow f\left(x_0\right)$ 得 $\lim_{r\to0}\sup_{x\in O\left(x_0,r\right)}f\left(x\right)\le f\left(x_0\right)$, 这正是 $f$ 在 $x_0$ 处上半连续. 由 $x_0$ 任取, $f$ 在 $X$ 上上半连续. $\blacksquare$

---

## 1.4-7 (可分空间开覆盖有可列子覆盖)

设 $X$ 是可分的度量空间, $A\subset X$, $\left\{O_\lambda:\lambda\in\Lambda\right\}$ 是 $A$ 的开覆盖. 证明: 可从 $\left\{O_\lambda:\lambda\in\Lambda\right\}$ 中选出至多可列个开集 $\left\{O_{\lambda_n}\right\}$, 使得 $\bigcup_n O_{\lambda_n}\supset A$.

### 解答 1.4-7

**第一步: 取可数稠密子集.** 因 $X$ 可分, 依据**定义 1.4.6 (可分性)**, 存在可数子集 $D=\left\{x_1,x_2,\cdots\right\}$ 在 $X$ 中稠密, 即依据**定义 1.4.5 (稠密性)**, $\overline D=X$.

**第二步: 证明可数开球族构成开基.** 断言: 对任意开集 $G\subset X$ 及任意 $x\in G$, 存在 $x_n\in D$ 与正有理数 $r$ 使 $x\in O\left(x_n,r\right)\subset G$. 事实上, 由 $G$ 是开集及**定义 1.4.1 (内点、内部与开集)**, 存在 $\varepsilon> 0$ 使 $O\left(x,\varepsilon\right)\subset G$. 由 $\overline D=X$ 及 $x\in X$, $x$ 是 $D$ 的闭包中的点, 故存在 $x_n\in D$ 使 $d\left(x,x_n\right)< \frac{\varepsilon}{2}$. 依据**基础知识: 有理数在实数中稠密**, 可取有理数 $r$ 使 $d\left(x,x_n\right)< r< \frac{\varepsilon}{2}$. 对任意 $y\in O\left(x_n,r\right)$, 依据**定义 1.1.1 (度量空间)** (iii) 的三角不等式,

$$
d\left(y,x\right)\le d\left(y,x_n\right)+d\left(x_n,x\right)< r+\frac{\varepsilon}{2}< \frac{\varepsilon}{2}+\frac{\varepsilon}{2}=\varepsilon,
$$

故 $y\in O\left(x,\varepsilon\right)\subset G$, 即 $O\left(x_n,r\right)\subset G$, 且 $x\in O\left(x_n,r\right)$. 断言得证.

**第三步: 构造至多可列子覆盖.** 考虑可数族

$$
\mathscr B=\left\{O\left(x_n,r\right):n=1,2,\cdots;\ r\in\mathbb Q,\ r> 0\right\}.
$$

因 $\mathbb N$ 与 $\mathbb Q$ 皆可数, 故 $\mathscr B$ 可数. 对每个 $B\in\mathscr B$, 若存在 $\lambda\in\Lambda$ 使 $B\subset O_\lambda$ 且 $B\cap A\ne\varnothing$, 则任取一个这样的 $\lambda$, 记为 $\lambda_B$. 令 $\mathscr B'=\left\{B\in\mathscr B:\text{存在这样的 }\lambda_B\right\}$, 则 $\left\{O_{\lambda_B}:B\in\mathscr B'\right\}$ 是至多可列集.

对任意 $x\in A$, 因 $\left\{O_\lambda\right\}$ 覆盖 $A$, 存在 $\lambda$ 使 $x\in O_\lambda$, 且 $O_\lambda$ 是开集. 由第二步, 存在 $B=O\left(x_n,r\right)\in\mathscr B$ 使 $x\in B\subset O_\lambda$, 且 $B\cap A\ni x\ne\varnothing$, 故 $B\in\mathscr B'$ 且 $x\in B\subset O_{\lambda_B}$. 因此 $\bigcup_{B\in\mathscr B'}O_{\lambda_B}\supset A$, 即从原开覆盖中选出了至多可列个开集覆盖 $A$. $\blacksquare$

---

## 1.4-9 ($C_{c}^{\infty}$ 在加权 $L^{p}$ 中稠密)

对 $1\le p< \infty$, 定义巴拿赫空间

$$
L^p\left(\mathbb R,\mathrm e^{-t^2}\mathrm dt\right)=\left\{f\;\text{在}\;\mathbb R\;\text{上勒贝格可测}:\left\|f\right\|_p=\left(\int_{\mathbb R}\left|f\left(t\right)\right|^p\mathrm e^{-t^2}\mathrm dt\right)^{1/p}< \infty\right\}.
$$

证明: $C_c^\infty\left(\mathbb R\right)$ 在 $L^p\left(\mathbb R,\mathrm e^{-t^2}\mathrm dt\right)$ 中稠密. 判断多项式全体是否为稠密集 (无须证明).

### 解答 1.4-9

**第一步: 把 $f$ 截断为支集有界的函数.** 对 $f\in L^p\left(\mathbb R,\mathrm e^{-t^2}\mathrm dt\right)$, 令 $f_N=f\cdot\chi_{\left[-N,N\right]}$. 因 $\left|f\right|^p\mathrm e^{-t^2}$ 非负可积, 依据**基础知识: 可积函数尾积分趋于零**,

$$
\left\|f-f_N\right\|_p^p=\int_{\left|t\right|> N}\left|f\left(t\right)\right|^p\mathrm e^{-t^2}\mathrm dt\to0\quad\left(N\to\infty\right).
$$

故对给定 $\varepsilon> 0$, 可取 $N$ 使 $\left\|f-f_N\right\|_p< \frac{\varepsilon}{2}$.

**第二步: 支集有界的函数可用 $C_c^\infty$ 在普通 $L^p\left(\mathbb R\right)$ 中逼近.** 在 $\left[-N,N\right]$ 上有 $\mathrm e^{-t^2}\ge\mathrm e^{-N^2}> 0$, 故

$$
\int_{\mathbb R}\left|f_N\right|^p\mathrm dt\le\mathrm e^{N^2}\int_{\mathbb R}\left|f_N\right|^p\mathrm e^{-t^2}\mathrm dt\le\mathrm e^{N^2}\int_{\mathbb R}\left|f\right|^p\mathrm e^{-t^2}\mathrm dt< \infty,
$$

即 $f_N\in L^p\left(\mathbb R\right)$. 依据**注 1.4.1 ($L^{p}$ 中的稠密子集)**, $C_c^\infty\left(\mathbb R\right)$ 在 $L^p\left(\mathbb R\right)$ 中稠密; 依据**定义 1.4.5 (稠密性)**, 存在 $\varphi\in C_c^\infty\left(\mathbb R\right)$ 使 $\left\|f_N-\varphi\right\|_{L^p\left(\mathbb R\right)}< \frac{\varepsilon}{2}$. 又因 $\mathrm e^{-t^2}\le1$ 对一切 $t$ 成立,

$$
\left\|f_N-\varphi\right\|_{L^p\left(\mathbb R,\mathrm e^{-t^2}\mathrm dt\right)}\le\left\|f_N-\varphi\right\|_{L^p\left(\mathbb R\right)}< \frac{\varepsilon}{2}.
$$

**第三步: 三角不等式合拢.** 依据**定义 1.2.2 (半范数与范数)** (iii) 的三角不等式,

$$
\left\|f-\varphi\right\|_p\le\left\|f-f_N\right\|_p+\left\|f_N-\varphi\right\|_p< \frac{\varepsilon}{2}+\frac{\varepsilon}{2}=\varepsilon.
$$

故对任意 $f$ 与 $\varepsilon> 0$, 存在 $\varphi\in C_c^\infty\left(\mathbb R\right)$ 使 $\left\|f-\varphi\right\|_p< \varepsilon$, 依据**定义 1.4.5 (稠密性)**, $C_c^\infty\left(\mathbb R\right)$ 在 $L^p\left(\mathbb R,\mathrm e^{-t^2}\mathrm dt\right)$ 中稠密.

**关于多项式全体:** 多项式全体也是稠密集. 依据**例 1.3.9 (埃尔米特多项式构成完备正交系)**, 埃尔米特多项式族关于权 $\mathrm e^{-t^2}$ 正交且完备, 因而它在 $L^2\left(\mathbb R,\mathrm e^{-t^2}\mathrm dt\right)$ 中按该范数张成的闭包为全空间, 故多项式全体在 $L^2\left(\mathbb R,\mathrm e^{-t^2}\mathrm dt\right)$ 中稠密; 对一般 $1\le p< \infty$ 亦然. $\blacksquare$

---

## 1.4-10 ($C_{2\pi}$ 中的稠密性)

设 $C_{2\pi}=\left\{f\in C\left[0,2\pi\right]:f\left(0\right)=f\left(2\pi\right)\right\}$, 并按范数 $\left\|f\right\|=\max_{0\le t\le2\pi}\left|f\left(t\right)\right|$ 成一赋范空间. 证明:

(i) 令 $\mathcal P=\left\{f\in C_{2\pi}:\text{存在多项式}\;P\;\text{使得}\;f\left(t\right)=P\left(t\right),\ \forall0\le t\le2\pi\right\}$, 则 $\mathcal P$ 在 $C_{2\pi}$ 中稠密.

(ii) $C_{2\pi}$ 在 $L^p\left[0,2\pi\right]$ ($1\le p< \infty$) 中稠密, 但不在 $L^\infty\left[0,2\pi\right]$ 中稠密.

(iii) 将 $C_{2\pi}$ 中函数零延拓为 $\left[0,4\pi\right]$ 上的函数, 则 $C_{2\pi}$ 在 $L^p\left[0,4\pi\right]$ ($1\le p< \infty$) 中不稠密.

### 解答 1.4-10

**(i) $\mathcal P$ 在 $C_{2\pi}$ 中稠密.** 设 $f\in C_{2\pi}$, $\varepsilon> 0$. 依据**例 1.4.5 (魏尔斯特拉斯第一逼近定理)**, 多项式全体在 $C\left[0,2\pi\right]$ 中稠密, 故存在多项式 $Q$ 使 $\left\|f-Q\right\|_{C\left[0,2\pi\right]}< \frac{\varepsilon}{4}$. 记 $\delta=Q\left(2\pi\right)-Q\left(0\right)$, 则

$$
\left|\delta\right|\le\left|Q\left(2\pi\right)-f\left(2\pi\right)\right|+\left|f\left(2\pi\right)-f\left(0\right)\right|+\left|f\left(0\right)-Q\left(0\right)\right|< \frac{\varepsilon}{4}+0+\frac{\varepsilon}{4}=\frac{\varepsilon}{2}.
$$

作多项式 $P\left(t\right)=Q\left(t\right)-\frac{\delta}{4\pi^2}t^2$. 则 $P\left(0\right)=Q\left(0\right)$, 且 $P\left(2\pi\right)=Q\left(2\pi\right)-\delta=Q\left(0\right)$, 故 $P\left(0\right)=P\left(2\pi\right)$, 即 $P\in\mathcal P$. 又

$$
\left\|P-Q\right\|_{C\left[0,2\pi\right]}=\max_{0\le t\le2\pi}\left|\frac{\delta}{4\pi^2}t^2\right|=\left|\delta\right|< \frac{\varepsilon}{2}.
$$

依据**定义 1.2.2 (半范数与范数)** (iii), $\left\|f-P\right\|\le\left\|f-Q\right\|+\left\|Q-P\right\|< \frac{\varepsilon}{4}+\frac{\varepsilon}{2}< \varepsilon$. 依据**定义 1.4.5 (稠密性)**, $\mathcal P$ 在 $C_{2\pi}$ 中稠密.

**(ii) 第一部分: $C_{2\pi}$ 在 $L^p\left[0,2\pi\right]$ 中稠密.** 设 $f\in L^p\left[0,2\pi\right]$, $\varepsilon> 0$. 依据**注 1.4.1 ($L^{p}$ 中的稠密子集)**, $C\left[0,2\pi\right]$ 在 $L^p\left[0,2\pi\right]$ 中稠密, 故存在 $g\in C\left[0,2\pi\right]$ 使 $\left\|f-g\right\|_p< \frac{\varepsilon}{2}$. 现把 $g$ 在左端点附近稍作修改以令其满足 $h\left(0\right)=h\left(2\pi\right)$: 取 $\eta> 0$ 充分小, 令

$$
h\left(t\right)=
\begin{cases}
\left(1-\frac{t}{\eta}\right)g\left(2\pi\right)+\frac{t}{\eta}g\left(\eta\right),&0\le t< \eta,\\
g\left(t\right),&\eta\le t\le2\pi.
\end{cases}
$$

则 $h$ 连续, 且 $h\left(0\right)=g\left(2\pi\right)$, $h\left(2\pi\right)=g\left(2\pi\right)$, 故 $h\left(0\right)=h\left(2\pi\right)$, 即 $h\in C_{2\pi}$. 又 $g,h$ 在 $\left[0,\eta\right]$ 上有界, 设 $\left|g\right|,\left|h\right|\le M$, 则 $\left\|g-h\right\|_p^p\le\int_0^\eta\left(2M\right)^p\mathrm dt=\left(2M\right)^p\eta$, 取 $\eta$ 足够小即得 $\left\|g-h\right\|_p< \frac{\varepsilon}{2}$. 依据**定义 1.2.2 (半范数与范数)** (iii), $\left\|f-h\right\|_p\le\left\|f-g\right\|_p+\left\|g-h\right\|_p< \varepsilon$. 依据**定义 1.4.5 (稠密性)**, $C_{2\pi}$ 在 $L^p\left[0,2\pi\right]$ 中稠密.

**(ii) 第二部分: $C_{2\pi}$ 不在 $L^\infty\left[0,2\pi\right]$ 中稠密.** 因 $C_{2\pi}\subset C\left[0,2\pi\right]$, 依据**例 1.4.9 ($C$ 与 $L^{p}$ 的可分性)**, $C\left[0,2\pi\right]$ 可分; 依据**命题 1.4.1 (可分空间的子空间可分)**, 其子空间 $C_{2\pi}$ 亦可分, 即存在可数稠密子集 $D\subset C_{2\pi}$. 若 $C_{2\pi}$ 在 $L^\infty\left[0,2\pi\right]$ 中稠密, 则依据**基础知识: 稠密关系的传递性**, $D$ 在 $L^\infty\left[0,2\pi\right]$ 中稠密, 从而 $L^\infty\left[0,2\pi\right]$ 可分; 但依据**例 1.4.11 ($L^{\infty}$ 不可分)**, $L^\infty\left[0,2\pi\right]$ 不可分, 矛盾. 故 $C_{2\pi}$ 不在 $L^\infty\left[0,2\pi\right]$ 中稠密.

**(iii) 零延拓不稠密.** 记 $Z=\left\{\widetilde f:f\in C_{2\pi}\right\}$, 其中 $\widetilde f$ 是 $f$ 零延拓到 $\left[0,4\pi\right]$ 所得, 故 $\widetilde f\equiv0$ 于 $\left(2\pi,4\pi\right]$. 取 $h=\chi_{\left[3\pi,4\pi\right]}\in L^p\left[0,4\pi\right]$. 对任意 $\widetilde f\in Z$, 因 $\widetilde f\equiv0$ 于 $\left(2\pi,4\pi\right]$,

$$
\left\|h-\widetilde f\right\|_p^p\ge\int_{\left[3\pi,4\pi\right]}\left|1-\widetilde f\right|^p\mathrm dt\ge\int_{\left[3\pi,4\pi\right]}1\,\mathrm dt=\pi,
$$

故 $\left\|h-\widetilde f\right\|_p\ge\pi^{1/p}> 0$ 对一切 $\widetilde f\in Z$ 成立, 即 $h$ 不在 $Z$ 的闭包中. 依据**定义 1.4.5 (稠密性)**, $Z$ 在 $L^p\left[0,4\pi\right]$ 中不稠密. $\blacksquare$

---

## 1.4-12 ($C_{0}$ 可分而 $C_{b}$ 不可分)

令 $C_b\left(\mathbb R\right)$ 为 $\mathbb R$ 上有界的连续函数全体构成的巴拿赫空间, 它的范数 $\left\|x\right\|=\sup_{t\in\mathbb R}\left|x\left(t\right)\right|$. 令 $C_0\left(\mathbb R\right)=\left\{f\in C_b\left(\mathbb R\right):\lim_{t\to\pm\infty}x\left(t\right)=0\right\}$ 为 $C_b\left(\mathbb R\right)$ 的线性子空间. 证明:

(i) $C_0\left(\mathbb R\right)$ 是可分的.

(ii) $C_b\left(\mathbb R\right)$ 不是可分的.

### 解答 1.4-12

**(i) $C_0\left(\mathbb R\right)$ 可分.**

**第一步: 紧支撑连续函数 $C_c\left(\mathbb R\right)$ 在 $C_0\left(\mathbb R\right)$ 中稠密.** 设 $f\in C_0\left(\mathbb R\right)$, $\varepsilon> 0$. 因 $\lim_{t\to\pm\infty}f\left(t\right)=0$, 存在 $M> 0$ 使 $\left|t\right|\ge M$ 时 $\left|f\left(t\right)\right|< \varepsilon$. 取连续函数 $\varphi$ 满足 $0\le\varphi\le1$, $\varphi\equiv1$ 于 $\left[-M,M\right]$, $\varphi\equiv0$ 于 $\left(-\infty,-M-1\right]\cup\left[M+1,\infty\right)$ (例如分段线性函数). 令 $g=f\varphi$, 则 $g\in C_c\left(\mathbb R\right)$, 且

$$
\left\|f-g\right\|_\infty=\sup_t\left|f\left(t\right)\right|\left|1-\varphi\left(t\right)\right|< \varepsilon,
$$

因为在 $\left[-M,M\right]$ 上 $1-\varphi=0$, 在 $\left|t\right|\ge M$ 上 $\left|f\left(t\right)\right|< \varepsilon$. 依据**定义 1.4.5 (稠密性)**, $C_c\left(\mathbb R\right)$ 在 $C_0\left(\mathbb R\right)$ 中稠密.

**第二步: $C_c\left(\mathbb R\right)$ 可分.** 记 $C_c\left(\left[-n,n\right]\right)=\left\{f\in C\left[-n,n\right]:\text{支集}\subset\left[-n,n\right]\right\}$, 则 $C_c\left(\mathbb R\right)=\bigcup_{n=1}^{\infty}C_c\left(\left[-n,n\right]\right)$. 依据**例 1.4.9 ($C$ 与 $L^{p}$ 的可分性)**, $C\left[-n,n\right]$ 可分; 依据**命题 1.4.1 (可分空间的子空间可分)**, 其子空间 $C_c\left(\left[-n,n\right]\right)$ 可分. 因可数多个可分空间之并仍可分, 故 $C_c\left(\mathbb R\right)$ 可分.

**第三步: 合成 $C_0\left(\mathbb R\right)$ 的可分性.** 由第一步, $C_c\left(\mathbb R\right)$ 在 $C_0\left(\mathbb R\right)$ 中稠密; 由第二步, $C_c\left(\mathbb R\right)$ 可分. 依据**基础知识: 稠密关系的传递性**, 稠密于 $C_0\left(\mathbb R\right)$ 中的可分空间 $C_c\left(\mathbb R\right)$ 的可数稠密子集也是 $C_0\left(\mathbb R\right)$ 的可数稠密子集, 故 $C_0\left(\mathbb R\right)$ 可分.

**(ii) $C_b\left(\mathbb R\right)$ 不可分.**

**第一步: $l^\infty$ 等距嵌入 $C_b\left(\mathbb R\right)$.** 对 $a=\left(a_n\right)_{n\in\mathbb Z}\in l^\infty$, 定义 $f_a\in C_b\left(\mathbb R\right)$ 为分片线性函数: $f_a\left(n\right)=a_n$ ($n\in\mathbb Z$), 且 $f_a$ 在每个区间 $\left[n,n+1\right]$ 上为线性. 则 $f_a$ 连续且有界. 依据**基础知识: 分片线性延拓保最大模**, $\left\|f_a\right\|_\infty=\sup_{t\in\mathbb R}\left|f_a\left(t\right)\right|=\sup_{n\in\mathbb Z}\left|a_n\right|=\left\|a\right\|_{l^\infty}$, 故 $a\mapsto f_a$ 是 $l^\infty$ 到 $C_b\left(\mathbb R\right)$ 的某个子空间的等距映射.

**第二步: 反证推出矛盾.** 若 $C_b\left(\mathbb R\right)$ 可分, 则依据**命题 1.4.1 (可分空间的子空间可分)**, 其上述子空间 (即 $l^\infty$ 的等距像) 也可分, 从而 $l^\infty$ 可分. 但依据**例 1.4.10 ($l^{\infty}$ 不可分)**, $l^\infty$ 不可分, 矛盾. 故 $C_b\left(\mathbb R\right)$ 不可分. $\blacksquare$

> $C_b\left(\mathbb R\right)$ 相较于 $C_0\left(\mathbb R\right)$, 放宽了边界条件, 这导致了 $C_b\left(\mathbb R\right)$ 中可以嵌入任意有界的数列, 从而导致其不可分; 反观 $C_0\left(\mathbb R\right)$ 中当然嵌入不进去.

---

## 1.4-13 (希尔伯特空间可分等价于可数正交基)

设 $H$ 是希尔伯特空间, 证明 $H$ 可分等价于 $H$ 存在一组可数的正交基.

### 解答 1.4-13

**先证 $\Leftarrow$ (存在可数正交基蕴含 $H$ 可分).** 设 $\left\{e_n:n=1,2,\cdots\right\}$ 是 $H$ 的一组可数标准正交基. 依据**定理 1.3.2 (标准正交基的等价条件)** (ii), $\overline{\mathrm{span}\left\{e_n\right\}}=H$. 令

$$
D=\left\{\sum_{k=1}^m\left(a_k+\mathrm i b_k\right)e_k:m\ge1,\ a_k,b_k\in\mathbb Q\right\}.
$$

因 $\mathbb Q$ 可数而 $m$ 可数, 故 $D$ 可数. 对任意 $x\in H$ 与 $\varepsilon> 0$, 由 $\mathrm{span}\left\{e_n\right\}$ 在 $H$ 中稠密 (依据**定义 1.4.5 (稠密性)**), 存在有限线性组合 $y=\sum_{k=1}^m c_k e_k$ 使 $\left\|x-y\right\|< \frac{\varepsilon}{2}$. 依据**基础知识: 有理数在实数中稠密**, 可取 $c'_k=a_k+\mathrm i b_k$ ($a_k,b_k\in\mathbb Q$) 使 $\left|c_k-c'_k\right|$ 充分小, 从而

$$
\left\|y-\sum_{k=1}^m c'_k e_k\right\|=\left\|\sum_{k=1}^m\left(c_k-c'_k\right)e_k\right\|\le\sum_{k=1}^m\left|c_k-c'_k\right|< \frac{\varepsilon}{2},
$$

其中不等式依据**定义 1.2.2 (半范数与范数)** (iii) 的三角不等式与 $\left\|e_k\right\|=1$. 于是 $\left\|x-\sum c'_k e_k\right\|< \varepsilon$, 即 $D$ 在 $H$ 中稠密. 依据**定义 1.4.6 (可分性)**, $H$ 可分.

**再证 $\Rightarrow$ ($H$ 可分蕴含存在可数正交基).** 依据**定理 1.3.3 (标准正交系可扩张为标准正交基)**, $H$ 存在一组标准正交基 $\mathcal E=\left\{e_\lambda:\lambda\in\Lambda\right\}$. 下面证明 $\mathcal E$ 可数. 对 $\lambda\ne\mu\in\Lambda$, 有 $e_\lambda\perp e_\mu$ 且 $\left\|e_\lambda\right\|=\left\|e_\mu\right\|=1$, 依据**定理 1.2.2 (毕达哥拉斯定理)**, $\left\|e_\lambda-e_\mu\right\|^2=\left\|e_\lambda\right\|^2+\left\|e_\mu\right\|^2=2$, 故 $\left\|e_\lambda-e_\mu\right\|=\sqrt2$.

因 $H$ 可分, 依据**定义 1.4.6 (可分性)**, 存在可数稠密子集 $\left\{x_n:n\in\mathbb N\right\}$. 对每个 $\lambda\in\Lambda$, 依据**定义 1.4.5 (稠密性)** 与 $\left\{x_n\right\}$ 的稠密性, 可取 $n\left(\lambda\right)\in\mathbb N$ 使 $\left\|e_\lambda-x_{n\left(\lambda\right)}\right\|< \frac13$. 现证映射 $\lambda\mapsto n\left(\lambda\right)$ 是单射: 若 $\lambda\ne\mu$ 而 $n\left(\lambda\right)=n\left(\mu\right)$, 则依据**定义 1.2.2 (半范数与范数)** (iii),

$$
\left\|e_\lambda-e_\mu\right\|\le\left\|e_\lambda-x_{n\left(\lambda\right)}\right\|+\left\|x_{n\left(\mu\right)}-e_\mu\right\|< \frac13+\frac13=\frac23,
$$

这与 $\left\|e_\lambda-e_\mu\right\|=\sqrt2$ 矛盾. 故 $\Lambda$ 单射入可数集 $\mathbb N$, 从而 $\Lambda$ 可数, 即 $H$ 存在一组可数 (标准) 正交基. $\blacksquare$

---

## 1.4-14 (傅里叶变换的黎曼-勒贝格引理)

对 $f\in L^1\left(\mathbb R\right)$, 证明:

$$
\lim_{\left|t\right|\to\infty}\int_{\mathbb R}f\left(x\right)\mathrm e^{-\mathrm i2\pi t x}\mathrm dx=0.
$$

### 解答 1.4-14

记 $F\left(t\right)=\int_{\mathbb R}f\left(x\right)\mathrm e^{-\mathrm i2\pi t x}\mathrm dx$.

**第一步: 对区间特征函数成立.** 对 $f=\chi_{\left[a,b\right]}$, 直接计算

$$
F\left(t\right)=\int_a^b\mathrm e^{-\mathrm i2\pi t x}\mathrm dx=\frac{\mathrm e^{-\mathrm i2\pi t b}-\mathrm e^{-\mathrm i2\pi t a}}{-\mathrm i2\pi t},
$$

故 $\left|F\left(t\right)\right|\le\frac{2}{2\pi\left|t\right|}\to0$ ($\left|t\right|\to\infty$).

**第二步: 对阶梯函数成立.** 设 $s=\sum_{k=1}^m c_k\chi_{\left[a_k,b_k\right]}$ 是有限个区间特征函数的线性组合 (阶梯函数). 由第一步及积分关于被积函数的线性性, $\int_{\mathbb R}s\left(x\right)\mathrm e^{-\mathrm i2\pi t x}\mathrm dx=\sum_k c_k\int_{a_k}^{b_k}\mathrm e^{-\mathrm i2\pi t x}\mathrm dx\to0$ ($\left|t\right|\to\infty$).

**第三步: 对一般 $f\in L^1\left(\mathbb R\right)$ 成立.** 依据**注 1.4.1 ($L^{p}$ 中的稠密子集)**, 阶梯函数全体在 $L^1\left(\mathbb R\right)$ 中稠密; 依据**定义 1.4.5 (稠密性)**, 对任意 $\varepsilon> 0$ 存在阶梯函数 $s$ 使 $\left\|f-s\right\|_1< \varepsilon$. 依据**基础知识: 积分三角不等式**,

$$
\left|F\left(t\right)\right|\le\int_{\mathbb R}\left|f-s\right|\mathrm dx+\left|\int_{\mathbb R}s\left(x\right)\mathrm e^{-\mathrm i2\pi t x}\mathrm dx\right|< \varepsilon+\left|\int_{\mathbb R}s\left(x\right)\mathrm e^{-\mathrm i2\pi t x}\mathrm dx\right|.
$$

由第二步, 右端第二项当 $\left|t\right|\to\infty$ 时趋于 $0$, 故 $\limsup_{\left|t\right|\to\infty}\left|F\left(t\right)\right|\le\varepsilon$. 因 $\varepsilon> 0$ 任意, 令 $\varepsilon\to0$ 得 $\lim_{\left|t\right|\to\infty}\left|F\left(t\right)\right|=0$, 即 $\lim_{\left|t\right|\to\infty}\int_{\mathbb R}f\left(x\right)\mathrm e^{-\mathrm i2\pi t x}\mathrm dx=0$. $\blacksquare$

---

## 1.4-15 (平均连续性)

对 $f\in L^p\left(\mathbb R\right)$, $1\le p< \infty$, 证明:

$$
\lim_{\left|h\right|\to0}\int_{\mathbb R}\left|f\left(x+h\right)-f\left(x\right)\right|^p\mathrm dx=0.
$$

### 解答 1.4-15

记平移算子 $\left(\tau_h f\right)\left(x\right)=f\left(x+h\right)$, 并记 $\left\|g\right\|_p=\left(\int_{\mathbb R}\left|g\right|^p\mathrm dx\right)^{1/p}$.

**第一步: 对 $C_c^\infty$ 函数成立.** 设 $\varphi\in C_c^\infty\left(\mathbb R\right)$, 其支集含于 $\left[-M,M\right]$. 不妨设 $\left|h\right|< 1$, 则 $\varphi$ 在紧集 $\left[-M-1,M+1\right]$ 上连续; 依据**基础知识: 紧区间上连续函数一致连续**, $\varphi$ 在 $\left[-M-1,M+1\right]$ 上一致连续, 即对任意 $\varepsilon> 0$ 存在 $\delta> 0$, 当 $\left|h\right|< \delta$ 时 $\sup_x\left|\varphi\left(x+h\right)-\varphi\left(x\right)\right|< \varepsilon$. 对 $\left|h\right|< 1$, 被积函数仅在 $\left[-M-1,M+1\right]$ 上可能非零, 故

$$
\left\|\tau_h\varphi-\varphi\right\|_p^p=\int_{\mathbb R}\left|\varphi\left(x+h\right)-\varphi\left(x\right)\right|^p\mathrm dx\le\left(2M+2\right)\varepsilon^p\to0.
$$

即 $\lim_{h\to0}\left\|\tau_h\varphi-\varphi\right\|_p=0$.

**第二步: 对一般 $f\in L^p\left(\mathbb R\right)$ 成立.** 依据**注 1.4.1 ($L^{p}$ 中的稠密子集)**, $C_c^\infty\left(\mathbb R\right)$ 在 $L^p\left(\mathbb R\right)$ 中稠密; 依据**定义 1.4.5 (稠密性)**, 对任意 $\varepsilon> 0$ 存在 $\varphi\in C_c^\infty\left(\mathbb R\right)$ 使 $\left\|f-\varphi\right\|_p< \varepsilon$. 依据**基础知识: 勒贝格测度平移不变性**, $\left\|\tau_h\left(f-\varphi\right)\right\|_p=\left\|f-\varphi\right\|_p$. 再依据**基础知识: 闵可夫斯基不等式**,

$$
\left\|\tau_h f-f\right\|_p\le\left\|\tau_h f-\tau_h\varphi\right\|_p+\left\|\tau_h\varphi-\varphi\right\|_p+\left\|\varphi-f\right\|_p=2\left\|f-\varphi\right\|_p+\left\|\tau_h\varphi-\varphi\right\|_p.
$$

令 $h\to0$, 由第一步 $\lim_{h\to0}\left\|\tau_h\varphi-\varphi\right\|_p=0$, 故 $\limsup_{\left|h\right|\to0}\left\|\tau_h f-f\right\|_p\le2\varepsilon$. 因 $\varepsilon> 0$ 任意, 令 $\varepsilon\to0$ 得 $\lim_{\left|h\right|\to0}\left\|\tau_h f-f\right\|_p=0$, 即 $\lim_{\left|h\right|\to0}\int_{\mathbb R}\left|f\left(x+h\right)-f\left(x\right)\right|^p\mathrm dx=0$. $\blacksquare$

---

## 1.4-16 (完备性等价于绝对收敛级数收敛)

对赋范线性空间 $X$, 证明: $X$ 是完备的当且仅当对任意 $X$ 中点列 $\left\{x_n\right\}$, 当 $\sum_{n=1}^{\infty}\left\|x_n\right\|< \infty$ 时, $\sum_{n=1}^{\infty}x_n$ 在 $X$ 中收敛.

### 解答 1.4-16

**先证 $\Rightarrow$ (完备则 $\sum\left\|x_n\right\|< \infty$ 蕴含级数收敛).** 设 $\left\{x_n\right\}$ 满足 $\sum_{n=1}^{\infty}\left\|x_n\right\|< \infty$, 记部分和 $S_n=\sum_{k=1}^n x_k$. 对 $m> n$, 依据**定义 1.2.2 (半范数与范数)** (iii) 的三角不等式,

$$
\left\|S_m-S_n\right\|=\left\|\sum_{k=n+1}^m x_k\right\|\le\sum_{k=n+1}^m\left\|x_k\right\|\le\sum_{k=n+1}^{\infty}\left\|x_k\right\|\to0\quad\left(n\to\infty\right),
$$

因为正项级数收敛时其余项趋于零. 故 $\left\{S_n\right\}$ 是基本点列 (依据**定义 1.4.7 (完备性)** (i)). 因 $X$ 完备 (依据**定义 1.4.7 (完备性)** (ii)), $\left\{S_n\right\}$ 收敛, 即 $\sum_{n=1}^{\infty}x_n$ 收敛.

**再证 $\Leftarrow$ (绝对收敛级数恒收敛蕴含 $X$ 完备).** 设 $\left\{y_n\right\}$ 是 $X$ 中的基本点列. 由**定义 1.4.7 (完备性)** (i), 对 $\varepsilon=\frac{1}{2^k}$ 依次归纳选取下标 $n_1< n_2< \cdots$: 取 $n_1=1$; 已取 $n_k$, 由基本点列定义存在 $N_k$ 使 $n,m\ge N_k$ 时 $\left\|y_n-y_m\right\|< \frac{1}{2^k}$, 取 $n_{k+1}> \max\left\{n_k,N_k\right\}$, 则

$$
\left\|y_{n_{k+1}}-y_{n_k}\right\|< \frac{1}{2^k},\quad k=1,2,\cdots.
$$

令 $z_1=y_{n_1}$, $z_k=y_{n_k}-y_{n_{k-1}}$ ($k\ge2$), 则 $\sum_{k=1}^{\infty}\left\|z_k\right\|\le\left\|y_{n_1}\right\|+\sum_{k=1}^{\infty}\frac1{2^k}< \infty$ (几何级数收敛). 由题设条件, 级数 $\sum_{k=1}^{\infty}z_k$ 在 $X$ 中收敛; 而其部分和恰为 $\sum_{k=1}^m z_k=y_{n_m}$, 故子列 $\left\{y_{n_m}\right\}$ 收敛于某点 $x\in X$. 依据**引理 1.4.1 (基本点列与完备性)** (ii), 基本点列若有收敛子列则自身收敛于同一极限, 故 $\left\{y_n\right\}$ 收敛于 $x$. 由 $\left\{y_n\right\}$ 任取, $X$ 中每个基本点列都收敛, 依据**定义 1.4.7 (完备性)** (ii), $X$ 完备. $\blacksquare$

---

## 1.4-18 (索伯列夫型空间 $H$ 是希尔伯特空间)

设 $H$ 是直线上勒贝格平方可积, 且导函数也平方可积的绝对连续函数全体. 按通常的线性运算及范数

$$
\left\|f\right\|=\sqrt{\int_{\mathbb R}\left|f\left(t\right)\right|^2\mathrm dt+\int_{\mathbb R}\left|f'\left(t\right)\right|^2\mathrm dt},
$$

$H$ 成为赋范线性空间. 证明: $H$ 是希尔伯特空间.

### 解答 1.4-18

**第一步: $H$ 是内积空间.** 对 $f,g\in H$, 定义

$$
\left\langle f,g\right\rangle=\int_{\mathbb R}f\left(t\right)\overline{g\left(t\right)}\mathrm dt+\int_{\mathbb R}f'\left(t\right)\overline{g'\left(t\right)}\mathrm dt.
$$

由 $f,f'\in L^2\left(\mathbb R\right)$ 及 $g,g'\in L^2\left(\mathbb R\right)$, 依据**引理 1.2.3 (柯西-施瓦茨不等式)**, 上式右端两项均有限, 故 $\left\langle f,g\right\rangle$ 有限. 它显然满足**定义 1.2.3 (内积空间)** 的共轭对称性与对第一变元的线性性; 正定性方面, $\left\langle f,f\right\rangle=0$ 蕴含 $\int\left|f\right|^2=0$ 与 $\int\left|f'\right|^2=0$, 即 $f=0$ 且 $f'=0$ 几乎处处; 依据**基础知识: 绝对连续函数的常数性**, $f$ 几乎处处为常数, 而 $f\in L^2\left(\mathbb R\right)$ 迫使该常数为零, 即 $f\equiv0$. 又 $\left\langle f,f\right\rangle^{1/2}=\left\|f\right\|$, 故 $H$ 是内积空间且其范数为题给范数. 依据**定义 1.4.7 (完备性)** (iv), 只须证 $H$ 完备, 即为希尔伯特空间.

**第二步: 把 $H$ 等距嵌入 $L^2\left(\mathbb R\right)\times L^2\left(\mathbb R\right)$.** 令乘积空间的范数为 $\left\|\left(u,v\right)\right\|=\sqrt{\left\|u\right\|_2^2+\left\|v\right\|_2^2}$. 依据**例 1.4.13 ($L^{p}\left(E\right)$ 是巴拿赫空间)**, $L^2\left(\mathbb R\right)$ 是希尔伯特空间; 依据**习题 1.2 第 13 题 (内积空间的可数直和)** (取 $R_1=R_2=L^2\left(\mathbb R\right)$), $L^2\left(\mathbb R\right)\times L^2\left(\mathbb R\right)$ 是希尔伯特空间. 作映射

$$
T\colon H\to L^2\left(\mathbb R\right)\times L^2\left(\mathbb R\right),\quad f\mapsto\left(f,f'\right).
$$

由 $\left\|Tf\right\|^2=\left\|f\right\|_2^2+\left\|f'\right\|_2^2=\left\|f\right\|^2$, $T$ 是保范线性映射, $T\left(H\right)$ 是 $L^2\times L^2$ 的线性子空间.

**第三步: 证明 $T\left(H\right)$ 是闭子空间.** 设 $\left(f_n,f'_n\right)\to\left(g,h\right)$ 于 $L^2\times L^2$, 即 $f_n\to g$, $f'_n\to h$ 于 $L^2\left(\mathbb R\right)$. 对任意 $\varphi\in C_c^\infty\left(\mathbb R\right)$, 因每个 $f_n$ 绝对连续, 分部积分给出

$$
\int_{\mathbb R}f_n\varphi'\mathrm dt=-\int_{\mathbb R}f'_n\varphi\mathrm dt.
$$

令 $n\to\infty$: 因 $f_n\to g$ 于 $L^2$ 且 $\varphi'\in L^2$, 依据**引理 1.2.3 (柯西-施瓦茨不等式)**, 左端趋于 $\int_{\mathbb R}g\varphi'\mathrm dt$; 同理右端趋于 $-\int_{\mathbb R}h\varphi\mathrm dt$. 故

$$
\int_{\mathbb R}g\varphi'\mathrm dt=-\int_{\mathbb R}h\varphi\mathrm dt,\quad\forall\varphi\in C_c^\infty\left(\mathbb R\right).
$$

依据**基础知识: 弱导数定义**, $g$ 的弱导数为 $h\in L^2$. 依据**基础知识: 弱导数绝对连续**, $g$ 绝对连续且 $g'=h$ 几乎处处, 故 $g\in H$ 且 $\left(g,h\right)=T\left(g\right)\in T\left(H\right)$. 因此 $T\left(H\right)$ 是 $L^2\times L^2$ 的闭线性子空间.

**第四步: 结论.** 由第二步, $L^2\times L^2$ 是希尔伯特空间 (完备); 由第三步, $T\left(H\right)$ 是其闭子集. 依据**引理 1.4.1 (基本点列与完备性)** (iii), 完备度量空间的闭子集是完备子空间, 故 $T\left(H\right)$ 完备. 又 $T$ 是保范线性同构: 其单射性由 $T\left(f\right)=0$ 即 $f=f'=0$ 几乎处处推出 $f\equiv0$ (同第一步), 故 $H$ 与完备空间 $T\left(H\right)$ 等距同构, 从而 $H$ 完备. 依据**定义 1.4.7 (完备性)** (iv), $H$ 是希尔伯特空间. $\blacksquare$

---

## 1.5-2 ($\alpha_{n}$ 条件下的迭代收敛)

设 $X$ 为完备度量空间, $\varphi$ 是 $X$ 到自身的映射, 记

$$
\alpha_n=\sup_{x\ne y}\frac{d\left(\varphi^n\left(x\right),\varphi^n\left(y\right)\right)}{d\left(x,y\right)}.
$$

(i) 若级数 $\sum_{n=1}^{\infty}\alpha_n< \infty$, 则对任何一个初值 $x_0$, 迭代程序 $\left\{\varphi^n\left(x_0\right)\right\}$ 收敛于映射 $\varphi$ 的唯一不动点, 并求出第 $n$ 次近似解与准确解 $\varphi\left(x\right)=x$ 的逼近程度.

(ii) 若 $\inf_n\alpha_n< 1$, 则 $\varphi$ 有唯一的不动点. 并给出一种收敛于准确解 $\varphi\left(x\right)=x$ 的迭代程序以及 $n$ 次近似解与准确解的逼近程度.

### 解答 1.5-2

**(i) $\sum_n\alpha_n< \infty$ 的情形.**

**第一步: 不动点的存在与唯一性.** 因 $\sum_n\alpha_n< \infty$, 级数收敛故通项 $\alpha_n\to0$, 从而存在正整数 $N$ 使 $\alpha_N< 1$. 由 $\alpha_N$ 的定义, $d\left(\varphi^N\left(x\right),\varphi^N\left(y\right)\right)\le\alpha_N d\left(x,y\right)$ 对一切 $x,y\in X$ 成立, 依据**定义 1.5.2 (压缩映射)**, $\varphi^N$ 是 $X$ 上的压缩映射. 依据**定理 1.5.2 ($\varphi^{n}$ 压缩蕴含唯一不动点)**, $\varphi$ 在 $X$ 中有唯一不动点 $x^*$.

**第二步: 迭代列是基本点列并收敛.** 记 $x_n=\varphi^n\left(x_0\right)$. 对任意 $n\ge1$, 由 $\alpha_n$ 的定义,

$$
d\left(x_{n+1},x_n\right)=d\left(\varphi^n\left(\varphi\left(x_0\right)\right),\varphi^n\left(x_0\right)\right)\le\alpha_n d\left(\varphi\left(x_0\right),x_0\right)=\alpha_n d\left(x_1,x_0\right).
$$

对 $m> n$, 依据**定义 1.1.1 (度量空间)** (iii) 的三角不等式,

$$
d\left(x_m,x_n\right)\le\sum_{k=n}^{m-1}d\left(x_{k+1},x_k\right)\le d\left(x_1,x_0\right)\sum_{k=n}^{m-1}\alpha_k\le d\left(x_1,x_0\right)\sum_{k=n}^{\infty}\alpha_k\to0\quad\left(n\to\infty\right),
$$

最后一步因正项级数余项趋于零. 故 $\left\{x_n\right\}$ 是基本点列 (依据**定义 1.4.7 (完备性)** (i)). 因 $X$ 完备, 依据**定义 1.4.7 (完备性)** (ii), 存在 $y\in X$ 使 $x_n\to y$.

**第三步: 极限是不动点.** 因 $\alpha_1< \infty$, $d\left(\varphi\left(x\right),\varphi\left(x'\right)\right)\le\alpha_1 d\left(x,x'\right)$, 故 $\varphi$ 连续. 于是

$$
\varphi\left(y\right)=\varphi\left(\lim_{n\to\infty}x_n\right)=\lim_{n\to\infty}\varphi\left(x_n\right)=\lim_{n\to\infty}x_{n+1}=y,
$$

即 $\varphi\left(y\right)=y$, 依据**定义 1.5.1 (不动点)**, $y$ 是 $\varphi$ 的不动点. 由第一步的唯一性, $y=x^*$, 故 $\left\{\varphi^n\left(x_0\right)\right\}$ 收敛于唯一不动点 $x^*$.

**第四步: 逼近程度.** 在第二步的不等式 $d\left(x_m,x_n\right)\le d\left(x_1,x_0\right)\sum_{k=n}^{\infty}\alpha_k$ 中令 $m\to\infty$. 依据**例 1.4.3 (距离函数连续)** (距离关于变元连续), 左端趋于 $d\left(x^*,x_n\right)$, 故

$$
d\left(x^*,x_n\right)\le d\left(x_1,x_0\right)\sum_{k=n}^{\infty}\alpha_k.
$$

即第 $n$ 次近似 $x_n=\varphi^n\left(x_0\right)$ 与准确解 $x^*$ 的逼近程度为上式.

**(ii) $\inf_n\alpha_n< 1$ 的情形.**

**第一步: $x^*$ 是 $\varphi$ 的唯一不动点.** 因 $\inf_n\alpha_n< 1$, 存在正整数 $N$ 使 $\alpha_N< 1$, 即 $\varphi^N$ 满足 $d\left(\varphi^N x,\varphi^N y\right)\le\alpha_N d\left(x,y\right)$, 依据**定义 1.5.2 (压缩映射)**, $\varphi^N$ 是压缩映射. 依据**定理 1.5.1 (巴拿赫不动点定理)**, $\varphi^N$ 在完备空间 $X$ 中有唯一不动点 $x^*$, 即 $\varphi^N\left(x^*\right)=x^*$. 由**定理 1.5.2 ($\varphi^{n}$ 压缩蕴含唯一不动点)**, $\varphi$ 有唯一不动点 $x^*$.

**第二步: 迭代程序与逼近程度.** 取迭代程序 $x_{n+1}=\varphi^N\left(x_n\right)$, 即考察子列 $\left\{\varphi^{Nk}\left(x_0\right)\right\}$. 因 $\varphi^N$ 是以 $\alpha_N< 1$ 为压缩系数的压缩映射, 且 $X$ 完备, 依据**定理 1.5.1 (巴拿赫不动点定理)** 与**注 1.5.1 (迭代法的误差估计)** 的式 (1.25), 迭代 $\left\{\left(\varphi^N\right)^k\left(x_0\right)\right\}=\left\{\varphi^{Nk}\left(x_0\right)\right\}$ 收敛于 $x^*$, 且

$$
d\left(x^*,\varphi^{Nk}\left(x_0\right)\right)\le\frac{\alpha_N^k}{1-\alpha_N}d\left(\varphi^N\left(x_0\right),x_0\right).
$$

故 $\left\{\varphi^{Nk}\left(x_0\right)\right\}$ 即是一种收敛于准确解 $\varphi\left(x\right)=x$ 的迭代程序, 其 $k$ 次近似与准确解的逼近程度由上式给出. $\blacksquare$

---

## 1.5-4 (常微分方程组解的存在唯一性)

写出并利用不动点原理证明, 关于方程组

$$
\frac{\mathrm dy_k}{\mathrm dx}=f_k\left(x,y_1,y_2,\cdots,y_n\right),\quad k=1,2,\cdots,n
$$

的解的存在性与唯一性定理.

### 解答 1.5-4

本题要求写出并证明方程组初值问题解的存在唯一性定理, 其陈述如下: 设 $f_k\left(x,y_1,\cdots,y_n\right)$ ($k=1,\cdots,n$) 在 $\mathbb R^{n+1}$ 的某区域上连续, 且关于 $\left(y_1,\cdots,y_n\right)$ 满足利普希茨条件, 即存在常数 $L> 0$, 使当 $\left(x,y\right),\left(x,z\right)$ 在该区域中时,

$$
\sum_{k=1}^n\left|f_k\left(x,y_1,\cdots,y_n\right)-f_k\left(x,z_1,\cdots,z_n\right)\right|\le L\sum_{k=1}^n\left|y_k-z_k\right|,
$$

则初值问题

$$
\frac{\mathrm dy_k}{\mathrm dx}=f_k\left(x,y_1,\cdots,y_n\right),\quad y_k\left(x_0\right)=y_k^0,\quad k=1,\cdots,n
$$

在 $x_0$ 的某个邻域上有唯一解 $y\left(x\right)=\left(y_1\left(x\right),\cdots,y_n\left(x\right)\right)$.

**证明.** 取 $h> 0$ 充分小, 考虑空间

$$
C_D=\left\{y=\left(y_1,\cdots,y_n\right)\in C\left(\left[x_0-h,x_0+h\right],\mathbb R^n\right):\left|y_k\left(x\right)-y_k^0\right|\le\lambda,\ \forall x,\ y\left(x_0\right)=y_0\right\},
$$

其中范数 $\left\|y\right\|=\max_{1\le k\le n}\max_{x\in\left[x_0-h,x_0+h\right]}\left|y_k\left(x\right)\right|$, $y_0=\left(y_1^0,\cdots,y_n^0\right)$.

**第一步: 问题化为积分方程.** 依据**基础知识: 微积分基本定理**, 初值问题等价于积分方程组

$$
y_k\left(x\right)=y_k^0+\int_{x_0}^x f_k\left(t,y_1\left(t\right),\cdots,y_n\left(t\right)\right)\mathrm dt,\quad k=1,\cdots,n.
$$

**第二步: 在 $C_D$ 上构造压缩映射.** 依据**定理 1.5.3 (初值问题解的存在唯一性)** 的思路, 记

$$
M=\max\left\{\left|f_k\left(x,y\right)\right|:1\le k\le n,\ \left|x-x_0\right|\le h,\ \left|y_k-y_k^0\right|\le\lambda\right\},
$$

因 $f_k$ 连续故在紧集上有界, $M< \infty$. 定义

$$
\left(Ay\right)_k\left(x\right)=y_k^0+\int_{x_0}^x f_k\left(t,y_1\left(t\right),\cdots,y_n\left(t\right)\right)\mathrm dt.
$$

取 $h< \min\left\{\frac{\lambda}{M},\frac1L\right\}$, 则当 $\left|x-x_0\right|\le h$ 时 $\left|\left(Ay\right)_k\left(x\right)-y_k^0\right|\le Mh< \lambda$, 且 $\left(Ay\right)_k\left(x_0\right)=y_k^0$, 故 $Ay\in C_D$, 即 $A:C_D\to C_D$. 对 $y,z\in C_D$, 由利普希茨条件,

$$
\left\|Ay-Az\right\|=\max_k\max_x\left|\int_{x_0}^x\left(f_k\left(t,y\right)-f_k\left(t,z\right)\right)\mathrm dt\right|\le Lh\left\|y-z\right\|.
$$

因 $Lh< 1$, 依据**定义 1.5.2 (压缩映射)**, $A$ 是 $C_D$ 上的压缩映射.

**第三步: 应用不动点原理.** 由**例 1.2.12 ($C\left[a,b\right]$ 是巴拿赫空间)**, $C\left(\left[x_0-h,x_0+h\right],\mathbb R^n\right)$ 按最大范数是完备的; 而 $C_D$ 由闭条件 $\left|y_k\left(x\right)-y_k^0\right|\le\lambda$ 与 $y\left(x_0\right)=y_0$ 定义, 是该巴拿赫空间的闭子集. 依据**引理 1.4.1 (基本点列与完备性)** (iii), $C_D$ 是完备度量空间. 依据**定理 1.5.1 (巴拿赫不动点定理)**, $A$ 在 $C_D$ 中有唯一不动点 $y$, 即 $Ay=y$. 由第一步, 该 $y$ 满足积分方程组, 从而是初值问题的解; 唯一性亦由不动点唯一性得到. $\blacksquare$

---

## 1.5-5 (开球内压缩的不动点)

设从完备度量空间 $X$ 到自身的映射 $T$ 满足如下条件: 在开球 $O\left(x_0,r\right)$ ($r> 0$) 内成立

$$
d\left(Tx,Tx'\right)< \theta d\left(x,x'\right),\quad 0< \theta< 1,\ x\ne x',
$$

并且

$$
d\left(x_0,Tx_0\right)\le\alpha r.
$$

那么,

(i) 当 $\alpha$ 满足怎样的条件时, $T$ 在 $O\left(x_0,r\right)$ 内有不动点, 并且唯一?

(ii) 当 $\alpha\le1-\theta$ 时, 若 $T$ 在闭球 $B\left(x_0,r\right)$ 上连续, 则 $T$ 在 $B\left(x_0,r\right)$ 内有不动点. 这时这唯一性是否成立? 证明你的结论.

### 解答 1.5-5

**(i) 条件为 $\alpha< 1-\theta$.**

**第一步: 选取闭子球.** 设 $\alpha< 1-\theta$, 则 $\frac{\alpha r}{1-\theta}< r$. 取实数 $\rho$ 使 $\frac{\alpha r}{1-\theta}< \rho< r$, 作闭球 $B\left(x_0,\rho\right)$. 由 $\rho< r$ 有 $B\left(x_0,\rho\right)\subset O\left(x_0,r\right)$.

**第二步: $T$ 把 $B\left(x_0,\rho\right)$ 映入自身.** 对任意 $x\in B\left(x_0,\rho\right)$, 依据**定义 1.1.1 (度量空间)** (iii) 的三角不等式, 并注意 $x,x_0\in O\left(x_0,r\right)$ 故压缩条件适用,

$$
d\left(Tx,x_0\right)\le d\left(Tx,Tx_0\right)+d\left(Tx_0,x_0\right)< \theta d\left(x,x_0\right)+\alpha r\le\theta\rho+\alpha r.
$$

由 $\rho$ 的选取 $\theta\rho+\alpha r< \theta\rho+\left(1-\theta\right)\rho=\rho$, 故 $Tx\in B\left(x_0,\rho\right)$. 同时 $B\left(x_0,\rho\right)$ 是完备空间 $X$ 的闭子集 (依据**例 1.4.2 (闭球是闭集)**), 依据**引理 1.4.1 (基本点列与完备性)** (iii), $B\left(x_0,\rho\right)$ 完备.

**第三步: 存在唯一不动点.** 由第二步, $T$ 是完备度量空间 $B\left(x_0,\rho\right)$ 到自身的映射, 且压缩条件 $d\left(Tx,Tx'\right)\le\theta d\left(x,x'\right)$ 在其上成立, 依据**定义 1.5.2 (压缩映射)** 与**定理 1.5.1 (巴拿赫不动点定理)**, $T$ 在 $B\left(x_0,\rho\right)$ 内有唯一不动点, 从而在 $O\left(x_0,r\right)$ 内存在不动点. 唯一性还可直接看出: 若 $x',x''\in O\left(x_0,r\right)$ 都是不动点且 $x'\ne x''$, 则 $d\left(x',x''\right)=d\left(Tx',Tx''\right)< \theta d\left(x',x''\right)< d\left(x',x''\right)$, 矛盾. 故 $T$ 在 $O\left(x_0,r\right)$ 内不动点唯一.

**(ii) 当 $\alpha\le1-\theta$ 且 $T$ 在 $B\left(x_0,r\right)$ 上连续时, $T$ 在 $B\left(x_0,r\right)$ 内有不动点, 且唯一性成立.**

**第一步: $T$ 把 $B\left(x_0,r\right)$ 映入自身.** 对 $x\in O\left(x_0,r\right)$, $d\left(x,x_0\right)< r$, 由压缩条件与 $\alpha\le1-\theta$,

$$
d\left(Tx,x_0\right)\le d\left(Tx,Tx_0\right)+d\left(Tx_0,x_0\right)< \theta d\left(x,x_0\right)+\alpha r< \theta r+\left(1-\theta\right)r=r,
$$

故 $Tx\in O\left(x_0,r\right)\subset B\left(x_0,r\right)$. 对边界点 $x\in B\left(x_0,r\right)\setminus O\left(x_0,r\right)$, 取 $x_m\in O\left(x_0,r\right)$ 使 $x_m\to x$ (例如沿径向趋近). 由 $T$ 连续, $Tx_m\to Tx$; 而 $Tx_m\in B\left(x_0,r\right)$ 且 $B\left(x_0,r\right)$ 闭 (依据**例 1.4.2 (闭球是闭集)**), 故 $Tx\in B\left(x_0,r\right)$. 于是 $T\left(B\left(x_0,r\right)\right)\subset B\left(x_0,r\right)$.

**第二步: $T$ 在 $B\left(x_0,r\right)$ 上满足压缩条件.** 对任意 $x,y\in B\left(x_0,r\right)$, 取 $x_m,y_m\in O\left(x_0,r\right)$ 使 $x_m\to x$, $y_m\to y$. 由开球内的严格压缩条件, $d\left(Tx_m,Ty_m\right)< \theta d\left(x_m,y_m\right)$. 令 $m\to\infty$, 由 $T$ 连续及距离函数的连续性, 得 $d\left(Tx,Ty\right)\le\theta d\left(x,y\right)$. 依据**定义 1.5.2 (压缩映射)**, $T$ 是 $B\left(x_0,r\right)$ 上以 $\theta< 1$ 为压缩系数的压缩映射.

**第三步: 应用不动点原理.** $B\left(x_0,r\right)$ 是完备空间 $X$ 的闭子集 (依据**例 1.4.2 (闭球是闭集)**), 依据**引理 1.4.1 (基本点列与完备性)** (iii), $B\left(x_0,r\right)$ 完备; 由第一步, $T$ 把它映入自身. 依据**定理 1.5.1 (巴拿赫不动点定理)**, $T$ 在 $B\left(x_0,r\right)$ 内有唯一不动点, 即唯一性成立. $\blacksquare$

---

## 1.5-6 (紧集上严格压缩映射的不动点)

设 $F$ 是 $n$ 维欧几里得空间 $\mathbb R^n$ 中的有界闭集, $\varphi$ 是 $F$ 到自身的映射并且满足如下条件: 对于任何 $x,y\in F$ ($x\ne y$), 有

$$
d\left(\varphi\left(x\right),\varphi\left(y\right)\right)< d\left(x,y\right),\quad x\ne y.
$$

证明: 映射 $\varphi$ 在 $F$ 中存在唯一的不动点. 对于不闭的有界集这个事实能否成立?

### 解答 1.5-6

**第一步: $F$ 是紧集, $\varphi$ 连续.** 由**例 1.6.1 (有限维空间中相对列紧等价于有界)**, $\mathbb R^n$ 中有界集相对列紧; 而 $F$ 是有界闭集, 相对列紧的闭集即紧集, 故 $F$ 是紧集. 由题设 $d\left(\varphi\left(x\right),\varphi\left(y\right)\right)< d\left(x,y\right)$, 对任意 $x_m\to x$ 于 $F$, 有 $d\left(\varphi\left(x_m\right),\varphi\left(x\right)\right)< d\left(x_m,x\right)\to0$, 依据**定义 1.1.2 (极限)**, $\varphi\left(x_m\right)\to\varphi\left(x\right)$, 故 $\varphi$ 连续.

**第二步: 在紧集 $F$ 上定义连续函数 $g$ 并取最小值.** 令 $g\left(x\right)=d\left(x,\varphi\left(x\right)\right)$ ($x\in F$). 依据**例 1.4.3 (距离函数连续)**, 距离函数连续; 又 $\varphi$ 连续, 故 $g$ 是紧集 $F$ 上的连续函数. 依据**推论 1.6.3 (连续函数达到上下确界)**, $g$ 在 $F$ 上达到下确界, 即存在 $x_0\in F$ 使 $g\left(x_0\right)=\min_{x\in F}g\left(x\right)$.

**第三步: 最小值点必为不动点.** 反设 $g\left(x_0\right)> 0$, 即 $\varphi\left(x_0\right)\ne x_0$. 因 $\varphi\left(x_0\right)\in F$ 且 $x_0\ne\varphi\left(x_0\right)$, 由题设严格压缩条件,

$$
g\left(\varphi\left(x_0\right)\right)=d\left(\varphi\left(x_0\right),\varphi\left(\varphi\left(x_0\right)\right)\right)< d\left(x_0,\varphi\left(x_0\right)\right)=g\left(x_0\right),
$$

这与 $g\left(x_0\right)$ 是 $g$ 在 $F$ 上的最小值矛盾. 故 $g\left(x_0\right)=0$, 即 $d\left(x_0,\varphi\left(x_0\right)\right)=0$. 依据**定义 1.1.1 (度量空间)** (i) 的正定性, $\varphi\left(x_0\right)=x_0$, 即 $x_0$ 是不动点.

**第四步: 唯一性.** 若 $x,y\in F$ 都是不动点且 $x\ne y$, 则由题设 $d\left(x,y\right)=d\left(\varphi\left(x\right),\varphi\left(y\right)\right)< d\left(x,y\right)$, 矛盾. 故不动点唯一.

**关于不闭的有界集:** 该事实不成立. 取 $F=\left(0,1\right]$ ($\mathbb R$ 中的有界非闭集), 定义 $\varphi\left(x\right)=\frac{x}{2}$. 对任意 $x\ne y\in F$, $d\left(\varphi\left(x\right),\varphi\left(y\right)\right)=\frac{\left|x-y\right|}{2}< d\left(x,y\right)$, 满足题设严格压缩条件; 但方程 $\frac{x}{2}=x$ 的解为 $x=0\notin F$, 故 $\varphi$ 在 $F$ 中无不动点. 因而对不闭的有界集, 该结论不成立. $\blacksquare$

> 不闭自然不完备, 因此多次压缩后的点很容易溜出定义域.

---

## 1.5-7 (牛顿迭代法的局部收敛性)

(牛顿迭代法) 设 $f$ 是定义在 $\left[a,b\right]$ 上的二次连续可微实函数, $\left[a,b\right]$ 中点 $\overline{x}$ 满足 $f\left(\overline{x}\right)=0$, $f'\left(\overline{x}\right)\ne0$. 证明: 存在点 $\overline{x}$ 的一个邻域 $U$, 使得对任意 $x_0\in U$, 迭代序列

$$
x_{n+1}=x_n-\frac{f\left(x_n\right)}{f'\left(x_n\right)},\quad n=0,1,2,\cdots
$$

都收敛于 $\overline{x}$.

### 解答 1.5-7

**第一步: 牛顿映射及其在根点处的导数.** 令 $N\left(x\right)=x-\frac{f\left(x\right)}{f'\left(x\right)}$, 其定义域为使 $f'\left(x\right)\ne0$ 的开集. 因 $f$ 二次连续可微且 $f'\left(\overline{x}\right)\ne0$, $N$ 在 $\overline{x}$ 的某邻域内连续可微, 且

$$
N'\left(x\right)=1-\frac{f'\left(x\right)^2-f\left(x\right)f''\left(x\right)}{f'\left(x\right)^2}=\frac{f\left(x\right)f''\left(x\right)}{f'\left(x\right)^2}.
$$

代入 $x=\overline{x}$ 并利用 $f\left(\overline{x}\right)=0$, 得 $N'\left(\overline{x}\right)=\frac{f\left(\overline{x}\right)f''\left(\overline{x}\right)}{f'\left(\overline{x}\right)^2}=0$.

**第二步: 选取压缩区间.** 因 $N'$ 连续且 $N'\left(\overline{x}\right)=0$, 存在 $\delta> 0$, 使当 $\left|x-\overline{x}\right|\le\delta$ 时 $\left|N'\left(x\right)\right|\le\frac12< 1$. 对任意 $x,y\in\left[\overline{x}-\delta,\overline{x}+\delta\right]$, 依据**基础知识: 微分中值定理**, 存在 $\xi$ 介于 $x,y$ 之间使

$$
\left|N\left(x\right)-N\left(y\right)\right|=\left|N'\left(\xi\right)\right|\left|x-y\right|\le\frac12\left|x-y\right|.
$$

故 $N$ 在闭区间 $\left[\overline{x}-\delta,\overline{x}+\delta\right]$ 上以 $\frac12$ 为压缩系数, 依据**定义 1.5.2 (压缩映射)**, $N$ 是该闭区间上的压缩映射.

**第三步: 取不变闭区间并应用不动点定理.** 记 $B=\left[\overline{x}-\delta,\overline{x}+\delta\right]$. 因 $N\left(\overline{x}\right)=\overline{x}-\frac{f\left(\overline{x}\right)}{f'\left(\overline{x}\right)}=\overline{x}$, 对任意 $x\in B$, 由第二步的压缩估计,

$$
\left|N\left(x\right)-\overline{x}\right|=\left|N\left(x\right)-N\left(\overline{x}\right)\right|\le\frac12\left|x-\overline{x}\right|\le\frac{\delta}{2}< \delta,
$$

故 $N\left(B\right)\subset B$. 又 $B$ 是完备度量空间 $\mathbb R$ 的闭子集, 依据**引理 1.4.1 (基本点列与完备性)** (iii), $B$ 完备. 依据**定理 1.5.1 (巴拿赫不动点定理)**, $N$ 在 $B$ 内有唯一不动点; 而 $N\left(\overline{x}\right)=\overline{x}$, 故该不动点即为 $\overline{x}$. 依据**注 1.5.1 (迭代法的误差估计)**, 从任意初值 $x_0\in B$ 出发的迭代 $x_{n+1}=N\left(x_n\right)$ 收敛于 $\overline{x}$.

故取 $U=B\left(\overline{x},\delta\right)$ ($\overline{x}$ 的邻域), 对任意 $x_0\in U$, 牛顿迭代序列 $x_{n+1}=x_n-\frac{f\left(x_n\right)}{f'\left(x_n\right)}$ 收敛于 $\overline{x}$. $\blacksquare$
