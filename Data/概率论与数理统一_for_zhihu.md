# 随机事件及概率

## 测度

###  <img src="https://www.zhihu.com/equation?tex=\sigma" alt="\sigma" class="ee_img tr_noresize" eeimg="1"> 代数

定义在集合 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 上的。

 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 为一集合，假设有子集族 <img src="https://www.zhihu.com/equation?tex=\mathcal{F} \subseteq \mathcal{P} ( X) ( \mathcal{P} ( X) " alt="\mathcal{F} \subseteq \mathcal{P} ( X) ( \mathcal{P} ( X) " class="ee_img tr_noresize" eeimg="1">  代表  <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1">  的**幂集**) 满足下列条件 <img src="https://www.zhihu.com/equation?tex=^{[1][2]}" alt="^{[1][2]}" class="ee_img tr_noresize" eeimg="1"> 
1.  <img src="https://www.zhihu.com/equation?tex=X\in\mathcal{F}\text{（这里也就是保证了}\emptyset\in \mathcal{F}\text{）}" alt="X\in\mathcal{F}\text{（这里也就是保证了}\emptyset\in \mathcal{F}\text{）}" class="ee_img tr_noresize" eeimg="1"> 
1.  <img src="https://www.zhihu.com/equation?tex=(\forall F\in\mathcal{F})\left[(F\in\mathcal{F})\Rightarrow(X-F\in\mathcal{F})\right]\text{（对补集封闭）}" alt="(\forall F\in\mathcal{F})\left[(F\in\mathcal{F})\Rightarrow(X-F\in\mathcal{F})\right]\text{（对补集封闭）}" class="ee_img tr_noresize" eeimg="1"> 
 3.  <img src="https://www.zhihu.com/equation?tex=(\forall\mathcal{A})\left\{[(\mathcal{A}\cong\mathbb{N})\land(\mathcal{A}\subseteq\mathcal{F})]\Rightarrow\left(\bigcup\mathcal{A}\in\mathcal{F}\right)\right\}\text{（如果有可数个集合 }A_1,A_2,\cdots\text{ 都在 }\mathcal{F}\text{ 中,那么它们的并集也在}\mathcal{F}\text{ 中）}" alt="(\forall\mathcal{A})\left\{[(\mathcal{A}\cong\mathbb{N})\land(\mathcal{A}\subseteq\mathcal{F})]\Rightarrow\left(\bigcup\mathcal{A}\in\mathcal{F}\right)\right\}\text{（如果有可数个集合 }A_1,A_2,\cdots\text{ 都在 }\mathcal{F}\text{ 中,那么它们的并集也在}\mathcal{F}\text{ 中）}" class="ee_img tr_noresize" eeimg="1"> 

则称  <img src="https://www.zhihu.com/equation?tex=\mathcal{F}" alt="\mathcal{F}" class="ee_img tr_noresize" eeimg="1">  是  <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1">  的一个  <img src="https://www.zhihu.com/equation?tex=\sigma" alt="\sigma" class="ee_img tr_noresize" eeimg="1"> -代数，

在测度论里有序对  <img src="https://www.zhihu.com/equation?tex=(X,\mathcal{F})" alt="(X,\mathcal{F})" class="ee_img tr_noresize" eeimg="1">  会被称为一个**可测空间**。而任何在  <img src="https://www.zhihu.com/equation?tex=F" alt="F" class="ee_img tr_noresize" eeimg="1">  中的子集  <img src="https://www.zhihu.com/equation?tex=A" alt="A" class="ee_img tr_noresize" eeimg="1"> , 则称为**可测集合** (measurable set); 

而在**概率论**中， <img src="https://www.zhihu.com/equation?tex=\mathcal{F}" alt="\mathcal{F}" class="ee_img tr_noresize" eeimg="1">  被称为**事件族** (family of events) ,  <img src="https://www.zhihu.com/equation?tex=\mathcal{F}" alt="\mathcal{F}" class="ee_img tr_noresize" eeimg="1">  中的子集  <img src="https://www.zhihu.com/equation?tex=A" alt="A" class="ee_img tr_noresize" eeimg="1">  则称为**事件**。

### 测度定义

设 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 是一个集合， <img src="https://www.zhihu.com/equation?tex=\Sigma" alt="\Sigma" class="ee_img tr_noresize" eeimg="1">  是一个 <img src="https://www.zhihu.com/equation?tex=\sigma" alt="\sigma" class="ee_img tr_noresize" eeimg="1"> 代数，若函数  <img src="https://www.zhihu.com/equation?tex=\mu:\Sigma\to[0,\infty)" alt="\mu:\Sigma\to[0,\infty)" class="ee_img tr_noresize" eeimg="1">  若满足：

*  <img src="https://www.zhihu.com/equation?tex=\mu(\varnothing)=0" alt="\mu(\varnothing)=0" class="ee_img tr_noresize" eeimg="1">  (空集合的测度为零)

* 可数可加性(  <img src="https://www.zhihu.com/equation?tex=\sigma" alt="\sigma" class="ee_img tr_noresize" eeimg="1"> -可加性): 

  若集合序列  <img src="https://www.zhihu.com/equation?tex=\{E_n\in\Sigma\}_{n\in\mathbb{N}}" alt="\{E_n\in\Sigma\}_{n\in\mathbb{N}}" class="ee_img tr_noresize" eeimg="1">  对所有不相等正整数  <img src="https://www.zhihu.com/equation?tex=i\neq j" alt="i\neq j" class="ee_img tr_noresize" eeimg="1">  都有：

   <img src="https://www.zhihu.com/equation?tex=E_i\cap E_j=\varnothing" alt="E_i\cap E_j=\varnothing" class="ee_img tr_noresize" eeimg="1"> ,则 <img src="https://www.zhihu.com/equation?tex=\mu\left(\bigcup_{n\in\mathbb{N}}E_n\right)=\sum_{n=1}^\infty\mu(E_n)" alt="\mu\left(\bigcup_{n\in\mathbb{N}}E_n\right)=\sum_{n=1}^\infty\mu(E_n)" class="ee_img tr_noresize" eeimg="1"> 

 那 <img src="https://www.zhihu.com/equation?tex=\mu" alt="\mu" class="ee_img tr_noresize" eeimg="1">  被称为定义在  <img src="https://www.zhihu.com/equation?tex=\Sigma" alt="\Sigma" class="ee_img tr_noresize" eeimg="1">  上的一个非负测度，或简称为测度。为了叙述简便起见，也可称  <img src="https://www.zhihu.com/equation?tex=(X,\Sigma,\mu)" alt="(X,\Sigma,\mu)" class="ee_img tr_noresize" eeimg="1">  为一测度空间。

![img](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a6/Measure_illustration.png/220px-Measure_illustration.png)

### 从测度到概率

概率是一种测度。

前文已经说到：

> 而在**概率论**中， <img src="https://www.zhihu.com/equation?tex=\mathcal{F}" alt="\mathcal{F}" class="ee_img tr_noresize" eeimg="1">  被称为**事件族** (family of events) ,  <img src="https://www.zhihu.com/equation?tex=\mathcal{F}" alt="\mathcal{F}" class="ee_img tr_noresize" eeimg="1">  中的子集  <img src="https://www.zhihu.com/equation?tex=A" alt="A" class="ee_img tr_noresize" eeimg="1">  则称为**事件**。

类比的，样本空间 <img src="https://www.zhihu.com/equation?tex=\Omega" alt="\Omega" class="ee_img tr_noresize" eeimg="1"> 对应于前文的集合 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> ，事件族 <img src="https://www.zhihu.com/equation?tex=\mathcal{F}" alt="\mathcal{F}" class="ee_img tr_noresize" eeimg="1"> 是 <img src="https://www.zhihu.com/equation?tex=\Omega" alt="\Omega" class="ee_img tr_noresize" eeimg="1"> 的 <img src="https://www.zhihu.com/equation?tex=\sigma" alt="\sigma" class="ee_img tr_noresize" eeimg="1"> -代数。

函数 <img src="https://www.zhihu.com/equation?tex=P(\mathcal{F})" alt="P(\mathcal{F})" class="ee_img tr_noresize" eeimg="1">  是事件到实数的一个映射，并且满足一下公理。

#### 非负性


<img src="https://www.zhihu.com/equation?tex=\forall A\in\mathcal{F},P(A)>0
" alt="\forall A\in\mathcal{F},P(A)>0
" class="ee_img tr_noresize" eeimg="1">

#### 归一性


<img src="https://www.zhihu.com/equation?tex=P(\Omega)=1
" alt="P(\Omega)=1
" class="ee_img tr_noresize" eeimg="1">

#### 可加性

任意两两不相交事件 <img src="https://www.zhihu.com/equation?tex=E_1,E_2,\ldots" alt="E_1,E_2,\ldots" class="ee_img tr_noresize" eeimg="1"> 的**可数**序列满足

<img src="https://www.zhihu.com/equation?tex=P(E_1\cup E_2\cup\cdots)=\sum P(E_i)
" alt="P(E_1\cup E_2\cup\cdots)=\sum P(E_i)
" class="ee_img tr_noresize" eeimg="1">
对应于测度中的 <img src="https://www.zhihu.com/equation?tex=\sigma" alt="\sigma" class="ee_img tr_noresize" eeimg="1"> 可加性。

则 <img src="https://www.zhihu.com/equation?tex=P(A)" alt="P(A)" class="ee_img tr_noresize" eeimg="1"> 称为事件 <img src="https://www.zhihu.com/equation?tex=A" alt="A" class="ee_img tr_noresize" eeimg="1"> 的概率。

#### 其他性质

* 可减性：

  如果 <img src="https://www.zhihu.com/equation?tex=B\supset A" alt="B\supset A" class="ee_img tr_noresize" eeimg="1"> ，则：

<img src="https://www.zhihu.com/equation?tex=P(B-A)=P(B)-P(A)
  " alt="P(B-A)=P(B)-P(A)
  " class="ee_img tr_noresize" eeimg="1">

*  <img src="https://www.zhihu.com/equation?tex=P(\bar{A})=1-P(A)" alt="P(\bar{A})=1-P(A)" class="ee_img tr_noresize" eeimg="1"> 

* 加法公式（容斥原理）：

<img src="https://www.zhihu.com/equation?tex=P(\bigcup_i^n A_i)=\sum_{1\leq i\leq n}P(A_i)-\sum_{1\leq i < j\leq n}P(A_iA_j)+\cdots+(-1)^{n-1}P(A_1A_2\cdots A_n)
  " alt="P(\bigcup_i^n A_i)=\sum_{1\leq i\leq n}P(A_i)-\sum_{1\leq i < j\leq n}P(A_iA_j)+\cdots+(-1)^{n-1}P(A_1A_2\cdots A_n)
  " class="ee_img tr_noresize" eeimg="1">

* [x] **下连续性与上连续性**：由无穷导致的。



## 条件概率

### 定义

设 <img src="https://www.zhihu.com/equation?tex=(\Omega,\mathcal{F},P)" alt="(\Omega,\mathcal{F},P)" class="ee_img tr_noresize" eeimg="1"> 是一个概率空间，设 <img src="https://www.zhihu.com/equation?tex=A\in\mathcal{F}" alt="A\in\mathcal{F}" class="ee_img tr_noresize" eeimg="1"> ，并且 <img src="https://www.zhihu.com/equation?tex=P(A)>0" alt="P(A)>0" class="ee_img tr_noresize" eeimg="1"> ，则对于任意的 <img src="https://www.zhihu.com/equation?tex=B\in\mathbf{F}" alt="B\in\mathbf{F}" class="ee_img tr_noresize" eeimg="1"> ，记：

<img src="https://www.zhihu.com/equation?tex=P(B|A)=\frac{P(AB)}{P(A)}
" alt="P(B|A)=\frac{P(AB)}{P(A)}
" class="ee_img tr_noresize" eeimg="1">
 <img src="https://www.zhihu.com/equation?tex=P(B|A)" alt="P(B|A)" class="ee_img tr_noresize" eeimg="1"> 为事件 <img src="https://www.zhihu.com/equation?tex=A" alt="A" class="ee_img tr_noresize" eeimg="1"> 发生的前提下，事件 <img src="https://www.zhihu.com/equation?tex=B" alt="B" class="ee_img tr_noresize" eeimg="1"> 发生的**条件概率**。

**条件概率满足概率公理。**

### 乘法公式



<img src="https://www.zhihu.com/equation?tex=P(A_1A_2\ldots A_n)=P(A_1)P(A_2|A_1)P(A_3|A_1A_2)\cdots P(A_n|A_1A_2\ldots A_{n-1})
" alt="P(A_1A_2\ldots A_n)=P(A_1)P(A_2|A_1)P(A_3|A_1A_2)\cdots P(A_n|A_1A_2\ldots A_{n-1})
" class="ee_img tr_noresize" eeimg="1">

### 答题

> 设 <img src="https://www.zhihu.com/equation?tex=A_1" alt="A_1" class="ee_img tr_noresize" eeimg="1"> ={“事件描述”}， <img src="https://www.zhihu.com/equation?tex=A_2" alt="A_2" class="ee_img tr_noresize" eeimg="1"> ={"事件描述"}。

在使用**可加性**之前，说明**事件互不相容**。

## 独立性

### 定义

若对概率空间中的两个事件 A, B, 有：

<img src="https://www.zhihu.com/equation?tex=P(AB)=P(A)P(B)
" alt="P(AB)=P(A)P(B)
" class="ee_img tr_noresize" eeimg="1">
 则称事件 A 与事件 B 是**相互独立**。否则称他们不相互独立，或相依的。

### 与**互不相容**区分

* **互不相容**讨论的是事件，可以理解为**定义域**。
* **独立**讨论的是实值，可以理解为**值域**。（但是归根结底也是独立）

* 需要注意！互不相容的事件（非空），相互间反而是不独立的。（如图）

