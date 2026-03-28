---
{"dg-publish":true,"permalink":"/literature-notes/convex-optimization/pp14-affine-mapping/","dg-note-properties":{}}
---

recall: [[Literature Notes/Convex Optimization/pp14_Euclidean ball的定義\|pp14_Euclidean ball的定義]]
## 定義
一個在$\mathbb{R}^n$空間中的p維橢球可以寫為對$\mathbb{R}^n$空間中以原點為圓心半徑為$r$之歐幾里德球體的affine mapping:
$$
E = \{\mathbf{Fx}+\mathbf{c} | \mathbf{x} \in B\}
$$
$B = \{ \mathbf{x} | \| \mathbf{x}\|_{2} \leq 1\}$
$rank(F) = p = \text{affdim}(E)$

## 直觀理解
affine mapping的過程是將球體對特定方向進行拉伸：
根據SVD: $\mathbf{F} = \mathbf{U}\mathbf{\Sigma}\mathbf{V^H}$
取球中任意一點$\mathbf{x} \in B$
$$\begin{align}
\mathbf{Fx} &= \mathbf{U}\mathbf{\Sigma}\mathbf{V^{H}}\mathbf{x}  \\
&= [\mathbf{u_{1}, u_{2}\dots}] \begin{bmatrix} 
\sigma_{1} & \\
&\sigma_{2} \\
&& \ddots
\end{bmatrix} 
\begin{bmatrix}
\mathbf{v_{1}^H} \\ \mathbf{v_{2}^H} \\ \vdots
\end{bmatrix}  \mathbf{x} \\
& = [\mathbf{u_{1}, u_{2}\dots}] \begin{bmatrix} 
\sigma_{1} & \\
&\sigma_{2} \\
&& \ddots
\end{bmatrix} 
\begin{bmatrix}
\mathbf{v_{1}^H}\mathbf{x} \\ \mathbf{v_{2}^H}\mathbf{x} \\ \vdots
\end{bmatrix} \tag{1} \\ 
& = [\mathbf{u_{1}, u_{2}\dots}]  
\begin{bmatrix}
\sigma_{1}\mathbf{v_{1}^H}\mathbf{x} \\ \sigma_{2}\mathbf{v_{2}^H}\mathbf{x} \\ \vdots
\end{bmatrix} \tag{2}\\
& = 
\begin{bmatrix}
\sigma_{1} \mathbf{u_{1}} (\mathbf{v_{1}^H}\mathbf{x}) \\ \sigma_{2}\mathbf{u_{2}} (\mathbf{v_{2}^H}\mathbf{x}) \\ \vdots
\end{bmatrix} \tag{3}\\
\end{align}
$$
(1) 因為V為[[Literature Notes/Convex Optimization/Unitary矩陣\|Unitary矩陣]] (行向量大小為1)，因此將其行向量與$\mathbf{x}$內積等同於將$\mathbf{x}$投影至行向量的方向且大小不變，等同於==旋轉==。
(2) 在旋轉過後的方向伸縮$\sigma_{i}$倍
(3) 最後旋轉至$u_{i}$方向

如果F是方陣且可以被EVD分解，則等同於是將球體往F之eigenvector方向拉伸eigenvalue倍。

假如p<N則是將高維度的歐幾里德球體轉換為低維度的橢球。