# week1

> **定义 1.1.1** (度量空间) 设 $X$ 是一个非空集合, 若对于 $X$ 中任意两个元素 $x,y$, 有一个实数 $d\left(x,y\right)$ 与它们对应, 而且满足下面条件:<br>(i) **(非负性与正定性)** 对任意 $x,y\in X$, $d\left(x,y\right)\ge0$, 并且 $d\left(x,y\right)=0$ 的充要条件是 $x=y$;<br>(ii) **(对称性)** 对任意 $x,y\in X$, $d\left(x,y\right)=d\left(y,x\right)$;<br>(iii) **(三角不等式)** 对任意 $x,y,z\in X$, $d\left(x,y\right)\le d\left(x,z\right)+d\left(z,y\right)$,<br>则称 $\left(X,d\right)$ 是一个**度量空间** (或**距离空间**), $d$ 为 $X$ 上的**度量** (或**距离**), $d\left(x,y\right)$ 为**点 $x,y$ 之间的距离**.

> **定义 1.1.2** (极限) 设 $\left(X,d\right)$ 是度量空间, $\left\{x_n\right\}_{n=1}^\infty$ 是 $X$ 中点列, $x_0\in X$, 若 $$\lim_{n\to\infty}d\left(x_n,x_0\right)=0,$$ 则称**点列 $\left\{x_n\right\}_{n=1}^\infty$ 按照度量 $d$ 收敛于 $x_0$**, 记为 $\lim_{n\to\infty}x_n=x_0$.

> **例 1.1.2** ($n$ 维欧几里得空间) 在 $n$ 个有序实数组 $x=\left(x_1,x_2,\cdots,x_n\right)$ 全体组成的集合 $X$ 中, 定义 $$d\left(x,y\right)=\sqrt{\sum_{i=1}^{n}\left(x_i-y_i\right)^2},$$ 则 $\left(X,d\right)$ 是度量空间, 称为 $n$ 维欧几里得空间, 通常记为 $\mathbb R^n$.

> **例 1.1.10** (一致收敛与度量收敛) 由例 1.1.10 的讨论可知, $C\left[a,b\right]$ 中点列按度量 $d$ 收敛等价于区间 $\left[a,b\right]$ 上的函数列一致收敛.

> **例 1.1.11** (等价度量) 设 $\left(X,d\right)$ 是度量空间, 我们还可以在 $X$ 上定义新的度量 $$d'\left(x,y\right)=\frac{d\left(x,y\right)}{1+d\left(x,y\right)},\quad d''\left(x,y\right)=\ln\left(1+d\left(x,y\right)\right),\quad\forall x,y\in X,$$ 它们是不同的度量. 但是容易验证, 对于空间 $X$ 中的点列 $\left\{x_n\right\}$, $$\lim_{n\to\infty}x_n\overset d=x_0\Leftrightarrow\lim_{n\to\infty}x_n\overset{d'}=x_0\Leftrightarrow\lim_{n\to\infty}x_n\overset{d''}=x_0.$$

> **例 1.1.12** (可测函数等价类空间) 对于有限区间 $\left[a,b\right]$, 记 $\mathfrak G=\left\{\left[a,b\right]\text{ 上几乎处处有限的勒贝格可测函数}\right\}$. $\mathfrak G$ 中两个函数 $f,g$ 是**等价**的, 是指它们满足 $f\underset{m}{\doteq}g$. 仍以 $f$ 来表示勒贝格可测函数 $f$ 在 $\mathcal S=\mathfrak G/\sim$ 中对应的等价类. 对于 $f,g\in\mathcal S$, 定义 $$d\left(f,g\right)=\int_{\left[a,b\right]}\frac{\left|f\left(t\right)-g\left(t\right)\right|}{1+\left|f\left(t\right)-g\left(t\right)\right|}\mathrm dm\left(t\right),$$ 容易验证这是一个度量, 进而 $\left(\mathcal S,d\right)$ 是完备的度量空间.