![img](https://raw.githubusercontent.com/cp-cp/Markdown4Zhihu/master/Data/概率论与数理统一/20190421095053392.png)



* 若A、B互不相容，A补并B补事件是必然事件。

那么对**独立**事件的理解，就是**不受其他影响**，而不是没有关系。

### 其他性质

* 特别的，必然事件 <img src="https://www.zhihu.com/equation?tex=\Omega" alt="\Omega" class="ee_img tr_noresize" eeimg="1"> 与不可能事件 <img src="https://www.zhihu.com/equation?tex=\emptyset" alt="\emptyset" class="ee_img tr_noresize" eeimg="1"> 与任何事件都独立。
* 任意独立
  * 需要证明 <img src="https://www.zhihu.com/equation?tex=2^n-n-1" alt="2^n-n-1" class="ee_img tr_noresize" eeimg="1"> 个等式成立。
  * 任意独立，可得两两独立；反之，不可。
  *  <img src="https://www.zhihu.com/equation?tex=\text{两两独立}\subset \text{任意独立} " alt="\text{两两独立}\subset \text{任意独立} " class="ee_img tr_noresize" eeimg="1"> 



## 全概率公式

### 完备事件集

定义：设 <img src="https://www.zhihu.com/equation?tex=A_1,...,A_n" alt="A_1,...,A_n" class="ee_img tr_noresize" eeimg="1"> 是一组事件，若它们两两互不相容，而且：

<img src="https://www.zhihu.com/equation?tex=\sum_{i=1}^n A_i=\Omega
" alt="\sum_{i=1}^n A_i=\Omega
" class="ee_img tr_noresize" eeimg="1">
则称它们是样本空间的一个**分割**，亦称**完备事件组**。

### 全概率公式

全概率公式：对于 <img src="https://www.zhihu.com/equation?tex=\Omega" alt="\Omega" class="ee_img tr_noresize" eeimg="1"> 的一个分割 <img src="https://www.zhihu.com/equation?tex=A_1,...,A_n,P(A_i)>0" alt="A_1,...,A_n,P(A_i)>0" class="ee_img tr_noresize" eeimg="1"> ,有：

<img src="https://www.zhihu.com/equation?tex=\forall B\in\mathscr{F},P(B)=\sum_{i=1}^nP(B|A_i)
" alt="\forall B\in\mathscr{F},P(B)=\sum_{i=1}^nP(B|A_i)
" class="ee_img tr_noresize" eeimg="1">
**形式化的分类讨论**。

### 答题

**对样本空间进行合理的划分。**

> P26页例1.5.4

利用全概率公式需要，划分事件集，并声明“A_1A_2A_3..为**完备事件集**”，之后才能使用全概率公式。

## 贝叶斯公式

贝叶斯公式：对于概率空间 <img src="https://www.zhihu.com/equation?tex=(\Omega,\mathscr{F},P)" alt="(\Omega,\mathscr{F},P)" class="ee_img tr_noresize" eeimg="1"> ， <img src="https://www.zhihu.com/equation?tex=A_1,A_2,...,A_n" alt="A_1,A_2,...,A_n" class="ee_img tr_noresize" eeimg="1"> 是样本空间的一个分割，则对任意 <img src="https://www.zhihu.com/equation?tex=B\in\mathscr{F}" alt="B\in\mathscr{F}" class="ee_img tr_noresize" eeimg="1"> ， <img src="https://www.zhihu.com/equation?tex=P(B)>0" alt="P(B)>0" class="ee_img tr_noresize" eeimg="1"> ，有：

<img src="https://www.zhihu.com/equation?tex=P(A_k|B)=\frac{P(A_k)P(B|A_k)}{\sum_{j=1}^n P(A_j)P(B|A_j)},k=1,2,...,n
" alt="P(A_k|B)=\frac{P(A_k)P(B|A_k)}{\sum_{j=1}^n P(A_j)P(B|A_j)},k=1,2,...,n
" class="ee_img tr_noresize" eeimg="1">

## 伯努利概型

若试验 <img src="https://www.zhihu.com/equation?tex=E_1" alt="E_1" class="ee_img tr_noresize" eeimg="1"> 的任一结果（事件）都与试验 <img src="https://www.zhihu.com/equation?tex=E_2" alt="E_2" class="ee_img tr_noresize" eeimg="1"> 的任一结果（事件）相互独立，则称这**两个试验相互独立**。

若试验 <img src="https://www.zhihu.com/equation?tex=E_1,...,E_n" alt="E_1,...,E_n" class="ee_img tr_noresize" eeimg="1"> 相互独立，并且这 <img src="https://www.zhihu.com/equation?tex=n" alt="n" class="ee_img tr_noresize" eeimg="1"> 个独立实验相同，则称其为**n重重复试验**。

* n重伯努利试验中，事件A发生k次的概率：

<img src="https://www.zhihu.com/equation?tex=P_n(k)=C_n^kp^k(1-p)^{n-k},P(A)=p
  " alt="P_n(k)=C_n^kp^k(1-p)^{n-k},P(A)=p
  " class="ee_img tr_noresize" eeimg="1">

# 随机变量及其分布

## 随机变量

### 定义

设 <img src="https://www.zhihu.com/equation?tex=X(\omega)" alt="X(\omega)" class="ee_img tr_noresize" eeimg="1"> 是定义在概率空间 <img src="https://www.zhihu.com/equation?tex=(\Omega,\mathscr{F},P)" alt="(\Omega,\mathscr{F},P)" class="ee_img tr_noresize" eeimg="1"> 上的单值实函数，即对每个 <img src="https://www.zhihu.com/equation?tex=\omega\in\Omega" alt="\omega\in\Omega" class="ee_img tr_noresize" eeimg="1"> ，都有 <img src="https://www.zhihu.com/equation?tex=X(\omega)\in R" alt="X(\omega)\in R" class="ee_img tr_noresize" eeimg="1"> ，并且对任意 <img src="https://www.zhihu.com/equation?tex=x\in R" alt="x\in R" class="ee_img tr_noresize" eeimg="1"> ， <img src="https://www.zhihu.com/equation?tex=\{\omega|X(\omega)\leq x\}" alt="\{\omega|X(\omega)\leq x\}" class="ee_img tr_noresize" eeimg="1"> 都是随机事件，

即有：

<img src="https://www.zhihu.com/equation?tex=\{\omega|X(\omega)\leq x\}\in\mathscr{F}
" alt="\{\omega|X(\omega)\leq x\}\in\mathscr{F}
" class="ee_img tr_noresize" eeimg="1">
则称 <img src="https://www.zhihu.com/equation?tex=X(\omega)" alt="X(\omega)" class="ee_img tr_noresize" eeimg="1"> 是概率空间上的**随机变量**。通常简记为 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 。

事件 <img src="https://www.zhihu.com/equation?tex=\{\omega|X(\omega)\leq x\}" alt="\{\omega|X(\omega)\leq x\}" class="ee_img tr_noresize" eeimg="1"> ，简记为 <img src="https://www.zhihu.com/equation?tex=\{X\leq x\}" alt="\{X\leq x\}" class="ee_img tr_noresize" eeimg="1"> 

### 分布函数

分布函数： <img src="https://www.zhihu.com/equation?tex=X\sim F(x)=P(X\leq x)" alt="X\sim F(x)=P(X\leq x)" class="ee_img tr_noresize" eeimg="1"> 。定理：

* 单调不减： <img src="https://www.zhihu.com/equation?tex=a<b\Rightarrow F(a)\leq F(b)" alt="a<b\Rightarrow F(a)\leq F(b)" class="ee_img tr_noresize" eeimg="1"> 。
*  <img src="https://www.zhihu.com/equation?tex=0\leq F(x)\leq 1,\lim_{n\rightarrow +\infin}F(x)=1,\lim_{n\rightarrow-\infin}F(x)=-1" alt="0\leq F(x)\leq 1,\lim_{n\rightarrow +\infin}F(x)=1,\lim_{n\rightarrow-\infin}F(x)=-1" class="ee_img tr_noresize" eeimg="1"> 。
* 右连续性： <img src="https://www.zhihu.com/equation?tex=F(x)" alt="F(x)" class="ee_img tr_noresize" eeimg="1"> 在任何点x处右连续。
  * 用 <img src="https://www.zhihu.com/equation?tex=\bigcap\{X\leq x+\frac{1}{n}\}=\{X\leq x\}" alt="\bigcap\{X\leq x+\frac{1}{n}\}=\{X\leq x\}" class="ee_img tr_noresize" eeimg="1"> 和右极限 <img src="https://www.zhihu.com/equation?tex==\lim_{n\rightarrow\infin}F(x+\frac{1}{n})" alt="=\lim_{n\rightarrow\infin}F(x+\frac{1}{n})" class="ee_img tr_noresize" eeimg="1"> 来证明。

* [x] 为什么没有左连续性？因为**取等条件**

## 离散型随机变量

### 定义

设离散型随机变量X的所有可能取得值为 <img src="https://www.zhihu.com/equation?tex=x_1,...,x_n" alt="x_1,...,x_n" class="ee_img tr_noresize" eeimg="1"> ，而X取 <img src="https://www.zhihu.com/equation?tex=x_k" alt="x_k" class="ee_img tr_noresize" eeimg="1"> 的概率为 <img src="https://www.zhihu.com/equation?tex=p_k" alt="p_k" class="ee_img tr_noresize" eeimg="1"> ，即 <img src="https://www.zhihu.com/equation?tex=P(X=x_k)=p_k(k=1,...,n)" alt="P(X=x_k)=p_k(k=1,...,n)" class="ee_img tr_noresize" eeimg="1"> 。

称上式为随机变量X的**概率分布律**。

### 常见分布

#### 退化分布

 <img src="https://www.zhihu.com/equation?tex=P(X=C)=1" alt="P(X=C)=1" class="ee_img tr_noresize" eeimg="1"> 

#### 两点分布

 <img src="https://www.zhihu.com/equation?tex=P(X=0)=p,P(X=1)=1-p" alt="P(X=0)=p,P(X=1)=1-p" class="ee_img tr_noresize" eeimg="1"> 

#### 二项分布

 <img src="https://www.zhihu.com/equation?tex=P(X=k)=C_n^kp^k(1-p)^{n-k}" alt="P(X=k)=C_n^kp^k(1-p)^{n-k}" class="ee_img tr_noresize" eeimg="1"> 

当 <img src="https://www.zhihu.com/equation?tex=(n+1)p" alt="(n+1)p" class="ee_img tr_noresize" eeimg="1"> 为整数时，在 <img src="https://www.zhihu.com/equation?tex=k=(n+1)p,(n+1)p-1" alt="k=(n+1)p,(n+1)p-1" class="ee_img tr_noresize" eeimg="1"> 处概率取得最大值。

若不为整数，则在 <img src="https://www.zhihu.com/equation?tex=[(n+1)p]" alt="[(n+1)p]" class="ee_img tr_noresize" eeimg="1"> 取得最大值。

于是 <img src="https://www.zhihu.com/equation?tex=[(n+1)p]" alt="[(n+1)p]" class="ee_img tr_noresize" eeimg="1"> 称为二项分布 <img src="https://www.zhihu.com/equation?tex=B(n,p)" alt="B(n,p)" class="ee_img tr_noresize" eeimg="1"> 的**最可能出现次数**，或称**最可能值**。

*  <img src="https://www.zhihu.com/equation?tex=E[X]=np,D(X)=np(1-p)" alt="E[X]=np,D(X)=np(1-p)" class="ee_img tr_noresize" eeimg="1"> 

#### 几何分布

 <img src="https://www.zhihu.com/equation?tex=P(X=k)=(1-p)^{k-1}p" alt="P(X=k)=(1-p)^{k-1}p" class="ee_img tr_noresize" eeimg="1"> ，记为 <img src="https://www.zhihu.com/equation?tex=X\sim G(p)" alt="X\sim G(p)" class="ee_img tr_noresize" eeimg="1"> 。有 <img src="https://www.zhihu.com/equation?tex=\sum_{i=1}^\infin P(X=k)=1" alt="\sum_{i=1}^\infin P(X=k)=1" class="ee_img tr_noresize" eeimg="1"> 。

#### 超几何分布

 <img src="https://www.zhihu.com/equation?tex=N" alt="N" class="ee_img tr_noresize" eeimg="1"> 件产品中有 <img src="https://www.zhihu.com/equation?tex=M" alt="M" class="ee_img tr_noresize" eeimg="1"> 件次品，现抽 <img src="https://www.zhihu.com/equation?tex=n" alt="n" class="ee_img tr_noresize" eeimg="1"> 件出来，其中的次品数服从超几何分布：

<img src="https://www.zhihu.com/equation?tex=P(X=k)=\frac{C_M^kC_{N-M}^{n-k}}{C_N^n},k=1,..,min(n,M)
" alt="P(X=k)=\frac{C_M^kC_{N-M}^{n-k}}{C_N^n},k=1,..,min(n,M)
" class="ee_img tr_noresize" eeimg="1">

### 柏松定理

设随机变量 <img src="https://www.zhihu.com/equation?tex=X_n\sim B(n,p_n),(n=1,2,...)" alt="X_n\sim B(n,p_n),(n=1,2,...)" class="ee_img tr_noresize" eeimg="1"> 。若有 <img src="https://www.zhihu.com/equation?tex=\lim_{n\rightarrow\infin}np_n=\lambda" alt="\lim_{n\rightarrow\infin}np_n=\lambda" class="ee_img tr_noresize" eeimg="1"> ，则有：

<img src="https://www.zhihu.com/equation?tex=\lim_{n\rightarrow\infin}P(X_n=k)=\frac{\lambda^k}{k!}e^{-\lambda}
" alt="\lim_{n\rightarrow\infin}P(X_n=k)=\frac{\lambda^k}{k!}e^{-\lambda}
" class="ee_img tr_noresize" eeimg="1">
记泊松分布为 <img src="https://www.zhihu.com/equation?tex=X\sim P(\lambda)" alt="X\sim P(\lambda)" class="ee_img tr_noresize" eeimg="1"> ：

<img src="https://www.zhihu.com/equation?tex=P(X=k)=\frac{\lambda^k}{k!}e^{-\lambda},k=0,1,2,...
" alt="P(X=k)=\frac{\lambda^k}{k!}e^{-\lambda},k=0,1,2,...
" class="ee_img tr_noresize" eeimg="1">
自然界很多稀疏现象都服从泊松分布，故其又称为**稀疏现象律**。泊松分布最可能值为 <img src="https://www.zhihu.com/equation?tex=\lambda,\lambda -1" alt="\lambda,\lambda -1" class="ee_img tr_noresize" eeimg="1"> 或 <img src="https://www.zhihu.com/equation?tex=[\lambda]" alt="[\lambda]" class="ee_img tr_noresize" eeimg="1"> 。 

*  <img src="https://www.zhihu.com/equation?tex=E[X]=\lambda,D(X)=\lambda" alt="E[X]=\lambda,D(X)=\lambda" class="ee_img tr_noresize" eeimg="1"> 

### 答题

#### 求二项分布极值？

前后项**做比值**。

#### 注意审题

注意是求的**分布**F还是**分布律**P。

## 连续型随机变量

定义：设随机变量X的概率分布函数为 <img src="https://www.zhihu.com/equation?tex=F(x)" alt="F(x)" class="ee_img tr_noresize" eeimg="1"> ，如果存在一个函数 <img src="https://www.zhihu.com/equation?tex=f(x)" alt="f(x)" class="ee_img tr_noresize" eeimg="1"> ，对于任意实数x，都有：

<img src="https://www.zhihu.com/equation?tex=F(x)=\int_{-\infin}^xf(t)dt,x\in R
" alt="F(x)=\int_{-\infin}^xf(t)dt,x\in R
" class="ee_img tr_noresize" eeimg="1">
则称X为**连续性随机变量**， <img src="https://www.zhihu.com/equation?tex=f(x)" alt="f(x)" class="ee_img tr_noresize" eeimg="1"> 为X的**概率密度函数**。

* 连续型随机变量有： <img src="https://www.zhihu.com/equation?tex=P(X=a)=0,P(a\leq X\leq b)=P(a<X\leq b)=P(a\leq X<b)=P(a<X<b)" alt="P(X=a)=0,P(a\leq X\leq b)=P(a<X\leq b)=P(a\leq X<b)=P(a<X<b)" class="ee_img tr_noresize" eeimg="1"> 。
* 一个事件概率为零，他并不一定是不可能事件（空集）。同样，概率为1的也不一定是必然事件。

### 常见分布

#### 均匀分布

 <img src="https://www.zhihu.com/equation?tex=X\sim U[a,b]" alt="X\sim U[a,b]" class="ee_img tr_noresize" eeimg="1"> ：

<img src="https://www.zhihu.com/equation?tex=f(x)=\begin{cases}\frac{1}{b-a}&a\leq x\leq b\\0&else\end{cases}
" alt="f(x)=\begin{cases}\frac{1}{b-a}&a\leq x\leq b\\0&else\end{cases}
" class="ee_img tr_noresize" eeimg="1">

#### 指数分布

 <img src="https://www.zhihu.com/equation?tex=X\sim E(\lambda)" alt="X\sim E(\lambda)" class="ee_img tr_noresize" eeimg="1"> :

<img src="https://www.zhihu.com/equation?tex=f(x)=\begin{cases}\lambda e^{-\lambda x}&x>0\\0&x\leq 0\end{cases}
" alt="f(x)=\begin{cases}\lambda e^{-\lambda x}&x>0\\0&x\leq 0\end{cases}
" class="ee_img tr_noresize" eeimg="1">

* 指数分布具有**无记忆性**： <img src="https://www.zhihu.com/equation?tex=P(X>s+t|X>s)=P(X>t)" alt="P(X>s+t|X>s)=P(X>t)" class="ee_img tr_noresize" eeimg="1"> 。

*  <img src="https://www.zhihu.com/equation?tex=E[X]=\frac{1}{\lambda},D(X)=\frac{1}{\lambda^2}" alt="E[X]=\frac{1}{\lambda},D(X)=\frac{1}{\lambda^2}" class="ee_img tr_noresize" eeimg="1"> 


#### 正态分布

 <img src="https://www.zhihu.com/equation?tex=X\sim N(\mu,\sigma^2)" alt="X\sim N(\mu,\sigma^2)" class="ee_img tr_noresize" eeimg="1"> :

<img src="https://www.zhihu.com/equation?tex=f(x)=\frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{(x-\mu)^2}{2\sigma^2}},x\in R
" alt="f(x)=\frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{(x-\mu)^2}{2\sigma^2}},x\in R
" class="ee_img tr_noresize" eeimg="1">

* 标准正态分布的概率函数和分布函数记为 <img src="https://www.zhihu.com/equation?tex=\varphi(x),\Phi(x)" alt="\varphi(x),\Phi(x)" class="ee_img tr_noresize" eeimg="1"> 。
* 有 <img src="https://www.zhihu.com/equation?tex=\Phi(-x)=1-\Phi(x)" alt="\Phi(-x)=1-\Phi(x)" class="ee_img tr_noresize" eeimg="1"> （关于y轴对称）。
* 3 <img src="https://www.zhihu.com/equation?tex=\sigma" alt="\sigma" class="ee_img tr_noresize" eeimg="1"> 原则：正态分布几何全部的取值都落在 <img src="https://www.zhihu.com/equation?tex=[\mu-3\sigma,\mu+3\sigma]" alt="[\mu-3\sigma,\mu+3\sigma]" class="ee_img tr_noresize" eeimg="1"> 内。

#### 多元正态分布（缺了点）

如果  <img src="https://www.zhihu.com/equation?tex=\Sigma" alt="\Sigma" class="ee_img tr_noresize" eeimg="1"> 是非奇异的，那么该分布可以由以下的概率密度函数来描述：


<img src="https://www.zhihu.com/equation?tex=f_\mathbf{x}(x_1,\ldots,x_k)=\frac1{\sqrt{(2\pi)^k|\boldsymbol{\Sigma}|}}\mathrm{e}^{-\frac12(\mathbf{x}-\boldsymbol{\mu})^\mathrm{T}\boldsymbol{\Sigma}^{-1}(\mathbf{x}-\boldsymbol{\mu})}
" alt="f_\mathbf{x}(x_1,\ldots,x_k)=\frac1{\sqrt{(2\pi)^k|\boldsymbol{\Sigma}|}}\mathrm{e}^{-\frac12(\mathbf{x}-\boldsymbol{\mu})^\mathrm{T}\boldsymbol{\Sigma}^{-1}(\mathbf{x}-\boldsymbol{\mu})}
" class="ee_img tr_noresize" eeimg="1">
 注意这里的 <img src="https://www.zhihu.com/equation?tex=|\Sigma|" alt="|\Sigma|" class="ee_img tr_noresize" eeimg="1"> 表示协方差矩阵的行列式。



从线性变换的角度理解：

设 <img src="https://www.zhihu.com/equation?tex=X=(x_1,x_2,\cdots,x_n)^T" alt="X=(x_1,x_2,\cdots,x_n)^T" class="ee_img tr_noresize" eeimg="1"> 为各维度均独立的正态分布 <img src="https://www.zhihu.com/equation?tex=\mathcal{N}(\mu,\sigma)" alt="\mathcal{N}(\mu,\sigma)" class="ee_img tr_noresize" eeimg="1"> 

<img src="https://www.zhihu.com/equation?tex=\begin{aligned}
f(x_1,x_2,\cdots,x_n)&=f(x_1)f(x_2)\cdots f(x_n)\\
										 &=\frac1{\sqrt{(2\pi)^k}\sigma^k}\mathrm{e}^{-\frac{(\mathbf{x}-\boldsymbol{\mu})^\mathrm{T}(\mathbf{x}-\boldsymbol{\mu})}{\sigma^k}}
\end{aligned}
" alt="\begin{aligned}
f(x_1,x_2,\cdots,x_n)&=f(x_1)f(x_2)\cdots f(x_n)\\
										 &=\frac1{\sqrt{(2\pi)^k}\sigma^k}\mathrm{e}^{-\frac{(\mathbf{x}-\boldsymbol{\mu})^\mathrm{T}(\mathbf{x}-\boldsymbol{\mu})}{\sigma^k}}
\end{aligned}
" class="ee_img tr_noresize" eeimg="1">
此时的协方差矩阵就是对角矩阵，且各个值均为 <img src="https://www.zhihu.com/equation?tex=\sigma" alt="\sigma" class="ee_img tr_noresize" eeimg="1"> 。

做线性变换

<img src="https://www.zhihu.com/equation?tex=Y=AX+B
" alt="Y=AX+B
" class="ee_img tr_noresize" eeimg="1">
此时将正态分布一般化。



## 随机变量函数的分布（？？？）

定理：设连续型随机变量 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 具有概率密度函数 <img src="https://www.zhihu.com/equation?tex=f_X(x)" alt="f_X(x)" class="ee_img tr_noresize" eeimg="1"> ，其可能的取值范围为 <img src="https://www.zhihu.com/equation?tex=(a,b)" alt="(a,b)" class="ee_img tr_noresize" eeimg="1"> （可以到无穷）。则：

* 若函数 <img src="https://www.zhihu.com/equation?tex=y=g(x)" alt="y=g(x)" class="ee_img tr_noresize" eeimg="1"> 在区间 <img src="https://www.zhihu.com/equation?tex=(a,b)" alt="(a,b)" class="ee_img tr_noresize" eeimg="1"> 上严格单调，其反函数 <img src="https://www.zhihu.com/equation?tex=x=g^{-1}(y)" alt="x=g^{-1}(y)" class="ee_img tr_noresize" eeimg="1"> 有连续的导函数，则 <img src="https://www.zhihu.com/equation?tex=Y=g(X)" alt="Y=g(X)" class="ee_img tr_noresize" eeimg="1"> 也是连续型随机变量，其概率密度函数为：

<img src="https://www.zhihu.com/equation?tex=f_Y(y)=\begin{cases}f_X(g^{-1}(y))|(g^{-1})'(y)|& min(g(a),g(b))<y<max(g(a),b(b))\\0&else\end{cases}
  " alt="f_Y(y)=\begin{cases}f_X(g^{-1}(y))|(g^{-1})'(y)|& min(g(a),g(b))<y<max(g(a),b(b))\\0&else\end{cases}
  " class="ee_img tr_noresize" eeimg="1">

* 若函数 <img src="https://www.zhihu.com/equation?tex=y=g(x)" alt="y=g(x)" class="ee_img tr_noresize" eeimg="1"> 在区间 <img src="https://www.zhihu.com/equation?tex=(a,b)" alt="(a,b)" class="ee_img tr_noresize" eeimg="1"> 中不重叠的区间 <img src="https://www.zhihu.com/equation?tex=I_1,...,I_n" alt="I_1,...,I_n" class="ee_img tr_noresize" eeimg="1"> 上逐段严格单调，其反函数 <img src="https://www.zhihu.com/equation?tex=h_1(y),...,h_n(y)" alt="h_1(y),...,h_n(y)" class="ee_img tr_noresize" eeimg="1"> 在段内均有连续导函数，则Y也是连续型随机变量：

<img src="https://www.zhihu.com/equation?tex=f_Y(y)=\sum_{i=1}^nf_X(h_i(y))|h_i'(y)|

  " alt="f_Y(y)=\sum_{i=1}^nf_X(h_i(y))|h_i'(y)|

  " class="ee_img tr_noresize" eeimg="1">





# 多维随机变量及其分布

## 二维随机变量及其分布

### 定义

设 <img src="https://www.zhihu.com/equation?tex=(X,Y)" alt="(X,Y)" class="ee_img tr_noresize" eeimg="1"> 是二位随机变量，对任意实数 <img src="https://www.zhihu.com/equation?tex=x,y" alt="x,y" class="ee_img tr_noresize" eeimg="1"> ，二元函数 <img src="https://www.zhihu.com/equation?tex= F(x,y)=P(X\leq x,Y\leq y)" alt=" F(x,y)=P(X\leq x,Y\leq y)" class="ee_img tr_noresize" eeimg="1"> 称为随机变量 <img src="https://www.zhihu.com/equation?tex=(X,Y)" alt="(X,Y)" class="ee_img tr_noresize" eeimg="1"> 的联合分布函数。

<img src="https://www.zhihu.com/equation?tex=F(x,y)=\int_{-\infin}^{x}\int_{-\infin}^yf(u,v)dudv
" alt="F(x,y)=\int_{-\infin}^{x}\int_{-\infin}^yf(u,v)dudv
" class="ee_img tr_noresize" eeimg="1">

* 特别地，如果二阶偏导数 <img src="https://www.zhihu.com/equation?tex=f(x,y)" alt="f(x,y)" class="ee_img tr_noresize" eeimg="1"> 连续（即与求偏导顺序无关），则定义 <img src="https://www.zhihu.com/equation?tex=f(x,y)=\frac{\partial^2F(x,y)}{\partial x\partial y}" alt="f(x,y)=\frac{\partial^2F(x,y)}{\partial x\partial y}" class="ee_img tr_noresize" eeimg="1"> 为**联合密度函数**。
  * 二维正态分布
  * 二维均匀分布

## 边缘分布

>记二维随机变量的分布函数 <img src="https://www.zhihu.com/equation?tex=F(x,y)" alt="F(x,y)" class="ee_img tr_noresize" eeimg="1"> 关于 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 和 <img src="https://www.zhihu.com/equation?tex=Y" alt="Y" class="ee_img tr_noresize" eeimg="1"> 的边缘分布函数为 <img src="https://www.zhihu.com/equation?tex=F_X(x)=F(x,+\infin),F_Y(y)=F(+\infin,y)" alt="F_X(x)=F(x,+\infin),F_Y(y)=F(+\infin,y)" class="ee_img tr_noresize" eeimg="1"> 。同样也有边缘概率密度函数： <img src="https://www.zhihu.com/equation?tex=f_X(x)=\int_{-\infin}^{+\infin}f(x,y)dy" alt="f_X(x)=\int_{-\infin}^{+\infin}f(x,y)dy" class="ee_img tr_noresize" eeimg="1"> 。

* 二维正态分布的边缘分布仍为正态分布。
* 边缘分布的理解就是不论y取什么，只考虑x的取值情况。**就像对多量子比特系统中，对单一比特进行测量之后引起的系统的坍塌。**

## 条件分布

### 定义

