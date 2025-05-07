## Exercise 1

尝试回答下列问题，把答案写在 `B-graph-lab-1.md` 中的对应部分

1. 在一般的算法题中，我们常使用那种方式来存图。
2. 如何使用并查集判断一个无向图有几个联通块

## Exercise 2

完成下列习题，并把 AC 代码复制到 `B-graph-lab-1.md` 中

- [How Many Tables](https://vjudge.net/problem/HDU-1213) 并查集
- [最长路](https://vjudge.net/problem/%E6%B4%9B%E8%B0%B7-P1807) 树的直径
- [车站分级](https://vjudge.net/problem/%E6%B4%9B%E8%B0%B7-P1983) 拓扑排序
- [Cow Picnic S](https://vjudge.net/problem/%E6%B4%9B%E8%B0%B7-P2853) 图的遍历
- [排序](https://www.luogu.com.cn/problem/P1347) 拓扑排序
- [会议](https://vjudge.net/problem/%E6%B4%9B%E8%B0%B7-P1395) 树的重心
- [村村通](https://vjudge.net/problem/%E6%B4%9B%E8%B0%B7-P1536) 并查集

## Exercise 3 欧拉回路

> 给出一个无向图，是否可以从一个点出发，不重复走同一条边，把所有的边走完呢？

这里就涉及到一个著名的[柯尼斯堡七桥问题](https://zh.wikipedia.org/wiki/%E6%9F%AF%E5%B0%BC%E6%96%AF%E5%A0%A1%E4%B8%83%E6%A1%A5%E9%97%AE%E9%A2%98)了

请自己阅读资料，回答下面问题：

1. 如何判断一个图是否能一笔画走完？
2. 如何确定起点？

然后完成下列习题：

- [The Necklace](https://vjudge.net/problem/UVA-10054#author=WMY520)
- [Wow! Such String!](https://vjudge.net/problem/HDU-4850#author=GPT_zh)

## Exercise 4 并查集拓展

并查集有很多种拓展，能实现多种高级的操作，比较常见的拓展有，拓展域并查集，带权并查集，启发式合并，下面让我们来学习吧

**拓展域并查集**

这里找了一篇博客，当然也叫种类并查集，能解决一些 "敌人的敌人是我的朋友" 的问题

[算法学习笔记(7)：种类并查集](https://zhuanlan.zhihu.com/p/97813717)

然后解决下面的题目

- [关押罪犯](https://vjudge.net/problem/%E6%B4%9B%E8%B0%B7-P1525)
- [食物链](https://vjudge.net/problem/%E6%B4%9B%E8%B0%B7-P2024)

**带权并查集**

并查集可以看成一颗树，可以给树边以边权，在路径压缩的时候维护这些边权

[算法学习笔记：并查集与带权并查集](https://zhuanlan.zhihu.com/p/662298315)

- [银河英雄传说](https://vjudge.net/problem/%E6%B4%9B%E8%B0%B7-P1196)
