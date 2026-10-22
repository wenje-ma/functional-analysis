# week1

> **定义 1.1.1 (度量空间)**<br>设 $X$ 是一个非空集合, 若对于 $X$ 中任意两个元素 $x,y$, 都有一个实数 $d(x,y)$ 与它们对应, 而且满足下面条件: (i) (非负性与正定性) 对任意 $x,y\in X$, $d(x,y)\ge0$, 并且 $d(x,y)=0$ 的充要条件是 $x=y$; (ii) (对称性) 对任意 $x,y\in X$, $d(x,y)=d(y,x)$; (iii) (三角不等式) 对任意 $x,y,z\in X$, $d(x,y)\le d(x,z)+d(z,y)$, 则称 $(X,d)$ 是一个度量空间, $d$ 为 $X$ 上的度量.

> **定义 1.1.2 (极限)**<br>设 $(X,d)$ 是度量空间, $\{x_n\}_{n=1}^\infty$ 是 $X$ 中点列, $x_0\in X$, 若 $\lim_{n\to\infty}d(x_n,x_0)=0$, 则称点列 $\{x_n\}$ 按照度量 $d$ 收敛于 $x_0$, 记为 $\lim_{n\to\infty}x_n=x_0$.

> **例 1.1.2 ($n$ 维欧几里得空间)**<br>在 $n$ 个有序实数组 $x=(x_1,x_2,\cdots,x_n)$ 全体组成的集合 $X$ 中, 定义 $d(x,y)=\sqrt{\sum_{i=1}^{n}(x_i-y_i)^2}$, 则 $(X,d)$ 是度量空间, 称为 $n$ 维欧几里得空间, 通常记为 $\mathbb R^n$.

> **例 1.1.10 (一致收敛与度量收敛)**<br>由例 1.1.6 的讨论可知, $C[a,b]$ 中点列按度量 $d(f,g)=\max_{x\in[a,b]}|f(x)-g(x)|$ 收敛等价于区间 $[a,b]$ 上的函数列一致收敛.

> **例 1.1.11 (等价度量)**<br>设 $(X,d)$ 是度量空间, 在 $X$ 上定义新的度量 $d'(x,y)=\frac{d(x,y)}{1+d(x,y)}$, $d''(x,y)=\ln(1+d(x,y))$, $\forall x,y\in X$, 它们是不同的度量; 且对于空间 $X$ 中的点列 $\{x_n\}$, $\lim_{n\to\infty}x_n\overset d=x_0\Leftrightarrow\lim_{n\to\infty}x_n\overset{d'}=x_0\Leftrightarrow\lim_{n\to\infty}x_n\overset{d''}=x_0$.

> **例 1.1.12 (可测函数等价类空间)**<br>对于有限区间 $[a,b]$, 记 $\mathfrak G=\{[a,b]\text{ 上几乎处处有限的 Lebesgue 可测函数}\}$, $f,g\in\mathfrak G$ 等价是指 $f\doteq_m g$, 仍以 $f$ 表示 $f$ 在 $\mathcal S=\mathfrak G/\sim$ 中对应的等价类; 对于 $f,g\in\mathcal S$, 定义 $d(f,g)=\int_{[a,b]}\frac{|f(t)-g(t)|}{1+|f(t)-g(t)|}\,\mathrm dm(t)$, 这是一个度量, 且 $d(f,g)=0$ 当且仅当 $f\doteq_m g$.

> **引理 1.2.3 (柯西-施瓦茨不等式)**<br>设 $x,y\in H$ ($H$ 为内积空间), 则 $|\langle x,y\rangle|^2\le\langle x,x\rangle\langle y,y\rangle$, 特别地当 $\|x\|=\|y\|=1$ 时 $|\langle x,y\rangle|\le1$.

> **基础知识: 实数绝对值的三角不等式**<br>对任意实数 $a,b$, 有 $|a+b|\le|a|+|b|$, 进而 $|\sum_{i=1}^{n}a_i|\le\sum_{i=1}^{n}|a_i|$.

> **基础知识: 夹逼定理**<br>若数列 $\{a_n\}$ 满足 $0\le a_n\le b_n$, 且 $b_n\to0$, 则 $a_n\to0$.