条件概率分布函数的定义为： <img src="https://www.zhihu.com/equation?tex=F_{Y|X}(y|x)=\frac{F(x,y)}{f_X(x)}=\int_{-\infin}^y\frac{f(x,v)dv}{f_X(x)}" alt="F_{Y|X}(y|x)=\frac{F(x,y)}{f_X(x)}=\int_{-\infin}^y\frac{f(x,v)dv}{f_X(x)}" class="ee_img tr_noresize" eeimg="1"> ，条件概率密度函数为 <img src="https://www.zhihu.com/equation?tex=f_{Y|X}(y|x)=\frac{f(x,y)}{f_X(x)}" alt="f_{Y|X}(y|x)=\frac{f(x,y)}{f_X(x)}" class="ee_img tr_noresize" eeimg="1"> 

## 随机变量的独立性

### 定义

若对二维随机变量 <img src="https://www.zhihu.com/equation?tex=(X,Y)" alt="(X,Y)" class="ee_img tr_noresize" eeimg="1"> ，有 <img src="https://www.zhihu.com/equation?tex=\forall x,y.F(x,y)=F_X(x)F_Y(y)" alt="\forall x,y.F(x,y)=F_X(x)F_Y(y)" class="ee_img tr_noresize" eeimg="1"> 或 <img src="https://www.zhihu.com/equation?tex=f(x,y)=f_X(x)f_Y(y)" alt="f(x,y)=f_X(x)f_Y(y)" class="ee_img tr_noresize" eeimg="1"> （两式等价），则称X与Y**相互独立**。

### 二维正态分布独立与相关

**独立**  <img src="https://www.zhihu.com/equation?tex=\rightarrow" alt="\rightarrow" class="ee_img tr_noresize" eeimg="1"> **相关**：

<img src="https://www.zhihu.com/equation?tex=Cov(X,Y)=E[XY]-EX\cdot EY=0
" alt="Cov(X,Y)=E[XY]-EX\cdot EY=0
" class="ee_img tr_noresize" eeimg="1">
**相关** <img src="https://www.zhihu.com/equation?tex=\rightarrow" alt="\rightarrow" class="ee_img tr_noresize" eeimg="1"> **独立**：

协方差矩阵非对角线元素为0，变成对角阵，然后由正态分布的概率公式拆分出独立的形式。（正态分布的指数为正定二次型，即可分离）



## 二维随机变量函数的分布

令 <img src="https://www.zhihu.com/equation?tex=Z=g(X,Y)" alt="Z=g(X,Y)" class="ee_img tr_noresize" eeimg="1"> ，一般会先求 <img src="https://www.zhihu.com/equation?tex=Z" alt="Z" class="ee_img tr_noresize" eeimg="1"> 的分布函数 <img src="https://www.zhihu.com/equation?tex=F_Z(z)=\iint_{g(x,y)\leq z}f(x,y)dxdy" alt="F_Z(z)=\iint_{g(x,y)\leq z}f(x,y)dxdy" class="ee_img tr_noresize" eeimg="1"> ，然后再求导得到 <img src="https://www.zhihu.com/equation?tex=f_Z(z)" alt="f_Z(z)" class="ee_img tr_noresize" eeimg="1"> 。

### 加法

若 <img src="https://www.zhihu.com/equation?tex=Z=X+Y" alt="Z=X+Y" class="ee_img tr_noresize" eeimg="1"> ，有 <img src="https://www.zhihu.com/equation?tex=f_Z(z)=\int_{-\infin}^{+\infin}f(x,z-x)dx=\int_{-\infin}^{+\infin}f(z-y,y)dy" alt="f_Z(z)=\int_{-\infin}^{+\infin}f(x,z-x)dx=\int_{-\infin}^{+\infin}f(z-y,y)dy" class="ee_img tr_noresize" eeimg="1"> 。（令 <img src="https://www.zhihu.com/equation?tex=u=x+y" alt="u=x+y" class="ee_img tr_noresize" eeimg="1"> ）**概率密度函数卷积公式**

### 乘法



<img src="https://www.zhihu.com/equation?tex=X\sim U(0,1),Y\sim U(0,1)\\
Z=XY\\
\text{求Z的概率密度函数}
" alt="X\sim U(0,1),Y\sim U(0,1)\\
Z=XY\\
\text{求Z的概率密度函数}
" class="ee_img tr_noresize" eeimg="1">


### 除法

若 <img src="https://www.zhihu.com/equation?tex=Z=\frac{X}{Y}" alt="Z=\frac{X}{Y}" class="ee_img tr_noresize" eeimg="1"> ，有 <img src="https://www.zhihu.com/equation?tex=f_Z(z)=\int_{-\infin}^{+\infin}f(yz,y)|y|dy" alt="f_Z(z)=\int_{-\infin}^{+\infin}f(yz,y)|y|dy" class="ee_img tr_noresize" eeimg="1"> 。

### Max

若 <img src="https://www.zhihu.com/equation?tex=Z=max(X,Y)" alt="Z=max(X,Y)" class="ee_img tr_noresize" eeimg="1"> ，有 <img src="https://www.zhihu.com/equation?tex=F_Z(z)=F_X(z)F_Y(z)" alt="F_Z(z)=F_X(z)F_Y(z)" class="ee_img tr_noresize" eeimg="1"> 。（若X，Y相互独立）

### Min

若 <img src="https://www.zhihu.com/equation?tex=Z=min(X,Y)" alt="Z=min(X,Y)" class="ee_img tr_noresize" eeimg="1"> ，有 <img src="https://www.zhihu.com/equation?tex=F_Z(z)=1-[1-F_X(z)][1-F_Y(z)]" alt="F_Z(z)=1-[1-F_X(z)][1-F_Y(z)]" class="ee_img tr_noresize" eeimg="1"> 。

# 随机变量的数学特征

## 数学期望

### 定义

设连续型随机变量 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 的概率密度函数为 <img src="https://www.zhihu.com/equation?tex=f(x)" alt="f(x)" class="ee_img tr_noresize" eeimg="1"> ，若积分 <img src="https://www.zhihu.com/equation?tex=\int_{-\infin}^{+\infin}xf(x)dx" alt="\int_{-\infin}^{+\infin}xf(x)dx" class="ee_img tr_noresize" eeimg="1"> 绝对收敛，则称该积分值为X的数学期望。

### 随机变量函数的期望

若积分 <img src="https://www.zhihu.com/equation?tex=\int_{-\infin}^{+\infin}g(x)f(x)dx" alt="\int_{-\infin}^{+\infin}g(x)f(x)dx" class="ee_img tr_noresize" eeimg="1"> 绝对收敛，则有：

<img src="https://www.zhihu.com/equation?tex=E[g(X)]=\int_{-\infin}^{+\infin}g(x)f(x)dx
" alt="E[g(X)]=\int_{-\infin}^{+\infin}g(x)f(x)dx
" class="ee_img tr_noresize" eeimg="1">

### 一些性质

1. 对**任意**随机变量X，Y都有 <img src="https://www.zhihu.com/equation?tex=E[X+Y]=E[X]+E[Y]" alt="E[X+Y]=E[X]+E[Y]" class="ee_img tr_noresize" eeimg="1"> 。
2. 但只有当它们独立时，才有 <img src="https://www.zhihu.com/equation?tex=E[XY]=E[X]E[Y]" alt="E[XY]=E[X]E[Y]" class="ee_img tr_noresize" eeimg="1"> 。
3. 柯西-施瓦泽不等式： <img src="https://www.zhihu.com/equation?tex=(E[XY])^2\leq E[X^2]E[Y^2]" alt="(E[XY])^2\leq E[X^2]E[Y^2]" class="ee_img tr_noresize" eeimg="1"> 。

### 条件期望（等待补充）



## 方差

### 定义


<img src="https://www.zhihu.com/equation?tex=D(X)=E[X-E(X)]^2
" alt="D(X)=E[X-E(X)]^2
" class="ee_img tr_noresize" eeimg="1">

标准差为： <img src="https://www.zhihu.com/equation?tex=\sqrt{D(X)}" alt="\sqrt{D(X)}" class="ee_img tr_noresize" eeimg="1"> 

### 性质

1.  <img src="https://www.zhihu.com/equation?tex=D(C)=0" alt="D(C)=0" class="ee_img tr_noresize" eeimg="1"> 
2.  <img src="https://www.zhihu.com/equation?tex=D(CX)=C^2D(X)" alt="D(CX)=C^2D(X)" class="ee_img tr_noresize" eeimg="1"> 
3. 若 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 与 <img src="https://www.zhihu.com/equation?tex=Y" alt="Y" class="ee_img tr_noresize" eeimg="1"> 相互独立，则 <img src="https://www.zhihu.com/equation?tex=D(X+Y)=D(X)+D(Y)" alt="D(X+Y)=D(X)+D(Y)" class="ee_img tr_noresize" eeimg="1"> 。

## 协方差与相关系数

### 定义 

*  <img src="https://www.zhihu.com/equation?tex=Cov(X,Y)=E[(X-E[X])(Y-E[Y])]=E[XY]-E[X]E[Y]" alt="Cov(X,Y)=E[(X-E[X])(Y-E[Y])]=E[XY]-E[X]E[Y]" class="ee_img tr_noresize" eeimg="1"> 称为随机变量 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 和 <img src="https://www.zhihu.com/equation?tex=Y" alt="Y" class="ee_img tr_noresize" eeimg="1"> 的**协方差**。

*  <img src="https://www.zhihu.com/equation?tex=\rho_{XY}=\frac{Cov(X,Y)}{\sqrt{D(X)}\sqrt{D(Y)}}" alt="\rho_{XY}=\frac{Cov(X,Y)}{\sqrt{D(X)}\sqrt{D(Y)}}" class="ee_img tr_noresize" eeimg="1"> 称为随机变量X和Y的**相关系数**。

### 性质

*  <img src="https://www.zhihu.com/equation?tex=Cov(X,Y)=Cov(Y,X)" alt="Cov(X,Y)=Cov(Y,X)" class="ee_img tr_noresize" eeimg="1"> 
*  <img src="https://www.zhihu.com/equation?tex=Cov(a_1X+b_1,a_2Y+b_2)=a_1a_2Cov(X,Y)" alt="Cov(a_1X+b_1,a_2Y+b_2)=a_1a_2Cov(X,Y)" class="ee_img tr_noresize" eeimg="1"> 
*  <img src="https://www.zhihu.com/equation?tex=Cov(X_1+X_2,Y)=Cov(X_1,Y)+Cov(X_2,y)" alt="Cov(X_1+X_2,Y)=Cov(X_1,Y)+Cov(X_2,y)" class="ee_img tr_noresize" eeimg="1"> 
*  <img src="https://www.zhihu.com/equation?tex=D(X\pm Y)=D(X)+D(Y)\pm 2Cov(X,Y)" alt="D(X\pm Y)=D(X)+D(Y)\pm 2Cov(X,Y)" class="ee_img tr_noresize" eeimg="1"> 
*  <img src="https://www.zhihu.com/equation?tex=X,Y" alt="X,Y" class="ee_img tr_noresize" eeimg="1"> 独立 <img src="https://www.zhihu.com/equation?tex=\Leftrightarrow Cov(X,Y)=0" alt="\Leftrightarrow Cov(X,Y)=0" class="ee_img tr_noresize" eeimg="1"> 
*  <img src="https://www.zhihu.com/equation?tex=|\rho_{XY}|\leq 1" alt="|\rho_{XY}|\leq 1" class="ee_img tr_noresize" eeimg="1"> ，且取等的充要条件是 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 和 <img src="https://www.zhihu.com/equation?tex=Y" alt="Y" class="ee_img tr_noresize" eeimg="1"> 呈线性关系。

### 独立与相关

* 一般来说， <img src="https://www.zhihu.com/equation?tex=|\rho_{XY}|" alt="|\rho_{XY}|" class="ee_img tr_noresize" eeimg="1"> 越大，X和Y的“线性相关”越强，若 <img src="https://www.zhihu.com/equation?tex=\rho_{XY}=0" alt="\rho_{XY}=0" class="ee_img tr_noresize" eeimg="1"> ，则它们独立。注意，当且仅当 <img src="https://www.zhihu.com/equation?tex=\rho_{XY}=0" alt="\rho_{XY}=0" class="ee_img tr_noresize" eeimg="1"> 时称他们**不相关**。
*  <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 和 <img src="https://www.zhihu.com/equation?tex=Y" alt="Y" class="ee_img tr_noresize" eeimg="1"> 独立 <img src="https://www.zhihu.com/equation?tex=\Rightarrow Cov(X,Y)=0" alt="\Rightarrow Cov(X,Y)=0" class="ee_img tr_noresize" eeimg="1"> ，反之不一定成立。譬如 <img src="https://www.zhihu.com/equation?tex=X\sim U[-1,1],Y=X^2" alt="X\sim U[-1,1],Y=X^2" class="ee_img tr_noresize" eeimg="1"> 。

### 矩

 <img src="https://www.zhihu.com/equation?tex=E(X^k)" alt="E(X^k)" class="ee_img tr_noresize" eeimg="1"> 为 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 的 <img src="https://www.zhihu.com/equation?tex=k" alt="k" class="ee_img tr_noresize" eeimg="1"> 阶原点矩。

 <img src="https://www.zhihu.com/equation?tex=E\{[X-E(X)]^k\}" alt="E\{[X-E(X)]^k\}" class="ee_img tr_noresize" eeimg="1"> 为 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 的 <img src="https://www.zhihu.com/equation?tex=k" alt="k" class="ee_img tr_noresize" eeimg="1"> 阶中心矩。

混合矩、混合中心矩。

### 协方差矩阵

设 <img src="https://www.zhihu.com/equation?tex=(X_1,X_2,\cdots,X_n)" alt="(X_1,X_2,\cdots,X_n)" class="ee_img tr_noresize" eeimg="1"> 为 <img src="https://www.zhihu.com/equation?tex=n" alt="n" class="ee_img tr_noresize" eeimg="1"> 维随机变量，记 <img src="https://www.zhihu.com/equation?tex=c_{ij}=Cov(X_i,X_j)" alt="c_{ij}=Cov(X_i,X_j)" class="ee_img tr_noresize" eeimg="1"> ，若都存在，则矩阵 <img src="https://www.zhihu.com/equation?tex=\Sigma" alt="\Sigma" class="ee_img tr_noresize" eeimg="1"> 为协方差矩阵。

# 极限定理

## 大数定理

### 切比雪夫不等式


<img src="https://www.zhihu.com/equation?tex=\forall \varepsilon>0,P(|X-E[X]|\geq\varepsilon)\leq\frac{D(X)}{\varepsilon^2}
" alt="\forall \varepsilon>0,P(|X-E[X]|\geq\varepsilon)\leq\frac{D(X)}{\varepsilon^2}
" class="ee_img tr_noresize" eeimg="1">

### 切比雪夫大数定理

设随机变量 <img src="https://www.zhihu.com/equation?tex=X_1,...,X_n,..." alt="X_1,...,X_n,..." class="ee_img tr_noresize" eeimg="1"> 相互**独立**，且有**相同的数学期望和方差**，即： <img src="https://www.zhihu.com/equation?tex=E[X_k]\equiv \mu,D(X_k)\equiv \sigma^2" alt="E[X_k]\equiv \mu,D(X_k)\equiv \sigma^2" class="ee_img tr_noresize" eeimg="1"> ，则有：

<img src="https://www.zhihu.com/equation?tex=\forall\varepsilon >0,\lim_{n\rightarrow\infin}P(|\frac{1}{n}\sum_{k=1}^nX_k-\mu|<\varepsilon)=1
" alt="\forall\varepsilon >0,\lim_{n\rightarrow\infin}P(|\frac{1}{n}\sum_{k=1}^nX_k-\mu|<\varepsilon)=1
" class="ee_img tr_noresize" eeimg="1">

### 辛钦大数定律：

设随机变量 <img src="https://www.zhihu.com/equation?tex=X_1,...,X_n,..." alt="X_1,...,X_n,..." class="ee_img tr_noresize" eeimg="1"> **独立同分布**，且有相同的**数学期望**，即 <img src="https://www.zhihu.com/equation?tex=E[X_k]\equiv\mu" alt="E[X_k]\equiv\mu" class="ee_img tr_noresize" eeimg="1"> ，则：

<img src="https://www.zhihu.com/equation?tex=\forall\varepsilon>0,\lim_{n\rightarrow\infin}P(|\frac{1}{n}\sum_{k=1}^{n}X_k-\mu|<\varepsilon)=1
" alt="\forall\varepsilon>0,\lim_{n\rightarrow\infin}P(|\frac{1}{n}\sum_{k=1}^{n}X_k-\mu|<\varepsilon)=1
" class="ee_img tr_noresize" eeimg="1">
它不要求方差的存在，但要求同分布。

* [ ] **同分布，数学期望与方差不是相等的吗？**

### 伯努利大数定律：

在伯努利概型中（n次独立重复试验，k为事件A发生的次数，每次试验A发生的概率为p），有：

<img src="https://www.zhihu.com/equation?tex=\forall\varepsilon>0,\lim_{n\rightarrow\infin}P(|\frac{k_n}{n}-p|<\varepsilon)=1
" alt="\forall\varepsilon>0,\lim_{n\rightarrow\infin}P(|\frac{k_n}{n}-p|<\varepsilon)=1
" class="ee_img tr_noresize" eeimg="1">
伯努利大数定律从理论上说明任一随机事件的**频率具有稳定性**。

因此可以在大量试验后，将发生的频率近似作为概率。



## 中心极限定理

很多独立随机变量的极限分布是**正态分布**。

### 列维-林德伯格中心极限定理：

设 <img src="https://www.zhihu.com/equation?tex=X_1,X_2,...,X_n,..." alt="X_1,X_2,...,X_n,..." class="ee_img tr_noresize" eeimg="1"> 是**独立同分布**的随机变量： <img src="https://www.zhihu.com/equation?tex=E[X_k]\equiv \mu,D(X_k)\equiv\sigma^2" alt="E[X_k]\equiv \mu,D(X_k)\equiv\sigma^2" class="ee_img tr_noresize" eeimg="1"> ，则有：

<img src="https://www.zhihu.com/equation?tex=\forall x,\lim_{n\rightarrow\infin}P(\frac{\sum_{i=1}^nX_k-n\mu}{\sigma\sqrt{n}}\leq x)=\Phi(x)
" alt="\forall x,\lim_{n\rightarrow\infin}P(\frac{\sum_{i=1}^nX_k-n\mu}{\sigma\sqrt{n}}\leq x)=\Phi(x)
" class="ee_img tr_noresize" eeimg="1">
即独立同分布的随机变量之和 <img src="https://www.zhihu.com/equation?tex=\sum_{i=1}^nX_k" alt="\sum_{i=1}^nX_k" class="ee_img tr_noresize" eeimg="1"> 近似于正态分布 <img src="https://www.zhihu.com/equation?tex=N(n\mu,n\sigma^2)" alt="N(n\mu,n\sigma^2)" class="ee_img tr_noresize" eeimg="1"> 。所以 <img src="https://www.zhihu.com/equation?tex=\frac{\bar{X}-\mu}{\sigma/\sqrt{n}}" alt="\frac{\bar{X}-\mu}{\sigma/\sqrt{n}}" class="ee_img tr_noresize" eeimg="1"> 近似服从 <img src="https://www.zhihu.com/equation?tex=N(0,1)" alt="N(0,1)" class="ee_img tr_noresize" eeimg="1"> 。

### 蒂莫夫-拉普拉斯中心极限定理：

设 <img src="https://www.zhihu.com/equation?tex=Y_n" alt="Y_n" class="ee_img tr_noresize" eeimg="1"> 服从**二项分布** <img src="https://www.zhihu.com/equation?tex=B(n,p)" alt="B(n,p)" class="ee_img tr_noresize" eeimg="1"> ，则有：

<img src="https://www.zhihu.com/equation?tex=\forall x,\lim_{n\rightarrow\infin}P(\frac{Y_n-np}{\sqrt{np(1-p)}}\leq x)=\Phi(x)
" alt="\forall x,\lim_{n\rightarrow\infin}P(\frac{Y_n-np}{\sqrt{np(1-p)}}\leq x)=\Phi(x)
" class="ee_img tr_noresize" eeimg="1">
即**n充分大**时，二项分布近似于服从 <img src="https://www.zhihu.com/equation?tex=N(np,np(1-p))" alt="N(np,np(1-p))" class="ee_img tr_noresize" eeimg="1"> 。

标准化后，查表得出对应的边界，然后恢复原形。

#### 对二项分布的估计

* 用泊松分布估计：
  *  <img src="https://www.zhihu.com/equation?tex=np\rightarrow \lambda" alt="np\rightarrow \lambda" class="ee_img tr_noresize" eeimg="1"> ，此时的 <img src="https://www.zhihu.com/equation?tex=p" alt="p" class="ee_img tr_noresize" eeimg="1"> 可以是变化量， <img src="https://www.zhihu.com/equation?tex=\lambda" alt="\lambda" class="ee_img tr_noresize" eeimg="1"> 较小。
  * 常常用来估计单点的正态分布，当然也可以求出范围。
