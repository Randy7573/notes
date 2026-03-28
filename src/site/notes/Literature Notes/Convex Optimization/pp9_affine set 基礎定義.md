---
{"dg-publish":true,"permalink":"/literature-notes/convex-optimization/pp9-affine-set/","dg-note-properties":{}}
---

## 敘述
若一個集合內的任意兩點滿足以下表示，則此集合為affine set：
$$
\theta x_{1} + (1-\theta) x_{2} \in C\ , \forall \theta \in \mathbb{R}, x_{1}, x_{2} \in C
$$
## 直觀理解
若集合內任意兩點形成之 ==直線== 都落在該集合內，則該集合為affine set。

## 與 convex 差異
在convex中要求 $\theta \in [0,1] \to$ 線段
但affine要求 $\theta \in \mathbb{R} \to$ 直線 