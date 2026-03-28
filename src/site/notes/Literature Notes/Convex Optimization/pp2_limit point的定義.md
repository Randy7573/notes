---
{"dg-publish":true,"permalink":"/literature-notes/convex-optimization/pp2-limit-point/","dg-note-properties":{}}
---

## 定義敘述
如果一個點被稱為一個集合中的limit point，代表此集合當中存在一個序列收斂於這個點：
$$
\exists \{\mathbf{p_{i}}\}_{i=1}^{\infty} \in C \text{ that converges to } \mathbf{p} 
$$
$\mathbf{p_{i}} \neq \mathbf{p}$ (排除孤立點自身形成的序列)
## 直觀理解
假如集合C是一個不規則實心狀集合：
* 任取內部一點，周圍都有點無限靠近此點，因此必能找到一個元素列逼近於此點，此點即為極限點。
* 而在邊界上，亦有內部之點無限靠近此點，因此必能找到一個序列無限逼近此點，邊界點亦為極限點。
* 即使集合Ｃ不包含邊界，但邊界上的點亦有內部的點逼近，因此仍是極限點。
* 假如集合內存在一點孤立點，即neighborhood沒有其他元素，則不是limit point.