* 用正态分布估计：
  * 不对 <img src="https://www.zhihu.com/equation?tex=p" alt="p" class="ee_img tr_noresize" eeimg="1"> 加以限制，但是要求 <img src="https://www.zhihu.com/equation?tex=n\rightarrow\infin" alt="n\rightarrow\infin" class="ee_img tr_noresize" eeimg="1"> ， <img src="https://www.zhihu.com/equation?tex=np" alt="np" class="ee_img tr_noresize" eeimg="1"> 可能很大。
  * 这里的用连续的随机变量估计离散的随机变量。
  * 不能计算出单点的概率，只能求范围。

### 不同分布的中心极限定理（考不考？不做考察 ）

设 <img src="https://www.zhihu.com/equation?tex=X_1,...,X_n,..." alt="X_1,...,X_n,..." class="ee_img tr_noresize" eeimg="1"> 是独立不同分布的随机变量， <img src="https://www.zhihu.com/equation?tex=D(X_i)=\sigma_i^2" alt="D(X_i)=\sigma_i^2" class="ee_img tr_noresize" eeimg="1"> 。若：

<img src="https://www.zhihu.com/equation?tex=\begin{cases}\lim_{n\rightarrow\infin}\sum_{i=1}^n\sigma_i^2=\infin\\\lim_{n\rightarrow\infin}\frac{max(\sigma_i^2)}{n}=0\end{cases}
" alt="\begin{cases}\lim_{n\rightarrow\infin}\sum_{i=1}^n\sigma_i^2=\infin\\\lim_{n\rightarrow\infin}\frac{max(\sigma_i^2)}{n}=0\end{cases}
" class="ee_img tr_noresize" eeimg="1">
则：

<img src="https://www.zhihu.com/equation?tex=Y=\lim_{n\rightarrow\infin}\frac{\sum_{i=1}^nX_i}{n}
" alt="Y=\lim_{n\rightarrow\infin}\frac{\sum_{i=1}^nX_i}{n}
" class="ee_img tr_noresize" eeimg="1">
服从正态分布。

它表示，由**足够多**的随机变量，但每个随机变量又**不起决定性作用**，他们的**平均随机变量服从正态分布**。

# 数理统计基本知识

## 总体与样本

* 所有成员数量指标的全体称为**总体**
* 每个成员的数量指标称为**个体**
* 请注意：这里的数量指标并非具体特性，也就是待观测的。

* 从整体中抽取的**待测**的个体组成的集合称为**样本**。（样本由若干个体组成，组成样本空间）
* 样本中的个体总数是**样本容量**。

### 简单随机样本

需要满足：

* 独立性： <img src="https://www.zhihu.com/equation?tex=X_1,...,X_n" alt="X_1,...,X_n" class="ee_img tr_noresize" eeimg="1"> 是相互独立的随机变量。
* 代表性： <img src="https://www.zhihu.com/equation?tex=X_1,...,X_n" alt="X_1,...,X_n" class="ee_img tr_noresize" eeimg="1"> 要与总体 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 有相同的分布。

>设 <img src="https://www.zhihu.com/equation?tex=X_1,...,X_n" alt="X_1,...,X_n" class="ee_img tr_noresize" eeimg="1"> 为来自总体 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 的简单随机样本，则有：
>
>*  <img src="https://www.zhihu.com/equation?tex=X_1,...,X_n" alt="X_1,...,X_n" class="ee_img tr_noresize" eeimg="1"> 的联合分布函数为： <img src="https://www.zhihu.com/equation?tex=F_{X_1,...,X_n}(x_1,...,x_n)=\prod_{i=1}^n F(x_i)" alt="F_{X_1,...,X_n}(x_1,...,x_n)=\prod_{i=1}^n F(x_i)" class="ee_img tr_noresize" eeimg="1"> ，其中 <img src="https://www.zhihu.com/equation?tex=F(x)" alt="F(x)" class="ee_img tr_noresize" eeimg="1"> 是总体 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 的分布函数。
>*  <img src="https://www.zhihu.com/equation?tex=E[X_i]\equiv E[X],D(X_i)\equiv D(X)" alt="E[X_i]\equiv E[X],D(X_i)\equiv D(X)" class="ee_img tr_noresize" eeimg="1"> 。

## 统计量

### 定义

不含任何**未知参数**（这里的未知参数是指的总体的参数），只关于样本的**实值函数**称为样本的一个统计量。

* 统计量依旧是随机变量

### 常用统计量

* 均值： <img src="https://www.zhihu.com/equation?tex=\bar{X}=\sum_{i=1}^nX_i" alt="\bar{X}=\sum_{i=1}^nX_i" class="ee_img tr_noresize" eeimg="1"> 
* 样本方差： <img src="https://www.zhihu.com/equation?tex=S^2=\frac{1}{n-1}\sum_{i=1}^n(X_i-\bar{X})^2=\frac{1}{n-1}(\sum_{i=1}^nX_i^2-n\bar{X})" alt="S^2=\frac{1}{n-1}\sum_{i=1}^n(X_i-\bar{X})^2=\frac{1}{n-1}(\sum_{i=1}^nX_i^2-n\bar{X})" class="ee_img tr_noresize" eeimg="1"> 
  * 这里为什么是除以 <img src="https://www.zhihu.com/equation?tex=n-1" alt="n-1" class="ee_img tr_noresize" eeimg="1"> 呢，是因为要保证标准差的无偏性，在后面“估计量的优劣评价”中会提到。

* 样本标准差： <img src="https://www.zhihu.com/equation?tex=S=\sqrt{S^2}" alt="S=\sqrt{S^2}" class="ee_img tr_noresize" eeimg="1"> 
* 样本k阶原点矩： <img src="https://www.zhihu.com/equation?tex=A_k=\frac{1}{n}\sum_{i=1}^nX_i^k" alt="A_k=\frac{1}{n}\sum_{i=1}^nX_i^k" class="ee_img tr_noresize" eeimg="1"> 
* 样本k阶中心矩： <img src="https://www.zhihu.com/equation?tex=B_k=\frac{1}{n}\sum_{i=1}^n(X_i-\bar{X})^2" alt="B_k=\frac{1}{n}\sum_{i=1}^n(X_i-\bar{X})^2" class="ee_img tr_noresize" eeimg="1"> 

### 顺序统计量

最小、最大统计量 <img src="https://www.zhihu.com/equation?tex=max(X_1,...,X_n),min(X_1,...,X_n)" alt="max(X_1,...,X_n),min(X_1,...,X_n)" class="ee_img tr_noresize" eeimg="1"> 



### 二维统计量

* 协方差： <img src="https://www.zhihu.com/equation?tex=S_{XY}^2=\frac{1}{n-1}\sum_{i=1}^n（X_i-\bar{X})(Y_i-\bar{Y})" alt="S_{XY}^2=\frac{1}{n-1}\sum_{i=1}^n（X_i-\bar{X})(Y_i-\bar{Y})" class="ee_img tr_noresize" eeimg="1"> 
* 样本相关系数： <img src="https://www.zhihu.com/equation?tex=\rho_{XY} = \frac{S_{XY}^2}{S_X S_Y}" alt="\rho_{XY} = \frac{S_{XY}^2}{S_X S_Y}" class="ee_img tr_noresize" eeimg="1"> 

## 三大分布(如何书写他们的分布函数：不需要)

###  <img src="https://www.zhihu.com/equation?tex=\chi^2" alt="\chi^2" class="ee_img tr_noresize" eeimg="1"> 分布（需要记住密度函数吗？不需要）

设随机变量 <img src="https://www.zhihu.com/equation?tex=X_1,...,X_n" alt="X_1,...,X_n" class="ee_img tr_noresize" eeimg="1"> 独立且都服从标准正态分布，则：

<img src="https://www.zhihu.com/equation?tex=\chi^2=X_1^2+...+X_n^2\\
f_{\chi^2}(x)=\begin{cases}\frac{1}{2^{n/2}\Gamma(n/2)}x^{\frac{n}{2}-1}e^{-n/2}&x>0\\0&x\leq 0\end{cases}
" alt="\chi^2=X_1^2+...+X_n^2\\
f_{\chi^2}(x)=\begin{cases}\frac{1}{2^{n/2}\Gamma(n/2)}x^{\frac{n}{2}-1}e^{-n/2}&x>0\\0&x\leq 0\end{cases}
" class="ee_img tr_noresize" eeimg="1">


*  <img src="https://www.zhihu.com/equation?tex=E[\chi^2(n)]=n,D[\chi^n(n)]=2n" alt="E[\chi^2(n)]=n,D[\chi^n(n)]=2n" class="ee_img tr_noresize" eeimg="1"> 。

* 可加性： <img src="https://www.zhihu.com/equation?tex=\chi^2(m)+\chi^2(n)=\chi^2(m+n)" alt="\chi^2(m)+\chi^2(n)=\chi^2(m+n)" class="ee_img tr_noresize" eeimg="1"> 。

### t分布（学生分布）

设随机变量 <img src="https://www.zhihu.com/equation?tex=X,Y" alt="X,Y" class="ee_img tr_noresize" eeimg="1"> 相互独立，且 <img src="https://www.zhihu.com/equation?tex=X\sim N(0,1),Y\sim\chi^2(n)" alt="X\sim N(0,1),Y\sim\chi^2(n)" class="ee_img tr_noresize" eeimg="1"> ，则：

<img src="https://www.zhihu.com/equation?tex=t=\frac{X}{\sqrt{Y/n}}\\
f_t(x)=\frac{\Gamma[(n+1)/2]}{\sqrt{n\pi}\Gamma(n/2)}(1+\frac{x^2}{n})^{-\frac{n+1}{2}}
" alt="t=\frac{X}{\sqrt{Y/n}}\\
f_t(x)=\frac{\Gamma[(n+1)/2]}{\sqrt{n\pi}\Gamma(n/2)}(1+\frac{x^2}{n})^{-\frac{n+1}{2}}
" class="ee_img tr_noresize" eeimg="1">

*  <img src="https://www.zhihu.com/equation?tex=E[t(n)]=0(n>1),D[t(n)]=\frac{n}{n-2}(n>2)" alt="E[t(n)]=0(n>1),D[t(n)]=\frac{n}{n-2}(n>2)" class="ee_img tr_noresize" eeimg="1"> 。

* 当 <img src="https://www.zhihu.com/equation?tex=n\geq 30" alt="n\geq 30" class="ee_img tr_noresize" eeimg="1"> 时，已经可以将t分布近似看成标准正态分布。

### F分布（需要记住这些期望吗？）F

设随机变量 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 和 <img src="https://www.zhihu.com/equation?tex=Y" alt="Y" class="ee_img tr_noresize" eeimg="1"> 相互独立，且 <img src="https://www.zhihu.com/equation?tex=X\sim\chi^2(m),Y\sim\chi^2(n)" alt="X\sim\chi^2(m),Y\sim\chi^2(n)" class="ee_img tr_noresize" eeimg="1"> ，则：

<img src="https://www.zhihu.com/equation?tex=F=\frac{X/m}{Y/n}\\
" alt="F=\frac{X/m}{Y/n}\\
" class="ee_img tr_noresize" eeimg="1">

*  <img src="https://www.zhihu.com/equation?tex=E[F(m,n)]=\frac{n}{n-2},D[F(m,n)]=\frac{2n^2(m+n-2)}{m(n-2)^2(n-4)}" alt="E[F(m,n)]=\frac{n}{n-2},D[F(m,n)]=\frac{2n^2(m+n-2)}{m(n-2)^2(n-4)}" class="ee_img tr_noresize" eeimg="1"> ，

* 倒数： <img src="https://www.zhihu.com/equation?tex=F\sim F(m,n)\Rightarrow\frac{1}{F}\sim F(n,m)" alt="F\sim F(m,n)\Rightarrow\frac{1}{F}\sim F(n,m)" class="ee_img tr_noresize" eeimg="1"> 

----

### 上分位数点（规范大小写，第三个需要记忆吗？）

随机变量 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 的分布函数为 <img src="https://www.zhihu.com/equation?tex=F(x)" alt="F(x)" class="ee_img tr_noresize" eeimg="1"> ，满足等式：

<img src="https://www.zhihu.com/equation?tex=P(X>x_\alpha)=1-F(x_\alpha)=\alpha
" alt="P(X>x_\alpha)=1-F(x_\alpha)=\alpha
" class="ee_img tr_noresize" eeimg="1">
则 <img src="https://www.zhihu.com/equation?tex=x_\alpha" alt="x_\alpha" class="ee_img tr_noresize" eeimg="1"> 称为X的上 <img src="https://www.zhihu.com/equation?tex=\alpha" alt="\alpha" class="ee_img tr_noresize" eeimg="1"> 分位点。



* 注意⚠️：这里的上分位数点，指的是随机变量的一个取值（x轴上的数）。

* 正态分布的上分位点记为 <img src="https://www.zhihu.com/equation?tex=u_\alpha" alt="u_\alpha" class="ee_img tr_noresize" eeimg="1"> 。

*  <img src="https://www.zhihu.com/equation?tex=n\geq 40" alt="n\geq 40" class="ee_img tr_noresize" eeimg="1"> 时， <img src="https://www.zhihu.com/equation?tex=\chi^2_\alpha(n)\approx\frac{1}{2}(u_\alpha+\sqrt{2n-1})^2" alt="\chi^2_\alpha(n)\approx\frac{1}{2}(u_\alpha+\sqrt{2n-1})^2" class="ee_img tr_noresize" eeimg="1"> （需要记吗？）

* 由t分布的对称性，有 <img src="https://www.zhihu.com/equation?tex=t_{1-\alpha}(n)=-t_\alpha(n)" alt="t_{1-\alpha}(n)=-t_\alpha(n)" class="ee_img tr_noresize" eeimg="1"> 

* 当 <img src="https://www.zhihu.com/equation?tex=n\geq 30" alt="n\geq 30" class="ee_img tr_noresize" eeimg="1"> 时， <img src="https://www.zhihu.com/equation?tex=t_\alpha(n)\approx u_\alpha" alt="t_\alpha(n)\approx u_\alpha" class="ee_img tr_noresize" eeimg="1"> 

*  <img src="https://www.zhihu.com/equation?tex=F_{1-\alpha}(m,n)=\frac{1}{F_\alpha(n,m)}" alt="F_{1-\alpha}(m,n)=\frac{1}{F_\alpha(n,m)}" class="ee_img tr_noresize" eeimg="1"> （为什么？）

<img src="https://www.zhihu.com/equation?tex=\begin{aligned}
  &\text{性质 }F_{1-\alpha}(n_1,n_2)=\frac1{F_\alpha(n_2,n_1)}\text{ 的推导过程。} \\
  &1-\alpha  =P\{F>F_{1-\boldsymbol{\alpha}}(n_1,n_2)\}  \\
  &=P\{\frac1F<\frac1{F_{1-\alpha}(n_1,n_2)}\} \\
  &=1-P\{\frac1F\geq\frac1{F_{1-\alpha}(n_1,n_2)}\} \\
  &=1-P\{\frac1F>\frac1{F_{1-\alpha}(n_1,n_2)}\} \\
  &\text{则}P\{\frac{1}{F}>\frac{1}{F_{1-\alpha}(n_{1},n_{2})}\}=\alpha  \\
  &\operatorname{且}\frac{1}{F}\sim F(n_{2},n_{1}) \\
  &\text{那么 }P\{\frac1F>F_\alpha(n_2,n_1)\}=\alpha  \\
  &\text{得证。}
  \end{aligned}
  " alt="\begin{aligned}
  &\text{性质 }F_{1-\alpha}(n_1,n_2)=\frac1{F_\alpha(n_2,n_1)}\text{ 的推导过程。} \\
  &1-\alpha  =P\{F>F_{1-\boldsymbol{\alpha}}(n_1,n_2)\}  \\
  &=P\{\frac1F<\frac1{F_{1-\alpha}(n_1,n_2)}\} \\
  &=1-P\{\frac1F\geq\frac1{F_{1-\alpha}(n_1,n_2)}\} \\
  &=1-P\{\frac1F>\frac1{F_{1-\alpha}(n_1,n_2)}\} \\
  &\text{则}P\{\frac{1}{F}>\frac{1}{F_{1-\alpha}(n_{1},n_{2})}\}=\alpha  \\
  &\operatorname{且}\frac{1}{F}\sim F(n_{2},n_{1}) \\
  &\text{那么 }P\{\frac1F>F_\alpha(n_2,n_1)\}=\alpha  \\
  &\text{得证。}
  \end{aligned}
  " class="ee_img tr_noresize" eeimg="1">
  
* 以上函数，都是可以看作是**分布函数**的反函数。

* 需要记住的他们下分位数的计算方法：

  *  <img src="https://www.zhihu.com/equation?tex=\chi_{1-\alpha}(n)" alt="\chi_{1-\alpha}(n)" class="ee_img tr_noresize" eeimg="1"> 单独计算
  *  <img src="https://www.zhihu.com/equation?tex=u_{1-\alpha}=-u_{\alpha}" alt="u_{1-\alpha}=-u_{\alpha}" class="ee_img tr_noresize" eeimg="1"> 
  *  <img src="https://www.zhihu.com/equation?tex=t_{1-\alpha}=-t_\alpha" alt="t_{1-\alpha}=-t_\alpha" class="ee_img tr_noresize" eeimg="1"> 
  *  <img src="https://www.zhihu.com/equation?tex=F_{1-\alpha}(m,n)=\frac{1}{F_\alpha(n,m)}" alt="F_{1-\alpha}(m,n)=\frac{1}{F_\alpha(n,m)}" class="ee_img tr_noresize" eeimg="1"> 


### 顺序统计量的分布(需要记忆吗？)

设总体X具有分布函数 <img src="https://www.zhihu.com/equation?tex=F(x)" alt="F(x)" class="ee_img tr_noresize" eeimg="1"> ，其密度函数为 <img src="https://www.zhihu.com/equation?tex=f(x)" alt="f(x)" class="ee_img tr_noresize" eeimg="1"> 。则：

*  <img src="https://www.zhihu.com/equation?tex=X_{(1)}=min(X_1,...,X_n),f_{X_{(1)}}(x) = nf(x) [1-F(x)]^{ n-1 }" alt="X_{(1)}=min(X_1,...,X_n),f_{X_{(1)}}(x) = nf(x) [1-F(x)]^{ n-1 }" class="ee_img tr_noresize" eeimg="1"> 
*  <img src="https://www.zhihu.com/equation?tex=X_{(n)}=max(X_1,...,X_n),f_{X_{(n)}}(x) = nf(x)[F(x)]^{ n-1 }" alt="X_{(n)}=max(X_1,...,X_n),f_{X_{(n)}}(x) = nf(x)[F(x)]^{ n-1 }" class="ee_img tr_noresize" eeimg="1"> 
*  <img src="https://www.zhihu.com/equation?tex=f_{X_{(1)},X_{(n)}}(x,y)=n(n-1)f(x)f(y)[F(y)-F(x)]^{n-2}(x\leq y)" alt="f_{X_{(1)},X_{(n)}}(x,y)=n(n-1)f(x)f(y)[F(y)-F(x)]^{n-2}(x\leq y)" class="ee_img tr_noresize" eeimg="1"> 。
*  <img src="https://www.zhihu.com/equation?tex=f_{X_{(k)}}(x)=kC_n^kF(x)^{k-1}[1-F(x)]^{n-k}f(x)" alt="f_{X_{(k)}}(x)=kC_n^kF(x)^{k-1}[1-F(x)]^{n-k}f(x)" class="ee_img tr_noresize" eeimg="1"> （为什么？）

## ☆正态总体的抽样分布

设 <img src="https://www.zhihu.com/equation?tex=X_1,...,X_n" alt="X_1,...,X_n" class="ee_img tr_noresize" eeimg="1"> 是来自正态总体 <img src="https://www.zhihu.com/equation?tex=X\sim N(\mu,\sigma^2)" alt="X\sim N(\mu,\sigma^2)" class="ee_img tr_noresize" eeimg="1"> 的一组样本，则：

*  <img src="https://www.zhihu.com/equation?tex=\bar{X}\sim N(\mu,\frac{\sigma^2}{n})" alt="\bar{X}\sim N(\mu,\frac{\sigma^2}{n})" class="ee_img tr_noresize" eeimg="1"> 
*  <img src="https://www.zhihu.com/equation?tex=\frac{(n-1)S^2}{\sigma^2}\sim\chi^2(n-1)" alt="\frac{(n-1)S^2}{\sigma^2}\sim\chi^2(n-1)" class="ee_img tr_noresize" eeimg="1"> 
*  <img src="https://www.zhihu.com/equation?tex=\frac{\bar{X}-\mu}{S/\sqrt{n}}\sim t(n-1)" alt="\frac{\bar{X}-\mu}{S/\sqrt{n}}\sim t(n-1)" class="ee_img tr_noresize" eeimg="1"> 
*  <img src="https://www.zhihu.com/equation?tex=\bar{X}" alt="\bar{X}" class="ee_img tr_noresize" eeimg="1"> 与 <img src="https://www.zhihu.com/equation?tex=S^2" alt="S^2" class="ee_img tr_noresize" eeimg="1"> 相互独立

