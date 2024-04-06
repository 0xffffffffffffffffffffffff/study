
[TOC]
# 基础公式
## 基础计算
1. $[x+n]=[x]+n$
1. $x-1<[x]\leq x$
1. $1^2+2^2+3^2+\cdots+n^2={n(n+1)(2n+1)\over 6}$
9.  $a^3-b^3=(a-b)(a^2+ab+b^2)$
10. $a^3+b^3=(a+b)(a^2+ab+b^2)$
## 三角函数
1. $1+\tan^2x=\sec^2x$
2. $1+\cot^2x=\csc^2x$
3. $\sin(\arcsin x)=x，x\in[-1,1]$
4. $\sin(\arccos x)=\sqrt{1-x^2}，x\in[-1,1]$
5. $\cos(\arccos x)=x，x\in[-1,1]$
6. $\cos(\arcsin x)=\sqrt{1-x^2}，x\in[-1,1]$
7. $\arcsin(\sin x)=x，x\in[-{2\over \pi},{2\over \pi}]$
8. $\arccos(\cos x)=x，x\in[-{2\over \pi},{2\over \pi}]$
9.  和差化积公式：$\sin x+\cos x = \sqrt{2}\sin(x+{\pi\over4})$
## 不等式
1. $| |a|-|b| | \leq |a-b|$
2. $1+{1\over 2}+{1\over 3}+\cdots+{1\over n}\leq n$
##
# 第一章 函数与极限
## 公式
1. $y=\ln(x+\sqrt{x^2+1})\Leftrightarrow x=\frac{e^y-e^{-y}}{2}$
2. $y=\ln(x+\sqrt{x^2-1})\Leftrightarrow x=\frac{e^y+e^{-y}}{2}$
3. $\lim\limits_{n\rightarrow\infty}\sqrt[n]{a_1^n+a_2^n+\cdots+a_k^n}=\max\{a_1,a_2,\cdots,a_k\}$
4. $x-\sin x = {1\over 6}x^3$
5. $\arcsin x - x = {1\over6}x^3$
6. $\tan x - x = {1\over 3}x^3$
7. $\tan x-\sin x = {1\over 2}x^3$
8. $x-\arctan x = {1\over 3}x^3$
9. $x\rightarrow 0 时，\ln{(x+\sqrt{x^2+1})}\sim x$
10. 若$\lim u^v为1^\infty型，则\lim u^v=e^{\lim (u-1)v}$
11. 常见奇函数:
    $\\
    y=\ln(x+\sqrt{x^2+1})\\
    y=e^x-e^{-x}\\$
## 定理
1. 连续函数的和、差、积、商（分母不0）是连续函数。
2. 严格单调函数必有反函数
3. $y=f(x)与x=f^{-1}(y)的图像完全重合。$
4. 单调的定义
    $\begin{cases}
    f(x)单调递增 \Leftrightarrow (x_1-x_2)[f(x_1)-f(x_2)]>0\\
    f(x)单调递减 \Leftrightarrow (x_1-x_2)[f(x_1)-f(x_2)]<0\\
    f(x)单调不减 \Leftrightarrow (x_1-x_2)[f(x_1)-f(x_2)]\geq 0\\
    f(x)单调不增 \Leftrightarrow (x_1-x_2)[f(x_1)-f(x_2)]\leq 0\\
    \end{cases}$
5. $F(x)=\int_a^xf(t)dt\Rightarrow
   \begin{cases}
   若f(x)可积，则F(x)连续\\
   若f(x)连续，则F(x)可导\\
   \end{cases}$
6. $\begin{cases}
   f(x)关于直线x=a对称，则f(x+a)=f(x-a)\\
   f(x)关于点(a,0)对称，则f(x+a)=-f(x-a)\\
   \end{cases}$
