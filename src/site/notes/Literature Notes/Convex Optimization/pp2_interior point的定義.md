---
{"dg-publish":true,"permalink":"/literature-notes/convex-optimization/pp2-interior-point/","dg-note-properties":{}}
---

## 敘述
如果在集合C內之一點，存在一個以該點為球心且半徑為 r >0 的球體，使得該球體仍在集合C內，則該點為interior point.
## 數學表示
$$
\mathbf{x} \text{ is a interior point} \Leftrightarrow \exists B = \{\mathbf{y}\mid ||\mathbf{y-x}|| <r\}\subseteq C
$$
集合內所有的interior points形成之集合為 $\mathbf{int} \ C$
## 直觀理解
取集合內之一點為圓心，如果存在一球在C內部，則該點就是內部點

recall: 