设 <img src="https://www.zhihu.com/equation?tex=X_1,...,X_n" alt="X_1,...,X_n" class="ee_img tr_noresize" eeimg="1"> 是来自正态总体 <img src="https://www.zhihu.com/equation?tex=X\sim N(\mu_1,\sigma_1^2)" alt="X\sim N(\mu_1,\sigma_1^2)" class="ee_img tr_noresize" eeimg="1"> 的一组样本，设 <img src="https://www.zhihu.com/equation?tex=Y_1,...,Y_n" alt="Y_1,...,Y_n" class="ee_img tr_noresize" eeimg="1"> 是来自正态总体 <img src="https://www.zhihu.com/equation?tex=Y\sim N(\mu_2,\sigma_2^2)" alt="Y\sim N(\mu_2,\sigma_2^2)" class="ee_img tr_noresize" eeimg="1"> 的一组样本，且两组样本间独立。则：

*  <img src="https://www.zhihu.com/equation?tex=\frac{S_X^2/\sigma_1^2}{S_Y^2/\sigma_2^2}\sim F(m-1,n-1)" alt="\frac{S_X^2/\sigma_1^2}{S_Y^2/\sigma_2^2}\sim F(m-1,n-1)" class="ee_img tr_noresize" eeimg="1"> 

* 当 <img src="https://www.zhihu.com/equation?tex=\sigma_1^2=\sigma_2^2=\sigma_3^2" alt="\sigma_1^2=\sigma_2^2=\sigma_3^2" class="ee_img tr_noresize" eeimg="1"> :

<img src="https://www.zhihu.com/equation?tex=\begin{aligned}\frac{(\overline{X}-\overline{Y})-(\mu_1-\mu_2)}{S_W\sqrt{1/m+1/n}}&\sim t(m+n-2).\\\text{其中}\quad S_W^2&=\frac{(m-1)S_X^2+(n-1)S_Y^2}{m+n-2}.\end{aligned}
  " alt="\begin{aligned}\frac{(\overline{X}-\overline{Y})-(\mu_1-\mu_2)}{S_W\sqrt{1/m+1/n}}&\sim t(m+n-2).\\\text{其中}\quad S_W^2&=\frac{(m-1)S_X^2+(n-1)S_Y^2}{m+n-2}.\end{aligned}
  " class="ee_img tr_noresize" eeimg="1">
  

# 参数估计

## 参数的点估计

>参数估计是根据**样本**对总体未知参数（如均值，方差）等进行估计的一种统计推断方法。

* 参数点估计：构造一个<u>统计量</u> <img src="https://www.zhihu.com/equation?tex=\hat{\theta}=\hat{\theta}(X_1,...,X_n)" alt="\hat{\theta}=\hat{\theta}(X_1,...,X_n)" class="ee_img tr_noresize" eeimg="1"> ，直接用 <img src="https://www.zhihu.com/equation?tex=\hat{\theta}" alt="\hat{\theta}" class="ee_img tr_noresize" eeimg="1"> 作为 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> 的估计值。

### 矩估计

* 矩估计法是用**样本的k阶原点矩**作为总体的**k阶原点矩 <img src="https://www.zhihu.com/equation?tex=E[X^k]" alt="E[X^k]" class="ee_img tr_noresize" eeimg="1"> **的估计。

考虑要估计的参数是 <img src="https://www.zhihu.com/equation?tex=\theta_1,...,\theta_m" alt="\theta_1,...,\theta_m" class="ee_img tr_noresize" eeimg="1"> ，于是可以列出方程组：

<img src="https://www.zhihu.com/equation?tex=\begin{cases}E[X]=f_1(\theta_1,...,\theta_m)=\frac{1}{n}\sum_{i=1}^n X_i\\
E[X^2]=f_2(\theta_1,...,\theta_m)=\frac{1}{n}\sum_{i = 1}^n X_i^2\\
...\\
E[X^m]=f_m(\theta_1,...,\theta_m)=\frac{1}{n}\sum_{i=1}^n X_i^m
\end{cases}
" alt="\begin{cases}E[X]=f_1(\theta_1,...,\theta_m)=\frac{1}{n}\sum_{i=1}^n X_i\\
E[X^2]=f_2(\theta_1,...,\theta_m)=\frac{1}{n}\sum_{i = 1}^n X_i^2\\
...\\
E[X^m]=f_m(\theta_1,...,\theta_m)=\frac{1}{n}\sum_{i=1}^n X_i^m
\end{cases}
" class="ee_img tr_noresize" eeimg="1">
然后可以解方程组得到一组解 <img src="https://www.zhihu.com/equation?tex=(\hat{\theta_1},...,\hat{\theta_m})" alt="(\hat{\theta_1},...,\hat{\theta_m})" class="ee_img tr_noresize" eeimg="1"> ，就可以作为参数 <img src="https://www.zhihu.com/equation?tex=(\theta_1,...,\theta_m)" alt="(\theta_1,...,\theta_m)" class="ee_img tr_noresize" eeimg="1"> 的估计。

根据大数定律，有：

<img src="https://www.zhihu.com/equation?tex=\forall\varepsilon>0,\lim_{n\rightarrow\infin}P(|\frac{1}{n}\sum_{i=1}^nX_i^m-E[X^m]|<\varepsilon)=1
" alt="\forall\varepsilon>0,\lim_{n\rightarrow\infin}P(|\frac{1}{n}\sum_{i=1}^nX_i^m-E[X^m]|<\varepsilon)=1
" class="ee_img tr_noresize" eeimg="1">
所以样本的k阶原点矩就是总体的k阶原点矩的一个合理估计。

>[例]：已知总体X的一组样本 <img src="https://www.zhihu.com/equation?tex=X_1,X_2,...,X_n" alt="X_1,X_2,...,X_n" class="ee_img tr_noresize" eeimg="1"> ，试估计总体的方差和均值。（假设它们存在）

* 列出方程组：

<img src="https://www.zhihu.com/equation?tex=\begin{cases}\mu=E[X]=\frac{1}{n}\sum_{i=1}^n X_i=\bar{X}\\
  \mu^2+\sigma^2=E[X^2]=\frac{1}{n}\sum_{i=1}^n X_i^2
  \end{cases}
  " alt="\begin{cases}\mu=E[X]=\frac{1}{n}\sum_{i=1}^n X_i=\bar{X}\\
  \mu^2+\sigma^2=E[X^2]=\frac{1}{n}\sum_{i=1}^n X_i^2
  \end{cases}
  " class="ee_img tr_noresize" eeimg="1">
  解得：

<img src="https://www.zhihu.com/equation?tex=\hat{\mu}=\bar{X}\\
  \hat{\sigma^2}=\frac{1}{n}\sum_{i=1}^nX_i^2-\bar{X}^2=\frac{1}{n}\sum_{i=1}^n(X_i-\bar{X})^2=\frac{n-1}{n}S^2
  " alt="\hat{\mu}=\bar{X}\\
  \hat{\sigma^2}=\frac{1}{n}\sum_{i=1}^nX_i^2-\bar{X}^2=\frac{1}{n}\sum_{i=1}^n(X_i-\bar{X})^2=\frac{n-1}{n}S^2
  " class="ee_img tr_noresize" eeimg="1">

* 从例题中，可以看到，估计实际上就是把总体的参数用以样本为自变量的函数来表示，当我们获得了一组样本值时，我们就可以对总体进行合理猜测，这就是统计，用获得的一部分数据去估计整体。

### 最大似然估计

考虑我们有一组样本值 <img src="https://www.zhihu.com/equation?tex=x_1,...,x_n" alt="x_1,...,x_n" class="ee_img tr_noresize" eeimg="1"> ，于是事件 <img src="https://www.zhihu.com/equation?tex=A=\{X_1=x_1,...,X_n=x_n\}" alt="A=\{X_1=x_1,...,X_n=x_n\}" class="ee_img tr_noresize" eeimg="1"> 发生的概率是一个关于参数 <img src="https://www.zhihu.com/equation?tex=\theta=(\theta_1,...,\theta_m)" alt="\theta=(\theta_1,...,\theta_m)" class="ee_img tr_noresize" eeimg="1"> 的函数 <img src="https://www.zhihu.com/equation?tex=L(\theta)" alt="L(\theta)" class="ee_img tr_noresize" eeimg="1"> 。我们希望取得 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> 的一个最大似然估计 <img src="https://www.zhihu.com/equation?tex=\hat{\theta}" alt="\hat{\theta}" class="ee_img tr_noresize" eeimg="1"> ，此时 <img src="https://www.zhihu.com/equation?tex=L(\hat{\theta})" alt="L(\hat{\theta})" class="ee_img tr_noresize" eeimg="1"> 取得最大值。

*  <img src="https://www.zhihu.com/equation?tex=L(\theta)" alt="L(\theta)" class="ee_img tr_noresize" eeimg="1"> 的确定：

  * 若总体是离散型的，则显然： <img src="https://www.zhihu.com/equation?tex=P(X_1=x_1,...,X_n=x_n)=\prod_{i=1}^nP(X_i=x_i)" alt="P(X_1=x_1,...,X_n=x_n)=\prod_{i=1}^nP(X_i=x_i)" class="ee_img tr_noresize" eeimg="1"> ，而 <img src="https://www.zhihu.com/equation?tex=P(X_i=x_i)" alt="P(X_i=x_i)" class="ee_img tr_noresize" eeimg="1"> 是关于 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> 的函数。
  * 若总体是连续型的，则要求 <img src="https://www.zhihu.com/equation?tex=L(\theta)=\prod_{i=1}^n \int_{x_i}^{x_i+dx_i}f(t)dt\approx\prod_{i=1}^nf(x_i)dx_i(dx_i\rightarrow 0)" alt="L(\theta)=\prod_{i=1}^n \int_{x_i}^{x_i+dx_i}f(t)dt\approx\prod_{i=1}^nf(x_i)dx_i(dx_i\rightarrow 0)" class="ee_img tr_noresize" eeimg="1"> ， <img src="https://www.zhihu.com/equation?tex=f(x)" alt="f(x)" class="ee_img tr_noresize" eeimg="1"> 是概率密度函数。

*  <img src="https://www.zhihu.com/equation?tex=\hat{\theta}" alt="\hat{\theta}" class="ee_img tr_noresize" eeimg="1"> 的确定：

  * 因为我们不关心 <img src="https://www.zhihu.com/equation?tex=L(\theta)" alt="L(\theta)" class="ee_img tr_noresize" eeimg="1"> 的最大值，而只关心取得最大值时 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> 的值。于是我们可以对 <img src="https://www.zhihu.com/equation?tex=L(\theta)" alt="L(\theta)" class="ee_img tr_noresize" eeimg="1"> 取自然对数再求导（不影响极值点），这也可以证明：

<img src="https://www.zhihu.com/equation?tex=lnL(\theta)=ln(\prod_{i=1}^nf(x_i)dx_i)=\sum_{i=1}^nln(f(x_i))+\sum_{i=1}^nln(dx_i)\\
    \frac{\partial lnL(\theta)}{\partial\theta}=\sum_{i=1}^n\frac{\partial ln(f(x_i))}{\partial\theta}
    " alt="lnL(\theta)=ln(\prod_{i=1}^nf(x_i)dx_i)=\sum_{i=1}^nln(f(x_i))+\sum_{i=1}^nln(dx_i)\\
    \frac{\partial lnL(\theta)}{\partial\theta}=\sum_{i=1}^n\frac{\partial ln(f(x_i))}{\partial\theta}
    " class="ee_img tr_noresize" eeimg="1">
    因为 <img src="https://www.zhihu.com/equation?tex=dx_i" alt="dx_i" class="ee_img tr_noresize" eeimg="1"> 与 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> 无关，因此连续型的最大似然估计也可以直接选为 <img src="https://www.zhihu.com/equation?tex=L(\theta)=\prod_{i=1}^nf(x_i)" alt="L(\theta)=\prod_{i=1}^nf(x_i)" class="ee_img tr_noresize" eeimg="1"> 。

>设 <img src="https://www.zhihu.com/equation?tex=X\sim N(\mu,\sigma^2)" alt="X\sim N(\mu,\sigma^2)" class="ee_img tr_noresize" eeimg="1"> ，已知 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 的一组样本观测值 <img src="https://www.zhihu.com/equation?tex=x_1,...,x_n" alt="x_1,...,x_n" class="ee_img tr_noresize" eeimg="1"> ，求 <img src="https://www.zhihu.com/equation?tex=\mu,\sigma^2" alt="\mu,\sigma^2" class="ee_img tr_noresize" eeimg="1"> 的最大似然估计。


<img src="https://www.zhihu.com/equation?tex=L(\mu,\sigma^2)=\prod_{i=1}^nf(x_i)=\prod_{i=1}^n\frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{(x_i-\mu)^2}{2\sigma^2}}\\
lnL(\mu,\sigma^2)=-\frac{n}{2}ln(2\pi)-\frac{n}{2}ln\sigma^2-\frac{1}{2\sigma^2}\sum_{i=1}^n(x_i-\mu)^2\\
\begin{cases}\frac{\partial lnL(\mu,\sigma^2)}{\partial\mu}=0\\
\frac{\partial lnL(\mu,\sigma^2)}{\partial\sigma^2}=0
\end{cases}
\Rightarrow \hat{\mu}=\bar{x},\hat{\sigma^2}=\frac{n-1}{n}s^2
" alt="L(\mu,\sigma^2)=\prod_{i=1}^nf(x_i)=\prod_{i=1}^n\frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{(x_i-\mu)^2}{2\sigma^2}}\\
lnL(\mu,\sigma^2)=-\frac{n}{2}ln(2\pi)-\frac{n}{2}ln\sigma^2-\frac{1}{2\sigma^2}\sum_{i=1}^n(x_i-\mu)^2\\
\begin{cases}\frac{\partial lnL(\mu,\sigma^2)}{\partial\mu}=0\\
\frac{\partial lnL(\mu,\sigma^2)}{\partial\sigma^2}=0
\end{cases}
\Rightarrow \hat{\mu}=\bar{x},\hat{\sigma^2}=\frac{n-1}{n}s^2
" class="ee_img tr_noresize" eeimg="1">

* 注意严格来说，最大似然估计是要知道样本的观测值的，当然也可以设成字母表示 <img src="https://www.zhihu.com/equation?tex=a_1,...,a_n" alt="a_1,...,a_n" class="ee_img tr_noresize" eeimg="1"> 。但用 <img src="https://www.zhihu.com/equation?tex=X_1,...,X_n" alt="X_1,...,X_n" class="ee_img tr_noresize" eeimg="1"> 来表示是不合理的。

### 估计量优劣的评价标准

>通常用**均方误差** <img src="https://www.zhihu.com/equation?tex=MSE(\hat{\theta})=E[(\theta-\hat{\theta})^2]" alt="MSE(\hat{\theta})=E[(\theta-\hat{\theta})^2]" class="ee_img tr_noresize" eeimg="1"> 来评价估计量的偏离程度。


<img src="https://www.zhihu.com/equation?tex=MSE(\hat{\theta})=E[[(\hat{\theta}-E[\hat{\theta}])+(E[\hat{\theta}]-\theta)]^2]\\
  =E[(\hat{\theta}-E[\hat{\theta}])^2]+2(E[\hat{\theta}]-\theta)E[\hat{\theta}-E[\hat{\theta}]]+E[(E[\hat{\theta}]-\theta)^2]\\
  =E[(\hat{\theta}-E[\hat{\theta}])^2]+(E[\hat{\theta}]-\theta)^2\\
  =D(\hat{\theta})+(E[\hat{\theta}]-\theta)^2
  " alt="MSE(\hat{\theta})=E[[(\hat{\theta}-E[\hat{\theta}])+(E[\hat{\theta}]-\theta)]^2]\\
  =E[(\hat{\theta}-E[\hat{\theta}])^2]+2(E[\hat{\theta}]-\theta)E[\hat{\theta}-E[\hat{\theta}]]+E[(E[\hat{\theta}]-\theta)^2]\\
  =E[(\hat{\theta}-E[\hat{\theta}])^2]+(E[\hat{\theta}]-\theta)^2\\
  =D(\hat{\theta})+(E[\hat{\theta}]-\theta)^2
  " class="ee_img tr_noresize" eeimg="1">

  其中，中间项为0是因为 <img src="https://www.zhihu.com/equation?tex=E[\hat{\theta}-E[\hat{\theta}]]=E[\hat{\theta}]-E[\hat{\theta}]=0" alt="E[\hat{\theta}-E[\hat{\theta}]]=E[\hat{\theta}]-E[\hat{\theta}]=0" class="ee_img tr_noresize" eeimg="1"> 。

  式子中将 <img src="https://www.zhihu.com/equation?tex=\hat{\theta}" alt="\hat{\theta}" class="ee_img tr_noresize" eeimg="1"> 作为随机变量，而把 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> 作为已知常量。我的理解是，先给出一组样本 <img src="https://www.zhihu.com/equation?tex=X_1,...,X_n" alt="X_1,...,X_n" class="ee_img tr_noresize" eeimg="1"> ，然后这些样本都是和总体同分布的随机变量，此时可以进行点估计： <img src="https://www.zhihu.com/equation?tex=\hat{\theta}=f(X_1,...,X_n)" alt="\hat{\theta}=f(X_1,...,X_n)" class="ee_img tr_noresize" eeimg="1"> ，所以可以对 <img src="https://www.zhihu.com/equation?tex=\hat{\theta}" alt="\hat{\theta}" class="ee_img tr_noresize" eeimg="1"> 取期望。然后假如已知了参数 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> ，此时我们可以 <img src="https://www.zhihu.com/equation?tex=\hat{\theta}" alt="\hat{\theta}" class="ee_img tr_noresize" eeimg="1"> 成了未知量，因为样本没有被观测。然后我们可以计算出 <img src="https://www.zhihu.com/equation?tex=\hat{\theta}" alt="\hat{\theta}" class="ee_img tr_noresize" eeimg="1"> 偏离已知的 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> 的距离的平方的期望。

* 当 <img src="https://www.zhihu.com/equation?tex=E[\hat{\theta}]-\theta=0" alt="E[\hat{\theta}]-\theta=0" class="ee_img tr_noresize" eeimg="1"> 时，即 <img src="https://www.zhihu.com/equation?tex=E[\hat{\theta}]=\theta" alt="E[\hat{\theta}]=\theta" class="ee_img tr_noresize" eeimg="1"> 时，我们称估计量是**无偏的**。这是好满足的。

* 但 <img src="https://www.zhihu.com/equation?tex=D(\hat{\theta})=0" alt="D(\hat{\theta})=0" class="ee_img tr_noresize" eeimg="1"> 是不可满足的，因为若 <img src="https://www.zhihu.com/equation?tex=\hat{\theta}" alt="\hat{\theta}" class="ee_img tr_noresize" eeimg="1"> 是一个常数而与样本无关了，那显然不太合理。通常我们在无偏的估计中，选择方差最小的，也就是最**有效的**，称为**最小无偏估计**。

>若 <img src="https://www.zhihu.com/equation?tex=E[\hat{\theta}]=\theta" alt="E[\hat{\theta}]=\theta" class="ee_img tr_noresize" eeimg="1"> ，则称 <img src="https://www.zhihu.com/equation?tex=\hat{\theta}" alt="\hat{\theta}" class="ee_img tr_noresize" eeimg="1"> 是 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> 的**无偏估计**，若 <img src="https://www.zhihu.com/equation?tex=\lim_{n\rightarrow\infin}E[\hat{\theta}]=\theta" alt="\lim_{n\rightarrow\infin}E[\hat{\theta}]=\theta" class="ee_img tr_noresize" eeimg="1"> ，则称 <img src="https://www.zhihu.com/equation?tex=\hat{\theta}" alt="\hat{\theta}" class="ee_img tr_noresize" eeimg="1"> 是 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> 的**渐进无偏估计**。否则就是有偏估计。

* 这里可以解释下之前留下的问题，为什么样本方差 <img src="https://www.zhihu.com/equation?tex=S^2" alt="S^2" class="ee_img tr_noresize" eeimg="1"> 中除以的是 <img src="https://www.zhihu.com/equation?tex=n-1" alt="n-1" class="ee_img tr_noresize" eeimg="1"> 。我们来证明： <img src="https://www.zhihu.com/equation?tex=E[S^2]=\sigma^2" alt="E[S^2]=\sigma^2" class="ee_img tr_noresize" eeimg="1"> ，即 <img src="https://www.zhihu.com/equation?tex=S^2" alt="S^2" class="ee_img tr_noresize" eeimg="1"> 是 <img src="https://www.zhihu.com/equation?tex=\sigma^2" alt="\sigma^2" class="ee_img tr_noresize" eeimg="1"> 的无偏估计。

<img src="https://www.zhihu.com/equation?tex=E[S^2]=\frac{1}{n-1}E[\sum_{i=1}^nX_i^2-2\bar{X}\sum_{i=1}^nX_i+\sum_{i=1}^n\bar{X}^2]\\
  =\frac{1}{n-1}E[\sum_{i=1}^nX_i^2-n\bar{X}^2]\\
  =\frac{1}{n-1}(\sum_{i=1}^nE[X_i^2]-nE[\bar{X}^2])\\
  =\frac{n}{n-1}(E[X^2]-E[\bar{X}^2])\\
  " alt="E[S^2]=\frac{1}{n-1}E[\sum_{i=1}^nX_i^2-2\bar{X}\sum_{i=1}^nX_i+\sum_{i=1}^n\bar{X}^2]\\
  =\frac{1}{n-1}E[\sum_{i=1}^nX_i^2-n\bar{X}^2]\\
  =\frac{1}{n-1}(\sum_{i=1}^nE[X_i^2]-nE[\bar{X}^2])\\
  =\frac{n}{n-1}(E[X^2]-E[\bar{X}^2])\\
  " class="ee_img tr_noresize" eeimg="1">
  而

