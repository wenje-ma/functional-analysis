# week1

> **基础知识: 实数绝对值的三角不等式**<br>对任意实数 $a,b$, 有 $\left|a+b\right|\le\left|a\right|+\left|b\right|$, 进而 $\left|\sum_{i=1}^{n}a_i\right|\le\sum_{i=1}^{n}\left|a_i\right|$.

> **基础知识: 夹逼定理**<br>若数列 $\left\{a_n\right\}$ 满足 $0\le a_n\le b_n$, 且 $b_n\to0$, 则 $a_n\to0$.

> **基础知识: 对数与指数函数的连续性**<br>$\ln$ 与 $\exp$ 分别在其定义域上连续, 即 $\lim_{u\to u_0}\ln u=\ln u_0$ ($u_0>0$), $\lim_{v\to v_0}e^v=e^{v_0}$.

> **基础知识: 二项式定理**<br>对任意 $x$ 与正整数 $k$, $\left(1-x\right)^k=\sum_{j=0}^{k}\binom{k}{j}\left(-x\right)^j$.

> **基础知识: 函数 $\varphi,\psi$ 的单调与凹性**<br>记 $\varphi\left(t\right)=\frac{t}{1+t}$, $\psi\left(t\right)=\ln\left(1+t\right)$, $t\ge0$. 则 $\varphi,\psi$ 在 $\left[0,\infty\right)$ 上都严格递增, $\varphi\left(0\right)=\psi\left(0\right)=0$, 且 $\varphi''\left(t\right)=-\frac{2}{\left(1+t\right)^3}<0$, $\psi''\left(t\right)=-\frac{1}{\left(1+t\right)^2}<0$, 即二者都是严格凹函数.

> **基础知识: 凹函数过原点的次可加性**<br>若 $f:\left[0,\infty\right)\to\left[0,\infty\right)$ 是凹函数且 $f\left(0\right)=0$, 则对任意 $a,b\ge0$ 有 $f\left(a+b\right)\le f\left(a\right)+f\left(b\right)$. 事实上, 凹函数的导函数 $f'$ 单调递减, 故 $f\left(a+b\right)-f\left(a\right)=\int_a^{a+b}f'\left(s\right)\,\mathrm ds\le\int_a^{a+b}f'\left(s-a\right)\,\mathrm ds=\int_0^bf'\left(u\right)\,\mathrm du=f\left(b\right)-f\left(0\right)=f\left(b\right)$.

> **基础知识: 幂函数的单调性**<br>对任意 $p>0$, $u\mapsto u^p$ 在 $\left[0,\infty\right)$ 上严格递增; 特别当 $0<p<1$ 时, $\left(u^p\right)''=p\left(p-1\right)u^{p-2}<0$ ($u>0$), 即 $t\mapsto t^p$ 在 $\left[0,\infty\right)$ 上是凹函数且 $0^p=0$.

> **基础知识: 非负可测函数积分为零的充要条件**<br>若 $g\ge0$ 是 $\left[0,1\right]$ 上的勒贝格可测函数, 则 $\int_0^1g\left(t\right)\,\mathrm dt=0$ 当且仅当 $g\left(t\right)=0$ 几乎处处成立.

> **基础知识: 单位向量内积与夹角**<br>设 $x,y\in\mathbb R^3$, $\left\|x\right\|=\left\|y\right\|=1$, $\theta\in\left[0,\pi\right]$ 为 $x,y$ 的夹角, 则 $x\cdot y=\cos\theta$, 且以 $x,y$ 为端点的大圆劣弧长等于 $\theta$ (单位球面).

> **基础知识: $\sin u\le u$**<br>对任意 $u\ge0$, 有 $\sin u\le u$.

> **基础知识: $\sin$ 在 $\left[0,\pi/2\right]$ 上的凹弦估计**<br>$\sin''u=-\sin u<0$ ($u\in\left(0,\pi/2\right)$), 故 $\sin$ 在 $\left[0,\pi/2\right]$ 上是凹函数, 其图像位于连接 $\left(0,0\right)$ 与 $\left(\pi/2,1\right)$ 的弦 $y=\frac{2}{\pi}u$ 之上, 即 $\sin u\ge\frac{2}{\pi}u$ ($0\le u\le\frac{\pi}{2}$).

> **基础知识: $\cos$ 在 $\left[0,\pi\right]$ 上严格递减**<br>若 $\gamma,\beta\in\left[0,\pi\right]$ 且 $\cos\gamma\ge\cos\beta$, 则 $\gamma\le\beta$.

