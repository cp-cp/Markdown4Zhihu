## 方程求根

### 二分法

条件：连续且异号

收敛速率：$$O(\frac{1}{2^n})$$

误差：$$|p_n-p|\leq\frac{|b_n-a_n|}{2}$$

### 不动点法

不动点定理：$$存在|k|<1,使得所有|g\prime(x)|\leq k$$

这里的函数$$g$$是变化后的。

误差：$$|p_n-p|\leq k^n |p_0-p|$$

### 牛顿法

理解：

​	几何上，为切线形式；代数上，为梯度形式。
$$
x_n=x_{n-1}-\frac{f(x_{n-1})}{f'(x_{n-1})}
$$
近似方法：

​	为了避免求导带来的额外运算，采用**割线**。
$$
x_{k+1}=x_k-f(x_k)\frac{x_k-x_{k-1}}{f(x_k)-f(x_{k-1})}
$$
错位方法：

​	加入二分法的判断。

重根情况：

​	求$$f$$的零点，可转化为求$$\mu$$的零点：
$$
\mu(x)=\frac{f(x)}{f^\prime(x)}
$$
​	$$\mu$$保证了单重根的性质。
$$
\begin{aligned}g(x)&= x-\frac{\mu(x)}{\mu'(x)}\\&= x-\frac{f(x)/f'(x)}{[f'(x)^2-f(x)f''(x)]/f'(x)^2},\end{aligned}
$$

### 收敛阶

$$\alpha$$阶收敛：$$\lim_{n\rightarrow\infin}\frac{|p_{n+1}-p|}{|p_{n}-p|^{\alpha}}=\lambda$$

对于不动点法$$p_n=g(p_{n-1})$$

* 当$$g(p)=p,g^\prime(p)=0$$时，方法二阶收敛。

* 牛顿法在单根条件下二阶收敛。

### Honor方法

实现多项式除法
$$
b_n=a_n\\
b_k-b_{k+1}x_0=a_k\\
b_0=p(x_0)
$$

### 加速方法

$$Aitken$$方法
$$
\hat p_n=p_n-\frac{(p_{n+1}-p_{n})^2}{p_{n+2}-2p_{n+1}+p_n}
$$
​	使用差分符号，改写为:
$$
\hat p_n=p_n-\frac{(\Delta p_n)^2}{\Delta^2p_n}
$$
Steffense方法

​	基于$$p_0$$，每次产生$$p_1,p_2$$，然后预估出更好的$$\hat p_0$$，更新$$p_0=\hat p_0$$

单点求值

​	Horner方法，多项式除法。

​	求多项式$$P(x)$$在$$x=x_0$$的取值，$$P(x)=Q(x)(x-x_0)+b_0$$
$$
b_n=a_n\\
b_k-b_{k+1}x_0=a_k\\
$$
​		直到求出$$b_0$$，即为$$P(x_0)$$

## 插值

### 拉格朗日插值

​	插值基函数
$$
L_{n,k}=\prod_{i=0\ i\neq k}^{n}\frac{(x-x_i)}{(x_k-x_i)}
$$
​	误差余项：
$$
f(x)=P_n(x)+\frac{f^{(n+1)}(\xi(x))}{(n+1)!}(x-x_0)(x-x_1)\cdots(x-x_n)
$$
​			**当$$n=1$$时**
$$
|f(x)-P_1(x)|=\frac{|f''(\xi)|}{2!}|(x-x_0)(x-x_1)|\leq\frac{M_2h^2}8
$$
​			当$$n=2$$时
$$
|f(x)-P_2(x)|=\frac{|f^{(3)}(\xi)|}{3!}|(x-x_0)(x-x_1)(x-x_2)|\leq\frac{M_3h^3}{9\sqrt{3}}
$$
​			当$$n=3$$时
$$
|f(x)-P_3(x)|=\frac{|f^{(4)}(\xi)|}{4!}|(x-x_0)(x-x_1)(x-x_2)(x-x_3)|\leq\frac{M_4h^4}{24}
$$
Neville方法：

​	递归生成某一点的拉格朗日多项式值。

### Newton方法：

​	离散形式的泰勒展开式：
$$
P_{n}(x)=f[x_0]+\sum_{k=1}^nf[x_0,x_1,\cdots,x_k](x-x_0)(x-x_1)\cdots(x-x_{k-1})
$$
​	等距情况下：               
$$
P_{n}(x)=f[x_0]+\sum_{k=1}^n\left(\begin{matrix}s\\k\end{matrix}\right)k!h^kf[x_0,x_1,\cdots,x_k]
$$
​	引入差商，向前差分：
$$
P_{n}(x)=f(x_0)+\sum_{k=1}^n\left(\begin{matrix}s\\k\end{matrix}\right)\Delta^kf(x_0)
$$

### Hermite插值

密切多项式

​	Taylor(x_0处高阶导数相等)+Lagrange(x_0与函数值相等，其他点为0）

Hermite多项式

​	在拉格朗日基础上，增加了**一阶导数相等**条件。
$$
H_{n,j}(x)=(1-2(x-x_j)L'_{n,j}(x_j))L_{n,j}^2(x)\\
\hat H_{n,j}(x)=(x-x_j)L_{n,j}^2(x)
$$
误差：
$$
f(x)=H_{2n+1}(x)+\frac{(x-x_0)^2(x-x_1)^2\cdots(x-x_n)^2}{(2n+2)!}f^{2n+2}(\xi)
$$
​	用类似拉格朗日形式推导。

差商形式导出：

​	将n个点变为2n个点。

​	需要将一阶差商进行替换。

> [Newton型的Hermite差值（数值计算方法）_重节点差商表怎么构造-CSDN博客](https://blog.csdn.net/qq_42294351/article/details/116124811)
>
> [Hermite插值 (ustc.edu.cn)](http://staff.ustc.edu.cn/~rui/ppt/num/num-interpolation-hermite.html#num-intp-hermite-error)

### 三次样条插值

分段线性插值：

**分段三次 Hermite 插值**：曲线在节点处不仅匹配函数值，还匹配**导数值**，因此曲线在节点处的斜率与给定的导数值相同。（需要知道**更多信息**）

**三次样条插值**：曲线在节点处不仅函数值连续，还确保**一阶导数和二阶导数的连续性**，形成更光滑的过渡。

### 误差说明

用到多少个点，误差阶数就是多大。

如，用到$$0,\dots,n$$共计$$(n+1)$$个点，则误差为：
$$
\frac{f^{(n+1)}(\xi(x))}{(n+1)!}(x-x_0)(x-x_1)\cdots(x-x_n)
$$

## 数值微分

### 差分公式：

向前差分公式：
$$
f'(x_0)=\frac{f(x_0+h)-f(x_0)}h-\frac h2f''(\xi)
$$
三点公式：
$$
\begin{aligned}
&\text{向前差分:}f^{\prime}(x_0)=\frac1{2h}(-3f(x_0)+4f(x_0+h)-f(x_0+2h))+\frac{h^2}3f^{(3)}(\xi_0)\\
&\text{向后差分:}f^{\prime}(x_0)=\frac1{2h}(f(x_0-2h)-4f(x_0+h)+3f(x_0))+\frac{h^2}3f^{(3)}(\xi_0)\\
&\text{中心差分:}f^{\prime}(x_0)=\frac1{2h}(-f(x_0-h)+f(x_0+h))-\frac{h^2}6f^{(3)}(\xi_0)
\end{aligned}
$$
​	特别的，将向前差分的h变为-h，就可以得到向后差分。

高阶导数：

​	在$$x_0$$处泰勒展开，并带入$$x_0+h$$与$$x_0-h$$作差。
$$
f^{\prime\prime}(x_{0})=\frac{1}{h^{2}}[f(x_{0}-h)-2f(x_{0})+f(x_{0}+h)]-\frac{h^{2}}{12}f^{(4)}(\xi).
$$
舍入误差：
$$
e(h)=\frac{\epsilon}{h}+\frac{h^2}{6}M
$$
​	求导求极值，可知$$h=\sqrt[3]{3\epsilon/M}$$为误差最小处。

外推法：

​	对于截断误差有规律的形式。

​	可以借助外推法迭代进行误差缩小。
$$
N_{j}(h)=N_{j-1}(\frac{h}{2})+\frac{N_{j-1}(h/2)-N_{j-1}(h)}{4^{j-1}-1}
$$

### 误差说明

误差是在取值点的拉格朗日误差的导数。
$$
\begin{aligned}f'(x_j)&=\sum_{k=0}^nf(x_k)L_k'(x_j)+\frac{f^{(n+1)}(\xi(x_j))}{(n+1)!}\prod_{k=0,k\neq j}^n(x_j-x_k)\end{aligned}
$$


## 数值积分

基本思路是使用拉格朗日插值近似$$f(x)$$。

### 基础公式

梯形公式：
$$
\int_a^bf(x)dx=\frac h2[f(x_0)+f(x_1)]-\frac{h^3}{12}f''(\xi)
$$
​	一阶精度

Simpson公式：
$$
\int_a^bf(x)dx=\frac{h}{3}[f(x_0)+4f(x_1)+f(x_2)]-\frac{h^5}{90}f^{(4)}(\xi)
$$
​	三阶精度

### 复合积分

复合梯形公式：
$$
\int_a^bf(x)=[f(a)+2\sum_{j=1}^{n-1}f(x_i)+f(b)]-\frac{b-a}{12}h^2f''(\xi)
$$
复合Simpson公式：
$$
\int_a^bf(x)=[f(a)+2\sum_{j=1}^{n/2-1}f(x_{2j})+4\sum_{j=1}^{n/2}f(x_{2j})+f(b)]-\frac{b-a}{180}h^4f^{(4)}(\xi)
$$
​	要求结点数为**偶数**。	

​	奇数位\*4+偶数位\*2+左右端点\*1

### 误差说明

误差是插值误差的积分。

## 常微分方程

### 初值问题基本理论

Lipschitz条件

​	**基本定义：**	

> 一个函数$$f(t,y)$$称为关于集合$$D\subset \mathbb{R}^2$$上的变量$$y$$满足 Lipschiz 条件，如果存在一个常数$$L>0$$使得对所有的$$(t,y_1),(t,y_2)\in D$$都满足：
> $$
> |f(t,y_1)-f(t,y_2)|\leq L|y_1-y_2|
> $$
> 常数$$L$$称为$$f$$的Lipschitz常数。

​	**凸集**：

> 集合$$D\subset\mathbf{R}^2$$是凸的，当且仅当如果$$(t_1,y_1),(t_2,y_2)\in D$$
> 那么点$$((1-\lambda)t_1+\lambda t_2,(1-\lambda)y_1+\lambda y_2)$$也属于$$D$$,对于任意 $$\lambda\in[0,1]$$

​	**判定定理：**

> 假设 $$f(t, y)$$ 定义在凸集$$ D \subset \mathbb{R}^2 $$上。如果存在一个常数 $$ L > 0 $$ 使得 
> $$
> \left| \frac{\partial f}{\partial y} f(t, y) \right| \leq L
> $$
> 对一切 $$ (t, y) \in D $$ 成立，则 $$ f $$ 在 $$ D $$ 上关于变量 $$ y $$ 满足 Lipschitz 常数为 $$ L $$ 的 Lipschitz 条件。

​	**唯一解定理：**

> 设$$D=\{(t,y)|a\leq t\leq b,-\infty<y<\infty\}$$,并且$$f(t,y)$$在$$D$$上连续。
> 如果$$f$$在$$D$$上满足Lipschitz条件，那么初值问题
> $$
> y^{\prime }( t) = f( t, y) ,\quad a< t\leq b,\quad y(a)=\alpha
> $$
> 对于$$a\leq t\leq b$$有唯一解$$y(t)$$

​	**适定条件**

> 一个初值问题被称为是适定的，如果它满足：
>
> 1. 该问题解存在且唯一；
>
> 2. 存在常数$$\epsilon_0>0$$和$$k>0$$，使得$$\forall \epsilon\in(0,\epsilon_0)$$，只要$$\delta(t)$$连续且对所有$$t\in[a,b]$$，满足$$|\delta(t)|<\epsilon$$，当$$|\delta_0|<\epsilon$$，初值问题：
>    $$
>    \frac{d{z}}{dt} = f( t, z)+\delta(t) ,\quad a\leq t\leq b,\quad y(a)=\alpha+\delta_0
>    $$
>    有唯一解且满足：
>    $$
>    \forall t\in[a,b]\quad |z(t)-y(t)|<k\epsilon
>    $$

​	**常数变易法**：
$$
y(x)=\left(\int{Q(x)}{\mathrm{e}^{-\int P(x)\mathrm{~d}x}}\mathrm{~d}x+C\right)\mathrm{e}^{\int P(x)\mathrm{~d}x}
$$
​	**分部积分法：**
$$
uv=\int udv+\int vdu
$$




### Euler方法

求解过程：解析问题→数值问题。连续问题→离散问题。

- 连续区间(对t)网格化
- 微分方程差分化

原理：**泰勒展开**，用f替换一阶导数，截断剩余项，进而逐项计算出y的具体走势。

基本公式：
$$
y(t_{j+1})=y(t_j)+hf(t_j,y(t_j))+\color{red}\frac{h^2}2y^{\prime\prime}(\xi_j)
$$
​	 红色为**截断误差**项。

累计误差：
$$
\mid y_{i+1}-w_{i+1}\mid\leqslant\frac{hM}{2L}(\mathrm{e}^{(t_{i+1}-a)L}-1)
$$

局部误差：
$$
\tau_{i+1}(h)\quad=\quad\frac{y_{i+1}-y_i}h-f(t_i,y_i)
$$
​	Euler方法中，局部误差为$$\frac{h}2y^{\prime\prime}(\xi_j)$$

​	仅考虑变化量的影响，$$h$$是作为位移。

​	描述的是**割线与切线的差距**。

### 高阶Taylor

$$
w_{0}=a\\w_{i+1}=w_{i}+hT^{(n)}\left(t_{i},w_{i}\right),\quad i=0,1,\cdots,N-1\\

T^{(n)}(t_{i},w_{i})=f(t_{i},w_{i})+\frac{h}{2}f^{'}(t_{i},w_{i})+\cdots+\frac{h^{n-1}}{n!}f^{(n-1)}(t_{i},w_{i})
$$

 局部截断误差：
$$
\tau_{i+1}(h)=\frac{y_{i+1}-y_{i}}{h}-T^{(n)}(t_{i},y_{i})=\frac{h^{n}}{(n+1)!}f^{(n)}(\xi_{i},y(\xi_{i}))
$$
n阶Taylor对应n阶近似

### Runge-Kutta方法

改进的Euler方法
$$
y_{i+1}=y_{i}+\frac{h}{2}[f(t_{i},y_{i})+f(t_{i+1},y_{i}+hf(t_{i},y_{i}))]
$$
​	引入对未来的预测。

4阶方法
$$
\begin{aligned}
{k_1} &=hf(t_i,y_i), \\
k_{2} &=hf(t_i+\frac h2,y_i+\frac12k_1), \\
k_{3} &=hf(t_i+\frac h2,y_i+\frac12k_2), \\
k_{4} &=hf(t_{i+1},y_i+k_3), \\
y_{i+1} &=y_{i}+\frac{1}{6}(k_{1}+2k_{2}+2k_{3}+k_{4})
\end{aligned}
$$

* k1：当前位置的斜率估计
* k2和 k3是在**半个时间步长**的中间点上计算的斜率，考虑了不同的修正。

* k4是在**整个时间步长结束**时计算的斜率。
* 通过斜率的加权平均（k2,k3权重高），获得更精确的新 y 值

### 显式与隐式

欧拉显式方法：
$$
y_{j+1}= y_j+hf(t_{j},y_{j})
$$
欧拉隐式方法：（如何用不定点求解？）
$$
y_{j+1}= y_j+hf(t_{j+1},y_{j+1})
$$
梯形隐式方法：
$$
y_{j+1} = y_{j}+\frac{h}{2}[f(t_{j},y_{j})+f(t_{j+1},y_{j+1})]
$$

### 稳定性（？）



 ### 误差说明

见高阶Taylor方法的局部截断误差。

## 线性方程组

### 基本概念

对角占优：
$$
|a_{ii}|\geq\sum_{j=1,j\neq i}^n|a_{ij}|
$$
​	恒大于时，为严格对角占优。

​	特别地：严格对角占优的矩阵时非奇异的。

正定矩阵：

​	对称且对于任意的$$x\neq 0 $$，满足$$x^tAx>0$$

​	特别地：正定矩阵$$A$$是正定的，当且仅当$$A$$可以被分解为$$LDL^t$$。（L的对角线元素均为1）

​	正定矩阵$$A$$是正定的，当且仅当$$A$$可以被分解为$$LL^t$$。

### 范数

向量范数
$$
||x||_k=\left\{\sum_{i=1}^{n}x_i^2\right\}^{1/k}
$$
​	性质：
$$
\|\mathbf{x}\|_\infty\leq\|\mathbf{x}\|_2\leq\sqrt{n}\|\mathbf{x}\|_\infty 
$$


矩阵范数：
$$
||A||=\max_{||x||=1}||Ax||
$$
​	矩阵无穷范数（行和范数）		

​	矩阵一范数（列和范数）

​	矩阵二范数（谱半径）
$$
||A||_2=[\rho(A^TA)]^{1/2}
$$

$$
其中：\rho(A)=\max|\lambda|
$$



### 高斯消元

列主元的高斯消元法

​	每次选择当前列最大的元素所在行，交换到当前行。

标度化列主元的高斯消元法
	通过行主元作为标度，将各个行进行归一化，然后再进行选择与交换。

### LU分解

​	一般形式：
$$
\left.\begin{aligned}\mathbf{LU}&=\left(\begin{array}{ccccc}1&0&0&\cdots&0\\l_{21}&1&0&\cdots&0\\l_{31}&l_{32}&1&\cdots&0\\\vdots&\vdots&\vdots&\ddots&\vdots\\l_{n1}&l_{n2}&l_{n3}&\cdots&1\end{array}\right)\left(\begin{array}{cccc}u_{11}&u_{12}&u_{13}&\cdots&u_{1n}\\0&u_{22}&u_{23}&\cdots&u_{2n}\\0&0&u_{33}&\cdots&u_{3n}\\\vdots&\vdots&\vdots&\ddots&\vdots\\0&0&0&\cdots&u_{nn}\end{array}\right)\\&=\left(\begin{array}{cccc}a_{11}&a_{12}&\cdots&a_{1m}\\a_{21}&a_{22}&\cdots&a_{2m}\\\vdots&\vdots&&\vdots\\a_{n1}&a_{n2}&\cdots&a_{nm}\end{array}\right)=\mathbf{A}.\end{aligned}\right.
$$
​	逆向应用矩阵乘法公式：（$$k<i<j$$）
$$
\begin{aligned}&u_{ij}&&=\quad\frac1{l_{ii}}[a_{ij}-\sum_{k=1}^{i-1}l_{ik}u_{kj}],(i\text{th row of U})\\&l_{ji}&&=\quad\frac1{u_{ii}}[a_{ji}-\sum_{k=1}^{i-1}l_{jk}u_{ki}],(i\text{th column of L})\end{aligned}
$$
LDL分解:
$$
d_{ii}= a_{ii}-\sum_{j=1}^{i-1} l_{ij}^2 d_{jj}
$$

$$
l_{ji}=\frac{a_{ij}-\sum_{k=1}^{i-1}l_{ik}l_{jk}d_{kk}}{d_{ii}}
$$

### 迭代方法

Jacobi:
$$
x_i=\frac{-\sum_{j=1,j\neq i}^n(a_{ij}XO_j)+b_i}{a_{ii}}
$$
Gaussion-Seidel:
$$
x_i^{(k)}=\frac{-\sum_{j=1}^{i-1}a_{ij}x_j^{(k)}-\sum_{j=i+1}^na_{ij}x_j^{(k-1)}+b_i}{a_{ii}}
$$
SOR：
$$
x_{i}^{(k)}=(1-\omega)x_{i}^{(k-1)}+\frac{\omega}{a_{ii}}\bigg[b_{i}-\sum_{j=1}^{i-1}a_{ij}x_{j}^{(k)}-\sum_{j=i+1}^na_{ij}x_j^{(k-1)}\bigg]
$$

### Something Else

* 算法的复杂性估计：每个算法的计算次数(乘除法或加减法)?
* 大型带状矩阵为稀疏矩阵，如何存储才能有效地减少存储空间？以及如何查询？
* 原始矩阵与计算矩阵如何存储才能减少存储空间？
* 当$$n$$ 足够大时，除了用矩阵的直接分解方法求解方程组，还有没有好的方法？
* 带状矩阵多出现在**偏微分方程**数值计算方法中，是常见的矩阵形式.

## 逼近论

### 直线拟合：

​		误差函数：
$$
E\equiv\min_{a_0,a_1}\sum_{i=1}^m[y_i-(a_1x_i+a_0)]^2
$$
​		系数解：
$$
a_0=\frac{\sum_{i=1}^mx_i^2\sum_{i=1}^my_i-\sum_{i=1}^mx_iy_i\sum_{i=1}^mx_i}{m\left(\sum_{i=1}^mx_i^2\right)-\left(\sum_{i=1}^mx_i\right)^2}\\
a_1=\frac{m\sum_{i=1}^mx_iy_i-\sum_{i=1}^mx_i\sum_{i=1}^my_i}{m\left(\sum_{i=1}^mx_i^2\right)-\left(\sum_{i=1}^mx_i\right)^2}
$$
### 一般多项式：

​		误差函数：
$$
\begin{aligned}\min_{a_0,a_1,\cdots,a_n}E&=\sum_{i=1}^m(y_i-P_n(x_i))^2\\&=\sum_{i=1}^m(y_i-\sum_{k=0}^na_kx_i^k)^2.\end{aligned}
$$
​		正规方程：
$$
\sum_{k=0}^na_k\sum_{i=1}^mx_i^{j+k}=\sum_{i=1}^my_ix_i^j,
$$
### 函数逼近：

​	误差函数：
$$
\begin{aligned}E&\equiv\quad E(a_0,a_1,\cdots,a_n)=\int_a^b[f(x)-P_n(x)]^2\mathrm{d}x\\&=\quad\int_a^b\left(f(x)-\sum_{k=0}^na_kx^k\right)^2\mathrm{d}x.\end{aligned}
$$
​	正规方程：
$$
\begin{aligned}\sum_{k=0}^na_k\int_a^bx^{j+k}\mathrm dx&=\int_a^bx^jf(x)\mathrm dx,&j=0,1,\cdots,n.\end{aligned}
$$



## 近似特征值

### 圆盘定理

$$
\mathbb{R}_i=\left\{z\in\mathcal{C}\Big||z-a_{ii}|\leq\sum_{j=1,j\neq i}^n|a_{ij}|\right\}
$$
   任何$$k$$个圆盘的并集，如果它与其余$$(n-k)$$个圆盘不相交，那么其中必定包含$$k$$个特征值。

谱半径
$$
\rho(A)=\max\{|\lambda|:\lambda\in\lambda(\mathbf{A})\}
$$


矩阵相似：
$$
\mathbf{A}=\mathbf{S}^{-1}\mathbf{BS}
$$
一些性质:

* 相似矩阵的特征值相同。
* 如果$$n\times n$$的矩阵$$A$$有$$n$$个不同的特征值，那么它相似于一个对角矩阵。
* 对称矩阵，可以被相似正交对角化
* 对称矩阵的特征值全为实数。
* 正定矩阵$$\iff$$所有特征值均为正数。

### 幂法：

 求矩阵的最大特征值。
$$
\mathbf{y}=A\mathbf x\\
求满足|\mathbf y_p|=||\mathbf y||_\infin的最小p\\
\mu=\mathbf y_p\\
\mathbf x=\frac{\mathbf y}{\mu}
$$
收敛速率：$$O(|\frac{\lambda_2}{\lambda_1}|^m)$$

### 加速方法：

 $$Aitken\Delta^2$$方法
$$
初始化:\mu_0=\mu_1=0\\
迭代:\\
\mu=y_p,\hat\mu=\mu_0-\frac{(\mu_1-\mu_0)^2}{\mu-2\mu_1+\mu_0}\\
\mu_1=\mu,\mu_0=\mu_1
$$
 对称幂法：

​	当矩阵$$A$$是对称矩阵时，可以将无穷范数改为二范数。

​	此时，收敛速率为$$O(|\frac{\lambda_2}{\lambda_1}|^{2m})$$

反幂法：

​	对逆矩阵进行幂法，求出矩阵最小特征值。

​	输出时要取倒数。

已知特征值求特征向量：

​	已知特征值$$q$$的情况下，可以对$$A-qI$$使用幂法或者对称幂法。

​	收敛速率为$$O(|\frac{\lambda_2-q}{\lambda_1-q}|^{m})$$ 或者$$O(|\frac{\lambda_2-q}{\lambda_1-q}|^{2m})$$

Rayleigh方法：

​	用$$q=\frac{x^TAx}{x^Tx}$$近似特征值。

​	以加速迭代。

### Householder方法

Householder矩阵
$$
H=I-2\frac{vv^T}{v^Tv}
$$
​	这种形式保证了矩阵H是**对称正定**的：
$$
H=H^{-1}=H^T
$$
​	对于一个向量$$x$$，希望找到一个对应的矩阵$$H$$，使得：
$$
Hx=\alpha e_1
$$
​	计算可得，$$v=x-\alpha e_1$$，$$\alpha=-sign(x_1)||a||_2$$

​	即：
$$
v=x+sign(x_1)||a||_2
$$

### Givens旋转

想要对一个向量进行旋转，以使得其成为单位向量。

构造如下的旋转矩阵：
$$
\begin{bmatrix}1&0&0&0&0\\0&c&0&s&0\\0&0&1&0&0\\0&-s&0&c&0\\0&0&0&0&1\end{bmatrix}
$$
其中:
$$
s=\frac{x_s}{\sqrt{x_s^2+x_c^2}}\\
c=\frac{x_c}{\sqrt{x_s^2+x_c^2}}
$$
该旋转矩阵正交。

 ### QR分解

对于矩阵A，首先进行列分块：
$$
A=[a_1,a_2,\cdots,a_n]
$$
依次对$$a_i$$，进行变换。

​	令$$x=a_1$$，计算得到$$v_1$$，进而得到$$H_1$$。

​	对A左乘$$H_1$$得到$$H_1A$$，然后的继续。

最终得到：
$$
R=H_{n-1}H_{n-2}\cdots H_1 A\\
Q=H_{1}H_{2}\cdots H_{n-1}想起来了，0范数
$$


## 考试 

* [Chap8.pdf (liangjiandeng.github.io)](https://liangjiandeng.github.io/teaching/Numer_Analy/Chap8.pdf)

* https://blog.csdn.net/m0_63155449/article/details/135509078

* https://wenku.baidu.com/view/f0b27023162ded630b1c59eef8c75fbfc67d946f?pcf=2&re=view&bfetype=new&bfetype=new&_wkts_=1718956533310

* **0范数**不是真正的范数，不满足**一阶齐次性**

* 什么是适定问题？适定问题：

  * 存在解
  * 解是唯一的
  * 解随着起始条件连续的改变

* 误差：描述数值计算之中近似值的近似程度

  * 误差按来源可分为：**模型误差、观测误差、截断误差、舍入误差**
  * **模型误差**：数学模型通常是由实际问题抽象得到的，一般带有误差，这种误差称为模型误差。（这个误差一般来说是不可避免的）
  * **观测误差**：数学模型中的一些参数时通过观测和实验得到的，难免带有误差，这种误差称为观测误差。
  * **截断误差**: 这种模型的准确解和由数值方法求出的近似解之间的误差称为**截断误差**。因为截断误差是数值计算方法固有的，因此又称**方法误差**。
  * 舍入误差：计算机只能对有限位数进行运算所以产生的误差
  * **舍入法**和**截断法**。
  * 如果$$p^*$$是$$p$$的近似数，则**绝对误差**是$$|p-p^*|$$ ,**相对误差**是$$\frac{|p-p^*|}{|p|},p\neq0$$
  * 数$$p^*$$称为逼近$$p$$到$$t$$位有效数字，如果$$t$$是最大的非负整数使得$$\frac{|p-p^*|}{|p|}<5\times10^{-t}$$。
  * **总体误差**：累积了所有前面步骤误差的数值解和精确解之间的差异。
  * **局部误差**：单步计算中数值解和精确解之间的差异。

* 稳定：

  * 当**初始数据变化**很小时，算法产生的结果也变化很小。
  * 若是满足一定条件的初始变量，那么**条件稳定**。

* 理解迭代序列的收敛性？误差的收敛阶(定义与表达),以及阶的估计表达。
  $$
  |\alpha_n-\alpha|\leq K|\beta_n|
  $$
  则记：
  $$
  a_n=a+O(\beta_n)
  $$

* 高次插值多项式的龙格现象
  * 插值节点的数目决定了插值多项式的次数
  * 当插值多项式的次数升高时，会带来不同程度的数值震荡，即发生所谓的龙格(Runge)现象：