<img src="https://www.zhihu.com/equation?tex=E[\bar{X}]=\mu,D[\bar{X}]=\frac{\sigma^2}{n}\Rightarrow E[\bar{X}^2]=\mu^2+\frac{\sigma^2}{n}\\
  E[X]=\mu,D[X]=\sigma^2\Rightarrow E[X^2]=\mu^2+\sigma^2\\
  \therefore E[S^2]=\frac{n}{n-1}(\mu^2+\sigma^2-\mu^2-\frac{\sigma^2}{n})=\sigma^2
  " alt="E[\bar{X}]=\mu,D[\bar{X}]=\frac{\sigma^2}{n}\Rightarrow E[\bar{X}^2]=\mu^2+\frac{\sigma^2}{n}\\
  E[X]=\mu,D[X]=\sigma^2\Rightarrow E[X^2]=\mu^2+\sigma^2\\
  \therefore E[S^2]=\frac{n}{n-1}(\mu^2+\sigma^2-\mu^2-\frac{\sigma^2}{n})=\sigma^2
  " class="ee_img tr_noresize" eeimg="1">
  因此 <img src="https://www.zhihu.com/equation?tex=S^2" alt="S^2" class="ee_img tr_noresize" eeimg="1"> 是 <img src="https://www.zhihu.com/equation?tex=\sigma^2" alt="\sigma^2" class="ee_img tr_noresize" eeimg="1"> 的一个无偏估计。

* 事实上，**样本均值和样本方差总是总体均值和总体方差的无偏估计**。

>若对任意的 <img src="https://www.zhihu.com/equation?tex=\varepsilon>0" alt="\varepsilon>0" class="ee_img tr_noresize" eeimg="1"> ，有 <img src="https://www.zhihu.com/equation?tex=\lim_{n\rightarrow \infin}P(|\theta-\hat{\theta_n}|\geq\varepsilon)=0" alt="\lim_{n\rightarrow \infin}P(|\theta-\hat{\theta_n}|\geq\varepsilon)=0" class="ee_img tr_noresize" eeimg="1"> ，则称 <img src="https://www.zhihu.com/equation?tex=\hat{\theta}(X_1,...,X_n)" alt="\hat{\theta}(X_1,...,X_n)" class="ee_img tr_noresize" eeimg="1"> 是 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> 的一个**相合（一致）估计**。

* 若 <img src="https://www.zhihu.com/equation?tex=\lim_{n\rightarrow\infin}E[\hat{\theta_n}]=\theta,\lim_{n\rightarrow\infin}D(\hat{\theta_n})=0" alt="\lim_{n\rightarrow\infin}E[\hat{\theta_n}]=\theta,\lim_{n\rightarrow\infin}D(\hat{\theta_n})=0" class="ee_img tr_noresize" eeimg="1"> ，则 <img src="https://www.zhihu.com/equation?tex=\hat{\theta}_n" alt="\hat{\theta}_n" class="ee_img tr_noresize" eeimg="1"> 是 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> 的一个**相合估计**。

## 参数的区间估计

>设 <img src="https://www.zhihu.com/equation?tex=\hat{\theta}_1,\hat{\theta}_2" alt="\hat{\theta}_1,\hat{\theta}_2" class="ee_img tr_noresize" eeimg="1"> 是两个统计量，若 <img src="https://www.zhihu.com/equation?tex=P(\hat{\theta}_1\leq \theta\leq\hat{\theta}_2)=1-\alpha" alt="P(\hat{\theta}_1\leq \theta\leq\hat{\theta}_2)=1-\alpha" class="ee_img tr_noresize" eeimg="1"> ，则称随即区间 <img src="https://www.zhihu.com/equation?tex=[\hat{\theta}_1,\hat{\theta}_2]" alt="[\hat{\theta}_1,\hat{\theta}_2]" class="ee_img tr_noresize" eeimg="1"> 是 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> 的一个区间估计或**置信区间**， <img src="https://www.zhihu.com/equation?tex=1-\alpha" alt="1-\alpha" class="ee_img tr_noresize" eeimg="1"> 称为置信水平或**置信度**。

* 一般来说，置信度越高，精确性（区间长度）越差（越长）。

求解置信区间的一般方法为：

* 找一个与要估计的参数 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> 有关的统计量 <img src="https://www.zhihu.com/equation?tex=T" alt="T" class="ee_img tr_noresize" eeimg="1"> ，一般是 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> 的一个良好的点估计 <img src="https://www.zhihu.com/equation?tex=\hat{\theta}" alt="\hat{\theta}" class="ee_img tr_noresize" eeimg="1"> 。
* 设法找出 <img src="https://www.zhihu.com/equation?tex=T" alt="T" class="ee_img tr_noresize" eeimg="1"> 和 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> 的某一函数 <img src="https://www.zhihu.com/equation?tex=H(T,\theta)" alt="H(T,\theta)" class="ee_img tr_noresize" eeimg="1"> ，要求H的分布已知且与 <img src="https://www.zhihu.com/equation?tex=T,\theta" alt="T,\theta" class="ee_img tr_noresize" eeimg="1"> 无关，称为**枢轴变量**。
* 寻找合适的常数 <img src="https://www.zhihu.com/equation?tex=c,d" alt="c,d" class="ee_img tr_noresize" eeimg="1"> 使得 <img src="https://www.zhihu.com/equation?tex=P(c\leq H\leq d)=1-\alpha" alt="P(c\leq H\leq d)=1-\alpha" class="ee_img tr_noresize" eeimg="1"> 。
* 将 <img src="https://www.zhihu.com/equation?tex=c\leq H\leq d" alt="c\leq H\leq d" class="ee_img tr_noresize" eeimg="1"> 等价变形为 <img src="https://www.zhihu.com/equation?tex=\hat{\theta}_1\leq\theta\leq\hat{\theta}_2" alt="\hat{\theta}_1\leq\theta\leq\hat{\theta}_2" class="ee_img tr_noresize" eeimg="1"> 。

正态分布的置信区间：

| 评估参数   | 条件           | 枢轴变量及其分布                                             | 置信区间                                                     |

| ---------- | -------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |

|  <img src="https://www.zhihu.com/equation?tex=\mu" alt="\mu" class="ee_img tr_noresize" eeimg="1">       |  <img src="https://www.zhihu.com/equation?tex=\sigma^2" alt="\sigma^2" class="ee_img tr_noresize" eeimg="1"> 已知 |  <img src="https://www.zhihu.com/equation?tex=\frac{\bar{X}-\mu}{\sigma/\sqrt{n}}\sim N(0,1)" alt="\frac{\bar{X}-\mu}{\sigma/\sqrt{n}}\sim N(0,1)" class="ee_img tr_noresize" eeimg="1">              |  <img src="https://www.zhihu.com/equation?tex=[\bar{X}-u_{\alpha/2}\frac{\sigma}{\sqrt{n}},\bar{X}+u_{\alpha/2}\frac{\sigma}{\sqrt{n}}]" alt="[\bar{X}-u_{\alpha/2}\frac{\sigma}{\sqrt{n}},\bar{X}+u_{\alpha/2}\frac{\sigma}{\sqrt{n}}]" class="ee_img tr_noresize" eeimg="1">  |

|  <img src="https://www.zhihu.com/equation?tex=\mu" alt="\mu" class="ee_img tr_noresize" eeimg="1">       |  <img src="https://www.zhihu.com/equation?tex=\sigma^2" alt="\sigma^2" class="ee_img tr_noresize" eeimg="1"> 未知 |  <img src="https://www.zhihu.com/equation?tex=\frac{\bar{X}-\mu}{S/\sqrt{n}}\sim t(n-1)" alt="\frac{\bar{X}-\mu}{S/\sqrt{n}}\sim t(n-1)" class="ee_img tr_noresize" eeimg="1">                   |  <img src="https://www.zhihu.com/equation?tex=[\bar{X}-t_{\alpha/2}(n-1)\frac{S}{\sqrt{n}},\bar{X}+t_{\alpha/2}(n-1)\frac{S}{\sqrt{n}}]" alt="[\bar{X}-t_{\alpha/2}(n-1)\frac{S}{\sqrt{n}},\bar{X}+t_{\alpha/2}(n-1)\frac{S}{\sqrt{n}}]" class="ee_img tr_noresize" eeimg="1">  |

|  <img src="https://www.zhihu.com/equation?tex=\sigma^2" alt="\sigma^2" class="ee_img tr_noresize" eeimg="1">  |  <img src="https://www.zhihu.com/equation?tex=\mu" alt="\mu" class="ee_img tr_noresize" eeimg="1"> 已知      |  <img src="https://www.zhihu.com/equation?tex=\frac{\sum_{i=1}^n(X_i-\mu)^2}{\sigma^2}\sim\chi^2(n)" alt="\frac{\sum_{i=1}^n(X_i-\mu)^2}{\sigma^2}\sim\chi^2(n)" class="ee_img tr_noresize" eeimg="1"> <br />（这个的证明由定义即可） |  <img src="https://www.zhihu.com/equation?tex=[\frac{\sum(X_i-\mu)^2}{\chi_{\alpha/2}^2(n)},\frac{\sum(X_i-\mu)^2}{\chi_{1-\alpha/2}^2(n)}]" alt="[\frac{\sum(X_i-\mu)^2}{\chi_{\alpha/2}^2(n)},\frac{\sum(X_i-\mu)^2}{\chi_{1-\alpha/2}^2(n)}]" class="ee_img tr_noresize" eeimg="1">  |

|  <img src="https://www.zhihu.com/equation?tex=\sigma^2" alt="\sigma^2" class="ee_img tr_noresize" eeimg="1">  |  <img src="https://www.zhihu.com/equation?tex=\mu" alt="\mu" class="ee_img tr_noresize" eeimg="1"> 未知      |  <img src="https://www.zhihu.com/equation?tex=\frac{(n-1)S^2}{\sigma^2}\sim\chi^2(n-1)" alt="\frac{(n-1)S^2}{\sigma^2}\sim\chi^2(n-1)" class="ee_img tr_noresize" eeimg="1">                    |  <img src="https://www.zhihu.com/equation?tex=[\frac{(n-1)S^2}{\chi_{\alpha/2}^2(n-1)},\frac{(n-1)S^2}{\chi_{1-\alpha/2}^2(n-1)}]" alt="[\frac{(n-1)S^2}{\chi_{\alpha/2}^2(n-1)},\frac{(n-1)S^2}{\chi_{1-\alpha/2}^2(n-1)}]" class="ee_img tr_noresize" eeimg="1">  |


# 假设检验

>只对总体的某些**未知参数**作出假设，通过**抽样**来判断假设是否成立，这种检验称为**参数检验**。
>
>只对未知分布函数的类型或者它的某些特性提出假设，然后对这种假设进行检验，被称为**非参数检验**。

参数检验的步骤——以对期望假设为例：

* 建立假设：

<img src="https://www.zhihu.com/equation?tex=H_0:\mu=5800,H_1:\mu\neq 5800
  " alt="H_0:\mu=5800,H_1:\mu\neq 5800
  " class="ee_img tr_noresize" eeimg="1">
   <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 称为**原假设**， <img src="https://www.zhihu.com/equation?tex=H_1" alt="H_1" class="ee_img tr_noresize" eeimg="1"> 称为**备择假设**。

* 选取检验统计量（不能含未知参数）：

  通过比较原假设成立时统计量的分布和备择假设成立时统计量的分布，得出对原假设**不利的事件**。若总体的方差已知，可以选择统计量：

<img src="https://www.zhihu.com/equation?tex=U=\frac{\bar{X}-5800}{\sigma/\sqrt{n}}
  " alt="U=\frac{\bar{X}-5800}{\sigma/\sqrt{n}}
  " class="ee_img tr_noresize" eeimg="1">
   <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 成立时， <img src="https://www.zhihu.com/equation?tex=U\sim N(0,1)" alt="U\sim N(0,1)" class="ee_img tr_noresize" eeimg="1"> ， <img src="https://www.zhihu.com/equation?tex=H_1" alt="H_1" class="ee_img tr_noresize" eeimg="1"> 成立时， <img src="https://www.zhihu.com/equation?tex=U\sim N(\frac{\mu-5800}{\sigma/\sqrt{n}},1)" alt="U\sim N(\frac{\mu-5800}{\sigma/\sqrt{n}},1)" class="ee_img tr_noresize" eeimg="1"> 。所以我们可以选择对 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 不利的事件为 <img src="https://www.zhihu.com/equation?tex=\{|U|>C\}" alt="\{|U|>C\}" class="ee_img tr_noresize" eeimg="1"> 。若事件发生了，我们便拒绝 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 。

* 选取检验显著性水平 <img src="https://www.zhihu.com/equation?tex=\alpha" alt="\alpha" class="ee_img tr_noresize" eeimg="1"> 与临界值，进而确定 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 的拒绝区域。

  在我们总是倾向于“保护“原假设的。于是我们默认在原假设成立的前提下，若对 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 不利的事件还是发生了，就拒绝原假设：

<img src="https://www.zhihu.com/equation?tex=P(|U|>C|H_0)=\alpha
  " alt="P(|U|>C|H_0)=\alpha
  " class="ee_img tr_noresize" eeimg="1">
  若 <img src="https://www.zhihu.com/equation?tex=\alpha=0.05" alt="\alpha=0.05" class="ee_img tr_noresize" eeimg="1"> ，则可以得出 <img src="https://www.zhihu.com/equation?tex=P(|U|>C|H_0)=0.05\Rightarrow C=u_{0.025}" alt="P(|U|>C|H_0)=0.05\Rightarrow C=u_{0.025}" class="ee_img tr_noresize" eeimg="1"> 。因为 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 成立时， <img src="https://www.zhihu.com/equation?tex=U" alt="U" class="ee_img tr_noresize" eeimg="1"> 是标准正态分布。

* 做判断：

  根据样本的观测值，计算 <img src="https://www.zhihu.com/equation?tex=U" alt="U" class="ee_img tr_noresize" eeimg="1"> ，和 <img src="https://www.zhihu.com/equation?tex=C" alt="C" class="ee_img tr_noresize" eeimg="1"> 进行比较。若 <img src="https://www.zhihu.com/equation?tex=|U|>C" alt="|U|>C" class="ee_img tr_noresize" eeimg="1"> 就拒绝 <img src="https://www.zhihu.com/equation?tex=H_1" alt="H_1" class="ee_img tr_noresize" eeimg="1"> 。

这里对 <img src="https://www.zhihu.com/equation?tex=P(|U|>C|H_0)=\alpha" alt="P(|U|>C|H_0)=\alpha" class="ee_img tr_noresize" eeimg="1"> 我的理解是：**若 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 成立的话，发生 <img src="https://www.zhihu.com/equation?tex=|U|>C" alt="|U|>C" class="ee_img tr_noresize" eeimg="1"> 的概率很小很小，所以现实中发生了的话我们只好认为 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 不成立了。**

>假设检验不一定原假设一定形如 <img src="https://www.zhihu.com/equation?tex=a=a_0" alt="a=a_0" class="ee_img tr_noresize" eeimg="1"> ，其本质是把参数 <img src="https://www.zhihu.com/equation?tex=\theta" alt="\theta" class="ee_img tr_noresize" eeimg="1"> 分成两个不相交的空间：

<img src="https://www.zhihu.com/equation?tex=>H_0:\theta\in\Theta_0,H_1:\theta\in\Theta-\Theta_0=\Theta_1
>" alt=">H_0:\theta\in\Theta_0,H_1:\theta\in\Theta-\Theta_0=\Theta_1
>" class="ee_img tr_noresize" eeimg="1">
>若 <img src="https://www.zhihu.com/equation?tex=\Theta_1" alt="\Theta_1" class="ee_img tr_noresize" eeimg="1"> 在 <img src="https://www.zhihu.com/equation?tex=\Theta_0" alt="\Theta_0" class="ee_img tr_noresize" eeimg="1"> 的两侧（如例子）就叫做**双侧检验**，否则也可以有 <img src="https://www.zhihu.com/equation?tex=\Theta_1" alt="\Theta_1" class="ee_img tr_noresize" eeimg="1"> 在 <img src="https://www.zhihu.com/equation?tex=\Theta_0" alt="\Theta_0" class="ee_img tr_noresize" eeimg="1"> 的右侧或左侧的**单侧检验**。

--------

>假设检验可能有两种错误，**弃真**和**存伪**

* **弃真**： <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 成立，但拒绝事件 <img src="https://www.zhihu.com/equation?tex=|U|>C" alt="|U|>C" class="ee_img tr_noresize" eeimg="1"> 发生了，所以拒绝了 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 。弃真的概率就是显著性水平 <img src="https://www.zhihu.com/equation?tex=\alpha" alt="\alpha" class="ee_img tr_noresize" eeimg="1"> 。
* **存伪**： <img src="https://www.zhihu.com/equation?tex=H_1" alt="H_1" class="ee_img tr_noresize" eeimg="1"> 成立，却接受了 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 。它的概率比较难以计算，记为 <img src="https://www.zhihu.com/equation?tex=\beta" alt="\beta" class="ee_img tr_noresize" eeimg="1"> 。

事实上，有当样本数 <img src="https://www.zhihu.com/equation?tex=n" alt="n" class="ee_img tr_noresize" eeimg="1"> 固定时， <img src="https://www.zhihu.com/equation?tex=\alpha" alt="\alpha" class="ee_img tr_noresize" eeimg="1"> 增大 <img src="https://www.zhihu.com/equation?tex=\beta" alt="\beta" class="ee_img tr_noresize" eeimg="1"> 就会减小， <img src="https://www.zhihu.com/equation?tex=\alpha" alt="\alpha" class="ee_img tr_noresize" eeimg="1"> 减小 <img src="https://www.zhihu.com/equation?tex=\beta" alt="\beta" class="ee_img tr_noresize" eeimg="1"> 就会增大。但增大样本数 <img src="https://www.zhihu.com/equation?tex=n" alt="n" class="ee_img tr_noresize" eeimg="1"> 可以使得 <img src="https://www.zhihu.com/equation?tex=\alpha" alt="\alpha" class="ee_img tr_noresize" eeimg="1"> 和 <img src="https://www.zhihu.com/equation?tex=\beta" alt="\beta" class="ee_img tr_noresize" eeimg="1"> 都减小。（抽样的值多了更准确）

>给出一个样本观测值 <img src="https://www.zhihu.com/equation?tex=U" alt="U" class="ee_img tr_noresize" eeimg="1"> ，能做出”拒绝 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> “的最小的 <img src="https://www.zhihu.com/equation?tex=\alpha" alt="\alpha" class="ee_img tr_noresize" eeimg="1"> 值称为检验的**p值**。

* 一般模拟抽样的软件不仅会告诉你模拟抽取的样本观测值，同样也会告诉你该观测值下的p值。这样你就不需要去比较 <img src="https://www.zhihu.com/equation?tex=U" alt="U" class="ee_img tr_noresize" eeimg="1"> 和 <img src="https://www.zhihu.com/equation?tex=u_{\alpha/2}" alt="u_{\alpha/2}" class="ee_img tr_noresize" eeimg="1"> 了，而只用比较 <img src="https://www.zhihu.com/equation?tex=\alpha" alt="\alpha" class="ee_img tr_noresize" eeimg="1"> 和p。

## 正态总体参数的假设检验

| 条件                      | 原假设 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1">               | 备选假设 <img src="https://www.zhihu.com/equation?tex=H_1" alt="H_1" class="ee_img tr_noresize" eeimg="1">             | 检验统计量                                                   | 拒绝域                                                       |

| ------------------------- | ------------------------ | ------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |

|  <img src="https://www.zhihu.com/equation?tex=\sigma^2=\sigma_0^2" alt="\sigma^2=\sigma_0^2" class="ee_img tr_noresize" eeimg="1"> 已知 |  <img src="https://www.zhihu.com/equation?tex=\mu=\mu_0" alt="\mu=\mu_0" class="ee_img tr_noresize" eeimg="1">               |  <img src="https://www.zhihu.com/equation?tex=\mu\neq\mu_0" alt="\mu\neq\mu_0" class="ee_img tr_noresize" eeimg="1">            |  <img src="https://www.zhihu.com/equation?tex=U=\frac{\bar{X}-\mu_0}{\sigma_0/\sqrt{n}}" alt="U=\frac{\bar{X}-\mu_0}{\sigma_0/\sqrt{n}}" class="ee_img tr_noresize" eeimg="1">                   |  <img src="https://www.zhihu.com/equation?tex=|U|>u_{\alpha/2}" alt="|U|>u_{\alpha/2}" class="ee_img tr_noresize" eeimg="1">                                            |

