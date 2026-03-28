---
{"dg-publish":true,"permalink":"/literature-notes/convex-optimization/pp8-property3-c-convex-closure-convex/","dg-note-properties":{}}
---

## 數學表示
$$
\text{If C is convex set then } \mathbf{cl}\ C \text{ is also convex set}
$$
## 直觀理解
$\mathbf{cl}\ C$ 外型與C一致，只是將C的邊界也納入集合中，
因此若C為convex set，即兩點間線段在集合中，則任意兩邊界上的點間的線段也必定在C內部。

## 數學證明
證明 cl C 是convex set，等效於證明 cl C中任取兩點的線段亦在 cl C 中
$$
\begin{align}
&\text{Let } \mathbf{x}, \mathbf{y} \in \mathbf{cl}\ C \text{ and } \theta \in [0,1] \\[1mm]
&\text{W.T.S }\ \theta \mathbf{x} + (1-\theta)\mathbf{y} \in \mathbf{cl}\ C  \Leftrightarrow \text{exist a sequence converge to } \theta \mathbf{x} + (1-\theta)\mathbf{y}  \\[1mm]
&\because \mathbf{x},\mathbf{y} \in \mathbf{cl}\ C \therefore \exists \{ x_{i} \}\in C,\{ y_{i} \} \in C \text{ converges to }\mathbf{x}, \mathbf{y} \text{ resp.} \\[1mm]
&\text{Since C is convex set, so that the line segment between }\mathbf{x}_{i},\mathbf{y}_{i} \text{ is also in C} \\[1mm]
&\text{That is, }\ \{ \mathbf{z}_{i} \mid \mathbf{z}_{i} = \theta \mathbf{x}_{i} + (1-\theta)\mathbf{y}_{i} \} \subseteq C \\[1mm]
&\{ \mathbf{z}_{i} \} \text{ will converge to } \theta \mathbf{x} + (1-\theta)\mathbf{y} \\[1mm]
&\text{so that } \theta \mathbf{x} + (1-\theta)\mathbf{y}  \text{ is also } \in \mathbf{cl}\ C \\[1mm]
&\text{Therefore } \mathbf{cl}\ C \text{ is convex set.}   

\end{align}$$

