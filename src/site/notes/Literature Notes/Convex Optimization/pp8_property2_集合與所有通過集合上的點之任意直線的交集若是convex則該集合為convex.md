---
{"dg-publish":true,"permalink":"/literature-notes/convex-optimization/pp8-property2-convex-convex/","dg-note-properties":{}}
---

## 定理敘述:
一個集合C是convex的 若且唯若 集合C上任意點在任意方向形成的所有直線，與集合C交集亦為convex的。
$$
C \subseteq \mathbb{R}^{n} \text{ is convex} \Leftrightarrow C \cap \mathcal{L}(\mathbf{x}_{0},\mathbf{v}) \text{ is convex}
$$
$\mathbf{v}$: 方向向量
## 直觀理解
只要穿越集合C的任何直線與C的交集沒有出現斷裂則可以證明C是convex set.
將原本的高維驗證convex問題降到一維

## 證明: 
($\Rightarrow$) 已知集合C是convex set，任意直線也是convex set (因為直線上任意兩點形成之線段仍在直線上)，兩個convex set之交集亦為 convex set

($\Leftarrow$) 證明集合 C 是convex set $\equiv$ 證明集合C上任兩點之線段在C中即：
$$
\theta\mathbf{x_{1}}+(1-\theta)\mathbf{x_{2}} \in C
$$
* 已知集合C上任意點在任意方向形成之所有直線與集合C交集是convex set
  (代表此交集中的任兩點形成之線段包含在該交集內)
1. 取集合C中的任兩點$\mathbf{x_{1},x_{2}}$ 
2. 此兩點必有一條直線涵蓋此兩點$\mathcal{L(\mathbf{x_{0},v})}$，$\mathbf{x_{0} = x_{1}, v = x_{2}-x_{1}}$ 
3. 線段 $\theta\mathbf{x_{1}}+(1-\theta)\mathbf{x_{2}}$ 必定包含在直線$\mathcal{L}$中
4. 直線和C交集是convex set 代表 線段 $\in$ 直線與C的交集 $\subseteq$ C
5. 得證 C is convex 