|                           |  <img src="https://www.zhihu.com/equation?tex=\mu\leq\mu_0" alt="\mu\leq\mu_0" class="ee_img tr_noresize" eeimg="1">            |  <img src="https://www.zhihu.com/equation?tex=\mu>\mu_0" alt="\mu>\mu_0" class="ee_img tr_noresize" eeimg="1">               | 服从正态分布                                                 |  <img src="https://www.zhihu.com/equation?tex=U>u_\alpha" alt="U>u_\alpha" class="ee_img tr_noresize" eeimg="1">                                                  |

|                           |  <img src="https://www.zhihu.com/equation?tex=\mu \geq\mu_0" alt="\mu \geq\mu_0" class="ee_img tr_noresize" eeimg="1">           |  <img src="https://www.zhihu.com/equation?tex=\mu <\mu_0" alt="\mu <\mu_0" class="ee_img tr_noresize" eeimg="1">              |                                                              |  <img src="https://www.zhihu.com/equation?tex=U<-u_\alpha" alt="U<-u_\alpha" class="ee_img tr_noresize" eeimg="1">                                                 |

|  <img src="https://www.zhihu.com/equation?tex=\sigma^2" alt="\sigma^2" class="ee_img tr_noresize" eeimg="1"> 未知            |  <img src="https://www.zhihu.com/equation?tex=\mu=\mu_0" alt="\mu=\mu_0" class="ee_img tr_noresize" eeimg="1">               |  <img src="https://www.zhihu.com/equation?tex=\mu\neq\mu_0" alt="\mu\neq\mu_0" class="ee_img tr_noresize" eeimg="1">            |  <img src="https://www.zhihu.com/equation?tex=T=\frac{\bar{X}-\mu_0}{S/\sqrt{n}}" alt="T=\frac{\bar{X}-\mu_0}{S/\sqrt{n}}" class="ee_img tr_noresize" eeimg="1"> 服从t分布                |  <img src="https://www.zhihu.com/equation?tex=|T|>t_{\alpha/2}(n-1)" alt="|T|>t_{\alpha/2}(n-1)" class="ee_img tr_noresize" eeimg="1">                                       |

|                           |  <img src="https://www.zhihu.com/equation?tex=\mu\leq\mu_0" alt="\mu\leq\mu_0" class="ee_img tr_noresize" eeimg="1">            |  <img src="https://www.zhihu.com/equation?tex=\mu>\mu_0" alt="\mu>\mu_0" class="ee_img tr_noresize" eeimg="1">               |                                                              |  <img src="https://www.zhihu.com/equation?tex=T>t_{\alpha}(n-1)" alt="T>t_{\alpha}(n-1)" class="ee_img tr_noresize" eeimg="1">                                           |

|                           |  <img src="https://www.zhihu.com/equation?tex=\mu \geq\mu_0" alt="\mu \geq\mu_0" class="ee_img tr_noresize" eeimg="1">           |  <img src="https://www.zhihu.com/equation?tex=\mu <\mu_0" alt="\mu <\mu_0" class="ee_img tr_noresize" eeimg="1">              |                                                              |  <img src="https://www.zhihu.com/equation?tex=T<-t_{\alpha}(n-1)" alt="T<-t_{\alpha}(n-1)" class="ee_img tr_noresize" eeimg="1">                                          |

|  <img src="https://www.zhihu.com/equation?tex=\mu=\mu_0" alt="\mu=\mu_0" class="ee_img tr_noresize" eeimg="1"> 已知           |  <img src="https://www.zhihu.com/equation?tex=\sigma^2=\sigma_0^2" alt="\sigma^2=\sigma_0^2" class="ee_img tr_noresize" eeimg="1">     |  <img src="https://www.zhihu.com/equation?tex=\sigma^2\neq\sigma_0^2" alt="\sigma^2\neq\sigma_0^2" class="ee_img tr_noresize" eeimg="1">  |  <img src="https://www.zhihu.com/equation?tex=\chi^2=\sum_{i=1}^n(\frac{X_i-\mu_0}{\sigma_0})^2" alt="\chi^2=\sum_{i=1}^n(\frac{X_i-\mu_0}{\sigma_0})^2" class="ee_img tr_noresize" eeimg="1"> 服从卡方分布 |  <img src="https://www.zhihu.com/equation?tex=\chi^2>\chi^2_{\alpha/2}(n)" alt="\chi^2>\chi^2_{\alpha/2}(n)" class="ee_img tr_noresize" eeimg="1"> 或 <img src="https://www.zhihu.com/equation?tex=\chi^2<\chi_{1-\alpha/2}^2(n)" alt="\chi^2<\chi_{1-\alpha/2}^2(n)" class="ee_img tr_noresize" eeimg="1">  |

|                           |  <img src="https://www.zhihu.com/equation?tex=\sigma^2\leq\sigma_0^2" alt="\sigma^2\leq\sigma_0^2" class="ee_img tr_noresize" eeimg="1">  |  <img src="https://www.zhihu.com/equation?tex=\sigma^2>\sigma_0^2" alt="\sigma^2>\sigma_0^2" class="ee_img tr_noresize" eeimg="1">     |                                                              |  <img src="https://www.zhihu.com/equation?tex=\chi^2>\chi_{\alpha}^2(n)" alt="\chi^2>\chi_{\alpha}^2(n)" class="ee_img tr_noresize" eeimg="1">                                   |

|                           |  <img src="https://www.zhihu.com/equation?tex=\sigma^2\geq\sigma_0^2" alt="\sigma^2\geq\sigma_0^2" class="ee_img tr_noresize" eeimg="1">  |  <img src="https://www.zhihu.com/equation?tex=\sigma^2<\sigma_0^2" alt="\sigma^2<\sigma_0^2" class="ee_img tr_noresize" eeimg="1">     |                                                              |  <img src="https://www.zhihu.com/equation?tex=\chi^2<\chi_{1-\alpha}^2(n)" alt="\chi^2<\chi_{1-\alpha}^2(n)" class="ee_img tr_noresize" eeimg="1">                                 |

|  <img src="https://www.zhihu.com/equation?tex=\mu" alt="\mu" class="ee_img tr_noresize" eeimg="1"> 未知                 |  <img src="https://www.zhihu.com/equation?tex=\sigma^2=\sigma_0^2" alt="\sigma^2=\sigma_0^2" class="ee_img tr_noresize" eeimg="1">     |  <img src="https://www.zhihu.com/equation?tex=\sigma^2\neq\sigma_0^2" alt="\sigma^2\neq\sigma_0^2" class="ee_img tr_noresize" eeimg="1">  |  <img src="https://www.zhihu.com/equation?tex=\chi^2=\frac{(n-1)S^2}{\sigma_0^2}" alt="\chi^2=\frac{(n-1)S^2}{\sigma_0^2}" class="ee_img tr_noresize" eeimg="1"> 服从卡方分布             |  <img src="https://www.zhihu.com/equation?tex=\chi^2>\chi_{\alpha/2}^2(n-1)" alt="\chi^2>\chi_{\alpha/2}^2(n-1)" class="ee_img tr_noresize" eeimg="1"> 或 <img src="https://www.zhihu.com/equation?tex=\chi^2<\chi_{1-\alpha/2}^2(n-1)" alt="\chi^2<\chi_{1-\alpha/2}^2(n-1)" class="ee_img tr_noresize" eeimg="1">  |

|                           |  <img src="https://www.zhihu.com/equation?tex=\sigma^2\leq\sigma_0^2" alt="\sigma^2\leq\sigma_0^2" class="ee_img tr_noresize" eeimg="1">  |  <img src="https://www.zhihu.com/equation?tex=\sigma^2>\sigma_0^2" alt="\sigma^2>\sigma_0^2" class="ee_img tr_noresize" eeimg="1">     |                                                              |  <img src="https://www.zhihu.com/equation?tex=\chi^2>\chi_{\alpha}^2(n-1)" alt="\chi^2>\chi_{\alpha}^2(n-1)" class="ee_img tr_noresize" eeimg="1">                                 |

|                           |  <img src="https://www.zhihu.com/equation?tex=\sigma^2\geq\sigma_0^2" alt="\sigma^2\geq\sigma_0^2" class="ee_img tr_noresize" eeimg="1">  |  <img src="https://www.zhihu.com/equation?tex=\sigma^2<\sigma_0^2" alt="\sigma^2<\sigma_0^2" class="ee_img tr_noresize" eeimg="1">     |                                                              |  <img src="https://www.zhihu.com/equation?tex=\chi^2<\chi_{1-\alpha}^2(n-1)" alt="\chi^2<\chi_{1-\alpha}^2(n-1)" class="ee_img tr_noresize" eeimg="1">                               |


简单证明下对方差估计的部分，怎么考虑不等号呢？以第八行的情况为例，若 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 成立，就有：

<img src="https://www.zhihu.com/equation?tex=\chi^2=\sum_{i=1}^n(\frac{X_i-\mu_0}{\sigma_0})^2=\frac{\sigma^2}{\sigma_0^2}\sum_{i=1}^n(\frac{X_i-\mu_0}{\sigma})^2\leq \chi^2(n)
" alt="\chi^2=\sum_{i=1}^n(\frac{X_i-\mu_0}{\sigma_0})^2=\frac{\sigma^2}{\sigma_0^2}\sum_{i=1}^n(\frac{X_i-\mu_0}{\sigma})^2\leq \chi^2(n)
" class="ee_img tr_noresize" eeimg="1">
若 <img src="https://www.zhihu.com/equation?tex=H_1" alt="H_1" class="ee_img tr_noresize" eeimg="1"> 成立，则有 <img src="https://www.zhihu.com/equation?tex=\chi^2>\chi^2(n)" alt="\chi^2>\chi^2(n)" class="ee_img tr_noresize" eeimg="1"> 。（ <img src="https://www.zhihu.com/equation?tex=\sigma^2" alt="\sigma^2" class="ee_img tr_noresize" eeimg="1"> 是真实的方差， <img src="https://www.zhihu.com/equation?tex=\sigma_0^2" alt="\sigma_0^2" class="ee_img tr_noresize" eeimg="1"> 是假设的方差）所以 <img src="https://www.zhihu.com/equation?tex=\chi^2" alt="\chi^2" class="ee_img tr_noresize" eeimg="1"> 的观测值越大，对 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 越不利，对 <img src="https://www.zhihu.com/equation?tex=X_1" alt="X_1" class="ee_img tr_noresize" eeimg="1"> 越有利。

<img src="https://www.zhihu.com/equation?tex=P(\chi^2>\chi_{\alpha}^2(n)|H_0)\leq P(\chi^2>\chi_{\alpha}^2(n)|\sigma^2=\sigma_0^2)=\alpha
" alt="P(\chi^2>\chi_{\alpha}^2(n)|H_0)\leq P(\chi^2>\chi_{\alpha}^2(n)|\sigma^2=\sigma_0^2)=\alpha
" class="ee_img tr_noresize" eeimg="1">
所以选择的拒绝域是 <img src="https://www.zhihu.com/equation?tex=\chi^2>\chi_{\alpha}^2(n)" alt="\chi^2>\chi_{\alpha}^2(n)" class="ee_img tr_noresize" eeimg="1"> 。

# 一元线性回归和方差分析

## 一元线性回归

>已知随机变量 <img src="https://www.zhihu.com/equation?tex=Y" alt="Y" class="ee_img tr_noresize" eeimg="1"> 满足以下关系：

<img src="https://www.zhihu.com/equation?tex=>\begin{cases}Y=\beta_0+\beta_1 X+\varepsilon\\E[\varepsilon]=0,D(\varepsilon)=\sigma^2\end{cases}
>" alt=">\begin{cases}Y=\beta_0+\beta_1 X+\varepsilon\\E[\varepsilon]=0,D(\varepsilon)=\sigma^2\end{cases}
>" class="ee_img tr_noresize" eeimg="1">
> <img src="https://www.zhihu.com/equation?tex=\sigma^2" alt="\sigma^2" class="ee_img tr_noresize" eeimg="1"> 未知。那么我们可以通过抽取一堆样本 <img src="https://www.zhihu.com/equation?tex=(x_1,y_1),...,(x_n,y_n)" alt="(x_1,y_1),...,(x_n,y_n)" class="ee_img tr_noresize" eeimg="1"> 去估计 <img src="https://www.zhihu.com/equation?tex=\beta_0" alt="\beta_0" class="ee_img tr_noresize" eeimg="1"> 和 <img src="https://www.zhihu.com/equation?tex=\beta_1" alt="\beta_1" class="ee_img tr_noresize" eeimg="1"> 的值，得到**回归直线** <img src="https://www.zhihu.com/equation?tex=Y=\hat{\beta_0}+\hat{\beta_1}X" alt="Y=\hat{\beta_0}+\hat{\beta_1}X" class="ee_img tr_noresize" eeimg="1"> 。
>
>再根据这条直线，可以给出 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 得到Y的估测值 <img src="https://www.zhihu.com/equation?tex=\hat{Y}" alt="\hat{Y}" class="ee_img tr_noresize" eeimg="1"> 。
>
>注意：一元线性回归中，默认自变量是**非随机变量**。怎么理解呢，可以理解为，给定一个 <img src="https://www.zhihu.com/equation?tex=x_0" alt="x_0" class="ee_img tr_noresize" eeimg="1"> ，有一个随机变量 <img src="https://www.zhihu.com/equation?tex=Y" alt="Y" class="ee_img tr_noresize" eeimg="1"> ，而 <img src="https://www.zhihu.com/equation?tex=x_0" alt="x_0" class="ee_img tr_noresize" eeimg="1"> 是随机变量 <img src="https://www.zhihu.com/equation?tex=Y" alt="Y" class="ee_img tr_noresize" eeimg="1"> 的一个参数，影响着 <img src="https://www.zhihu.com/equation?tex=Y" alt="Y" class="ee_img tr_noresize" eeimg="1"> 的分布。而这个影响实际上就是线性影响着。但参数 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 总是会被给出的，而参数 <img src="https://www.zhihu.com/equation?tex=\beta_0,\beta_1" alt="\beta_0,\beta_1" class="ee_img tr_noresize" eeimg="1"> 是可以用样本估计的，于是这三个参数都有值了后就可以讨论 <img src="https://www.zhihu.com/equation?tex=Y" alt="Y" class="ee_img tr_noresize" eeimg="1"> 的分布。而回归问题，其实就是默认参数 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 的值已知非随机的情况下，分析 <img src="https://www.zhihu.com/equation?tex=Y" alt="Y" class="ee_img tr_noresize" eeimg="1"> 和 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 的关系。

### **最小二乘法**：

* 定义**偏差平方和**：

<img src="https://www.zhihu.com/equation?tex=Q(\beta_0,\beta_1)=\sum_{i=1}^n[y_i-(\beta_0+\beta_1x_i)]^2
  " alt="Q(\beta_0,\beta_1)=\sum_{i=1}^n[y_i-(\beta_0+\beta_1x_i)]^2
  " class="ee_img tr_noresize" eeimg="1">
  我们要找出 <img src="https://www.zhihu.com/equation?tex=\beta_0" alt="\beta_0" class="ee_img tr_noresize" eeimg="1"> 和 <img src="https://www.zhihu.com/equation?tex=\beta_1" alt="\beta_1" class="ee_img tr_noresize" eeimg="1"> 的合理取值 <img src="https://www.zhihu.com/equation?tex=\hat{\beta_0},\hat{\beta_1}" alt="\hat{\beta_0},\hat{\beta_1}" class="ee_img tr_noresize" eeimg="1"> ，使得 <img src="https://www.zhihu.com/equation?tex=Q(\hat{\beta_0},\hat{\beta_1})" alt="Q(\hat{\beta_0},\hat{\beta_1})" class="ee_img tr_noresize" eeimg="1"> 尽量小。于是有：

<img src="https://www.zhihu.com/equation?tex=\begin{cases}\frac{\partial Q(\beta_0,\beta_1)}{\partial\beta_0}=0\\\frac{\partial Q(\beta_0,\beta_1)}{\partial\beta_1}=0\end{cases}
  \Rightarrow\begin{cases}\hat{\beta_0}+\bar{x}\hat{\beta_1}=\bar{y}\\n\bar{x}\hat{\beta_0}+\hat{\beta_1}\sum_{i=1}^nx_i^2=\sum_{i=1}^nx_iy_i\end{cases}
  " alt="\begin{cases}\frac{\partial Q(\beta_0,\beta_1)}{\partial\beta_0}=0\\\frac{\partial Q(\beta_0,\beta_1)}{\partial\beta_1}=0\end{cases}
  \Rightarrow\begin{cases}\hat{\beta_0}+\bar{x}\hat{\beta_1}=\bar{y}\\n\bar{x}\hat{\beta_0}+\hat{\beta_1}\sum_{i=1}^nx_i^2=\sum_{i=1}^nx_iy_i\end{cases}
  " class="ee_img tr_noresize" eeimg="1">
  解得：

<img src="https://www.zhihu.com/equation?tex=\hat{\beta_1}=\frac{L_{xy}}{L_{xx}},\hat{\beta_0}=\bar{y}-\bar{x}\hat{\beta_1}\\
  L_{xy}=\sum_{i=1}^n(x_i-\bar{x})(y_i-\bar{y})=\sum_{i=1}^nx_iy_i-n\bar{x}\bar{y}\\
  L_{xx}=\sum_{i=1}^n(x_i-\bar{x})^2=\sum_{i=1}^nx_i^2-n\bar{x}^2\\
  " alt="\hat{\beta_1}=\frac{L_{xy}}{L_{xx}},\hat{\beta_0}=\bar{y}-\bar{x}\hat{\beta_1}\\
  L_{xy}=\sum_{i=1}^n(x_i-\bar{x})(y_i-\bar{y})=\sum_{i=1}^nx_iy_i-n\bar{x}\bar{y}\\
  L_{xx}=\sum_{i=1}^n(x_i-\bar{x})^2=\sum_{i=1}^nx_i^2-n\bar{x}^2\\
  " class="ee_img tr_noresize" eeimg="1">
  这样估计的参数 <img src="https://www.zhihu.com/equation?tex=\beta_0,\beta_1" alt="\beta_0,\beta_1" class="ee_img tr_noresize" eeimg="1"> 的值的方法称为最小二乘法（OLS），得到了一元线性回归方程，显然它一定过 <img src="https://www.zhihu.com/equation?tex=(\bar{x},\bar{y})" alt="(\bar{x},\bar{y})" class="ee_img tr_noresize" eeimg="1"> 。

* 最小二乘法估计是无偏的：

<img src="https://www.zhihu.com/equation?tex=E[\hat{\beta_0}]=\beta_0,E[\hat{\beta_1}]=\beta_1
  " alt="E[\hat{\beta_0}]=\beta_0,E[\hat{\beta_1}]=\beta_1
  " class="ee_img tr_noresize" eeimg="1">
  注意：在一元线性回归中，默认自变量是非随机变量，于是有：

<img src="https://www.zhihu.com/equation?tex=\hat{\beta_1}=\frac{\sum_{i=1}^n(x_i-\bar{x})(y_i-\bar{y})}{L_{xx}}=\sum_{i=1}^n\frac{x_i-\bar{x}}{L_{xx}}y_i\\
  E[\hat{\beta_1}]=\sum_{i=1}^n\frac{x_i-\bar{x}}{L_{xx}}E[y_i]\\
  \because E[y_i]=\beta_0+\beta_1x_i+E[\varepsilon]=\beta_0+\beta_1x_i\\
  \therefore E[\hat{\beta_1}]=\sum_{i=1}^n\frac{x_i-\bar{x}}{L_{xx}}(\beta_0+\beta_1x_i)=\sum_{i=1}^n\frac{x_i-\bar{x}}{L_{xx}}\beta_1 x_i\\
  =\beta_1\sum_{i=1}^n\frac{(x_i-\bar{x})^2}{L_{xx}}=\beta_1
  " alt="\hat{\beta_1}=\frac{\sum_{i=1}^n(x_i-\bar{x})(y_i-\bar{y})}{L_{xx}}=\sum_{i=1}^n\frac{x_i-\bar{x}}{L_{xx}}y_i\\
  E[\hat{\beta_1}]=\sum_{i=1}^n\frac{x_i-\bar{x}}{L_{xx}}E[y_i]\\
  \because E[y_i]=\beta_0+\beta_1x_i+E[\varepsilon]=\beta_0+\beta_1x_i\\
  \therefore E[\hat{\beta_1}]=\sum_{i=1}^n\frac{x_i-\bar{x}}{L_{xx}}(\beta_0+\beta_1x_i)=\sum_{i=1}^n\frac{x_i-\bar{x}}{L_{xx}}\beta_1 x_i\\
  =\beta_1\sum_{i=1}^n\frac{(x_i-\bar{x})^2}{L_{xx}}=\beta_1
  " class="ee_img tr_noresize" eeimg="1">
  注意到 <img src="https://www.zhihu.com/equation?tex=Y=\beta_0+\beta_1X+\varepsilon" alt="Y=\beta_0+\beta_1X+\varepsilon" class="ee_img tr_noresize" eeimg="1"> 中随机变量实际上只有 <img src="https://www.zhihu.com/equation?tex=Y" alt="Y" class="ee_img tr_noresize" eeimg="1"> 和 <img src="https://www.zhihu.com/equation?tex=\varepsilon" alt="\varepsilon" class="ee_img tr_noresize" eeimg="1"> 。而 <img src="https://www.zhihu.com/equation?tex=x_i,\beta_0,\beta_1" alt="x_i,\beta_0,\beta_1" class="ee_img tr_noresize" eeimg="1"> 都是固定参数。此外上述推导过程反复用到了 <img src="https://www.zhihu.com/equation?tex=C*\sum_{i=1}^n\frac{x_i-\bar{x}}{L_{xx}}=0" alt="C*\sum_{i=1}^n\frac{x_i-\bar{x}}{L_{xx}}=0" class="ee_img tr_noresize" eeimg="1"> 。