7. 函数极限的局部保号性：$\begin{cases}
    如果\lim\limits_{x\rightarrow x_0}f(x)>0，则在x_0的邻域内有f(\delta)>0\\
    如果在x_0的去心邻域内f(x)>0，则\lim\limits_{x\rightarrow x_0}f(x)>0\\
    \end{cases}$
8.  极限的复合运算法则：$\lim\limits_{x\rightarrow x_0}\varphi(x)=u_0$，$\lim\limits_{u\rightarrow u_0}f(x)=A$ $\Rightarrow$ $\lim\limits_{x\rightarrow x_0}f[\varphi(x)]=A$
9.  $若\lim f(x)存在，且n为正整数，则\lim[f(x)]^n=[\lim f(x)]^n$
10. 极限的保号性：若$\lim\limits_{x \rightarrow 0^+}{f(x)\over x}>0$，则$\exist \delta>0$，使得当$x\in(0,\delta)$时，$f(x)>0$
11. 极限的保序性：若$f(x)>g(x)$，且$\lim f(x)$与$\lim g(x)均存在，则\lim f(x) \geq \lim g(x)$
12. 若$\alpha，\beta是同一变化趋势下的无穷小，\lim {\alpha\over\beta^k}=c\neq 0，则\alpha是\beta的k阶无穷小$
13. 海涅定理：对任何以$x_0$为极限的数列$\{x_n\}(x_n \neq x_0)$，都有$\lim\limits_{n\rightarrow\infty}f(x_n)=A$。海涅定理常用于证明$\lim\limits_{x\rightarrow\infty}\sin(x)$不存在。
14. 数列极限的保号性：若$\lim\limits_{n\rightarrow\infty}{x_n}>0$，则$\exist$正整数$N$，当$n>N$时，$x_n>0$
15. 数列极限的保序性：若$x_n>y_n$，且$\lim\limits_{n\rightarrow \infty}x_n$与$\lim\limits_{n\rightarrow \infty} y_n$均存在，则$\lim\limits_{n\rightarrow \infty}x_n \geq \lim\limits_{n\rightarrow \infty} y_n$ 
16. $\lim\limits_{n\rightarrow \infty}a_n=a \Leftrightarrow \lim\limits_{k\rightarrow \infty}a_{2k}=\lim\limits_{k\rightarrow \infty}a_{2k-1}=a$
17. $\lim\limits_{n\rightarrow \infty}a_n=A \Rightarrow \lim\limits_{n\rightarrow \infty}|a_n|=|A|$
18. $\lim\limits_{n\rightarrow \infty}|a_n|=0 \Rightarrow \lim\limits_{n\rightarrow \infty}a_n=0$
19. $任意f(x)可以表示为一个偶函数和一个奇函数的和，
    \begin{cases}
    偶函数：f_1(x)={f(x)+f(-x)\over 2}\\
    奇函数：f_2(x)={f(x)-f(-x)\over 2}\\
    \end{cases}$
## 重要结论
1. 并不是任意两个无穷小都可以进行比较的，比值可能不存在。
2. 复合函数的单调性(同增异减)$
   \begin{cases}
   增[增]\Rightarrow 增\\
   减[减]\Rightarrow 增\\
   增[减]\Rightarrow 减\\
   减[增]\Rightarrow 减\\
   \end{cases}$
3. 复合函数的奇偶性$
    (内偶则偶，内奇同外)
    \begin{cases}
    奇[偶]\Rightarrow 偶\\
    偶[偶]\Rightarrow 偶\\
    奇[奇]\Rightarrow 奇\\
    偶[奇]\Rightarrow 偶\\
    \end{cases}$
4. $f(x+y)=f(x)+f(y)\Rightarrow f(x)是奇函数$
5. 若$f(x)$是可导的周期函数，则$f^\prime(x)$与$f(x)$有相同的周期。
6. $若f(x)以T为周期，则f(ax+b)以{T\over |a|}为周期$
7. $若g(x)是周期函数，则f[g(x)]也是周期函数$
8. $若f(x)可导且以T为周期，则f^\prime(x)也以T为周期$
9.  $\left\{\begin{matrix}
    f(x)连续\\
    f(x)以T为周期\\
    \int_0^Tf(t)dt=0\\
    \end{matrix}\right\}
    \Rightarrow \int_0^xf(t)dt以T为周期$
