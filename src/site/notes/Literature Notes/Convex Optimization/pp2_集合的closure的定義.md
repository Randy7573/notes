---
{"dg-publish":true,"permalink":"/literature-notes/convex-optimization/pp2-closure/","dg-note-properties":{}}
---

Recall: [[Literature Notes/Convex Optimization/pp2_limit point的定義\|pp2_limit point的定義]]
# 定義敘述
一個集合的closure定義為所有limit point形成的集合，寫為 $\mathbf{cl}\ C$

# 直觀理解
使集合C是一個不包含邊界的實心不規則體
* $\mathbf{cl }\ C$ 則為集合C與其邊界形成的集合
* 即使集合C不包含邊界，但邊界亦是 limit point，即集合C之邊界周圍存在點無限接近邊界。
就像是果實(集合)的closure為果實(集合)以及皮(邊界)

# 等效表示
$\mathbf{cl}\ C = \mathbb{R}^{n} \setminus \mathbf{int}\ \{\mathbb{R}^{n} \setminus C\}$
## 直觀理解
* $\mathbf{int}\ \{\mathbb{R}^{n} \setminus C\}$ : $R^n$空間中具有C的缺口，並且因為取內部點，所以內部缺口的邊界沒有包含在此集合中。
* $\mathbb{R}^{n} \setminus \mathbf{int}\ \{\mathbb{R}^{n} \setminus C\}$: 將$R^{n}$空間去除上述集合，則可得到包含C的邊界點和C中所有元素的集合。