> **基础知识: 对数与指数函数的连续性**<br>$\ln$ 与 $\exp$ 分别在其定义域上连续, 即 $\lim_{u\to u_0}\ln u=\ln u_0$ ($u_0>0$), $\lim_{v\to v_0}e^v=e^{v_0}$.

> **基础知识: 二项式定理**<br>对任意 $x$ 与正整数 $k$, $(1-x)^k=\sum_{j=0}^{k}\binom{k}{j}(-x)^j$.

> **基础知识: 函数 $\varphi,\psi$ 的单调与凹性**<br>记 $\varphi(t)=\frac{t}{1+t}$, $\psi(t)=\ln(1+t)$, $t\ge0$. 则 $\varphi,\psi$ 在 $[0,\infty)$ 上都严格递增, $\varphi(0)=\psi(0)=0$, 且 $\varphi''(t)=-\frac{2}{(1+t)^3}<0$, $\psi''(t)=-\frac{1}{(1+t)^2}<0$, 即二者都是严格凹函数.

> **基础知识: 凹函数过原点的次可加性**<br>若 $f:[0,\infty)\to[0,\infty)$ 是凹函数且 $f(0)=0$, 则对任意 $a,b\ge0$ 有 $f(a+b)\le f(a)+f(b)$. 事实上, 凹函数的导函数 $f'$ 单调递减, 故 $f(a+b)-f(a)=\int_a^{a+b}f'(s)\,\mathrm ds\le\int_a^{a+b}f'(s-a)\,\mathrm ds=\int_0^bf'(u)\,\mathrm du\le f(b)-f(0)=f(b)$.

> **基础知识: 幂函数的单调性**<br>对任意 $p>0$, $u\mapsto u^p$ 在 $[0,\infty)$ 上严格递增; 特别当 $0<p<1$ 时, $(u^p)''=p(p-1)u^{p-2}<0$ ($u>0$), 即 $t\mapsto t^p$ 在 $[0,\infty)$ 上是凹函数且 $0^p=0$.

> **基础知识: 非负可测函数积分为零的充要条件**<br>若 $g\ge0$ 是 $[0,1]$ 上的 Lebesgue 可测函数, 则 $\int_0^1g(t)\,\mathrm dt=0$ 当且仅当 $g(t)=0$ 几乎处处成立.

> **基础知识: 单位向量内积与夹角**<br>设 $x,y\in\mathbb R^3$, $\|x\|=\|y\|=1$, $\theta\in[0,\pi]$ 为 $x,y$ 的夹角, 则 $x\cdot y=\cos\theta$, 且以 $x,y$ 为端点的大圆劣弧长等于 $\theta$ (单位球面).

> **基础知识: $\sin u\le u$**<br>对任意 $u\ge0$, 有 $\sin u\le u$.

> **基础知识: $\sin$ 在 $[0,\pi/2]$ 上的凹弦估计**<br>$\sin''u=-\sin u<0$ ($u\in(0,\pi/2)$), 故 $\sin$ 在 $[0,\pi/2]$ 上是凹函数, 其图像位于连接 $(0,0)$ 与 $(\pi/2,1)$ 的弦 $y=\frac{2}{\pi}u$ 之上, 即 $\sin u\ge\frac{2}{\pi}u$ ($0\le u\le\frac{\pi}{2}$).

> **基础知识: $\cos$ 在 $[0,\pi]$ 上严格递减**<br>若 $\gamma,\beta\in[0,\pi]$ 且 $\cos\gamma\ge\cos\beta$, 则 $\gamma\le\beta$.

---

## 1.1-2

设 $(X,d)$ 是度量空间, 证明: **例 1.1.11 (等价度量)** 引进的 $d'$ 和 $d''$ 也是 $X$ 上的度量, 并且 $(X,d')$, $(X,d'')$ 中点列的收敛性和在 $(X,d)$ 中是一致的.

其中按**例 1.1.11 (等价度量)** 的定义,

$$
d'(x,y)=\frac{d(x,y)}{1+d(x,y)},\quad d''(x,y)=\ln(1+d(x,y)),\quad \forall x,y\in X.
$$

### 解答 1.1-2