## 技巧
1.  证明数列单调常用方法：
   $\begin{cases}
   x_{n+1}-x_{n}>0\\
   {x_{n+1}\over x_{n}}>1\\
   数学归纳法\\
   常用不等式\\
   拉格朗日中值定理\\
   结论：x_{n+1}=f(x_n)
   \begin{cases}
   若f^\prime(x)>0，\{x_n\}单调\\
   若f^\prime(x)<0，\{x_n\}不单调\\
   \end{cases}
   \end{cases}$
2.  $\left\{\begin{matrix}z_n\leq A\leq y_n\\ \lim\limits_{n\rightarrow \infty}(y_n-z_n)=0\end{matrix}\right\} \Rightarrow \lim\limits_{n\rightarrow\infty}y_n = \lim\limits_{n\rightarrow\infty}
z_n = A$
1. $证明f(x)有界，一般证|f(x)|\leq M$
2. 研究最值的方法：$
    \begin{cases}
    见到\sqrt{u}、\sqrt[3]{u}，可用u来研究最值\\
    见到|u|，|u|=\sqrt{u^2}，可用u^2来研究最值\\
    见到{1\over u}，可用u来研究最值\\
    \end{cases}$
3. 判断函数有界性的方法：$\begin{cases}
   f(x)在[a,b]上连续 \Rightarrow f(x)在[a,b]内有界 \\
   f(x)在(a,b)内连续，且\lim\limits_{x\rightarrow a^+}f(x)和\lim\limits_{x\rightarrow b^-}f(x)均存在 \Rightarrow f(x)在(a,b)内有界\\
   f^\prime(x)在有限区间(a,b)内有界 \Rightarrow f(x)在(a,b)内有界，反之不一定成立\\
   \end{cases}$
4. 放缩常用方法
   $\begin{cases}
   n \cdot u_{min} \leq u_1+u_2+\cdots+u_n \leq n \cdot u_{max}\\
   u_i\geq 0时，u_{max} \leq u_1+u_2+\cdots+u_n \leq n \cdot u_{max}\\
   ||a|-|b||\leq |a-b|\\
   |a_1 \pm a_2 \pm \cdots \pm a_n| \leq |a_1|+|a_2|+\cdots+|a_n|\\
   |ab|\leq {a^2+b^2\over 2}\\
   \sqrt{ab} \leq {a+b\over 2} \leq \sqrt{a^2+b^2\over 2}，(a\geq 0，b\geq 0)\\
   \sqrt[3]{abc} \leq {a+b+c\over 2} \leq \sqrt{a^2+b^2+c^2\over 2}，(a\geq 0，b\geq 0，c\geq 0)\\
   1+{1\over 2}+{1\over 3}+\cdots+{1\over n}\leq n\\
   若0<a<x<b，0<c<f(x)<d，则{c\over b}<{f(x)\over x}<{d\over a}\\
   \sin x < x，(x>0)\\
   \sin x <x <\tan x，(0<x<{\pi\over 2})\\
   \sin x >{2\over \pi}x，(0<x<{\pi\over 2})\\
   x<\tan x<{4\over \pi}x，(0<x<{\pi\over 4})\\
   \arctan x\leq x\leq\arcsin x，(0\leq x \leq 1)\\
   e^x \geq x+1\\
   x-1 \geq \ln x，(x>0)\\
   {1\over 1+x}< \ln{(1+{1\over x})} < {1\over x}，(x>0)\\
   {x\over 1+x}< \ln(1+x) < x，(x>0)\\
   连续函数在闭区间上必有最大最小值\\
   若|x_{n+1}-a|\leq k|x_n-a|，(0<k<1)，则\lim\limits_{n\rightarrow \infty}x_n=a\\
   若x_{n+1}=f(x)，f(x)可导，a是f(x)=x的唯一解，且|f^\prime(x)|\leq k<1，则\lim\limits_{n\rightarrow \infty}x_n=a\\
   \end{cases}$

