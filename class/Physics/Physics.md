﻿﻿﻿# 大学物理

---

## 1.质点运动学

### 1.1 参考系 坐标系 物理模型

#### 运动的性质

- 运动的绝对性：运动是物体的基本属性，任何物体都在任何时刻不停地运动着
- 运动的相对性：通常研究物体的运动状态都是在一定的环境和固定的条件下，比如参考系，坐标系

#### 参考系

确定研究对象的位置前先选定一个作为标准的物体或者物体群

#### 坐标系

- 直角坐标系(笛卡尔坐标系)

  基于 $x$ , $y$ , $z$ 三条射线, 分别用三个单位矢量 $i$, $j$, $k$ 表示.

  ![2023-02-14 19-36-54屏幕截图](https://s2.loli.net/2023/02/14/NvQr8zpCsIRJG9H.png)

- 自然坐标系

  质点的轨迹已知, 在运动轨迹上任取一点 $O$ 作为坐标原点, 用质点距离原点的轨道长度 $s$ 来确定质点任意时刻的位置, 以轨迹切线和法向量来构建坐标系

  ![2023-02-14 19-52-39屏幕截图](https://s2.loli.net/2023/02/14/onD7bdkaiW5gK8t.png)

### 1.2 位矢 位移 速度 加速度

#### 位置矢量

假设从原点 $O$ 到 $P$ 点的有向线段 $\vec{OP} = \vec{r}$ 表示，矢量 $\vec{r}$ 叫做 `位置矢量`, 即 `位矢`, 可以表示成

$$
\vec{r} = x\vec{i} + y\vec{j} + z\vec{k} \\
|\vec{r}| = \sqrt{x^2 + y^2 + z^2}
$$

运动方程：

$$
x = x(t),  y = y(t),  z = z(t) \\
\vec{r} = r(x)
$$

#### 位移

设质点沿曲线轨道$\widehat{AB}$运动，在$t$时刻质点在$A$处，在$t + \Delta t$时刻质点运动到$B$处，$A , B$两点的位矢分别由$r_{1}$和$r_{2}$表示，质点在$\Delta t$时间间隔内位矢内的增量

$$
\Delta r = r_{1} - r_{2}
$$

![Screenshot_20230307_154452.jpg](https://img1.imgtp.com/2023/03/07/KvOlwV81.jpg)

这种增量称为位移，它是描述物体位置变动大小和方向的物理量，如图，就是由起始位置$A$指向$B$的矢量

##### 位移的大小

位移的模只能记作$|\Delta r|$ 不能记作$\Delta r$， $\Delta r$ 通常表示两个位矢的模的增量，即

$$
\Delta r = |r_{2}| - |r_{1}|
$$

而$|\Delta r|$表示位矢增量的模，在通常情况下$|\Delta r| \neq \Delta r$。

在直角坐标系中，位移的表达式为

$$
\Delta r = (x_{2} - x_{1})i + (y_{2} - y_{1}) j + (z_{2} - z_{1})k = \Delta xi + \Delta yj + \Delta zk
$$

位移的模为

$$
|\Delta r| = \sqrt{(x_{2} - x_{1})^2 + (y_{2} - y_{1})^2 + (z_{2} - z_{1})^ 2}
$$

位移和路程的单位均是长度单位，国际单位制中为$m$

#### 速度

假设在时刻$t$到时刻$t + \Delta t$这段时间内，质点的位移为$\Delta r$，那么$\Delta r 和 \Delta t$的比值，称为质点在时刻$t$附近$\Delta t$ 时间内的`平均速度`即

$$
\bar{v} = \frac{\vec{AB}}{\Delta t} = \frac{\Delta r}{\Delta t}
$$

这就是说，平均速度的方向与位移$\Delta r$的方向相同，平均速度的大小与在相应的时间$\Delta t$内单位时间的位移大小相同

如果要精确地知道质点在某一时刻或某一位置的实际运动情况，则应使$\Delta t$尽量小，即$\Delta t \rightarrow 0$，用平均速度的极限值---瞬时速度来描述

$$
v = \lim\limits_{\Delta t \to 0} \frac{\Delta r}{\Delta t} = \frac{dr}{dt}
$$

可见，速度等于位矢对时间的一阶导数  
速度的方向就是$\Delta t$趋近于 0 时，平均速度$\frac{\Delta r}{\Delta t}$或位移$\Delta r$的极限方向，即沿质点所在处轨道的切线方向，并指向质点前进的一方

##### 速率

速率是标量，等于质点在单位时间内所行经的路程，而不考虑质点运动的方向  
平均速率和平均速度不能等同看待，例如，在某一段时间内，质点环行了一个闭合路径，显然质点的位移等于 0，平均速度也为 0，而质点的平均速率不等于 0

虽然如此，但在$\Delta t \rightarrow 0 $的极限条件下，曲线弧$\widehat{AB}$的长度$\Delta s$与线段$AB$的长度$|\Delta r|$相等，即在$\Delta t \rightarrow 0$时，$ds = |dr|$，所以顺势速率

$$
v = \lim\limits_{\Delta t \to 0} \frac{\Delta s}{\Delta t} = \frac{ds}{dt} = \frac{|dr|}{dt} = |v|
$$

`即瞬时速率就是瞬时速度的模`

在直角坐标系中，速度可以表示成

$$
v = \frac{dr}{dt} = \frac{dx}{dt}i + \frac{dy}{dt}j + \frac{dz}{dt}k = v_{x}i + v_{y}j + v_{z}k
$$

式中，$v_{x} = \frac{dx}{dt} , v_{y} = \frac{dy}{dt} , v_{z} = \frac{dz}{dt}$分别叫做速度在$x , y , z$轴的分量，这是速度的模可以表示成

$$
v = |v| = \sqrt{v_{x}^2 + v_{y}^2 + v_{z}^2}
$$

#### 加速度

#### 习题

例题 1. 已知某点的运动方程为 $r(t) = x(t)\vec{i} + y(t)\vec{j}$ , 其中 $x(t) = 3\sin{{\pi \over 6}t}, y(t) = 3\cos{{\pi \over 6}t}$ , 求质点的轨道方程 [例题 1 答案](#1_1.2_problem1)

## 4. 机械振动与机械波

### 4.1 简谐振动的动力学特征

#### 1. 弹簧振子模型

![Screenshot_20230307_162513_com.newskyer.draw.jpg](https://img1.imgtp.com/2023/03/07/pYF7NBHE.jpg)

如图所示，将弹簧振子水平放置，使振子在水平官话的支撑面上振动，以弹簧处于自然状态的稳定平衡，位置为坐标原点，当振子偏离平衡位置的位移为$x$，其受到的弹簧力作用为

$$
F = -kx
$$

$k$为刚度系数，符号表示弹力的方向与振子的位移相反

振子的微分方程为

$$
-kx = m \frac{d^2x}{dt^2}
$$

$$
\omega ^2 = \frac{k}{m} = (2\pi f)^2
$$

$$
\frac{d^2x}{dt^2} + \omega ^2x = 0
$$

$$
\omega = 2 \pi v = \frac{2\pi}{T} = \sqrt{\frac{k}{m}}
$$

### 4.2 简谐运动的方程

该微分方程

$$
\frac{d^2x}{dt^2} + \omega ^2x = 0
$$

的解为

$$
x = A\cos (\omega t + \phi_{0})
$$

$$
\omega = 2 \pi v = \frac{2\pi}{T} = \sqrt{\frac{k}{m}}
$$

##### 相位和初相位

$$
\phi = \omega t + \phi_{0}
$$

##### 旋转矢量图

将$x = A\cos (\omega t + \phi)$ 映射到几何图形上
![Screenshot_20230310_081139_com.newskyer.draw.jpg](https://img1.imgtp.com/2023/03/10/RSKkMmpc.jpg)

例题 1. 已知一个质点沿$x$轴方向作简谐运动，振幅$A = 0.06m$，周期$T = 2s$，初始时刻质点位于$x_{0} = 0.03m$处且向$x$轴正方向运动。求： (1)初相位 (2)在$x = -0.03m$处且向$x$轴负方向运动时物体回到平衡位置所需要的最短时间[例题 1 答案](#4_4.2_problem1)

### 4.4 机械波的形成与传播

#### 1. 波动

- 机械振动在连续`介质`内的传播叫作机械波
- 电磁振动在真空或介质中的传播叫做电磁波

#### 2. 机械波的产生条件

1. 有做机械振动的物理(波源)
2. 有连续的介质(气体、固体、液体)

#### 3. 横波与纵波

1. 横波
   - 振动方向与传播方向垂直的波叫做`横波`
   - 光波
2. 纵波
   - 振动方向与传播方向平行的波叫做`纵波`
   - 可以在固体、液体、气体中传播(声波)

![IMG_20230315_102023_edit_139172637865397.jpg](https://img1.imgtp.com/2023/03/15/QLg4nlAz.jpg)

> 由波的传播方向向前看去，前面各质点的振动相位都依次落后于波源的振动相位

#### 4. 描述波动的三个物理量

##### 1. 波速

波动是振动状态的传播，振动状态在单位时间内传播的距离叫做`波速`，因此波速又称`相速`，用`u`表示  
对于机械波，`通常由介质的性质决定`

$$
u = \frac{\lambda}{T} =\lambda \nu \\
\lambda = \frac{u}{\nu} = T u
$$


##### 2. 波动周期和频率
> 只决定波源的振动

波动周期是指一个完整波形通过介质中某固定点所需的时间,用$T$表示，周期的倒数叫`频率`，波动频率即为单位时间内通过介质中某固定点完整波的数目，用$\nu$表示.  
由于波源每完成一次振动，就有一个完整的波形传播出去，由此可知  
`当波源相对于介质静止时，波动周期即为波源的振动周期，波动频率即为波源的振动频率`  
波动周期$T$与频率$\nu$之间亦有  
$$
T = \frac{2\pi}{\omega} = \frac{1}{\nu}
$$


##### 3. 波长

同一波线上相邻的相位差为$2\phi$的两质点之间的距离叫做波长，用$\lambda$表示  
当波源做一次全振动后，波传播的距离就等于一个波长。因此波长反映了波的空间周期性  
显然，波长与波速、周期、频率的关系为

$$
\lambda = u T = \frac{u}{\nu}
$$



### 4.5 平面间谐波的波函数
![Screenshot_20230315_104207_com.newskyer.draw.jpg](https://img1.imgtp.com/2023/03/15/aaGkoJ0L.jpg)

设一平面间谐波，在理想介质中沿$x$轴正向传播，$x$轴即为某一波线，在此波线上任取一点为坐标原点，并在原点振动相位为0时开始计时
则原点的振动方程为

$$
y_{0} = A \cos \omega t
$$

设P为$x$轴上任一点，其坐标为$x$，而用$y$表示该处质点偏离平衡位置的位移，求P点的振动方程  

设波动在介质中的传播速度为$u$，则原点的振动状态传到P点所需要的时间为$\Delta t = \frac{x}{u}$. 因此，P点在t时刻将重复原点在$t\longleftrightarrow\frac{x}{u}$时刻的振动状态，即P点在$t$时刻的振动方程为

$$
y = A\cos \omega   \left(t - \frac{x}{u}\right) 
$$

该式就是`沿x轴正向传播的平面间谐波的波函数`


> 式中的$-\frac{x}{u}$也可理解为P点的振动落后于原点的振动时间


如果P点的振动落后于原点振动的时间，显然，这列波若沿$x$轴负方向传播，则P点的振动状态超前于原点的振动状态，超前的时间为$+\frac{x}{u}$，此时P的振动方程为
$$
y = A\cos \omega \left(t + \frac{x}{u}\right)
$$

---

## 习题答案

### 1.质点运动学

#### 1.2 位矢 位移 速度 加速度

<span id='1_1.2_problem1'></span>

例题 1.

$$
{y(t) \over x(t)} = \sqrt{3} \\
轨道方程：y = \sqrt{3} x \\
\\
由圆周运动的分量方程知：\\
x = R\sin{\omega t}, y = R\cos{\omega t}\\
\\
轨道方程可归纳为：\\
x^2 + y^2 = 9
$$

### 4. 机械振动与机械波

#### 4.2 简谐运动方程

<span id='4_4.2_problem1'></span>

例题 1.
(1)

$$
由题意得

\omega = \frac{2\pi}{T} \\
$$

由题意得，初相位在第四象限
![Screenshot_20230310_083845_com.newskyer.draw.jpg](https://img1.imgtp.com/2023/03/10/l5ALF4O2.jpg)

$$
所以 \phi = -\frac{\pi}{3} = \frac{5\pi}{3} \\
$$

(2)
由题意得，质点位于第二象限的$M_{0}$,移动到平衡位置$M_{2}$
![Screenshot_20230310_085951_com.newskyer.draw.jpg](https://img1.imgtp.com/2023/03/10/rcyqipYq.jpg)$$

$$
由图可得 \theta = \frac{\pi}{3} \\

\omega \Delta t = \frac{\pi}{3} + \frac{\pi}{2} = \frac{5\pi}{6} \\

所以\Delta t = \frac{5}{6}s
$$