> **定义 1.1.1 (度量空间)**<br>设 $X$ 是一个非空集合, 若对于 $X$ 中任意两个元素 $x,y$, 都有一个实数 $d\left(x,y\right)$ 与它们对应, 而且满足下面条件:<br>(i) (非负性与正定性) 对任意 $x,y\in X$, $d\left(x,y\right)\ge0$, 并且 $d\left(x,y\right)=0$ 的充要条件是 $x=y$;<br>(ii) (对称性) 对任意 $x,y\in X$, $d\left(x,y\right)=d\left(y,x\right)$;<br>(iii) (三角不等式) 对任意 $x,y,z\in X$, $d\left(x,y\right)\le d\left(x,z\right)+d\left(z,y\right)$, 则称 $\left(X,d\right)$ 是一个度量空间, $d$ 为 $X$ 上的度量.

> **定义 1.1.2 (极限)**<br>设 $\left(X,d\right)$ 是度量空间, $\left\{x_n\right\}_{n=1}^\infty$ 是 $X$ 中点列, $x_0\in X$, 若 $\lim_{n\to\infty}d\left(x_n,x_0\right)=0$, 则称点列 $\left\{x_n\right\}$ 按照度量 $d$ 收敛于 $x_0$, 记为 $\lim_{n\to\infty}x_n=x_0$.

> **例 1.1.2 ($n$ 维欧几里得空间)**<br>在 $n$ 个有序实数组 $x=\left(x_1,x_2,\cdots,x_n\right)$ 全体组成的集合 $X$ 中, 定义 $d\left(x,y\right)=\sqrt{\sum_{i=1}^{n}\left(x_i-y_i\right)^2}$, 则 $\left(X,d\right)$ 是度量空间, 称为 $n$ 维欧几里得空间, 通常记为 $\mathbb R^n$.

> **例 1.1.10 (一致收敛与度量收敛)**<br>由例 1.1.6 的讨论可知, $C\left[a,b\right]$ 中点列按度量 $d\left(f,g\right)=\max_{x\in\left[a,b\right]}\left|f\left(x\right)-g\left(x\right)\right|$ 收敛等价于区间 $\left[a,b\right]$ 上的函数列一致收敛.

> **例 1.1.12 (可测函数等价类空间)**<br>对于有限区间 $\left[a,b\right]$, 记 $\mathfrak G=\left\{\left[a,b\right]\,\text{上几乎处处有限的勒贝格可测函数}\right\}$, $f,g\in\mathfrak G$ 等价是指 $f\overset m= g$, 仍以 $f$ 表示 $f$ 在 $\mathcal S=\mathfrak G/\sim$ 中对应的等价类; 对于 $f,g\in\mathcal S$, 定义 $d\left(f,g\right)=\int_{\left[a,b\right]}\frac{\left|f\left(t\right)-g\left(t\right)\right|}{1+\left|f\left(t\right)-g\left(t\right)\right|}\,\mathrm dm\left(t\right)$, 这是一个度量, 且 $d\left(f,g\right)=0$ 当且仅当 $f\overset m= g$.

> **引理 1.2.3 (柯西-施瓦茨不等式)**<br>设 $x,y\in H$ ($H$ 为内积空间), 则 $\left|\left\langle x,y\right\rangle\right|^2\le\left\langle x,x\right\rangle\left\langle y,y\right\rangle$, 特别地当 $\left\|x\right\|=\left\|y\right\|=1$ 时 $\left|\left\langle x,y\right\rangle\right|\le1$.

---

## 1.1-2

设 $\left(X,d\right)$ 是度量空间, 证明:

$$
d'\left(x,y\right)=\frac{d\left(x,y\right)}{1+d\left(x,y\right)},\quad d''\left(x,y\right)=\ln\left(1+d\left(x,y\right)\right),\quad \forall x,y\in X.
$$

