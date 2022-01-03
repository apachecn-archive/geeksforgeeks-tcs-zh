# 群论中的商群

> 原文:[https://www . geesforgeks . org/商群理论/](https://www.geeksforgeeks.org/quotient-group-in-group-theory/)

**先决条件:** [群体知识](https://www.geeksforgeeks.org/groups-discrete-mathematics/)[陪集](https://www.geeksforgeeks.org/cosets-in-mathematics/)。

**简介:**
我们可以说“o”是集合 G 上的二进制运算如果:G 是非空集合& G * G = { (a，b) : a，b∈ G }和 o:G * G–>G .这里，aob 表示函数/运算 o 下的有序对(a，b)的图像
**例–**“+”在 G(任意非空集合)上称为二进制运算如果:&只有当:a+b∀ a，b ∈G 和 a+b 每次相加得出相同的结果。

**代数结构:**
配备 1/多二进制运算的非空集合 G 称为代数结构。
**例–**a .(N，+)和 b. (R，+，。)，其中 N 是一组自然数& R 是一组实数。给你。(点)指定乘法运算。

**GROUP :**
一种代数结构(G，o ),其中 G 是非空集合&“o”是在 G 上定义的二进制运算，如果二进制运算“o”满足以下性质，则称为 GROUP–

闭包–a∈G，b∈G = > AOB∈G；∀ a，b ∈ G

1.  **关联性–**(AOB)oc = ao(BOC)；∀ a，b，c ∈ G
2.  **身份元素–**在 G 中存在 e，使得 AOE = eoa = a；∀ a ∈ G(例如–例如，恒等式为 0)。
3.  **逆的存在–**对于每个元素 a∈G；存在逆(a-1)∈ G，使得:AOA-1 = a-10a = e

**阿贝尔群:**
其中 G 是非空集的代数结构(G，o)&‘o’是在 G 上定义的二元运算，如果它是一个群(即它满足 G1，G2，G3 & G4)并且另外满足

```
Commutative - aob = boa ∀ a,b ∈ G
```

**正规子群:**
让 G 成为一个艾伯连群&G 中的成分用多重性来表示。
设 H 为 G 的任意子群，若 x 为 G 的任意元素，则 Hx 为 G 中 H 的右陪集& xH 为 G 中 H 的左陪集，则 G 称为正规子群，若–

```
Hx = xH ; ∀x ∈ G or
xhx-1 ∈ H ; ∀x ∈ G & h ∈ H
```

**商群:**
设 G 为任意群&设 N 为 G 的任意**正规子群**，如果‘a’是 G 的元素，那么 an 是 G 中 N 的左陪集，既然 N 在 G 中是正规的，aN = Na(左陪集=右陪集)。
我们可以说 Na 是 G 中 N 的陪集
G/N 表示 G 中 N 的所有陪集的集合

```
Quotient/Factor Group = G/N = {Na ; a ∈ G } = {aN ; a ∈ G} (As aN = Na)
```

如果 G 是一个群& N 是 G 的正规子群，那么，G 中 N 的所有陪集的集合 G/N 相对于 G/N 中的陪集的乘积是一个群，称之为 G 乘 N 的商/因子群
有时称之为‘G 模 N 的剩余类’。
如果组中的成分是加法，'+'，那么 G/H 定义为:

```
Quotient/Factor Group = G/N = {N+a ; a ∈ G } = {a+N ; a ∈ G} (As a+N = N+a)
```

**注–**G/N 的恒等式元素为 N.
**例 1–**考虑加模为 6 的群 G，其中 G = {0，1，2，3，4，5}。设 N = {0，3)，
则商/因子组为:
G/N = { aN；a ∈ G } = { a{0，3 }；a∑{ 0，1，2，3，4，5}}
= {0{0，3}，1{0，3}，2{0，3}，3{0，3}，4{0，3}，5{0，3 } }
= {(0+0)mod6，(0+3) mod6 }，{ (1+0) mod6，(1+3) mod6 }，{ (2+0) mod6，(2+3) mod6 }，{ (3

**例 2–**让 G = {1，-1，I，-i }和 H = {1，-1 }；h 是二元运算'，'中 G 的正规子群。商群会是什么；G/H？
G/N = { aN；a ∈ G } = {a{1，-1 }；a∑{ 1，-1，I，-i}
= {1。{1,-1}, -1.{1，-1}，i{1，-1}，-i.{1，-1}}
={{1.1，1。-1}, {-1.1,-1.-1}、{i.1，I-1}、{-i.1，-I-1} }
= { { 1，-1}、{-1，1 }、{i，-i}、{-i，i}}
={ {1，-1 }、{i，-i}}
换句话说，我们可以说，如果 G 是一个群& N 是 G 的正规子群，那么 G 中 N 的所有陪集的 G/N 连同由下式定义的二元组合:

```
NaNb = Nab ; where Na ∈ G/N, Nb ∈ G/N is a group.
```

G/N 被称为 G 乘 N 的商群。

**商/因子组的属性:**

1.  如果 N 是有限群 G 的正规子群，那么–
    O(G/N)= O(G)/O(N)，其中:O(G/N)=>G 中 N 的不同右/左陪集数
2.  如果 N 是有限群 G 的正规子群，使得 G 中 N 的指数是素数，则因子群 G/N 是循环的。
3.  阿贝尔群的因子群是阿贝尔群，但反之则不是。
4.  循环群的每个因子群都是循环的，但反之则不然。