> **引理 1.2.3** (柯西-施瓦茨不等式) 设 $x,y\in H$, 则成立不等式 $$ \left|\left\langle x,y\right\rangle\right|^2\le\left\langle x,x\right\rangle\left\langle y,y\right\rangle. $$

> **预备 (关键引理)** 记 $\varphi\left(t\right)=\frac{t}{1+t}$, $\psi\left(t\right)=\ln\left(1+t\right)$, $t\ge0$. 则 $\varphi,\psi$ 在 $\left[0,\infty\right)$ 上都是**凹函数**且 $\varphi\left(0\right)=\psi\left(0\right)=0$. 求其二阶导易证.

## 1.1-2

设 $\left(X,d\right)$ 是度量空间, 在 $X$ 上定义

$$
d'\left(x,y\right)=\frac{d\left(x,y\right)}{1+d\left(x,y\right)},\quad\forall x,y\in X
$$

和

$$
d''\left(x,y\right)=\ln\left(1+d\left(x,y\right)\right),\quad\forall x,y\in X.
$$

证明: $d'$ 和 $d''$ 都是 $X$ 上的度量, 并且 $\left(X,d'\right)$, $\left(X,d''\right)$ 中点列的收敛性和在 $\left(X,d\right)$ 中是一致的.

### 解答 1.1-2

**第一步: 验证 $d'$ 是 $X$ 上的度量.**

依据**定义 1.1.1 (度量空间)**, 需逐条验证 $d'$ 满足 (i)(ii)(iii).

**(i) 非负性与正定性.** 由 $d$ 是度量, 对任意 $x,y\in X$ 有 $d\left(x,y\right)\ge0$, 且 $d\left(x,y\right)=0\Leftrightarrow x=y$ (**定义 1.1.1 (i)** (度量空间)). 又因为 $\varphi\left(t\right)\ge0$ 对所有 $t\ge0$ 成立, 且 $\varphi$ 在 $\left[0,\infty\right)$ 严格递增且 $\varphi\left(0\right)=0$, 则 $\varphi\left(t\right)=0\Leftrightarrow t=0$. 于是 $d'\left(x,y\right)=\varphi\left(d\left(x,y\right)\right)\ge0$, 且 $d'\left(x,y\right)=0\Leftrightarrow\varphi\left(d\left(x,y\right)\right)=0\Leftrightarrow d\left(x,y\right)=0\Leftrightarrow x=y$. 故 (i) 成立.

**(ii) 对称性.** 由 $d$ 的对称性 (**定义 1.1.1 (ii)** (度量空间)), $d\left(x,y\right)=d\left(y,x\right)$.于是 $d'\left(x,y\right)=\varphi\left(d\left(x,y\right)\right)=\varphi\left(d\left(y,x\right)\right)=d'\left(y,x\right)$. 故 (ii) 成立.

**(iii) 三角不等式.** 由 $d$ 满足三角不等式 (**定义 1.1.1 (iii)** (度量空间)), $d\left(x,y\right)\le d\left(x,z\right)+d\left(z,y\right)$. 因 $\varphi$ 在 $\left[0,\infty\right)$ 单调递增, 上式两边作用 $\varphi$ 得 $d'\left(x,y\right)=\varphi\left(d\left(x,y\right)\right)\le\varphi\left(d\left(x,z\right)+d\left(z,y\right)\right)$. 由**预备** (关键引理), $\varphi\left(d\left(x,z\right)+d\left(z,y\right)\right)\le\varphi\left(d\left(x,z\right)\right)+\varphi\left(d\left(z,y\right)\right)=d'\left(x,z\right)+d'\left(z,y\right)$. 故 $d'\left(x,y\right)\le d'\left(x,z\right)+d'\left(z,y\right)$, (iii) 成立.

由 (i)(ii)(iii) 全部成立, 依据**定义 1.1.1 (度量空间)**, $d'$ 是 $X$ 上的度量. $\blacksquare$

**第二步: 验证 $d''$ 是 $X$ 上的度量.**

