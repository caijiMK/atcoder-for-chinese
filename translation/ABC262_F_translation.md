## 题意

给定一个排列 $p$。你可以最多执行 $k$ 次操作。

- 删除一个数。

- 将 $p$ 中末尾的数移到开头。

找出字典序最小的 $p$。

## 数据范围

- $1 \leq n \leq 2 \times 10^5$

- $0 \leq k \leq n-1$

- $1 \leq p_i \leq n$

- 保证 $p$ 是个排列。

## 输入格式

第一行两个整数 $n$ 和 $k$。

第二行 $n$ 个整数表示排列 $p$。

## 输出格式

输出一个序列表示字典序 $p$。

## 样例

### 样例输入1

```
5 3
4 5 2 3 1
```

### 样例输出1

```
1 2 3
```

### 样例解释1

- 将 $4$ 删去。

- 将 $1$ 移到最前面。

- 将 $5$ 删去。

### 样例输入2

```
3 0
3 2 1
```

### 样例输出2

```
3 2 1
```



### 样例输入3

```
15 10
12 10 7 2 8 11 9 1 6 14 3 15 13 5 4
```

### 样例输出3

```
1 3 4 7 2 8 11 9
```