## 易错点
1. $当x\rightarrow0 时，{1\over x^2}\sin{1\over x}无界但非无穷大，是x=0震荡点。$
2. 极限的四则运算是充分非必要条件：$\lim\limits_{x\rightarrow 0}a(x)=\infty,\lim\limits_{x\rightarrow 0}b(x)=\infty$ $\nRightarrow$ $\lim\limits_{x\rightarrow 0}a(x)+b(x)=\infty$
3. $f(a)=A \nRightarrow \lim\limits_{x\rightarrow a}f(x)=A，x=a有可能是第一类间断点。$
4.  洛必达法则的使用条件：
   $\begin{cases}
   {0\over 0}型或{\infty\over\infty}型\\
   f(x)和g(x)都可导，且g^\prime(x)\neq 0\\
   \lim{f^\prime(x)\over g^\prime(x)}=A或\infty，不能震荡。判断求导后震荡的常用反例为\sin({1\over x})或\cos({1\over x})。\\
   \end{cases}$



# 导数与微分
## 公式
1. $(\tan x)^\prime=\sec^2 x$
2. $(\cot x)^\prime=-\csc^2 x$
3. $(\sec x)^\prime=\sec x \tan x$
4. $(\csc x)^\prime=-\csc x \cot x$
5. $(\arcsin x)^\prime={1\over {\sqrt{1-x^2}}}={1\over (\sin y)^\prime}$
6. $(\arccos x)^\prime=-{1\over {\sqrt{1-x^2}}}$
7. $[\ln{(x+\sqrt{x^2+1})}]^\prime = {1\over \sqrt{x^2+1}}$
8. $[\ln{(x+\sqrt{x^2-1})}]^\prime = {1\over \sqrt{x^2-1}}$
9.  $y_{xx}^{\prime\prime}=-{x_{yy}^{\prime\prime}\over({x_y^\prime})^3}$，$x_{yy}^{\prime\prime}=-{y_{xx}^{\prime\prime}\over({y_x^\prime})^3}$,
10. $\begin{cases}
   x=x(t) \\ y=y(t)
   \end{cases}$，则${d^2y\over dx^2}={d({dy\over dx})\over dt}\cdot{dt\over dx}={{y^{\prime\prime}(t)\cdot x^\prime(t)-y^\prime(t)x^{\prime\prime}(t)}\over [x^\prime(t)]^3}$（套公式往往计算量巨大）
11. ${(e^{ax+b})}^{(n)}=a^ne^{ax+b}$
12. $({1\over ax+b})^{(n)}=(-1)^n{a^n\cdot n! \over (ax+b)^{n+1}}$
13. $(\sin ax+b)^{(n)}=a^n\sin(ax+b+n\cdot{\pi\over 2})$
14. $(\cos ax+b)^{(n)}=a^n\cos(ax+b+n\cdot{\pi\over 2})$
## 定理
1. 若$f(x)在x_0处可导,则f(x)在x_0处连续$。
2. $f(x)，g(x)互为反函数，则f^\prime(x)\cdot g^\prime(y)=1$
4.  $f(x)在x_0处可微\Leftrightarrow f(x)在x_0处可导$
3.  $f(x)在x_0处，\lim\limits_{x\rightarrow x_0}{f(x)-f(x_0)\over x-x_0}=\lim\limits_{x\rightarrow x_0}f^\prime(x)$，则$f(x)在x_0处导数连续$。
6. $f(x)在x_0处n阶可导，则0~n-1阶导数连续$
## 重要结论
1. $f(x)在x_0处可导，g(x)在x_0处不可导，则F(x)=f(x)\cdot g(x)在x_0处可导的充要条件是f(x_0)=0$。
2. 设$f(x)在x_0处可导$：
   $\begin{cases}
   f(x_0)\neq 0 \Rightarrow y=|f(x)|在x_0处可导\\
   f(x_0)=0，f^\prime(x_0)\neq 0 \Rightarrow y=|f(x)|在x_0处不可导\\
   f(x_0)=0，f^\prime(x_0)=0 \Rightarrow y=|f(x)|在x_0处可导，且导数为0\\
   \end{cases}$