依据**定义 1.1.1 (度量空间)**, 同样逐条验证.

**(i) 非负性与正定性.** 因 $d\left(x,y\right)\ge0$, $\ln$ 严格递增且 $\psi\left(0\right)=0$, $\psi\left(t\right)=\ln\left(1+t\right)\ge0$, $\psi\left(t\right)=0\Leftrightarrow t=0$, 于是 $d''\left(x,y\right)=\psi\left(d\left(x,y\right)\right)\ge0$, 且 $d''\left(x,y\right)=0\Leftrightarrow d\left(x,y\right)=0\Leftrightarrow x=y$. 故 (i) 成立.

**(ii) 对称性.**

$d''\left(x,y\right)=\psi\left(d\left(x,y\right)\right)=\psi\left(d\left(y,x\right)\right)=d''\left(y,x\right)$. 故 (ii) 成立.

**(iii) 三角不等式.** 由 $d\left(x,y\right)\le d\left(x,z\right)+d\left(z,y\right)$ 及 $\psi$ 单调递增, $d''\left(x,y\right)=\psi\left(d\left(x,y\right)\right)\le\psi\left(d\left(x,z\right)+d\left(z,y\right)\right)$. 由**预备** (关键引理) 中 $\psi$ 的次可加性, $\psi\left(d\left(x,z\right)+d\left(z,y\right)\right)\le\psi\left(d\left(x,z\right)\right)+\psi\left(d\left(z,y\right)\right)=d''\left(x,z\right)+d''\left(z,y\right)$. 故 (iii) 成立.

故 $d''$ 也是 $X$ 上的度量. $\blacksquare$

**第三步: 三种度量下收敛性一致.**

依据**定义 1.1.2 (极限)**, 设 $\epsilon_n=d\left(x_n,x_0\right)$, 则

$$
x_n\overset d\to x_0\Leftrightarrow\epsilon_n\to0.
$$

只需证 $\epsilon_n\to0\Leftrightarrow d'\left(x_n,x_0\right)\to0\Leftrightarrow d''\left(x_n,x_0\right)\to0$.