* 最小二乘法估计是有效的：

  在所有 <img src="https://www.zhihu.com/equation?tex=\hat{\beta_0},\hat{\beta_1}" alt="\hat{\beta_0},\hat{\beta_1}" class="ee_img tr_noresize" eeimg="1"> 关于 <img src="https://www.zhihu.com/equation?tex=y_1,..,y_n" alt="y_1,..,y_n" class="ee_img tr_noresize" eeimg="1"> 是线性的函数估计中，最小二乘法是方差最小的。再强调一遍 <img src="https://www.zhihu.com/equation?tex=x_i" alt="x_i" class="ee_img tr_noresize" eeimg="1"> 只是给定的固定参数。

* 最小二乘法估计的可靠性：

  最小二乘法做出的估计值可以使得**残差平方和**最小：

<img src="https://www.zhihu.com/equation?tex=Q(\hat{\beta_0},\hat{\beta_1})=\sum_{i=1}^n[y_i-\hat{\beta_0}-\hat{\beta_1}x_i]^2
  " alt="Q(\hat{\beta_0},\hat{\beta_1})=\sum_{i=1}^n[y_i-\hat{\beta_0}-\hat{\beta_1}x_i]^2
  " class="ee_img tr_noresize" eeimg="1">
  用正交变换可以证明：

<img src="https://www.zhihu.com/equation?tex=\frac{Q(\hat{\beta_0},\hat{\beta_1})}{\sigma^2}\sim\chi^2(n-2)
  " alt="\frac{Q(\hat{\beta_0},\hat{\beta_1})}{\sigma^2}\sim\chi^2(n-2)
  " class="ee_img tr_noresize" eeimg="1">
  因此 <img src="https://www.zhihu.com/equation?tex=E[\frac{Q(\hat{\beta_0},\hat{\beta_1})}{\sigma^2}]=n-2,E[\frac{Q(\hat{\beta_0},\hat{\beta_1})}{n-2}]=\sigma^2" alt="E[\frac{Q(\hat{\beta_0},\hat{\beta_1})}{\sigma^2}]=n-2,E[\frac{Q(\hat{\beta_0},\hat{\beta_1})}{n-2}]=\sigma^2" class="ee_img tr_noresize" eeimg="1"> 。即 <img src="https://www.zhihu.com/equation?tex=\hat{\sigma^2}=\frac{Q(\hat{\beta_0},\hat{\beta_1})}{n-2}" alt="\hat{\sigma^2}=\frac{Q(\hat{\beta_0},\hat{\beta_1})}{n-2}" class="ee_img tr_noresize" eeimg="1"> 是一个 <img src="https://www.zhihu.com/equation?tex=\sigma^2" alt="\sigma^2" class="ee_img tr_noresize" eeimg="1"> 的一个无偏估计，称为**剩余方差**。

  这里是对Y的方差进行估计，而 <img src="https://www.zhihu.com/equation?tex=D(Y)=D(\beta_0)+D(\beta_1X)+D(\varepsilon)=D(\varepsilon)=\sigma^2" alt="D(Y)=D(\beta_0)+D(\beta_1X)+D(\varepsilon)=D(\varepsilon)=\sigma^2" class="ee_img tr_noresize" eeimg="1"> 。强调X也是非随机变量。

### 回归方程的显著性检验

多数情况下是不知道 <img src="https://www.zhihu.com/equation?tex=Y" alt="Y" class="ee_img tr_noresize" eeimg="1"> 与 <img src="https://www.zhihu.com/equation?tex=X" alt="X" class="ee_img tr_noresize" eeimg="1"> 是否是线性相关的，于是需要进行假设检验。 <img src="https://www.zhihu.com/equation?tex=|\beta_1|" alt="|\beta_1|" class="ee_img tr_noresize" eeimg="1"> 越大，说明线性性越强。做假设：

<img src="https://www.zhihu.com/equation?tex=H_0:\beta_1=0,H_1:\beta_1\neq 0
" alt="H_0:\beta_1=0,H_1:\beta_1\neq 0
" class="ee_img tr_noresize" eeimg="1">
可以证明有以下等式：

<img src="https://www.zhihu.com/equation?tex=L_{yy}=Q+U\\
L_{yy}=\sum_{i=1}^n(y_i-\bar{y})^2\\
Q=\sum_{i=1}^n(y_i-\hat{\beta_0}-\hat{\beta_1}x_i)^2\\
U=\sum_{i=1}^n(\hat{\beta_0}+\hat{\beta_1}x_i-\bar{y})^2=\hat{\beta_1}^2L_{xx}
" alt="L_{yy}=Q+U\\
L_{yy}=\sum_{i=1}^n(y_i-\bar{y})^2\\
Q=\sum_{i=1}^n(y_i-\hat{\beta_0}-\hat{\beta_1}x_i)^2\\
U=\sum_{i=1}^n(\hat{\beta_0}+\hat{\beta_1}x_i-\bar{y})^2=\hat{\beta_1}^2L_{xx}
" class="ee_img tr_noresize" eeimg="1">
其中，即为**离差平方和** <img src="https://www.zhihu.com/equation?tex=L_{yy}=" alt="L_{yy}=" class="ee_img tr_noresize" eeimg="1"> **残差平方和** <img src="https://www.zhihu.com/equation?tex=Q+" alt="Q+" class="ee_img tr_noresize" eeimg="1"> **回归平方和** <img src="https://www.zhihu.com/equation?tex=U" alt="U" class="ee_img tr_noresize" eeimg="1"> 。它表明：

>Y的n个观测值的离散程度 <img src="https://www.zhihu.com/equation?tex=L_{yy}" alt="L_{yy}" class="ee_img tr_noresize" eeimg="1"> 可分解为两部分：Q表示样本值没有落在回归直线上引起的，U表示由回归系数 <img src="https://www.zhihu.com/equation?tex=\hat{\beta}" alt="\hat{\beta}" class="ee_img tr_noresize" eeimg="1"> 本身引起的。因此，若 <img src="https://www.zhihu.com/equation?tex=Q" alt="Q" class="ee_img tr_noresize" eeimg="1"> 越大，就表示线性性越差，反之，若 <img src="https://www.zhihu.com/equation?tex=Q=0" alt="Q=0" class="ee_img tr_noresize" eeimg="1"> ，则样本都落在回归直线上，说明线性性很强。

不难证明， <img src="https://www.zhihu.com/equation?tex=F=\frac{U}{Q/(n-2)}\sim F(1,n-2)" alt="F=\frac{U}{Q/(n-2)}\sim F(1,n-2)" class="ee_img tr_noresize" eeimg="1"> 。结论是，若 <img src="https://www.zhihu.com/equation?tex=F>F_\alpha(1,n-2)" alt="F>F_\alpha(1,n-2)" class="ee_img tr_noresize" eeimg="1"> ，则拒绝 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> ，认为存在线性性。

-----

预测：给定一个 <img src="https://www.zhihu.com/equation?tex=x_0" alt="x_0" class="ee_img tr_noresize" eeimg="1"> ， <img src="https://www.zhihu.com/equation?tex=Y_0" alt="Y_0" class="ee_img tr_noresize" eeimg="1"> 的点预测值为 <img src="https://www.zhihu.com/equation?tex=\hat{Y_i}=\hat{\beta_0}+\hat{\beta_1}x_0" alt="\hat{Y_i}=\hat{\beta_0}+\hat{\beta_1}x_0" class="ee_img tr_noresize" eeimg="1"> ，同样也可以对它进行置信区间预测。 <img src="https://www.zhihu.com/equation?tex=Y_0" alt="Y_0" class="ee_img tr_noresize" eeimg="1"> 的置信水平为 <img src="https://www.zhihu.com/equation?tex=1-\alpha" alt="1-\alpha" class="ee_img tr_noresize" eeimg="1"> 的置信区间为：

<img src="https://www.zhihu.com/equation?tex=[\hat{Y_0}-\delta(x_0),\hat{Y_0}+\delta(x_0)]\\
\delta(x_0)=\sqrt{\hat{\sigma^2}}t_{\alpha/2}(n-2)\sqrt{1+\frac{1}{n}+\frac{(x_0-\bar{x})^2}{L_{xx}}}
" alt="[\hat{Y_0}-\delta(x_0),\hat{Y_0}+\delta(x_0)]\\
\delta(x_0)=\sqrt{\hat{\sigma^2}}t_{\alpha/2}(n-2)\sqrt{1+\frac{1}{n}+\frac{(x_0-\bar{x})^2}{L_{xx}}}
" class="ee_img tr_noresize" eeimg="1">

## 单因素方差分析

设因素A有r个水平 <img src="https://www.zhihu.com/equation?tex=A_1,A_2,...,A_r" alt="A_1,A_2,...,A_r" class="ee_img tr_noresize" eeimg="1"> ，水平 <img src="https://www.zhihu.com/equation?tex=A_i" alt="A_i" class="ee_img tr_noresize" eeimg="1"> 条件下试验结果的全体记为总体 <img src="https://www.zhihu.com/equation?tex=X_i" alt="X_i" class="ee_img tr_noresize" eeimg="1"> ，假定 <img src="https://www.zhihu.com/equation?tex=X_i\sim N(\mu_i,\sigma^2)" alt="X_i\sim N(\mu_i,\sigma^2)" class="ee_img tr_noresize" eeimg="1"> 。在水平 <img src="https://www.zhihu.com/equation?tex=A_i" alt="A_i" class="ee_img tr_noresize" eeimg="1"> 的条件下进行 <img src="https://www.zhihu.com/equation?tex=n_i" alt="n_i" class="ee_img tr_noresize" eeimg="1"> 次独立试验，即：

<img src="https://www.zhihu.com/equation?tex=\begin{cases}X_{ij}\sim N(\mu_i,\sigma^2)\\
X_{ij}相互独立,i=1,...,r,j=1,...,n_i\\
\mu_i,\sigma^2未知
\end{cases}
" alt="\begin{cases}X_{ij}\sim N(\mu_i,\sigma^2)\\
X_{ij}相互独立,i=1,...,r,j=1,...,n_i\\
\mu_i,\sigma^2未知
\end{cases}
" class="ee_img tr_noresize" eeimg="1">
而单因素方差分析，就是分析不同水平下的方差有无明显差异。作假设：

<img src="https://www.zhihu.com/equation?tex=H_0:\mu_1=\mu_2=...=\mu_r,H_1=\neg(\mu_1=\mu_2=...=\mu_r)
" alt="H_0:\mu_1=\mu_2=...=\mu_r,H_1=\neg(\mu_1=\mu_2=...=\mu_r)
" class="ee_img tr_noresize" eeimg="1">
记 <img src="https://www.zhihu.com/equation?tex=\varepsilon_{ij}=X_{ij}-\mu_i" alt="\varepsilon_{ij}=X_{ij}-\mu_i" class="ee_img tr_noresize" eeimg="1"> 表示一些不可估计的随机因素对试验的影响，被称为**随机误差**， <img src="https://www.zhihu.com/equation?tex=\varepsilon_{ij}\sim N(0,\sigma^2)" alt="\varepsilon_{ij}\sim N(0,\sigma^2)" class="ee_img tr_noresize" eeimg="1"> 。于是模型等价于：

<img src="https://www.zhihu.com/equation?tex=\begin{cases}X_{ij}=\mu_i+\varepsilon_{ij}\\
\varepsilon_{ij}\sim N(0,\sigma^2)且相互独立\\
\mu_i,\sigma^2未知
\end{cases}
" alt="\begin{cases}X_{ij}=\mu_i+\varepsilon_{ij}\\
\varepsilon_{ij}\sim N(0,\sigma^2)且相互独立\\
\mu_i,\sigma^2未知
\end{cases}
" class="ee_img tr_noresize" eeimg="1">
为了方便讨论，引入一些量：

*  <img src="https://www.zhihu.com/equation?tex=n=\sum_{i=1}^rn_i" alt="n=\sum_{i=1}^rn_i" class="ee_img tr_noresize" eeimg="1"> 为样本总数。
*  <img src="https://www.zhihu.com/equation?tex=\mu=\frac{1}{n}\sum_{i=1}^r\mu_i" alt="\mu=\frac{1}{n}\sum_{i=1}^r\mu_i" class="ee_img tr_noresize" eeimg="1"> 为理论总均值。
*  <img src="https://www.zhihu.com/equation?tex=\alpha_i=\mu_i-\mu" alt="\alpha_i=\mu_i-\mu" class="ee_img tr_noresize" eeimg="1"> 为水平 <img src="https://www.zhihu.com/equation?tex=A_i" alt="A_i" class="ee_img tr_noresize" eeimg="1"> 的效应。

易得， <img src="https://www.zhihu.com/equation?tex=H_0\Leftrightarrow \alpha_1=\alpha_2=...=\alpha_r=0" alt="H_0\Leftrightarrow \alpha_1=\alpha_2=...=\alpha_r=0" class="ee_img tr_noresize" eeimg="1"> 。于是继续变换模型：

<img src="https://www.zhihu.com/equation?tex=\begin{cases}X_{ij}=\mu+\alpha_i+\varepsilon_{ij}\\
\sum_{i=1}^rn_i\alpha_i=0\\
\varepsilon_{ij}\sim N(0,\sigma^2)\\
\mu,\alpha_i,\sigma^2未知
\end{cases}
" alt="\begin{cases}X_{ij}=\mu+\alpha_i+\varepsilon_{ij}\\
\sum_{i=1}^rn_i\alpha_i=0\\
\varepsilon_{ij}\sim N(0,\sigma^2)\\
\mu,\alpha_i,\sigma^2未知
\end{cases}
" class="ee_img tr_noresize" eeimg="1">
于是可以进行假设检验。设样本总均值 <img src="https://www.zhihu.com/equation?tex=\bar{X}=\frac{1}{n}\sum_{i=1}^r\sum_{j=1}^{n_i}X_{ij}" alt="\bar{X}=\frac{1}{n}\sum_{i=1}^r\sum_{j=1}^{n_i}X_{ij}" class="ee_img tr_noresize" eeimg="1"> ， <img src="https://www.zhihu.com/equation?tex=\bar{X_i}=\frac{1}{n_i}\sum_{j=1}^{n_i}X_{ij}" alt="\bar{X_i}=\frac{1}{n_i}\sum_{j=1}^{n_i}X_{ij}" class="ee_img tr_noresize" eeimg="1"> 引入**总偏差平方和**：

<img src="https://www.zhihu.com/equation?tex=S_T=\sum_{i=1}^r\sum_{j=1}^{n_i}(X_{ij}-\bar{X})^2\\
=\sum_{i=1}^r\sum_{j=1}^{n_i}[(X_{ij}-\bar{X_i})+(\bar{X_i}-\bar{X})]^2\\
=\sum_{i=1}^r\sum_{j=1}^{n_i}(X_{ij}-\bar{X_i})^2+\sum_{i=1}^r\sum_{j=1}^{n_i}(\bar{X_i}-\bar{X})^2\\
=S_e+S_A
" alt="S_T=\sum_{i=1}^r\sum_{j=1}^{n_i}(X_{ij}-\bar{X})^2\\
=\sum_{i=1}^r\sum_{j=1}^{n_i}[(X_{ij}-\bar{X_i})+(\bar{X_i}-\bar{X})]^2\\
=\sum_{i=1}^r\sum_{j=1}^{n_i}(X_{ij}-\bar{X_i})^2+\sum_{i=1}^r\sum_{j=1}^{n_i}(\bar{X_i}-\bar{X})^2\\
=S_e+S_A
" class="ee_img tr_noresize" eeimg="1">
其中，交叉项 <img src="https://www.zhihu.com/equation?tex=2\sum_{i=1}^r\sum_{j=1}^{n_i}(X_{ij}-\bar{X_i})(\bar{X_i}-\bar{X})=2\sum_{i=1}^r(\bar{X_i}-\bar{X})\sum_{j=1}^{n_i}(X_{ij}-\bar{X_i})=0" alt="2\sum_{i=1}^r\sum_{j=1}^{n_i}(X_{ij}-\bar{X_i})(\bar{X_i}-\bar{X})=2\sum_{i=1}^r(\bar{X_i}-\bar{X})\sum_{j=1}^{n_i}(X_{ij}-\bar{X_i})=0" class="ee_img tr_noresize" eeimg="1"> 。

而 <img src="https://www.zhihu.com/equation?tex=S_e=\sum_{i=1}^r\sum_{j=1}^{n_i}(X_{ij}-\bar{X_i})^2=\sum_{i=1}^r(n_i-1)S_i^2" alt="S_e=\sum_{i=1}^r\sum_{j=1}^{n_i}(X_{ij}-\bar{X_i})^2=\sum_{i=1}^r(n_i-1)S_i^2" class="ee_img tr_noresize" eeimg="1"> 反映了第 <img src="https://www.zhihu.com/equation?tex=i" alt="i" class="ee_img tr_noresize" eeimg="1"> 组样本下内部的差异，而 <img src="https://www.zhihu.com/equation?tex=S_A=\sum_{i=1}^r\sum_{j=1}^{n_i}(\bar{X_i}-\bar{X})^2=\sum_{i=1}^rn_i(\bar{X_i}-\bar{X})^2" alt="S_A=\sum_{i=1}^r\sum_{j=1}^{n_i}(\bar{X_i}-\bar{X})^2=\sum_{i=1}^rn_i(\bar{X_i}-\bar{X})^2" class="ee_img tr_noresize" eeimg="1"> 反映了组与组之间的差异。

于是 <img src="https://www.zhihu.com/equation?tex=S_e" alt="S_e" class="ee_img tr_noresize" eeimg="1"> 被称为**误差平方和**或**组内平方和**， <img src="https://www.zhihu.com/equation?tex=S_A" alt="S_A" class="ee_img tr_noresize" eeimg="1"> 被称为**因素平方和**或**组间平方和**，根据定理：

<img src="https://www.zhihu.com/equation?tex=\frac{S_E}{\sigma^2}\sim \chi^2(n-r)\\
\frac{S_A}{\sigma^2}\sim \chi^2(r - 1)
" alt="\frac{S_E}{\sigma^2}\sim \chi^2(n-r)\\
\frac{S_A}{\sigma^2}\sim \chi^2(r - 1)
" class="ee_img tr_noresize" eeimg="1">
故有

<img src="https://www.zhihu.com/equation?tex=E[S_e]=(n-r)\sigma^2\\
E[S_A]=(r-1)\sigma^2+\sum_{i=1}^rn_i\alpha_i^2
" alt="E[S_e]=(n-r)\sigma^2\\
E[S_A]=(r-1)\sigma^2+\sum_{i=1}^rn_i\alpha_i^2
" class="ee_img tr_noresize" eeimg="1">
若 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 成立，则有 <img src="https://www.zhihu.com/equation?tex=E[\frac{S_e}{n-r}]=E[\frac{S_A}{r-1}]=\sigma^2" alt="E[\frac{S_e}{n-r}]=E[\frac{S_A}{r-1}]=\sigma^2" class="ee_img tr_noresize" eeimg="1"> ，即可以把 <img src="https://www.zhihu.com/equation?tex=\frac{S_e}{n-r},\frac{S_A}{r-1}" alt="\frac{S_e}{n-r},\frac{S_A}{r-1}" class="ee_img tr_noresize" eeimg="1"> 都当作 <img src="https://www.zhihu.com/equation?tex=\sigma^2" alt="\sigma^2" class="ee_img tr_noresize" eeimg="1"> 的一个无偏估计。考虑这样一个统计量：

<img src="https://www.zhihu.com/equation?tex=F=\frac{S_A/(r-1)}{S_e/(n-r)}\sim F(r-1,n-r)
" alt="F=\frac{S_A/(r-1)}{S_e/(n-r)}\sim F(r-1,n-r)
" class="ee_img tr_noresize" eeimg="1">
显然 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 成立时， <img src="https://www.zhihu.com/equation?tex=F" alt="F" class="ee_img tr_noresize" eeimg="1"> 应趋近于1，而 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 不成立时， <img src="https://www.zhihu.com/equation?tex=F" alt="F" class="ee_img tr_noresize" eeimg="1"> 会大于1。于是若 <img src="https://www.zhihu.com/equation?tex=F>F_{\alpha}(r-1,n-r)" alt="F>F_{\alpha}(r-1,n-r)" class="ee_img tr_noresize" eeimg="1"> 就拒绝 <img src="https://www.zhihu.com/equation?tex=H_0" alt="H_0" class="ee_img tr_noresize" eeimg="1"> 。