3. 设$f(x)=(x-x_0)^k|x-x_0|，则f(x)在x_0处k阶可导，k+1阶不可导$。
## 技巧
1. 三步判别一元函数可微：
   $\begin{cases}
   ①，增量\Delta y=f(x_0+\Delta x)-f(x_0)\\
   ②，线性增量A\Delta x = f^\prime(x_0)\Delta x\\
   ③，若\lim\limits_{\Delta x \rightarrow 0}{\Delta y-A\Delta x \over \Delta x}=0，则f(x)在x_0处可微，否则不可微\\
   \end{cases}$
2.  求高阶导数的常用方法：
    $\begin{cases}
    找规律\\
    利用莱布尼茨公式：(uv)^{(n)}=\sum\limits_{i=0}^{n}C_n^ku^{(n-k)}v^{(k)}\\
    求某一点处的高阶导数也可以用泰勒公式\\
    \end{cases}$
## 易错点
1. $\sqrt[3]x在x=0处不可导$
2. $f^\prime(x)>0 \Rightarrow f(x)单调递增，反之不一定成立$?为什么!
3.  $f^\prime(0)>0 \nRightarrow f(x)在x_0的邻域内单调递增，有可能震荡$。

# 导数的应用
## 公式
1. 斜渐近线：$y=kx+b，k=\lim\limits_{x\rightarrow\infty}{f(x)\over x}，b=\lim\limits_{x\rightarrow\infty}[f(x)-kx]$
2. $曲率：K={|y^{\prime\prime}|\over[1+(y^\prime)^2]^{3\over 2}}，曲率半径R={1\over K}$
## 定理
1. 极值点不能在区间的端点取得。
2. 驻点不一定是极值点，极值点也不一定是驻点。
3. 极小值点的定义：$在x_0的某邻域内，f(x_0)\leq f(x)$
4. $开区间内的最值点一定是极值点$
5. $若f(x)在[a,b]上连续，(a,b)内可导，f^\prime(x)\geq 0，且等号仅在有限个点处成立，则f(x)在[a,b]上严格单调增加$
6. $f^{\prime\prime}(x)在x=x_0两侧异号，则(x_0,f(x_0))是拐点。$
## 重要结论
1. $f(x)在x_0处的切线为：y=f(x_0)+f^\prime(x_0)(x-x_0)$
2. $函数图形为凹时，f(\lambda_1x_1+\lambda_2x_2)<\lambda_1f(x_1)+\lambda_2f(x_2)，其中0<\lambda_1<1，0<\lambda_2<1，\lambda_1+\lambda_2=1$
3. $若\alpha 是多项式f(x)=0的m重根，则\alpha是f^\prime(x)=0的m-1重根$
4. 曲线的可导点不可同时为极值点和拐点，曲线的不可导点可以同时为极值点和拐点。
5. $设多项式函数f(x)=(x-a)^ng(x)，(n>1)且g(a)\neq 0，则
   \begin{cases}
   n为偶数\Rightarrow x=a是f(x)的极值点\\
   n为奇数\Rightarrow (a,0)是f(x)的拐点\\
   \end{cases}$