**(a) $d'$ 与 $d$.** 由定义 $d'\left(x_n,x_0\right)=\varphi\left(\epsilon_n\right)=\frac{\epsilon_n}{1+\epsilon_n}$. 若 $\epsilon_n\to0$, 则 $\epsilon_n\ge0$ 且 $0\le\frac{\epsilon_n}{1+\epsilon_n}\le\epsilon_n$, 由夹逼定理 $\frac{\epsilon_n}{1+\epsilon_n}\to0$, 即 $d'\left(x_n,x_0\right)\to0$. 反之若 $d'\left(x_n,x_0\right)=\frac{\epsilon_n}{1+\epsilon_n}\to0$, 注意到 $\epsilon_n=\frac{\epsilon_n/\left(1+\epsilon_n\right)}{1-\epsilon_n/\left(1+\epsilon_n\right)}$, 而 $\frac{\epsilon_n}{1+\epsilon_n}\to0\implies1-\frac{\epsilon_n}{1+\epsilon_n}\to1\ne0$, 故 $\epsilon_n\to0$. 于是 $x_n\overset d\to x_0\Leftrightarrow x_n\overset{d'}\to x_0$.

**(b) $d''$ 与 $d$.** 由定义 $d''\left(x_n,x_0\right)=\psi\left(\epsilon_n\right)=\ln\left(1+\epsilon_n\right)$. 因 $\ln$ 在 $\left(0,\infty\right)$ 严格递增且连续, $\ln\left(1+\epsilon_n\right)\to0\Leftrightarrow\epsilon_n\to0$ (用 $\epsilon_n=\mathrm e^{\ln\left(1+\epsilon_n\right)}-1$, 及 $\epsilon_n\ge0$). 故 $x_n\overset d\to x_0\Leftrightarrow x_n\overset{d''}\to x_0$.

综上, 由 (a)(b) 得

$$
\lim_{n\to\infty}x_n\overset d=x_0\Leftrightarrow\lim_{n\to\infty}x_n\overset{d'}=x_0\Leftrightarrow\lim_{n\to\infty}x_n\overset{d''}=x_0.
$$

即 $\left(X,d'\right)$, $\left(X,d''\right)$ 中点列的收敛性和在 $\left(X,d\right)$ 中是一致的. $\blacksquare$

## 1.1-4

设 $X$ 是 $\left[0,1\right]$ 上多项式全体. 对于 $P,Q\in X$, $P\left(x\right)-Q\left(x\right)=\sum_{i=0}^{n}a_ix^i$, 令

$$
\begin{aligned}d_1\left(P,Q\right)&=\max_{x\in\left[0,1\right]}\left|P\left(x\right)-Q\left(x\right)\right|,\\
d_2\left(P,Q\right)&=\sum_{i=0}^{n}\left|a_i\right|.
\end{aligned}
$$

证明

(1) $d_1,d_2$ 都是 $X$ 上的度量.

(2) 多项式按 $d_1$ 收敛等价于在 $\left[0,1\right]$ 上一致收敛于某一多项式.

(3) 按 $d_2$ 收敛可以推出按 $d_1$ 收敛, 但反之不真 (即存在多项式列 $\left\{P_k\right\},d_1\left(P_k,0\right)\to 0$, 但 $d_2\left(P_k,0\right)\not\rightarrow 0$).

### 解答 1.1-4

**(1) $d_1$ 是 $X$ 上的度量.**

依据**定义 1.1.1 (度量空间)**, 逐条验证.

**(i) 非负性与正定性.** 对任意 $x\in\left[0,1\right]$, $\left|P\left(x\right)-Q\left(x\right)\right|\ge0$, 故 $d_1\left(P,Q\right)\ge0$. 且 $d_1\left(P,Q\right)=0\Leftrightarrow\max_{x\in\left[0,1\right]}\left|P\left(x\right)-Q\left(x\right)\right|=0\Leftrightarrow\left|P\left(x\right)-Q\left(x\right)\right|=0\ \left(\forall x\in\left[0,1\right]\right)\Leftrightarrow P\left(x\right)-Q\left(x\right)\equiv0\Leftrightarrow P=Q$. 故 (i) 成立.

**(ii) 对称性.** $\left|P\left(x\right)-Q\left(x\right)\right|=\left|Q\left(x\right)-P\left(x\right)\right|$ 对任意 $x$ 成立, 故 $d_1\left(P,Q\right)=\max\left|P-Q\right|=\max\left|Q-P\right|=d_1\left(Q,P\right)$. 故 (ii) 成立.

**(iii) 三角不等式.** 由实数绝对值的三角不等式, 对任意 $R\in X$ 与 $x\in\left[0,1\right]$,

$$
\left|P\left(x\right)-Q\left(x\right)\right|\le\left|P\left(x\right)-R\left(x\right)\right|+\left|R\left(x\right)-Q\left(x\right)\right|\le d_1\left(P,R\right)+d_1\left(R,Q\right).
$$

对 $x$ 取最大值 (第一个不等式对一切 $x$ 成立, 右端与 $x$ 无关), 得 $d_1\left(P,Q\right)\le d_1\left(P,R\right)+d_1\left(R,Q\right)$. 故 (iii) 成立.

由 (i)(ii)(iii), $d_1$ 是 $X$ 上的度量. $\blacksquare$

**(1) $d_2$ 是 $X$ 上的度量.**

依据**定义 1.1.1 (度量空间)**, 逐条验证.

**(i) 非负性与正定性.** $\left|a_i\right|\ge0$ 对每个 $i$, 故 $d_2\left(P,Q\right)=\sum_{i=0}^{n}\left|a_i\right|\ge0$. 且 $d_2\left(P,Q\right)=0\Leftrightarrow\sum_{i=0}^{n}\left|a_i\right|=0\Leftrightarrow a_i=0\ \left(\forall i\right)\Leftrightarrow P-Q\equiv0\Leftrightarrow P=Q$. 故 (i) 成立.

**(ii) 对称性.** 若 $P-Q=\sum a_ix^i$, 则 $Q-P=\sum\left(-a_i\right)x^i$, 且 $\left|-a_i\right|=\left|a_i\right|$, 故 $d_2\left(P,Q\right)=\sum\left|a_i\right|=\sum\left|-a_i\right|=d_2\left(Q,P\right)$. 故 (ii) 成立.

**(iii) 三角不等式.** 设 $P-R=\sum_{i=0}^{n}a_ix^i$, $R-Q=\sum_{i=0}^{n}b_ix^i$, 则 $P-Q=\left(P-R\right)+\left(R-Q\right)=\sum_{i=0}^{n}\left(a_i+b_i\right)x^i$. 由实数绝对值的三角不等式, $\left|a_i+b_i\right|\le\left|a_i\right|+\left|b_i\right|$ 对每个 $i$ 成立, 求和得

$$
d_2\left(P,Q\right)=\sum_{i=0}^{n}\left|a_i+b_i\right|\le\sum_{i=0}^{n}\left|a_i\right|+\sum_{i=0}^{n}\left|b_i\right|=d_2\left(P,R\right)+d_2\left(R,Q\right).
$$

故 (iii) 成立.

由 (i)(ii)(iii), $d_2$ 也是 $X$ 上的度量. $\blacksquare$

**(2) 按 $d_1$ 收敛 $\Leftrightarrow$ 在 $\left[0,1\right]$ 上一致收敛.**

依据**定义 1.1.2 (极限)** 与 $d_1$ 的定义,

$$
P_k\overset{d_1}\to P\Leftrightarrow d_1\left(P_k,P\right)=\max_{x\in\left[0,1\right]}\left|P_k\left(x\right)-P\left(x\right)\right|\to0.
$$

而 $\max_{x\in\left[0,1\right]}\left|P_k\left(x\right)-P\left(x\right)\right|\to0$ 正是 $\left\{P_k\right\}$ 在 $\left[0,1\right]$ 上一致收敛于 $P$ 的定义 (即**例 1.1.10** (一致收敛与度量收敛) 在多项式子空间上的情形). 故 (2) 成立. $\blacksquare$

**(3) 按 $d_2$ 收敛推出按 $d_1$ 收敛.**

设 $P_k\overset{d_2}\to Q$, 记 $P_k-Q=\sum_{i=0}^{n_k}a_i^{\left(k\right)}x^i$, 则由定义 $d_2\left(P_k,Q\right)=\sum_{i=0}^{n_k}\left|a_i^{\left(k\right)}\right|\to0$. 对任意 $x\in\left[0,1\right]$, 有 $x^i\le1$ 对每个 $i$ 成立, 故由三角不等式

$$
\left|P_k\left(x\right)-Q\left(x\right)\right|=\left|\sum_{i=0}^{n_k}a_i^{\left(k\right)}x^i\right|\le\sum_{i=0}^{n_k}\left|a_i^{\left(k\right)}\right|x^i\le\sum_{i=0}^{n_k}\left|a_i^{\left(k\right)}\right|=d_2\left(P_k,Q\right)\to0.
$$

上式对一切 $x\in\left[0,1\right]$ 一致成立, 故 $d_1\left(P_k,Q\right)=\max_{x}\left|P_k\left(x\right)-Q\left(x\right)\right|\to0$, 即 $P_k\overset{d_1}\to Q$. $\blacksquare$

**(3) 反之不真 (存在反例).**

取 $P_k\left(x\right)=x^k\left(1-x\right)^k=\sum_{j=0}^{k}\binom{k}{j}\left(-1\right)^jx^{k+j}$ (用二项式定理展开). 一方面,

$$
d_1\left(P_k,0\right)=\max_{x\in\left[0,1\right]}\left|P_k\left(x\right)\right|=\max_{x\in\left[0,1\right]}\left[x\left(1-x\right)\right]^k=\left(\max_{x\in\left[0,1\right]}x\left(1-x\right)\right)^k=\left(\frac14\right)^k\to0,
$$

其中 $\max_{x\in\left[0,1\right]}x\left(1-x\right)=\frac14$ 在 $x=\frac12$ 取到. 另一方面, $d_2\left(P_k,0\right)=\sum_{j=0}^{k}\binom{k}{j}=2^k\to\infty\not\to0$. 故存在多项式列 $\left\{P_k\right\}$ 使 $d_1\left(P_k,0\right)\to0$ 而 $d_2\left(P_k,0\right)\not\to0$. $\blacksquare$

> **构造思路** 要找一个函数值很小但系数很大的多项式: 需函数中含大量正负抵消项, 而 $\left(-1\right)^n$ 天然合适, 二项式展开恰好提供交错系数, 故取 $x^k\left(1-x\right)^k$, 其 $d_2$-系数和恰为 $2^k$.

## 1.1-5

对 $0<p<1$, 记 $L^p\left[0,1\right]$ 是区间 $\left[a,b\right]$ 上勒贝格可测且 $p$ 次可积的函数全体. 令

$$
d\left(f,g\right)=\int_{0}^{1}\left|f\left(t\right)-g\left(t\right)\right|^p\mathrm dt.
$$

证明:

(1) 当数 $a,b>0$ 时, $\left(a+b\right)^p \le a^p+b^p$.

(2) $d$ 是伪度量, 即 $d$ 是非负的且满足定义 1.1.1 (ii) 及 (iii).

(3) 若等价关系 $f\sim g$ 是指两个函数 $f,g$ 满足 $f\underset{m}{\doteq}g$, 仍以 $f$ 来表示 $p$ 次可积函数 $f$ 在 $L^p\left[a,b\right]=L^p\left[a,b\right]/\sim$ 中对应的等价类, 则 $\left(L^p\left[a,b\right],d\right)$ 是度量空间.

### 解答 1.1-5

**(1) 对 $a,b>0$, $\left(a+b\right)^p\le a^p+b^p$.**

因 $0<p<1$, 函数 $t\mapsto t^p$ 在 $\left(0,\infty\right)$ 上是**凹函数** ($\left(t^p\right)''=p\left(p-1\right)t^{p-2}<0$), 且 $\left(t^p\right)$ 在 $t=0$ 处取值为 $0$, 故它是次可加的. 于是对任意 $a,b\ge0$, $\left(a+b\right)^p\le a^p+b^p$. 特别对 $a,b>0$ 成立. $\blacksquare$

**(2) $d$ 是伪度量.**

依据**定义 1.1.1 (度量空间)**, 验证非负性, 对称性 (ii) 与三角不等式 (iii).

**(非负性)**. 对任意 $f,g$, 逐点有 $\left|f\left(t\right)-g\left(t\right)\right|^p\ge0$, 故 $d\left(f,g\right)=\int_0^1\left|f-g\right|^p\mathrm dt\ge0$.

**(对称性 (ii))**. $\left|f\left(t\right)-g\left(t\right)\right|=\left|g\left(t\right)-f\left(t\right)\right|$ 逐点成立, 故 $d\left(f,g\right)=d\left(g,f\right)$.

**(三角不等式 (iii))**. 对任意可测函数 $h$ 与每个 $t$, 由实数三角不等式 $\left|f\left(t\right)-g\left(t\right)\right|\le\left|f\left(t\right)-h\left(t\right)\right|+\left|h\left(t\right)-g\left(t\right)\right|$. 因 $u\mapsto u^p$ 在 $\left[0,\infty\right)$ 单调递增, 上式两边取 $p$ 次方得

$$
\left|f\left(t\right)-g\left(t\right)\right|^p\le\left(\left|f\left(t\right)-h\left(t\right)\right|+\left|h\left(t\right)-g\left(t\right)\right|\right)^p.
$$

由 (1) 的次可加性, 右端 $\le\left|f\left(t\right)-h\left(t\right)\right|^p+\left|h\left(t\right)-g\left(t\right)\right|^p$ 逐点成立. 逐点积分即得 $d\left(f,g\right)\le d\left(f,h\right)+d\left(h,g\right)$. 故 (iii) 成立.

故 $d$ 是非负的且满足 (ii)(iii), 即 $d$ 是伪度量. $\blacksquare$

**(3) 商空间 $\left(L^p\left[0,1\right]/\sim,d\right)$ 是度量空间.**

依据**定义 1.1.1 (度量空间)**, 由 (2) 已知非负性, 对称性与三角不等式在商空间上仍成立, 只需验证**正定性** (构造方式同**例 1.1.12** (可测函数等价类空间)). 在商空间 $L^p\left[0,1\right]/\sim$ 上, $d\left(\left[f\right],\left[g\right]\right)=0$ 当且仅当 $\int_0^1\left|f-g\right|^p\mathrm dt=0$. 因被积函数 $\left|f-g\right|^p\ge0$ 且可测, 由积分的性质, $\int_0^1\left|f-g\right|^p\mathrm dt=0\Leftrightarrow\left|f-g\right|^p=0$ a.e. $\Leftrightarrow f=g$ a.e. $\Leftrightarrow f\sim g\Leftrightarrow\left[f\right]=\left[g\right]$. 故正定性成立, 于是 $\left(L^p\left[0,1\right]/\sim,d\right)$ 是度量空间. $\blacksquare$

## 1.1-7

在三维欧几里得空间 $\mathbb R^3$ 中, 考虑单位球面

$$
S^2=\left\{x\in\mathbb R^3:x=\left(x_1,x_2,x_3\right),x_1^2+x_2^2+x_3^2=1\right\}.
$$

对于 $x,y\in S^2$, 规定 $d\left(x,y\right)$ 为过 $x,y$ 两点的大圆上以 $x,y$ 为端点的劣弧的弧长, 它在三维欧几里得空间的正交变换下是保持不变的.

(1) 对于 $x_1^2+x_2^2=1$, 计算 $d\left(\left(1,0,0\right),\left(x_1,x_2,0\right)\right)$.

(2) 如果用 $\rho\left(x,y\right)$ 表示欧几里得距离, 证明:

$$
\rho\left(x,y\right)\le d\left(x,y\right)\le\frac{\pi}{2}\rho\left(x,y\right).
$$

(3) 证明: $d$ 是 $S^2$ 上的度量.

### 解答 1.1-7

**(1) 计算 $d\left(\left(1,0,0\right),\left(x_1,x_2,0\right)\right)$.**

设 $\theta$ 为两点在赤道大圆上的中心角, 则由球面距离定义 $d=\theta$. 因 $\left(1,0,0\right)\cdot\left(x_1,x_2,0\right)=x_1=\cos\theta$, 且 $x_1\in\left[-1,1\right]$, 故 $\theta=\arccos x_1$. 又由 $x_1^2+x_2^2=1$ 得 $x_1=\pm\sqrt{1-x_2^2}$, 且 $\theta=\arcsin x_2$ 在 $x_2\ge0$ 时成立. 故 $d\left(\left(1,0,0\right),\left(x_1,x_2,0\right)\right)=\arccos x_1=\arcsin x_2$. $\blacksquare$

**(2) 证明 $\rho\left(x,y\right)\le d\left(x,y\right)\le\frac{\pi}{2}\rho\left(x,y\right)$.**

设 $\theta=d\left(x,y\right)\in\left[0,\pi\right]$ 为 $x,y$ 的中心角, 则弦长 $\rho\left(x,y\right)=\left\|x-y\right\|=2\sin\frac{\theta}{2}$.

**左边.** 因 $\sin$ 在 $\left[0,\frac{\pi}{2}\right]$ 上凹且 $\sin0=0$, 图像在弦之下, 但更直接地由 $\sin u\le u$ ($u\ge0$) 得 $2\sin\frac{\theta}{2}\le2\cdot\frac{\theta}{2}=\theta$. 于是 $\rho\left(x,y\right)=2\sin\frac{\theta}{2}\le\theta=d\left(x,y\right)$. 左边得证.

**右边.** 令 $u=\frac{\theta}{2}\in\left[0,\frac{\pi}{2}\right]$. 因 $\sin$ 在 $\left[0,\frac{\pi}{2}\right]$ 上是凹函数, 其图像位于连接 $\left(0,0\right)$ 与 $\left(\frac{\pi}{2},1\right)$ 的弦 $y=\frac{2}{\pi}u$ 之上方, 即 $\sin u\ge\frac{2}{\pi}u$. 于是 $d\left(x,y\right)=\theta=2u\le\pi\sin u=\frac{\pi}{2}\cdot2\sin\frac{\theta}{2}=\frac{\pi}{2}\rho\left(x,y\right)$. 右边得证.

合并得 $\rho\left(x,y\right)\le d\left(x,y\right)\le\frac{\pi}{2}\rho\left(x,y\right)$. $\blacksquare$

**(3) $d$ 是 $S^2$ 上的度量.**

依据**定义 1.1.1 (度量空间)**, 逐条验证.

**(i) 非负性与正定性.** 弧长非负, 故 $d\left(x,y\right)\ge0$; 且 $d\left(x,y\right)=0\Leftrightarrow$ 两端点重合的劣弧长为 $0\Leftrightarrow x=y$. 故 (i) 成立.

**(ii) 对称性.** $x$ 到 $y$ 的劣弧与 $y$ 到 $x$ 的劣弧长度相同, 故 $d\left(x,y\right)=d\left(y,x\right)$. 故 (ii) 成立.

**(iii) 三角不等式.** 设 $\alpha=d\left(x,y\right)$, $\beta=d\left(y,z\right)$, $\gamma=d\left(x,z\right)\in\left[0,\pi\right]$.

若 $\alpha+\beta\ge\pi$, 则因 $\gamma\le\pi$, 有 $\gamma\le\pi\le\alpha+\beta$, 不等式 $d\left(x,z\right)\le d\left(x,y\right)+d\left(y,z\right)$ 成立.

若 $\alpha+\beta<\pi$: 取单位向量 $u,v\perp y$ 使得

$$
x=\cos\alpha\, y+\sin\alpha\, u,\quad z=\cos\beta\, y+\sin\beta\, v.
$$

即: 将 $x,z$ 沿 $y$ 正交分解为平行与垂直两部分, 垂直部分单位化得 $u,v$. 则由内积及 $u,v\perp y$, $\left\|u\right\|=\left\|v\right\|=1$:

$$
\cos\gamma=x\cdot z=\cos\alpha\cos\beta+\sin\alpha\sin\beta\left(u\cdot v\right)\ge\cos\alpha\cos\beta-\sin\alpha\sin\beta=\cos\left(\alpha+\beta\right),
$$

其中用了**引理 1.2.3** (柯西-施瓦茨不等式): $u\cdot v\ge-\left\|u\right\|\left\|v\right\|=-1$. 由于 $\gamma,\alpha+\beta\in\left[0,\pi\right]$ 且 $\cos$ 在 $\left[0,\pi\right]$ 上严格递减, 由 $\cos\gamma\ge\cos\left(\alpha+\beta\right)$ 得 $\gamma\le\alpha+\beta$, 即 $d\left(x,z\right)\le d\left(x,y\right)+d\left(y,z\right)$.

故三角不等式成立, 由 (i)(ii)(iii), $d$ 是 $S^2$ 上的度量. $\blacksquare$

> **证明技巧** 将 $x,z$ 沿 $y$ 正交分解: 平行于 $y$ 与垂直于 $y$ 的部分, 而 $x,z$ 各自垂直于 $y$ 的分量内积必然 $\ge-1$, 由此放缩证得三角不等式.