也是 $X$ 上的度量, 并且 $\left(X,d'\right)$, $\left(X,d''\right)$ 中点列的收敛性和在 $\left(X,d\right)$ 中是一致的.

### 解答 1.1-2

记 $\varphi\left(t\right)=\frac{t}{1+t}$, $\psi\left(t\right)=\ln\left(1+t\right)$ ($t\ge0$). 由**基础知识: 函数 $\varphi,\psi$ 的单调与凹性**, $\varphi,\psi$ 在 $\left[0,\infty\right)$ 上严格递增, $\varphi\left(0\right)=\psi\left(0\right)=0$, 且二者都是严格凹函数. 由**基础知识: 凹函数过原点的次可加性**, $\varphi$ 与 $\psi$ 都满足 $f\left(a+b\right)\le f\left(a\right)+f\left(b\right)$ ($a,b\ge0$).

**第一步: 验证 $d'$ 是 $X$ 上的度量.** 依据**定义 1.1.1 (度量空间)**, 逐条验证 (i)(ii)(iii).

(i) 非负性与正定性. 由 $d$ 是 $X$ 上的度量 (**定义 1.1.1 (度量空间)**(i)), 对任意 $x,y\in X$ 有 $d\left(x,y\right)\ge0$, 且 $d\left(x,y\right)=0$ 当且仅当 $x=y$. 因 $\varphi$ 的自变量非负, $\varphi\left(t\right)\ge0$ ($t\ge0$), 故 $d'\left(x,y\right)=\varphi\left(d\left(x,y\right)\right)\ge0$. 又因 $\varphi$ 严格递增且 $\varphi\left(0\right)=0$, $\varphi\left(t\right)=0$ 当且仅当 $t=0$, 故

$$
d'\left(x,y\right)=0\Leftrightarrow\varphi\left(d\left(x,y\right)\right)=0\Leftrightarrow d\left(x,y\right)=0\Leftrightarrow x=y.
$$

于是 (i) 成立.

(ii) 对称性. 由**定义 1.1.1 (度量空间)**(ii), $d\left(x,y\right)=d\left(y,x\right)$, 故 $d'\left(x,y\right)=\varphi\left(d\left(x,y\right)\right)=\varphi\left(d\left(y,x\right)\right)=d'\left(y,x\right)$. 于是 (ii) 成立.

(iii) 三角不等式. 由**定义 1.1.1 (度量空间)**(iii), $d\left(x,y\right)\le d\left(x,z\right)+d\left(z,y\right)$. 因 $\varphi$ 严格递增, 两端作用 $\varphi$ 得 $d'\left(x,y\right)=\varphi\left(d\left(x,y\right)\right)\le\varphi\left(d\left(x,z\right)+d\left(z,y\right)\right)$. 由 $\varphi$ 的次可加性 (**基础知识: 凹函数过原点的次可加性**),

$$
\varphi\left(d\left(x,z\right)+d\left(z,y\right)\right)\le\varphi\left(d\left(x,z\right)\right)+\varphi\left(d\left(z,y\right)\right)=d'\left(x,z\right)+d'\left(z,y\right).
$$

故 $d'\left(x,y\right)\le d'\left(x,z\right)+d'\left(z,y\right)$, (iii) 成立. 由 (i)(ii)(iii) 全部成立, 依据**定义 1.1.1 (度量空间)**, $d'$ 是 $X$ 上的度量.

**第二步: 验证 $d''$ 是 $X$ 上的度量.** 同样依据**定义 1.1.1 (度量空间)** 逐条验证.

(i) 由 $d\left(x,y\right)\ge0$ 及 $\psi$ 严格递增、$\psi\left(0\right)=0$, $\psi\left(t\right)\ge0$ 且 $\psi\left(t\right)=0$ 当且仅当 $t=0$, 故 $d''\left(x,y\right)=\psi\left(d\left(x,y\right)\right)\ge0$, 且 $d''\left(x,y\right)=0\Leftrightarrow d\left(x,y\right)=0\Leftrightarrow x=y$. (i) 成立.

(ii) 由 $d\left(x,y\right)=d\left(y,x\right)$, $d''\left(x,y\right)=\psi\left(d\left(x,y\right)\right)=\psi\left(d\left(y,x\right)\right)=d''\left(y,x\right)$. (ii) 成立.

(iii) 由 $d\left(x,y\right)\le d\left(x,z\right)+d\left(z,y\right)$ 及 $\psi$ 严格递增, $d''\left(x,y\right)\le\psi\left(d\left(x,z\right)+d\left(z,y\right)\right)$; 再由 $\psi$ 的次可加性 (**基础知识: 凹函数过原点的次可加性**), $\psi\left(d\left(x,z\right)+d\left(z,y\right)\right)\le\psi\left(d\left(x,z\right)\right)+\psi\left(d\left(z,y\right)\right)=d''\left(x,z\right)+d''\left(z,y\right)$. (iii) 成立. 故 $d''$ 也是 $X$ 上的度量.

**第三步: 三种度量下收敛性一致.** 依据**定义 1.1.2 (极限)**, 记 $\varepsilon_n=d\left(x_n,x_0\right)$, 则

$$
x_n\overset d\to x_0\Leftrightarrow\varepsilon_n\to0.
$$

只需证明 $\varepsilon_n\to0\Leftrightarrow d'\left(x_n,x_0\right)\to0\Leftrightarrow d''\left(x_n,x_0\right)\to0$.

(a) $d'$ 与 $d$. 由定义 $d'\left(x_n,x_0\right)=\varphi\left(\varepsilon_n\right)=\frac{\varepsilon_n}{1+\varepsilon_n}$. 若 $\varepsilon_n\to0$, 则 $0\le\frac{\varepsilon_n}{1+\varepsilon_n}\le\varepsilon_n$, 由**基础知识: 夹逼定理** 得 $\frac{\varepsilon_n}{1+\varepsilon_n}\to0$, 即 $d'\left(x_n,x_0\right)\to0$. 反之, 若 $d'\left(x_n,x_0\right)=\frac{\varepsilon_n}{1+\varepsilon_n}\to0$, 则由恒等式 $\varepsilon_n=\frac{\varepsilon_n/\left(1+\varepsilon_n\right)}{1-\varepsilon_n/\left(1+\varepsilon_n\right)}$, 其分子趋于 $0$ 而分母趋于 $1\ne0$, 故 $\varepsilon_n\to0$. 于是 $x_n\overset d\to x_0\Leftrightarrow x_n\overset{d'}\to x_0$.

(b) $d''$ 与 $d$. 由定义 $d''\left(x_n,x_0\right)=\psi\left(\varepsilon_n\right)=\ln\left(1+\varepsilon_n\right)$. 若 $\varepsilon_n\to0$, 则 $1+\varepsilon_n\to1$, 由**基础知识: 对数与指数函数的连续性**, $\ln\left(1+\varepsilon_n\right)\to\ln1=0$, 即 $d''\left(x_n,x_0\right)\to0$. 反之, 若 $\ln\left(1+\varepsilon_n\right)\to0$, 则由恒等式 $\varepsilon_n=e^{\ln\left(1+\varepsilon_n\right)}-1$ 及**基础知识: 对数与指数函数的连续性**, $e^{\ln\left(1+\varepsilon_n\right)}-1\to e^0-1=0$, 即 $\varepsilon_n\to0$. 于是 $x_n\overset d\to x_0\Leftrightarrow x_n\overset{d''}\to x_0$.

综合 (a)(b),

$$
\lim_{n\to\infty}x_n\overset d=x_0\Leftrightarrow\lim_{n\to\infty}x_n\overset{d'}=x_0\Leftrightarrow\lim_{n\to\infty}x_n\overset{d''}=x_0,
$$

即 $\left(X,d'\right)$, $\left(X,d''\right)$ 中点列的收敛性和在 $\left(X,d\right)$ 中是一致的. $\blacksquare$

---

## 1.1-4

设 $X$ 是 $\left[0,1\right]$ 上多项式全体. 对于 $P,Q\in X$, $P\left(x\right)-Q\left(x\right)=\sum_{i=0}^{n}a_ix^i$, 令

$$
d_1\left(P,Q\right)=\max_{x\in\left[0,1\right]}\left|P\left(x\right)-Q\left(x\right)\right|,\quad d_2\left(P,Q\right)=\sum_{i=0}^{n}\left|a_i\right|.
$$

证明:

(i) $d_1,d_2$ 都是 $X$ 上的度量.

(ii) 多项式按 $d_1$ 收敛等价于在 $\left[0,1\right]$ 上一致收敛于某一多项式.

(iii) 按 $d_2$ 收敛可以推出按 $d_1$ 收敛, 但反之不真 (即存在多项式列 $\left\{P_k\right\}$, $d_1\left(P_k,0\right)\to0$, 但 $d_2\left(P_k,0\right)\not\to0$).

### 解答 1.1-4

**(i) $d_1$ 是 $X$ 上的度量.** 依据**定义 1.1.1 (度量空间)** 逐条验证.

(i) 对任意 $x\in\left[0,1\right]$, $\left|P\left(x\right)-Q\left(x\right)\right|\ge0$, 故 $d_1\left(P,Q\right)=\max_{x\in\left[0,1\right]}\left|P\left(x\right)-Q\left(x\right)\right|\ge0$. 且 $d_1\left(P,Q\right)=0$ 当且仅当 $\max_{x\in\left[0,1\right]}\left|P\left(x\right)-Q\left(x\right)\right|=0$, 当且仅当 $\left|P\left(x\right)-Q\left(x\right)\right|=0$ 对一切 $x\in\left[0,1\right]$ 成立, 当且仅当 $P\left(x\right)\equiv Q\left(x\right)$, 即 $P=Q$. 非负性与正定性成立.

(ii) 由 $\left|P\left(x\right)-Q\left(x\right)\right|=\left|Q\left(x\right)-P\left(x\right)\right|$ 对任意 $x$ 成立, $d_1\left(P,Q\right)=d_1\left(Q,P\right)$. 对称性成立.

(iii) 对任意 $R\in X$ 与 $x\in\left[0,1\right]$, 由**基础知识: 实数绝对值的三角不等式**,

$$
\left|P\left(x\right)-Q\left(x\right)\right|\le\left|P\left(x\right)-R\left(x\right)\right|+\left|R\left(x\right)-Q\left(x\right)\right|\le d_1\left(P,R\right)+d_1\left(R,Q\right).
$$

该不等式右端与 $x$ 无关, 故对左端关于 $x\in\left[0,1\right]$ 取最大值, 得 $d_1\left(P,Q\right)\le d_1\left(P,R\right)+d_1\left(R,Q\right)$. 三角不等式成立. 故 $d_1$ 是 $X$ 上的度量.

**(i) $d_2$ 是 $X$ 上的度量.** 同样依据**定义 1.1.1 (度量空间)** 逐条验证.

(i) 由 $\left|a_i\right|\ge0$ ($\forall i$), $d_2\left(P,Q\right)=\sum_{i=0}^{n}\left|a_i\right|\ge0$. 且 $d_2\left(P,Q\right)=0$ 当且仅当 $\sum_{i=0}^{n}\left|a_i\right|=0$, 当且仅当 $a_i=0$ ($\forall i$), 当且仅当 $P-Q\equiv0$, 即 $P=Q$. 非负性与正定性成立.

(ii) 若 $P-Q=\sum_{i=0}^{n}a_ix^i$, 则 $Q-P=\sum_{i=0}^{n}\left(-a_i\right)x^i$, 由 $\left|-a_i\right|=\left|a_i\right|$ 得 $d_2\left(P,Q\right)=\sum_{i=0}^{n}\left|a_i\right|=\sum_{i=0}^{n}\left|-a_i\right|=d_2\left(Q,P\right)$. 对称性成立.

(iii) 设 $P-R=\sum_{i=0}^{n}a_ix^i$, $R-Q=\sum_{i=0}^{n}b_ix^i$, 则 $P-Q=\left(P-R\right)+\left(R-Q\right)=\sum_{i=0}^{n}\left(a_i+b_i\right)x^i$. 由**基础知识: 实数绝对值的三角不等式**, $\left|a_i+b_i\right|\le\left|a_i\right|+\left|b_i\right|$ 对每个 $i$ 成立, 对 $i$ 求和得

$$
d_2\left(P,Q\right)=\sum_{i=0}^{n}\left|a_i+b_i\right|\le\sum_{i=0}^{n}\left|a_i\right|+\sum_{i=0}^{n}\left|b_i\right|=d_2\left(P,R\right)+d_2\left(R,Q\right).
$$

三角不等式成立. 故 $d_2$ 也是 $X$ 上的度量.

**(ii) 按 $d_1$ 收敛等价于在 $\left[0,1\right]$ 上一致收敛.** 依据**定义 1.1.2 (极限)** 与 $d_1$ 的定义,

$$
P_k\overset{d_1}\to P\Leftrightarrow d_1\left(P_k,P\right)=\max_{x\in\left[0,1\right]}\left|P_k\left(x\right)-P\left(x\right)\right|\to0.
$$

而 $\max_{x\in\left[0,1\right]}\left|P_k\left(x\right)-P\left(x\right)\right|\to0$ 正是函数列 $\left\{P_k\right\}$ 在 $\left[0,1\right]$ 上一致收敛于 $P$ 的定义. 由**例 1.1.10 (一致收敛与度量收敛)**, $C\left[a,b\right]$ 中点列按最大模范量收敛等价于在 $\left[a,b\right]$ 上一致收敛; 多项式空间 $X\subset C\left[0,1\right]$ 作为子空间继承这一对应. 故按 $d_1$ 收敛等价于在 $\left[0,1\right]$ 上一致收敛于某一多项式.

**(iii) 按 $d_2$ 收敛推出按 $d_1$ 收敛.** 设 $P_k\overset{d_2}\to Q$, 记 $P_k-Q=\sum_{i=0}^{n_k}a_i^{\left(k\right)}x^i$, 则 $d_2\left(P_k,Q\right)=\sum_{i=0}^{n_k}\left|a_i^{\left(k\right)}\right|\to0$. 对任意 $x\in\left[0,1\right]$, 有 $0\le x^i\le1$ 对每个 $i$ 成立, 由**基础知识: 实数绝对值的三角不等式**,

$$
\left|P_k\left(x\right)-Q\left(x\right)\right|=\left|\sum_{i=0}^{n_k}a_i^{\left(k\right)}x^i\right|\le\sum_{i=0}^{n_k}\left|a_i^{\left(k\right)}\right|x^i\le\sum_{i=0}^{n_k}\left|a_i^{\left(k\right)}\right|=d_2\left(P_k,Q\right).
$$

上式对一切 $x\in\left[0,1\right]$ 一致成立且右端趋于 $0$, 故 $d_1\left(P_k,Q\right)=\max_{x\in\left[0,1\right]}\left|P_k\left(x\right)-Q\left(x\right)\right|\to0$, 即 $P_k\overset{d_1}\to Q$.

**(iii) 反之不真.** 取 $P_k\left(x\right)=x^k\left(1-x\right)^k$. 由**基础知识: 二项式定理**,

$$
P_k\left(x\right)=x^k\sum_{j=0}^{k}\binom{k}{j}\left(-x\right)^j=\sum_{j=0}^{k}\binom{k}{j}\left(-1\right)^jx^{k+j}.
$$

一方面, $x\left(1-x\right)=\frac14-\left(x-\frac12\right)^2\le\frac14$, 等号在 $x=\frac12$ 处成立, 故 $\max_{x\in\left[0,1\right]}x\left(1-x\right)=\frac14$; 又 $u\mapsto u^k$ 在 $\left[0,\infty\right)$ 上严格递增 (**基础知识: 幂函数的单调性**), 所以

$$
d_1\left(P_k,0\right)=\max_{x\in\left[0,1\right]}\left[x\left(1-x\right)\right]^k=\left(\max_{x\in\left[0,1\right]}x\left(1-x\right)\right)^k=\left(\frac14\right)^k\to0.
$$

另一方面, $d_2\left(P_k,0\right)=\sum_{j=0}^{k}\left|\binom{k}{j}\left(-1\right)^j\right|=\sum_{j=0}^{k}\binom{k}{j}=2^k\to\infty$, 不趋于 $0$. 故存在多项式列 $\left\{P_k\right\}$ 使 $d_1\left(P_k,0\right)\to0$ 而 $d_2\left(P_k,0\right)\not\to0$, 反之不真. $\blacksquare$

> 构造思路: 要找一个函数值很小但系数很大的多项式, 需函数中含大量正负抵消项; $\left(-1\right)^j$ 天然合适, 二项式展开恰好提供交错系数, 故取 $x^k\left(1-x\right)^k$, 其 $d_2$-系数和恰为 $2^k$.

---

## 1.1-5

对 $0<p<1$, 记 $\mathcal L^p\left[0,1\right]$ 是区间 $\left[a,b\right]$ 上勒贝格可测且 $p$ 次可积的函数全体. 令

$$
d\left(f,g\right)=\int_0^1\left|f\left(t\right)-g\left(t\right)\right|^p\,\mathrm dt.
$$

证明:

(i) 当数 $a,b>0$ 时, $\left(a+b\right)^p\le a^p+b^p$.

(ii) $d$ 是伪度量, 即 $d$ 是非负的且满足定义 1.1.1(ii) 及 (iii).

(iii) 若等价关系 $f\sim g$ 是指两个函数 $f,g$ 满足 $f\overset m= g$, 仍以 $f$ 来表示 $p$ 次可积函数 $f$ 在 $L^p\left[a,b\right]=\mathcal L^p\left[a,b\right]/\sim$ 中对应的等价类, 则 $\left(L^p\left[a,b\right],d\right)$ 是度量空间.

### 解答 1.1-5

**(i) 对 $a,b>0$, 证明 $\left(a+b\right)^p\le a^p+b^p$.** 令 $f\left(t\right)=t^p$ ($t\ge0$). 由 $0<p<1$, $\left(t^p\right)''=p\left(p-1\right)t^{p-2}<0$ ($t>0$), 且 $f\left(0\right)=0$, 故 $f$ 是 $\left[0,\infty\right)$ 上的凹函数 (**基础知识: 幂函数的单调性**). 由**基础知识: 凹函数过原点的次可加性**, $f\left(a+b\right)\le f\left(a\right)+f\left(b\right)$, 即 $\left(a+b\right)^p\le a^p+b^p$ 对 $a,b\ge0$ 成立, 特别对 $a,b>0$ 成立.

**(ii) 验证 $d$ 是伪度量.** 依据**定义 1.1.1 (度量空间)**, 验证非负性、(ii) 对称性与 (iii) 三角不等式 (不要求 (i) 中的正定性).

非负性: 对任意 $f,g$, 逐点有 $\left|f\left(t\right)-g\left(t\right)\right|^p\ge0$, 故 $d\left(f,g\right)=\int_0^1\left|f\left(t\right)-g\left(t\right)\right|^p\,\mathrm dt\ge0$.

(ii) 对称性: 逐点有 $\left|f\left(t\right)-g\left(t\right)\right|=\left|g\left(t\right)-f\left(t\right)\right|$, 故 $\left|f\left(t\right)-g\left(t\right)\right|^p=\left|g\left(t\right)-f\left(t\right)\right|^p$, 积分得 $d\left(f,g\right)=d\left(g,f\right)$.

(iii) 三角不等式: 对任意第三个可测函数 $h$ 与每个 $t$, 由**基础知识: 实数绝对值的三角不等式**, $\left|f\left(t\right)-g\left(t\right)\right|\le\left|f\left(t\right)-h\left(t\right)\right|+\left|h\left(t\right)-g\left(t\right)\right|$. 因 $u\mapsto u^p$ 在 $\left[0,\infty\right)$ 上严格递增 (**基础知识: 幂函数的单调性**), 两端取 $p$ 次幂得

$$
\left|f\left(t\right)-g\left(t\right)\right|^p\le\left(\left|f\left(t\right)-h\left(t\right)\right|+\left|h\left(t\right)-g\left(t\right)\right|\right)^p.
$$

对右端用已证的 (i), 取 $a=\left|f\left(t\right)-h\left(t\right)\right|$, $b=\left|h\left(t\right)-g\left(t\right)\right|$, 得

$$
\left(\left|f\left(t\right)-h\left(t\right)\right|+\left|h\left(t\right)-g\left(t\right)\right|\right)^p\le\left|f\left(t\right)-h\left(t\right)\right|^p+\left|h\left(t\right)-g\left(t\right)\right|^p.
$$

两式合并得逐点不等式 $\left|f\left(t\right)-g\left(t\right)\right|^p\le\left|f\left(t\right)-h\left(t\right)\right|^p+\left|h\left(t\right)-g\left(t\right)\right|^p$, 对 $t$ 在 $\left[0,1\right]$ 上积分即得

$$
d\left(f,g\right)\le\int_0^1\left|f\left(t\right)-h\left(t\right)\right|^p\,\mathrm dt+\int_0^1\left|h\left(t\right)-g\left(t\right)\right|^p\,\mathrm dt=d\left(f,h\right)+d\left(h,g\right).
$$

(iii) 成立. 综上, $d$ 是非负的且满足 (ii)(iii), 即 $d$ 是伪度量.

**(iii) 商空间 $\left(L^p\left[a,b\right],d\right)$ 是度量空间.** 由 (ii), 非负性、对称性与三角不等式在商空间 $L^p\left[a,b\right]=\mathcal L^p\left[a,b\right]/\sim$ 上仍然成立, 依据**定义 1.1.1 (度量空间)** 只需再验证正定性. 对等价类 $\left[f\right],\left[g\right]$,

$$
d\left(\left[f\right],\left[g\right]\right)=0\Leftrightarrow\int_0^1\left|f\left(t\right)-g\left(t\right)\right|^p\,\mathrm dt=0.
$$

因被积函数 $\left|f\left(t\right)-g\left(t\right)\right|^p\ge0$ 且可测, 由**基础知识: 非负可测函数积分为零的充要条件**, 上式当且仅当 $\left|f\left(t\right)-g\left(t\right)\right|^p=0$ 几乎处处成立, 当且仅当 $f\left(t\right)=g\left(t\right)$ 几乎处处成立, 即 $f\overset m= g$, 亦即 $f\sim g$, 故 $\left[f\right]=\left[g\right]$. 这一"几乎处处相等作商、$d=0$ 当且仅当等价"的构造与**例 1.1.12 (可测函数等价类空间)** 相同. 于是正定性成立, $\left(L^p\left[a,b\right],d\right)$ 是度量空间. $\blacksquare$

---

## 1.1-7

在三维 Euclid 空间 $\mathbb R^3$ 中, 考虑单位球面

$$
S^2=\left\{x\in\mathbb R^3:\ x=\left(x_1,x_2,x_3\right),\ x_1^2+x_2^2+x_3^2=1\right\}.
$$

对于 $x,y\in S^2$, 规定 $d\left(x,y\right)$ 为过 $x,y$ 两点的大圆上以 $x,y$ 为端点的劣弧的弧长, 它在三维 Euclid 空间的正交变换下是保持不变的.

(i) 对于 $x_1^2+x_2^2=1$, 计算 $d\left(\left(1,0,0\right),\left(x_1,x_2,0\right)\right)$.

(ii) 如果用 $\rho\left(x,y\right)$ 表示 Euclid 距离, 证明:

$$
\rho\left(x,y\right)\le d\left(x,y\right)\le\frac{\pi}{2}\rho\left(x,y\right).
$$

(iii) 证明: $d$ 是 $S^2$ 上的度量.

### 解答 1.1-7

其中 $\rho\left(x,y\right)=\left\|x-y\right\|$ 即**例 1.1.2 ($n$ 维欧几里得空间)** 中的欧几里得距离.

**(i) 计算 $d\left(\left(1,0,0\right),\left(x_1,x_2,0\right)\right)$.** 设 $\theta$ 为两点在赤道大圆上的中心角. 两点都是单位向量且都在赤道平面 $x_3=0$ 上, 由**基础知识: 单位向量内积与夹角**,

$$
\cos\theta=\left(1,0,0\right)\cdot\left(x_1,x_2,0\right)=x_1.
$$

因 $\theta\in\left[0,\pi\right]$, $\theta=\arccos x_1$. 又由单位球面上以两点为端点的大圆劣弧长等于其中心角, $d\left(\left(1,0,0\right),\left(x_1,x_2,0\right)\right)=\theta$. 故

$$
d\left(\left(1,0,0\right),\left(x_1,x_2,0\right)\right)=\arccos x_1.
$$

结合 $x_1^2+x_2^2=1$, 当 $x_2\ge0$ 时, 也可写为 $d\left(\left(1,0,0\right),\left(x_1,x_2,0\right)\right)=\arcsin x_2$.

**(ii) 证明 $\rho\left(x,y\right)\le d\left(x,y\right)\le\frac{\pi}{2}\rho\left(x,y\right)$.** 设 $\theta=d\left(x,y\right)\in\left[0,\pi\right]$ 为 $x,y$ 的中心角. 由 $\left\|x\right\|=\left\|y\right\|=1$ 及 $x\cdot y=\cos\theta$ (**基础知识: 单位向量内积与夹角**),

$$
\rho\left(x,y\right)^2=\left\|x-y\right\|^2=\left\|x\right\|^2+\left\|y\right\|^2-2x\cdot y=2\left(1-\cos\theta\right)=4\sin^2\frac{\theta}{2},
$$

故 $\rho\left(x,y\right)=2\sin\frac{\theta}{2}$ (因 $\frac{\theta}{2}\in\left[0,\frac{\pi}{2}\right]$, $\sin\frac{\theta}{2}\ge0$).

左边: 令 $u=\frac{\theta}{2}\ge0$, 由**基础知识: $\sin u\le u$**, $2\sin\frac{\theta}{2}\le2\cdot\frac{\theta}{2}=\theta=d\left(x,y\right)$, 即 $\rho\left(x,y\right)\le d\left(x,y\right)$.

右边: 令 $u=\frac{\theta}{2}\in\left[0,\frac{\pi}{2}\right]$, 由**基础知识: $\sin$ 在 $\left[0,\pi/2\right]$ 上的凹弦估计**, $\sin u\ge\frac{2}{\pi}u$, 故

$$
d\left(x,y\right)=\theta=2u\le\pi\sin u=\pi\cdot\frac{\rho\left(x,y\right)}{2}=\frac{\pi}{2}\rho\left(x,y\right).
$$

合并两边即得 $\rho\left(x,y\right)\le d\left(x,y\right)\le\frac{\pi}{2}\rho\left(x,y\right)$.

**(iii) 验证 $d$ 是 $S^2$ 上的度量.** 依据**定义 1.1.1 (度量空间)** 逐条验证.

(i) 劣弧长非负, 故 $d\left(x,y\right)\ge0$; 且 $d\left(x,y\right)=0$ 当且仅当两端点重合的劣弧长度为 $0$, 当且仅当 $x=y$. 非负性与正定性成立.

(ii) $x$ 到 $y$ 的劣弧与 $y$ 到 $x$ 的劣弧是同一段弧, 长度相同, 故 $d\left(x,y\right)=d\left(y,x\right)$. 对称性成立.

(iii) 三角不等式. 记 $\alpha=d\left(x,y\right)$, $\beta=d\left(y,z\right)$, $\gamma=d\left(x,z\right)$, 三者都属于 $\left[0,\pi\right]$.

若 $\alpha+\beta\ge\pi$, 则 $\gamma\le\pi\le\alpha+\beta$, 即 $d\left(x,z\right)\le d\left(x,y\right)+d\left(y,z\right)$, 三角不等式成立.

若 $\alpha+\beta<\pi$, 将 $x,z$ 沿 $y$ 的方向作正交分解: 由 $\left\|x\right\|=\left\|y\right\|=\left\|z\right\|=1$, 存在单位向量 $u,v\perp y$ 使得

$$
x=\cos\alpha\,y+\sin\alpha\,u,\quad z=\cos\beta\,y+\sin\beta\,v.
$$

即把 $x,z$ 平行于 $y$ 的分量取为 $\cos\alpha\,y$, $\cos\beta\,y$, 垂直分量单位化得 $u,v$. 于是

$$
\cos\gamma=x\cdot z=\cos\alpha\cos\beta+\sin\alpha\sin\beta\,\left(u\cdot v\right).
$$

由**引理 1.2.3 (柯西-施瓦茨不等式)** 及 $\left\|u\right\|=\left\|v\right\|=1$, $\left|u\cdot v\right|\le1$, 故 $u\cdot v\ge-1$, 代入上式得

$$
\cos\gamma\ge\cos\alpha\cos\beta-\sin\alpha\sin\beta=\cos\left(\alpha+\beta\right).
$$

因 $\gamma,\alpha+\beta\in\left[0,\pi\right]$ 且由**基础知识: $\cos$ 在 $\left[0,\pi\right]$ 上严格递减**, $\cos\gamma\ge\cos\left(\alpha+\beta\right)$ 推出 $\gamma\le\alpha+\beta$, 即 $d\left(x,z\right)\le d\left(x,y\right)+d\left(y,z\right)$. 三角不等式成立.

由 (i)(ii)(iii) 全部成立, $d$ 是 $S^2$ 上的度量. $\blacksquare$

> 证明技巧: 将 $x,z$ 沿 $y$ 正交分解为平行于 $y$ 与垂直于 $y$ 两部分, 垂直分量的内积由柯西-施瓦茨不等式控制在 $\ge-1$, 由此放缩 $\cos\gamma\ge\cos\left(\alpha+\beta\right)$, 再用 $\cos$ 的严格单调性得到三角不等式.
