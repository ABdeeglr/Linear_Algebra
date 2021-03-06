# Linear Algebra

## Chapter I	Matrices and Gaussian Elimination

阅读本章后，你将了解线性代数面对的**基本问题**是什么，以及较为古典的时期数学家们使用了何种**数学工具**解决这一问题。

### 1.1	Introduction：行列式的意义

线性代数最基本和最核心的第一个问题是：如何解决线性方程组问题。何为线性方程组？线性方程组，顾名思义，方程组中的每一个方程都是线性的，即未知数的幂为1。下列都是线性方程组。
$$
\begin{equation}
1x+2y=3\\
4x+5y=6.
\end{equation}

\tag{二元线性方程组}
$$

$$
\begin{align}
2x&+3y&+4z&=&12\\
5x&&+7z&=&9\\
6x&+4y&+3z&=&18
\end{align}
\tag{三元线性方程组}
$$

面对任何一个线性方程组求解问题，都遵循两个步骤。首先是，确定这个方程组的**解的情况**如何？其次是，在确定了这个方程组的解的情况下，**如何求解**？

#### 判断解的情况

以二元线性方程组为例，**求解二元线性方程组，可以看作是求xy坐标系上两条直线的交集如何**。我们很容易就可以得到以下结果：

1. 只有一个解——对应了两条直线相交。
2. 无解——对于两条直线相互平行。
3. 有无穷个解——两条直线相重合。

我们面对的问题是，通过何种数学工具来判断这个线性方程组的解的情况，在只有两个未知数的情况下，我们当然可以直接通过画图来判断，但是在未知数更多的情况下，我们如何进行抽象刻画，从而判断其解的情况呢？当然是通过行列式理论中的方法了。

#### 如何求解

在判断出解的情况后，求解就相对轻松很多了，我们仍然以简单的例子为例：
$$
\begin{align}
2x&+3y&+4z&=&12\\
5x&&+7z&=&9\\
6x&+4y&+3z&=&18
\end{align}
$$
在中学时期，我们已经习得了这类方程组的求解方法——消元法。

但通常来说，消元法只在未知数较少的情况下比较实用，所以中学的考试中只对三个或三个以下的未知数进行求解。数学家们则拓展了消元法，使其能够针对任意多的未知数进行求解，能够做到这一结果的数学工具正是行列式。

> 不过在现代，在未知数特别多的情况下，我们仍然不使用手工计算，而是将行列式内在的方法通过计算机进行编码，然后交给计算机进行计算。

#### 行列式是什么

说了那么多，行列式究竟是什么呢？行列式是每一个线性方程组所对应的一个数阵。以上述方程组举例：

$$
\begin{align}
1x+2y&=3\\
4x+5y&=6.
\end{align}
$$

这个线性方程组对应的行列式是：
$$
\left|
\begin{array}
&1&	2&	3\\

4&	5&	6
\end{array}
\right|
$$
对这种表达进行抽象化，即为以下对应方式：













#### 总结

行列式方法则告诉了我们，如何通过这些线性方程组中未知数上的**系数**和等号右边的**常数项**来判断解的情况，在已知解的情况后，如何进行**求解**。这也是我们解线性方程组的一般规则：**首先判断该方程组的解的情况，而后在可解的情况下，对该方程组求解**。

### 1.2	线性方程组求解法则

对于任意的线性方程组，将其常数项和未知数项分隔开后，我们能够得到线性方程组的一般表达式：
$$
\begin{case}
a_1x_1

\end{case}
$$
