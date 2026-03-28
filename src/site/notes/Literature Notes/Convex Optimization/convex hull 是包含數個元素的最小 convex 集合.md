---
{"dg-publish":true,"permalink":"/literature-notes/convex-optimization/convex-hull-convex/","dg-note-properties":{}}
---

recall: [[Literature Notes/Convex Optimization/convex 集合定義_集合內任意兩點形成之線段仍在該集合內\|convex 集合定義_集合內任意兩點形成之線段仍在該集合內]]

假如有數個向量空間中的元素 (點) $\{\mathbf {s_{1}, s_{2}, s_{3}\dots,s_{n}\}, s_{i}} \in \mathbb{R}^{n}$ 
則包含以上元素的最小 convex set 則是 convex hull
定義成以下
$$
\mathbf{conv}\{ \mathbf{s_{1}} \mathbf{s_{2}}\dots,\mathbf{s_{n}}\} = 
\left\{  \sum^{n}_{i=1} \theta_{i} \mathbf{s_{i}} \mid \theta_{i} \geq 0, \sum^{n}_{i=1}\theta_{i}=1  \right\}
$$
## 直觀理解:
取集合中任意兩個點 $\mathbf{s_{i},s_{j}}$ 兩點形成之線段必在 convex hull 中，為 convex hull 其他係數都取零的情況。

## 幾何理解:
係數 $\theta_{i}$ 給每個頂點 $\mathbf{s_{i}}$ 不同的大於零的權重，總和不超過一的係數將形成由頂點形成之多面體。

推導: 可由兩點之情況由數學歸納法擴展到多點

[[Literature Notes/Convex Optimization/任意數量元素之集合的convex hull\|任意數量元素之集合的convex hull]]