6. $设多项式函数f(x)=(x-a_1)^{n_1}(x-a_2)^{n_2}\cdots(x-a_k)^{n_k}，其中n_i为正整数，a_i两两不相等，\\
   记\left\{\begin{matrix}
   k_1为n_i=1的个数\\
   k_2为n_i>1且n_i为偶数的个数\\
   k_3为n_i>1且n_i为奇数的个数\\
   \end{matrix}\right\}，则
   \begin{cases}
   f(x)的极值点个数：k_1+2k_2+k_3-1\\
   f(x)的拐点个数：k_1+2k_2+3k_3-2\\
   \end{cases}$
## 技巧
1. $设f(x)在x_0处有n阶导数，且f^{(k)}(x_0)=0(k<n),f^{(n)}(x_0)\neq 0$
    $\begin{cases}
    n为偶数\begin{cases}
            f^{(n)}(x_0)<0 \Rightarrow x=x_0是极大值点\\
            f^{(n)}(x_0)>0 \Rightarrow x=x_0是极小值点\\
            \end{cases}\\
    n为奇数 \Rightarrow (x_0,f(x_0))是拐点\\
    \end{cases}$
2. $极值点\in \{驻点、不可导点\}$
3. $闭区间上的最值\in \{驻点、不可导点、端点\}$
4. $开区间上的最值\in \{驻点、不可导点\}$，如果端点的极限为最值，则最值不存在。
5. 当找不到函数值为0的点时，不妨取无穷大。
6. 作函数f(x)的图像一般步骤：
   $\begin{cases}
   ①确定定义域，考察奇偶性、周期性\\
   ②一阶导确定单调区间、极值点\\
   ③二阶导确定凹凸区间、拐点\\
   ④考察渐近线\\
   ⑤作表格\\
   ⑥做出函数图像\\
   \end{cases}$
7. 讨论含参方程$f(x,k)=0$的实根个数：
   $\begin{cases}
   ①求f(x,k)的极值\\
   ②讨论每个极值与x轴的位置关系\\
   \end{cases}$
## 易错点
1. 无穷间断点也可以是极值点或拐点，主要看定义。
2. 极值点是$x=x_0$，驻点是？，拐点是$(x_0,f(x_0))$
3. 拐点必须是连续的点



# 中值定理与泰勒公式
## 公式
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
## 定理
1. 零点定理：若$f(a)\cdot f(b)<0 \Rightarrow \exist \xi\in (a,b)$，使得$f(\xi)=0$
    1. 可以用极限的保号性证明
    1. 可以用单调性证明
2. 介值定理：$f(x)在[a,b]上连续$
   $\begin{cases}
   若f(a)<C<f(b)，则\exist\xi\in(a,b)，使得f(\xi)=C\\
   若Min \leq C \leq Max，则\exist\xi\in[a,b]，使得f(\xi)=C\\
   \end{cases}$
3. 平均值定理（离散）：$当a<x_1<x_2<\cdots<x_n<b时，\exist \xi\in[x_1,x_n]，使得f(\xi)={f(x_1)+f(x_2)+\cdots+f(x_n)\over n}$
4. 平均值定理（连续）：$f(x)在[a,b]内连续，则\exist\xi\in[a,b]，使得f(\xi)={1\over b-a}\int_a^bf(x)dx$
5. 费马定理：$如果f(x)在极值点x=x_0处可导，则f^\prime(x_0)=0$
6. 罗尔定理：$f(x)$满足
   $\left\{\begin{matrix}
   在[a,b]上连续\\ 
   在(a,b)上可导\\
   f(a)=f(b)\\
   \end{matrix}\right\} 
   \Rightarrow 则至少存在一点\xi\in(a,b),使得f^\prime(\xi)=0。$
7. 拉格朗日中值定理：$f(x)$满足：
    $\left\{\begin{matrix}
    在[a,b]上连续\\
    在(a,b)内可导\\
    \end{matrix}\right\}$
    $\Rightarrow$
    $\begin{cases}
    f(b)-f(a)=f^\prime(\xi)(b-a),a<\xi<b\\
    f(b)-f(a)=f^\prime[a+\theta(b-a)](b-a),0<\theta<1\\
    \end{cases}$
