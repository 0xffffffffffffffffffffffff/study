
[TOC]
# 基础公式
## 基础计算
## 三角函数
2. 和差化积公式：$\sin x+\cos x = \sqrt{2}\sin(x+{\pi\over4})$
## 不等式
1. $1+{1\over 2}+{1\over 3}+\cdots+{1\over n}\leq n$
##
# 第一章 函数与极限
## 公式
1. $y=\ln(x+\sqrt{x^2,y^2})$的反函数为$x=\frac{e^y-e^{-y}}{2}$
2. $\lim\limits_{n\rightarrow\infty}\sqrt[n]{a_1^n+a_2^n+\cdots+a_k^n}=\max\{a_1,a_2,\cdots,a_k\}$
## 定理
1. 连续函数的和、差、积、商（分母不0）是连续函数。
2. 判断函数有界性的方法：
    1. $f(x)$在$[a,b]$上连续 $\Rightarrow$ $f(x)$在$[a,b]$内有界。 
    2. $f(x)$在$(a,b)$内连续，且$\lim\limits_{x\rightarrow a^+}f(x)$和$\lim\limits_{x\rightarrow b^-}f(x)$均存在 $\Rightarrow$ $f(x)$在$(a,b)$内有界。
    3. $f^\prime(x)$在有限区间$(a,b)$内有界 $\Rightarrow$ $f(x)$在$(a,b)$内有界，反之不一定成立。
