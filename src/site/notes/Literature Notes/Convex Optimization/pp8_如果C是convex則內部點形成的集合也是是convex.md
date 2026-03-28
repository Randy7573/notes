---
{"dg-publish":true,"permalink":"/literature-notes/convex-optimization/pp8-c-convex-convex/","dg-note-properties":{}}
---

## 直觀理解
使C是convex set，只取其內部點，也就是剔除外殼的核心部分，convex性質會維持，因為任意兩點在內部，兩點連線亦在內部。

## 證明
根據內部點的定義，內部點存在則代表必有一球以該點為球心，並處在該集合內部。
想要證明intC是convex等效於證明intC中任兩點形成之線段亦在intC中：
* 先取intC內任意兩點，以此兩點為球心且半徑r之球體亦在C中
* 取此兩點對應之球體聯集的convex hull，則兩球中的任意兩點連線段必包含於此convex hull
* 因為C是convex，則此convex hull必包含於C[^1]
* 這兩點形成的連線段上的點為球心且同樣半徑為r的球體亦會在convex hull中，則亦包含於C中，得證。

註1:
recall: 
[[Literature Notes/Convex Optimization/pp2_interior point的定義\|pp2_interior point的定義]] 
[[Literature Notes/Convex Optimization/convex hull 是包含數個元素的最小 convex 集合\|convex hull 是包含數個元素的最小 convex 集合]]

[^1]: 大convex set內部之數個小convex set的聯集之convex hull亦在大convex set中：因為小convex set間的連線段亦在大convex set內，convex hull則是將這些連線段納入集合的結果。
