---
{"dg-publish":true,"permalink":"/literature-notes/convex-optimization/convex-hull/","dg-note-properties":{}}
---

當一個集合 $C$ 內的元素是連續的時候就無法使用[[Literature Notes/Convex Optimization/convex hull 是包含數個元素的最小 convex 集合\|convex hull]]當中提到的定義。
從convex hull的基本定義出發：
* 包含其中集合內所有元素的最小convex set
以及 convex set 的特性
* convex set的交集仍是 convex

從上述兩點可知，只要找到所有包含集合 $C$ 的 convex set，並取交集，則可以得到包含C的最小convex set.

數學表示如下:
$$
\begin{align}
\mathbf{conv}\ C \triangleq \cap_{i\in \mathcal{F}} \ C_{i} 
\end{align}
$$
$\{C_{i}\mid i\in\mathcal{F}\}$ 收集了所有包含C的convex set