8.  柯西中值定理：$f(x)，g(x)$满足：
    $\left\{\begin{matrix}
    在[a,b]上连续\\
    在(a,b)内可导\\
    g^\prime(x)\neq 0\\
    \end{matrix}\right\}$
    $\Rightarrow$
    ${f(b)-f(a)\over g(b)-g(b)}={f^\prime(\xi)\over g^\prime(\xi)},a<\xi<b\\$
9.  积分中值定理：$f(x)在[a,b]上连续，则\exist\xi\in[a,b]，\int_a^bf(x)dx=f(\xi)(b-a)。$
10. 推广的积分中值定理：$f(x)和g(x)都在[a,b]上连续，且g(x)不变号，则\exist\xi\in[a,b]，\int_a^bf(x)g(x)dx=f(\xi)\int_a^bg(x)dx。$
11. $f(x)在x=a处带拉格朗日余项的一阶泰勒公式：f(x)=f(a)+f^\prime(a)(x-a)+{f^{\prime\prime}(\xi)\over 2}(x-a)^2，\xi在x和a之间$
12. $f(x)在x=a处带佩亚诺余项的一阶泰勒公式：f(x)=f(a)+f^\prime(a)(x-a)+o((x-a))$
13. $f(x)带拉格朗日余项的二阶麦克劳林公式：f(x)=f(0)+f^\prime(0)x+{f^{\prime\prime}(0)\over 2}x^2+{f^{\prime\prime\prime}(\xi)\over 6}x^3，\xi在x和a之间$
## 重要结论
1. 罗尔定理的有关应用:
   $\begin{cases}
   证明f^{\prime\prime}(x)至少有一个零点：
   \begin{cases}
   f^\prime(x)至少有两个零点\\
   f(x)至少有三个零点\\
   \int_a^xf(t)dt至少四个零点\\
   \end{cases}\\
   若在(a,b)上f^{(n)}(x)\neq 0恒成立，则f(x)在(a,b)上至多有n个零点。\\
   构造函数证明等式
   \begin{cases}
   见到f(x)f^\prime(x)，令F(x)=f^2(x)\\
   见到[f^\prime(x)]^2+f(x)f^{\prime\prime}(x)，令F(x)=f(x)f^\prime(x)\\
   见到f^\prime(x)+\varphi^\prime(x)f(x)，令F(x)=f(x)e^{\varphi(x)}\\
   见到f^\prime(x)x-f(x)，x\neq 0，令F(x)={f(x)\over x}\\
   见到f^{\prime\prime}(x)f(x)-[f^\prime(x)]^2，令F(x)={f^\prime(x)\over f(x)}或F(x)=\ln f(x)
   \end{cases} \\
   \end{cases}$
2. 罗尔原话：$若f^{(n)}(x)=0至多有k个根，则f(x)=0至多有k+n个根$
3. 奇次多项式至少有一个实根。
4. 连续函数在区间内有唯一极值点，该极值点也是最值点。

## 技巧
1. 证明零点存在且唯一：
   $\begin{cases}
   ①零点定理证存在\\
   ②单调性证唯一，或用罗尔定理的推论\\
   \end{cases}$
2. 证明含有两个中值的等式一般有三种情况：
   $\begin{cases}
   不同函数在同一区间上\\
   同一函数在不同区间上\\
   综合运用柯西中值定理和拉格朗日中值定理或泰勒公式\\
   \end{cases}$
3. 中值定理证明题的等式里如果有$a+b，可令a+b={b^2-a^2\over b-a}。$
## 易错点
1. $拉格朗日余项{f^{(n+1)}(\xi)\over (n+1)!}x^{n+1}，其中\xi与x相关，\xi=\xi(x)$



---
1. $\int_0^{2x_0}(x-x_0)dx=0$