3. 若$f(x)$是可导的周期函数，则$f^\prime(x)$与$f(x)$有相同的周期。
4. $若f(x)单调递增，g(x)单调递减\Rightarrow 
   \left\{\begin{matrix}
   f[f(x)]，g[g(x)]单调递增\\
   f[g(x)]，g[f(x)]单调递减\\
   \end{matrix}\right.$
5. $若f(x)是偶函数，g(x)是奇函数\Rightarrow 
   \left\{\begin{matrix}
   f[f(x)]，f[g(x)]，g[f(x)]是偶函数\\
   g[g(x)]是奇函数\qquad\qquad\qquad\qquad\\
   \end{matrix}\right.$
6. $F(x)=\int_a^xf(t)dt\Rightarrow
   \left\{\begin{matrix}
   若f(x)可积，则F(x)连续\\
   若f(x)连续，则F(x)可导\\
   \end{matrix}\right.$
7. $\left\{\begin{matrix}
   f(x)关于直线x=a对称，则f(x+a)=f(x-a)\\
   f(x)关于点(a,0)对称，则f(x+a)=-f(x-a)\\
   \end{matrix}\right.$
8. 极限的复合运算法则：$\lim\limits_{x\rightarrow x_0}\varphi(x)=u_0$，$\lim\limits_{u\rightarrow u_0}f(x)=A$ $\Rightarrow$ $\lim\limits_{x\rightarrow x_0}f[\varphi(x)]=A$
9. 极限的保号性：若$\lim\limits_{x \rightarrow 0^+}{f(x)\over x}>0$，则$\exist \delta>0$，使得当$x\in(0,\delta)$时，$f(x)>0$
10. 极限的保序性：若$f(x)>g(x)$，且$\lim f(x)$与$\lim g(x)$均存在，则$\lim f(x) \geq \lim g(x)$
11. 若$\alpha$，$\beta$是同一变化趋势下的无穷小，$\lim {\alpha\over\beta^k}=c\neq0$，则$\alpha$是$\beta$的$k$阶无穷小
12. 海涅定理：对任何以$x_0$为极限的数列$\{x_n\}(x_n \neq x_0)$，都有$\lim\limits_{n\rightarrow\infty}f(x_n)=A$。海涅定理常用于证明$\lim\limits_{x\rightarrow\infty}\sin(x)$不存在。
13. 数列极限的保号性：若$\lim\limits_{n\rightarrow\infty}{x_n}>0$，则$\exist$正整数$N$，当$n>N$时，$x_n>0$
14. 数列极限的保序性：若$x_n>y_n$，且$\lim\limits_{n\rightarrow \infty}x_n$与$\lim\limits_{n\rightarrow \infty} y_n$均存在，则$\lim\limits_{n\rightarrow \infty}x_n \geq \lim\limits_{n\rightarrow \infty} y_n$ 
15. $任意f(x)可以表示为一个偶函数和一个奇函数的和，
    \left\{\begin{matrix}
    偶函数：f_1(x)={f(x)+f(-x)\over 2}\\
    奇函数：f_2(x)={f(x)-f(-x)\over 2}\\
    \end{matrix}\right.
    $
## 技巧
1.  证明数列单调常用方法：
    1. $x_{n+1}-x_{n}>0$
    2. ${x_{n+1}\over x_{n}}>1$
    3. 常用不等式
    4. 拉格朗日中值定理
2.  $\left\{\begin{matrix}z_n\leq A\leq y_n\\ \lim\limits_{n\rightarrow \infty}(y_n-z_n)=0\end{matrix}\right. \Rightarrow \lim\limits_{n\rightarrow\infty}y_n = \lim\limits_{n\rightarrow\infty}z_n = A$
## 易错点
1. $当x\rightarrow0 时，{1\over x^2}\sin{1\over x}无界但非无穷大，是x=0震荡点。$
2. 极限的四则运算是充分非必要条件：$\lim\limits_{x\rightarrow 0}a(x)=\infty,\lim\limits_{x\rightarrow 0}b(x)=\infty$ $\nRightarrow$ $\lim\limits_{x\rightarrow 0}a(x)+b(x)=\infty$
3. $f(a)=A \nRightarrow \lim\limits_{x\rightarrow a}f(x)=A，x=a有可能是第一类间断点。$
4.  洛必达法则的使用条件：
    1.  $0\over 0$型或$\infty\over\infty$型
    2.  $f(x)和g(x)都可导，且g^\prime(x)\neq 0$
    3.  $\lim{f^\prime(x)\over g^\prime(x)}=A或\infty，不能震荡。判断求导后震荡的常用反例为\sin({1\over x})或\cos({1\over x})。$



# 导数与微分
## 公式
1. $(\sin x)^{(n)}=\sin(x+n\cdot{\pi\over 2})$，$(\cos x)^{(n)}=\cos(x+n\cdot{\pi\over 2})$
2. $y_{xx}^{\prime\prime}=-{x_{yy}^{\prime\prime}\over({x_y^\prime})^3}$，$x_{yy}^{\prime\prime}=-{y_{xx}^{\prime\prime}\over({y_x^\prime})^3}$,
3. $\left\{\begin{matrix}x=x(t) \\ y=y(t)\end{matrix}\right.$，则${d^2y\over dx^2}={{y^\prime\prime(t)\cdot x^\prime(t)-y^\prime(t)x^\prime\prime(t)}\over [x^\prime(t)]^3}$
## 定理
1. 若$f(x)在x_0处可导,则f(x)在x_0处连续$。
2. $f^\prime(x)>0 \Rightarrow f(x)单调递增，反之不一定成立$
2. $f^\prime(0)>0 \nRightarrow f(x)在x_0的邻域内单调递增$。
3. $f(x)在x_0处可导，g(x)在x_0处不可导，则F(x)=f(x)\cdot g(x)在x_0处可导的充要条件是f(x_0)=0$。
4. 设$f(x)$在$x_0$处可导：
    1. $f(x_0)\neq 0 \Rightarrow y=|f(x)|在x_0处可导$
    2. $f(x_0)=0，f^\prime(x_0)\neq 0 \Rightarrow y=|f(x)|在x_0处不可导$
    3. $f(x_0)=0，f^\prime(x_0)=0 \Rightarrow y=|f(x)|在x_0处可导，且导数为0$
5. 设$f(x)=(x-x_0)^k|x-x_0|，则f(x)在x_0处k阶可导，k+1阶不可导$。
6. $f(x)，g(x)互为反函数，则f^\prime(x)\cdot g^\prime(y)=1$
7. $\sqrt[3]x在x=0处不可导$
8. $a^3-b^3=(a-b)(a^2+ab+b^2)，a^3+b^3=(a+b)(a^2+ab+b^2)$
9. 求$f^{(n)}(x)$的常用方法：
    1. 找规律
    2. 利用莱布尼茨公式：$(uv)^{(n)}=\sum\limits_{i=0}^{n}C_n^ku^{(n-k)}v^{(k)}$
    3. 求某一点处的高阶导数也可以用泰勒公式
10. $f(x)在x_0处，\lim\limits_{x\rightarrow x_0}{f(x)-f(x_0)\over x-x_0}=\lim\limits_{x\rightarrow x_0}f^\prime(x)$，则$f(x)在x_0处导数连续$。
# 导数的应用
## 公式
1. 斜渐近线：$y=kx+b，k=\lim\limits_{x\rightarrow\infty}{f(x)\over x}，b=\lim\limits_{x\rightarrow\infty}[f(x)-kx]$
2. $曲率：K={|y^{\prime\prime}|\over[1+(y^\prime)^2]^{3\over 2}}，曲率半径R={1\over K}$
## 结论
1. 极值点不能在区间的端点取得。
1. 驻点不一定是极值点，极值点也不一定是驻点。
1. $f^{\prime\prime}(x)在x=x_0两侧异号，则(x_0,f(x_0))是拐点。$
1. 极值点是$x=x_0$，拐点是$(x_0,f(x_0))$
1. $设f(x)在x_0处有n阶导数，且f^{(k)}(x_0)=0(k<n),f^{(n)}(x_0)\neq 0$
    $\left\{\begin{matrix}
    n为偶数\left\{\begin{matrix}
            f^{(n)}(x_0)<0 \Rightarrow x=x_0是极大值点\\
            f^{(n)}(x_0)>0 \Rightarrow x=x_0是极小值点\\
            \end{matrix}\right.\\
    n为奇数\left\{\begin{matrix}
            f^{(n)}(x_0)<0 \Rightarrow (x_0,f(x_0))是拐点\\
            f^{(n)}(x_0)>0 \Rightarrow (x_0,f(x_0))是拐点\\
            \end{matrix}\right.\\
    \end{matrix}\right.$
1. $闭区间上的最值\in \{驻点、不可导点、端点\}$
1. $开区间上的最值\in \{驻点、不可导点\}$，如果端点的极限为最值，则最值不存在。
1. 当找不到函数值为0的点时，不妨取无穷大。
1. 讨论含参方程$f(x,k)=0$的实根个数：
    1. $求f(x,k)的极值$
    2. $讨论每个极值与x轴的位置关系$




# 中值定理
1. 零点定理：若$f(a)\cdot f(b)<0 \Rightarrow \exist \xi\in (a,b)$，使得$f(\xi)=0$
    1. 可以用极限的保号性证明
    1. 可以用单调性证明
2. 介值定理1：若$f(a)<C<f(b)$，则$\exist\xi\in(a,b)，使得f(\xi)=C$
3. 介值定理2：$若Min \leq C \leq Max$，则$\exist\xi\in[a,b]，使得f(\xi)=C$
4. 罗尔定理：$f(x)$满足
   $\left\{\begin{matrix}
   在[a,b]上连续\\ 
   在(a,b)上可导\\
   f(a)=f(b)\\
   \end{matrix}\right. 
   \Rightarrow 则至少存在一点\xi\in(a,b),使得f^\prime(\xi)=0。
   $
5. 罗尔定理的有关应用:
   1. 证明$f^{\prime\prime}(x)至少有一个零点$：
   $\left\{\begin{matrix}
   f^\prime(x)至少有两个零点\\
   f(x)至少有三个零点\\
   \int_a^xf(t)dt至少四个零点\\
   \end{matrix}\right.$
   2. $若在(a,b)上f^{(n)}(x)\neq 0恒成立，则f(x)在(a,b)上至多有n个零点。$
   3. 构造函数证明等式。
6. 常用罗尔定理的构造函数：
   1. $u^\prime v+uv^\prime=0，构造uv$
   2. $u^\prime v-uv^\prime=0，构造{u\over v}$
   3. $\lambda f(x)+xf^\prime(x)=0，构造x^\lambda f(x)$
   4. $\lambda f(x)+f^\prime(x)=0，构造e^{\lambda x}f(x)$
   5. $当等式中仅存在f(x)和f^{\prime\prime}(x)时，要加减f^\prime(x)$
7. 拉格朗日中值定理：$f(x)$满足：
    $\left\{\begin{matrix}
    在[a,b]上连续\\
    在(a,b)内可导\\
    \end{matrix}\right.$
    $\Rightarrow$
    $\left\{\begin{matrix}
    f(b)-f(a)=f^\prime(\xi)(b-a),a<\xi<b\\
    f(b)-f(a)=f^\prime[a+\theta(b-a)](b-a),0<\theta<1\\
    \end{matrix}\right.$
8. 柯西中值定理：$f(x)，g(x)$满足：
    $\left\{\begin{matrix}
    在[a,b]上连续\\
    在(a,b)内可导\\
    g^\prime(x)\neq 0\\
    \end{matrix}\right.$
    $\Rightarrow$
    ${f(b)-f(a)\over g(b)-g(b)}={f^\prime(\xi)\over g^\prime(\xi)},a<\xi<b\\$
9. 证明含有两个中值的等式一般有三种情况：
   1. 不同函数在同一区间上
   2. 同一函数在不同区间上
   3. 综合运用柯西中值定理和拉格朗日中值定理或泰勒公式
10. 积分中值定理：$f(x)在[a,b]上连续，则\exist\xi\in[a,b]，\int_a^bf(x)dx=f(\xi)(b-a)。$
11. 推广的积分中值定理：$f(x)和g(x)都在[a,b]上连续，且g(x)不变号，则\exist\xi\in[a,b]，\int_a^bf(x)g(x)d(x)=f(\xi)\int_a^bg(x)dx。$

# 泰勒公式
## 麦克劳林公式
1. $e^x=1+x+{1\over 2}x^2+{1\over 6}x^3+o(x^3)=\sum\limits_{i=0}^\infty {x^i\over i!}$
2. $\sin x=x-{1\over 6}x^3+{1\over 120}x^5+o(x^5)=\sum\limits_{i=0}^\infty{(-1)}^i{x^{2i+1}\over (2i+1)!}$
3. $\cos x=1-{1\over 2}x^2+{1\over 24}x^4+o(x^4)=\sum\limits_{i=0}^\infty(-1)^n{x^{2i}\over (2i)!}$
4. $\tan x=x+{1\over 3}x^3+o(x^3)$
5. $\arcsin x=x+{1\over 6}x^3+o(x^3)$
6. $\arctan x=x-{1\over 3}x^3+{1\over 5}x^5+o(x^5)=4$
7. $\ln{(1+x)}=x-{1\over 2}x^2+{1\over 3}x^3+o(x^3)$
8. $-\ln{(1-x)}=x+{1\over 2}x^2+{1\over 3}x^3+o(x^3)$
9. ${1\over 1+x}=1-x+x^2-x^3+o(x^3)$
10. ${1\over 1-x}=1+x+x^2+x^3+o(x^3)$
11. ${(1+x)^\alpha}=1+\alpha x+{\alpha(\alpha-1)\over2}x^2+o(x^2)$
## 结论 
1. $f(x)在x=a处带拉格朗日余项的一阶泰勒公式：f(x)=f(a)+f^\prime(a)(x-a)+{f^{\prime\prime}(\xi)\over 2}(x-a)^2，\xi在x和a之间$
2. $f(x)带拉格朗日余项的二阶麦克劳林公式：f(x)=f(0)+f^\prime(0)x+{f^{\prime\prime}(0)\over 2}x^2+{f^{\prime\prime\prime}(\xi)\over 6}x^3，\xi在x和a之间$