记 $\varphi(t)=\frac{t}{1+t}$, $\psi(t)=\ln(1+t)$ ($t\ge0$). 由**基础知识: 函数 $\varphi,\psi$ 的单调与凹性**, $\varphi,\psi$ 在 $[0,\infty)$ 上严格递增, $\varphi(0)=\psi(0)=0$, 且二者都是严格凹函数. 由**基础知识: 凹函数过原点的次可加性**, $\varphi$ 与 $\psi$ 都满足 $f(a+b)\le f(a)+f(b)$ ($a,b\ge0$).

**第一步: 验证 $d'$ 是 $X$ 上的度量.** 依据**定义 1.1.1 (度量空间)**, 逐条验证 (i)(ii)(iii).

(i) 非负性与正定性. 由 $d$ 是 $X$ 上的度量 (**定义 1.1.1 (度量空间)**(i)), 对任意 $x,y\in X$ 有 $d(x,y)\ge0$, 且 $d(x,y)=0$ 当且仅当 $x=y$. 因 $\varphi$ 的自变量非负, $\varphi(t)\ge0$ ($t\ge0$), 故 $d'(x,y)=\varphi(d(x,y))\ge0$. 又因 $\varphi$ 严格递增且 $\varphi(0)=0$, $\varphi(t)=0$ 当且仅当 $t=0$, 故

$$
d'(x,y)=0\Leftrightarrow\varphi(d(x,y))=0\Leftrightarrow d(x,y)=0\Leftrightarrow x=y.
$$

于是 (i) 成立.

(ii) 对称性. 由**定义 1.1.1 (度量空间)**(ii), $d(x,y)=d(y,x)$, 故 $d'(x,y)=\varphi(d(x,y))=\varphi(d(y,x))=d'(y,x)$. 于是 (ii) 成立.

(iii) 三角不等式. 由**定义 1.1.1 (度量空间)**(iii), $d(x,y)\le d(x,z)+d(z,y)$. 因 $\varphi$ 严格递增, 两端作用 $\varphi$ 得 $d'(x,y)=\varphi(d(x,y))\le\varphi(d(x,z)+d(z,y))$. 由 $\varphi$ 的次可加性 (**基础知识: 凹函数过原点的次可加性**),

$$
\varphi(d(x,z)+d(z,y))\le\varphi(d(x,z))+\varphi(d(z,y))=d'(x,z)+d'(z,y).
$$

故 $d'(x,y)\le d'(x,z)+d'(z,y)$, (iii) 成立. 由 (i)(ii)(iii) 全部成立, 依据**定义 1.1.1 (度量空间)**, $d'$ 是 $X$ 上的度量.

**第二步: 验证 $d''$ 是 $X$ 上的度量.** 同样依据**定义 1.1.1 (度量空间)** 逐条验证.

(i) 由 $d(x,y)\ge0$ 及 $\psi$ 严格递增、$\psi(0)=0$, $\psi(t)\ge0$ 且 $\psi(t)=0$ 当且仅当 $t=0$, 故 $d''(x,y)=\psi(d(x,y))\ge0$, 且 $d''(x,y)=0\Leftrightarrow d(x,y)=0\Leftrightarrow x=y$. (i) 成立.

(ii) 由 $d(x,y)=d(y,x)$, $d''(x,y)=\psi(d(x,y))=\psi(d(y,x))=d''(y,x)$. (ii) 成立.

(iii) 由 $d(x,y)\le d(x,z)+d(z,y)$ 及 $\psi$ 严格递增, $d''(x,y)\le\psi(d(x,z)+d(z,y))$; 再由 $\psi$ 的次可加性 (**基础知识: 凹函数过原点的次可加性**), $\psi(d(x,z)+d(z,y))\le\psi(d(x,z))+\psi(d(z,y))=d''(x,z)+d''(z,y)$. (iii) 成立. 故 $d''$ 也是 $X$ 上的度量.

**第三步: 三种度量下收敛性一致.** 依据**定义 1.1.2 (极限)**, 记 $\epsilon_n=d(x_n,x_0)$, 则

$$
x_n\overset d\to x_0\Leftrightarrow\epsilon_n\to0.
$$

只需证明 $\epsilon_n\to0\Leftrightarrow d'(x_n,x_0)\to0\Leftrightarrow d''(x_n,x_0)\to0$.

