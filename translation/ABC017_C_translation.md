### 题意 

高桥君非常喜欢打电动。

现在他在玩的这个游戏中有 $N$ 个遗迹，你可以按照你喜欢的顺序去探索这些遗迹（不一定都要探索）。在探索遗迹的过程中会获得宝石，游戏中一共有 $M$ 种宝石。

当你探索过第 $i(1\le i \le N)$ 个遗迹后，你的得分将增加 $s_i$，同时，你将得到所有种类编号在 $l_i$ 到 $r_i$ 之间的宝石各一个，但是再一次探索同一个遗迹的话，你将什么都无法得到。

获得的宝石无法被丢弃，当所有种类的宝石都获得之后，会复活魔王导致得分清零且不再能得分。

高桥君想要得到尽可能高的分数，请求出在不复活魔王的情况下，可以得到的分数最高能是多少。

### 数据范围

- $1\le N \le 10^5$
- $1\le M \le 10^5$
- $1\le l_i,r_i \le M$
- $1\le s_i \le 5\times 10^3$
- 所有读入的数值都是整数。

---

### 输入格式

输入是由标准输入提供的，格式如下：

```
N M
l1 r1 s1
l2 r2 s2
:
lN rN sN
```

### 输出格式

一行一个整数，表示你的答案。**注意在最后输出一个换行**。

---

### 样例输入1

```
4 6
1 3 30
2 3 40
3 6 25
6 6 10
```

### 样例输出1

```
80
```

### 样例解释1

按照下面的顺序探索以下三个遗迹：

- 探索遗迹 $1$，得到 $30$ 分，并且获得宝石 $1,2,3$。
- 探索遗迹 $2$，得到 $40$ 分，并且获得宝石 $2,3$。
- 探索遗迹 $4$，得到 $10$ 分，并且获得宝石 $6$。

最后获得了 $1,2,3,6$ 四中种类的宝石，没有复活魔王，得到最高得分 $80$。

---

### 样例输入2

```
2 7
1 3 90
5 7 90
```

### 样例输出2

```
180
```

### 样例解释2

探索所有的遗迹也不会复活魔王。

---

### 样例输入3

```
1 4
1 4 70
```

### 样例输出3

```
0
```

### 样例解释3

探索这个遗迹会立即让魔王复活，你不能探索任何遗迹。