(a) $d'$ 与 $d$. 由定义 $d'(x_n,x_0)=\varphi(\epsilon_n)=\frac{\epsilon_n}{1+\epsilon_n}$. 若 $\epsilon_n\to0$, 则 $0\le\frac{\epsilon_n}{1+\epsilon_n}\le\epsilon_n$, 由**基础知识: 夹逼定理** 得 $\frac{\epsilon_n}{1+\epsilon_n}\to0$, 即 $d'(x_n,x_0)\to0$. 反之, 若 $d'(x_n,x_0)=\frac{\epsilon_n}{1+\epsilon_n}\to0$, 则由恒等式 $\epsilon_n=\frac{\epsilon_n/(1+\epsilon_n)}{1-\epsilon_n/(1+\epsilon_n)}$, 其分子趋于 $0$ 而分母趋于 $1\ne0$, 故 $\epsilon_n\to0$. 于是 $x_n\overset d\to x_0\Leftrightarrow x_n\overset{d'}\to x_0$.

(b) $d''$ 与 $d$. 由定义 $d''(x_n,x_0)=\psi(\epsilon_n)=\ln(1+\epsilon_n)$. 若 $\epsilon_n\to0$, 则 $1+\epsilon_n\to1$, 由**基础知识: 对数与指数函数的连续性**, $\ln(1+\epsilon_n)\to\ln1=0$, 即 $d''(x_n,x_0)\to0$. 反之, 若 $\ln(1+\epsilon_n)\to0$, 则由恒等式 $\epsilon_n=e^{\ln(1+\epsilon_n)}-1$ 及**基础知识: 对数与指数函数的连续性**, $e^{\ln(1+\epsilon_n)}-1\to e^0-1=0$, 即 $\epsilon_n\to0$. 于是 $x_n\overset d\to x_0\Leftrightarrow x_n\overset{d''}\to x_0$.

综合 (a)(b),

$$
\lim_{n\to\infty}x_n\overset d=x_0\Leftrightarrow\lim_{n\to\infty}x_n\overset{d'}=x_0\Leftrightarrow\lim_{n\to\infty}x_n\overset{d''}=x_0,
$$

即 $(X,d')$, $(X,d'')$ 中点列的收敛性和在 $(X,d)$ 中是一致的. $\blacksquare$

---

## 1.1-4

设 $X$ 是 $[0,1]$ 上多项式全体. 对于 $P,Q\in X$, $P(x)-Q(x)=\sum_{i=0}^{n}a_ix^i$, 令

$$
d_1(P,Q)=\max_{x\in[0,1]}|P(x)-Q(x)|,\quad d_2(P,Q)=\sum_{i=0}^{n}|a_i|.
$$

证明:

(i) $d_1,d_2$ 都是 $X$ 上的度量.

(ii) 多项式按 $d_1$ 收敛等价于在 $[0,1]$ 上一致收敛于某一多项式.

(iii) 按 $d_2$ 收敛可以推出按 $d_1$ 收敛, 但反之不真 (即存在多项式列 $\{P_k\}$, $d_1(P_k,0)\to0$, 但 $d_2(P_k,0)\not\to0$).

### 解答 1.1-4

**(i) $d_1$ 是 $X$ 上的度量.** 依据**定义 1.1.1 (度量空间)** 逐条验证.

(i) 对任意 $x\in[0,1]$, $|P(x)-Q(x)|\ge0$, 故 $d_1(P,Q)=\max_{x\in[0,1]}|P(x)-Q(x)|\ge0$. 且 $d_1(P,Q)=0$ 当且仅当 $\max_{x\in[0,1]}|P(x)-Q(x)|=0$, 当且仅当 $|P(x)-Q(x)|=0$ 对一切 $x\in[0,1]$ 成立, 当且仅当 $P(x)\equiv Q(x)$, 即 $P=Q$. 非负性与正定性成立.

(ii) 由 $|P(x)-Q(x)|=|Q(x)-P(x)|$ 对任意 $x$ 成立, $d_1(P,Q)=d_1(Q,P)$. 对称性成立.

(iii) 对任意 $R\in X$ 与 $x\in[0,1]$, 由**基础知识: 实数绝对值的三角不等式**,

$$
|P(x)-Q(x)|\le|P(x)-R(x)|+|R(x)-Q(x)|\le d_1(P,R)+d_1(R,Q).
$$

该不等式右端与 $x$ 无关, 故对左端关于 $x\in[0,1]$ 取最大值, 得 $d_1(P,Q)\le d_1(P,R)+d_1(R,Q)$. 三角不等式成立. 故 $d_1$ 是 $X$ 上的度量.

**(i) $d_2$ 是 $X$ 上的度量.** 同样依据**定义 1.1.1 (度量空间)** 逐条验证.

(i) 由 $|a_i|\ge0$ ($\forall i$), $d_2(P,Q)=\sum_{i=0}^{n}|a_i|\ge0$. 且 $d_2(P,Q)=0$ 当且仅当 $\sum_{i=0}^{n}|a_i|=0$, 当且仅当 $a_i=0$ ($\forall i$), 当且仅当 $P-Q\equiv0$, 即 $P=Q$. 非负性与正定性成立.

(ii) 若 $P-Q=\sum_{i=0}^{n}a_ix^i$, 则 $Q-P=\sum_{i=0}^{n}(-a_i)x^i$, 由 $|-a_i|=|a_i|$ 得 $d_2(P,Q)=\sum_{i=0}^{n}|a_i|=\sum_{i=0}^{n}|-a_i|=d_2(Q,P)$. 对称性成立.

(iii) 设 $P-R=\sum_{i=0}^{n}a_ix^i$, $R-Q=\sum_{i=0}^{n}b_ix^i$, 则 $P-Q=(P-R)+(R-Q)=\sum_{i=0}^{n}(a_i+b_i)x^i$. 由**基础知识: 实数绝对值的三角不等式**, $|a_i+b_i|\le|a_i|+|b_i|$ 对每个 $i$ 成立, 对 $i$ 求和得

$$
d_2(P,Q)=\sum_{i=0}^{n}|a_i+b_i|\le\sum_{i=0}^{n}|a_i|+\sum_{i=0}^{n}|b_i|=d_2(P,R)+d_2(R,Q).
$$

三角不等式成立. 故 $d_2$ 也是 $X$ 上的度量.

**(ii) 按 $d_1$ 收敛等价于在 $[0,1]$ 上一致收敛.** 依据**定义 1.1.2 (极限)** 与 $d_1$ 的定义,

$$
P_k\overset{d_1}\to P\Leftrightarrow d_1(P_k,P)=\max_{x\in[0,1]}|P_k(x)-P(x)|\to0.
$$

而 $\max_{x\in[0,1]}|P_k(x)-P(x)|\to0$ 正是函数列 $\{P_k\}$ 在 $[0,1]$ 上一致收敛于 $P$ 的定义. 由**例 1.1.10 (一致收敛与度量收敛)**, $C[a,b]$ 中点列按最大模范量收敛等价于在 $[a,b]$ 上一致收敛; 多项式空间 $X\subset C[0,1]$ 作为子空间继承这一对应. 故按 $d_1$ 收敛等价于在 $[0,1]$ 上一致收敛于某一多项式.

**(iii) 按 $d_2$ 收敛推出按 $d_1$ 收敛.** 设 $P_k\overset{d_2}\to Q$, 记 $P_k-Q=\sum_{i=0}^{n_k}a_i^{(k)}x^i$, 则 $d_2(P_k,Q)=\sum_{i=0}^{n_k}|a_i^{(k)}|\to0$. 对任意 $x\in[0,1]$, 有 $0\le x^i\le1$ 对每个 $i$ 成立, 由**基础知识: 实数绝对值的三角不等式**,

$$
|P_k(x)-Q(x)|=\left|\sum_{i=0}^{n_k}a_i^{(k)}x^i\right|\le\sum_{i=0}^{n_k}|a_i^{(k)}|x^i\le\sum_{i=0}^{n_k}|a_i^{(k)}|=d_2(P_k,Q).
$$

上式对一切 $x\in[0,1]$ 一致成立且右端趋于 $0$, 故 $d_1(P_k,Q)=\max_{x\in[0,1]}|P_k(x)-Q(x)|\to0$, 即 $P_k\overset{d_1}\to Q$.

**(iii) 反之不真.** 取 $P_k(x)=x^k(1-x)^k$. 由**基础知识: 二项式定理**,

$$
P_k(x)=x^k\sum_{j=0}^{k}\binom{k}{j}(-x)^j=\sum_{j=0}^{k}\binom{k}{j}(-1)^jx^{k+j}.
$$

一方面, $x(1-x)=\frac14-(x-\frac12)^2\le\frac14$, 等号在 $x=\frac12$ 处成立, 故 $\max_{x\in[0,1]}x(1-x)=\frac14$; 又 $u\mapsto u^k$ 在 $[0,\infty)$ 上严格递增 (**基础知识: 幂函数的单调性**), 所以

$$
d_1(P_k,0)=\max_{x\in[0,1]}[x(1-x)]^k=\left(\max_{x\in[0,1]}x(1-x)\right)^k=\left(\frac14\right)^k\to0.
$$

另一方面, $d_2(P_k,0)=\sum_{j=0}^{k}\left|\binom{k}{j}(-1)^j\right|=\sum_{j=0}^{k}\binom{k}{j}=2^k\to\infty$, 不趋于 $0$. 故存在多项式列 $\{P_k\}$ 使 $d_1(P_k,0)\to0$ 而 $d_2(P_k,0)\not\to0$, 反之不真. $\blacksquare$

> 构造思路: 要找一个函数值很小但系数很大的多项式, 需函数中含大量正负抵消项; $(-1)^j$ 天然合适, 二项式展开恰好提供交错系数, 故取 $x^k(1-x)^k$, 其 $d_2$-系数和恰为 $2^k$.

---

## 1.1-5

对 $0<p<1$, 记 $\mathcal L^p[0,1]$ 是区间 $[a,b]$ 上 Lebesgue 可测且 $p$ 次可积的函数全体. 令

$$
d(f,g)=\int_0^1|f(t)-g(t)|^p\,\mathrm dt.
$$

证明:

(i) 当数 $a,b>0$ 时, $(a+b)^p\le a^p+b^p$.

(ii) $d$ 是伪度量, 即 $d$ 是非负的且满足定义 1.1.1(ii) 及 (iii).

(iii) 若等价关系 $f\sim g$ 是指两个函数 $f,g$ 满足 $f\doteq_m g$, 仍以 $f$ 来表示 $p$ 次可积函数 $f$ 在 $L^p[a,b]=\mathcal L^p[a,b]/\sim$ 中对应的等价类, 则 $(L^p[a,b],d)$ 是度量空间.

### 解答 1.1-5

**(i) 对 $a,b>0$, 证明 $(a+b)^p\le a^p+b^p$.** 令 $f(t)=t^p$ ($t\ge0$). 由 $0<p<1$, $(t^p)''=p(p-1)t^{p-2}<0$ ($t>0$), 且 $f(0)=0$, 故 $f$ 是 $[0,\infty)$ 上的凹函数 (**基础知识: 幂函数的单调性**). 由**基础知识: 凹函数过原点的次可加性**, $f(a+b)\le f(a)+f(b)$, 即 $(a+b)^p\le a^p+b^p$ 对 $a,b\ge0$ 成立, 特别对 $a,b>0$ 成立.

**(ii) 验证 $d$ 是伪度量.** 依据**定义 1.1.1 (度量空间)**, 验证非负性、(ii) 对称性与 (iii) 三角不等式 (不要求 (i) 中的正定性).

非负性: 对任意 $f,g$, 逐点有 $|f(t)-g(t)|^p\ge0$, 故 $d(f,g)=\int_0^1|f(t)-g(t)|^p\,\mathrm dt\ge0$.

(ii) 对称性: 逐点有 $|f(t)-g(t)|=|g(t)-f(t)|$, 故 $|f(t)-g(t)|^p=|g(t)-f(t)|^p$, 积分得 $d(f,g)=d(g,f)$.

(iii) 三角不等式: 对任意第三个可测函数 $h$ 与每个 $t$, 由**基础知识: 实数绝对值的三角不等式**, $|f(t)-g(t)|\le|f(t)-h(t)|+|h(t)-g(t)|$. 因 $u\mapsto u^p$ 在 $[0,\infty)$ 上严格递增 (**基础知识: 幂函数的单调性**), 两端取 $p$ 次幂得

$$
|f(t)-g(t)|^p\le\left(|f(t)-h(t)|+|h(t)-g(t)|\right)^p.
$$

对右端用已证的 (i), 取 $a=|f(t)-h(t)|$, $b=|h(t)-g(t)|$, 得

$$
\left(|f(t)-h(t)|+|h(t)-g(t)|\right)^p\le|f(t)-h(t)|^p+|h(t)-g(t)|^p.
$$

两式合并得逐点不等式 $|f(t)-g(t)|^p\le|f(t)-h(t)|^p+|h(t)-g(t)|^p$, 对 $t$ 在 $[0,1]$ 上积分即得

$$
d(f,g)\le\int_0^1|f(t)-h(t)|^p\,\mathrm dt+\int_0^1|h(t)-g(t)|^p\,\mathrm dt=d(f,h)+d(h,g).
$$

(iii) 成立. 综上, $d$ 是非负的且满足 (ii)(iii), 即 $d$ 是伪度量.

**(iii) 商空间 $(L^p[a,b],d)$ 是度量空间.** 由 (ii), 非负性、对称性与三角不等式在商空间 $L^p[a,b]=\mathcal L^p[a,b]/\sim$ 上仍然成立, 依据**定义 1.1.1 (度量空间)** 只需再验证正定性. 对等价类 $[f],[g]$,

$$
d([f],[g])=0\Leftrightarrow\int_0^1|f(t)-g(t)|^p\,\mathrm dt=0.
$$

因被积函数 $|f(t)-g(t)|^p\ge0$ 且可测, 由**基础知识: 非负可测函数积分为零的充要条件**, 上式当且仅当 $|f(t)-g(t)|^p=0$ 几乎处处成立, 当且仅当 $f(t)=g(t)$ 几乎处处成立, 即 $f\doteq_m g$, 亦即 $f\sim g$, 故 $[f]=[g]$. 这一"几乎处处相等作商、$d=0$ 当且仅当等价"的构造与**例 1.1.12 (可测函数等价类空间)** 相同. 于是正定性成立, $(L^p[a,b],d)$ 是度量空间. $\blacksquare$

---

## 1.1-7

在三维 Euclid 空间 $\mathbb R^3$ 中, 考虑单位球面

$$
S^2=\{x\in\mathbb R^3:\ x=(x_1,x_2,x_3),\ x_1^2+x_2^2+x_3^2=1\}.
$$

对于 $x,y\in S^2$, 规定 $d(x,y)$ 为过 $x,y$ 两点的大圆上以 $x,y$ 为端点的劣弧的弧长, 它在三维 Euclid 空间的正交变换下是保持不变的.

(i) 对于 $x_1^2+x_2^2=1$, 计算 $d((1,0,0),(x_1,x_2,0))$.

(ii) 如果用 $\rho(x,y)$ 表示 Euclid 距离, 证明:

$$
\rho(x,y)\le d(x,y)\le\frac{\pi}{2}\rho(x,y).
$$

(iii) 证明: $d$ 是 $S^2$ 上的度量.

### 解答 1.1-7

其中 $\rho(x,y)=\left\|x-y\right\|$ 即**例 1.1.2 ($n$ 维欧几里得空间)** 中的欧几里得距离.

**(i) 计算 $d((1,0,0),(x_1,x_2,0))$.** 设 $\theta$ 为两点在赤道大圆上的中心角. 两点都是单位向量且都在赤道平面 $x_3=0$ 上, 由**基础知识: 单位向量内积与夹角**,

$$
\cos\theta=(1,0,0)\cdot(x_1,x_2,0)=x_1.
$$

因 $\theta\in[0,\pi]$, $\theta=\arccos x_1$. 又由单位球面上以两点为端点的大圆劣弧长等于其中心角, $d((1,0,0),(x_1,x_2,0))=\theta$. 故

$$
d((1,0,0),(x_1,x_2,0))=\arccos x_1.
$$

结合 $x_1^2+x_2^2=1$, 当 $x_2\ge0$ 时, 也可写为 $d((1,0,0),(x_1,x_2,0))=\arcsin x_2$.

**(ii) 证明 $\rho(x,y)\le d(x,y)\le\frac{\pi}{2}\rho(x,y)$.** 设 $\theta=d(x,y)\in[0,\pi]$ 为 $x,y$ 的中心角. 由 $\|x\|=\|y\|=1$ 及 $x\cdot y=\cos\theta$ (**基础知识: 单位向量内积与夹角**),

$$
\rho(x,y)^2=\left\|x-y\right\|^2=\|x\|^2+\|y\|^2-2x\cdot y=2(1-\cos\theta)=4\sin^2\frac{\theta}{2},
$$

故 $\rho(x,y)=2\sin\frac{\theta}{2}$ (因 $\frac{\theta}{2}\in[0,\frac{\pi}{2}]$, $\sin\frac{\theta}{2}\ge0$).

左边: 令 $u=\frac{\theta}{2}\ge0$, 由**基础知识: $\sin u\le u$**, $2\sin\frac{\theta}{2}\le2\cdot\frac{\theta}{2}=\theta=d(x,y)$, 即 $\rho(x,y)\le d(x,y)$.

右边: 令 $u=\frac{\theta}{2}\in[0,\frac{\pi}{2}]$, 由**基础知识: $\sin$ 在 $[0,\pi/2]$ 上的凹弦估计**, $\sin u\ge\frac{2}{\pi}u$, 故

$$
d(x,y)=\theta=2u\le\pi\sin u=\pi\cdot\frac{\rho(x,y)}{2}=\frac{\pi}{2}\rho(x,y).
$$

合并两边即得 $\rho(x,y)\le d(x,y)\le\frac{\pi}{2}\rho(x,y)$.

**(iii) 验证 $d$ 是 $S^2$ 上的度量.** 依据**定义 1.1.1 (度量空间)** 逐条验证.

(i) 劣弧长非负, 故 $d(x,y)\ge0$; 且 $d(x,y)=0$ 当且仅当两端点重合的劣弧长度为 $0$, 当且仅当 $x=y$. 非负性与正定性成立.

(ii) $x$ 到 $y$ 的劣弧与 $y$ 到 $x$ 的劣弧是同一段弧, 长度相同, 故 $d(x,y)=d(y,x)$. 对称性成立.

(iii) 三角不等式. 记 $\alpha=d(x,y)$, $\beta=d(y,z)$, $\gamma=d(x,z)$, 三者都属于 $[0,\pi]$.

若 $\alpha+\beta\ge\pi$, 则 $\gamma\le\pi\le\alpha+\beta$, 即 $d(x,z)\le d(x,y)+d(y,z)$, 三角不等式成立.

若 $\alpha+\beta<\pi$, 将 $x,z$ 沿 $y$ 的方向作正交分解: 由 $\|x\|=\|y\|=\|z\|=1$, 存在单位向量 $u,v\perp y$ 使得

$$
x=\cos\alpha\,y+\sin\alpha\,u,\quad z=\cos\beta\,y+\sin\beta\,v.
$$

即把 $x,z$ 平行于 $y$ 的分量取为 $\cos\alpha\,y$, $\cos\beta\,y$, 垂直分量单位化得 $u,v$. 于是

$$
\cos\gamma=x\cdot z=\cos\alpha\cos\beta+\sin\alpha\sin\beta\,(u\cdot v).
$$

由**引理 1.2.3 (柯西-施瓦茨不等式)** 及 $\|u\|=\|v\|=1$, $|u\cdot v|\le1$, 故 $u\cdot v\ge-1$, 代入上式得

$$
\cos\gamma\ge\cos\alpha\cos\beta-\sin\alpha\sin\beta=\cos(\alpha+\beta).
$$

因 $\gamma,\alpha+\beta\in[0,\pi]$ 且由**基础知识: $\cos$ 在 $[0,\pi]$ 上严格递减**, $\cos\gamma\ge\cos(\alpha+\beta)$ 推出 $\gamma\le\alpha+\beta$, 即 $d(x,z)\le d(x,y)+d(y,z)$. 三角不等式成立.

由 (i)(ii)(iii) 全部成立, $d$ 是 $S^2$ 上的度量. $\blacksquare$

> 证明技巧: 将 $x,z$ 沿 $y$ 正交分解为平行于 $y$ 与垂直于 $y$ 两部分, 垂直分量的内积由柯西-施瓦茨不等式控制在 $\ge-1$, 由此放缩 $\cos\gamma\ge\cos(\alpha+\beta)$, 再用 $\cos$ 的严格单调性得到三角不等式.
