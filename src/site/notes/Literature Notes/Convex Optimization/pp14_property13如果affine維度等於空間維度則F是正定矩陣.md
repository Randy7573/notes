---
{"dg-publish":true,"permalink":"/literature-notes/convex-optimization/pp14-property13-affine-f/","dg-note-properties":{}}
---

recall: 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/literature-notes/convex-optimization/pp14-affine-mapping/#" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



## 定義
一個在$\mathbb{R}^n$空間中的p維橢球可以寫為對$\mathbb{R}^n$空間中以原點為圓心半徑為$r$之歐幾里德球體的affine mapping:
$
E = \{\mathbf{Fx}+\mathbf{c} | \mathbf{x} \in B\}
$
$B = \{ \mathbf{x} | \| \mathbf{x}\|_{2} \leq 1\}$
$rank(F) = p = \text{affdim}(E)$


</div></div>

## 敘述
如果p=n，則可以假定，不失一般性，F是對稱正定矩陣
## 證明
根據SVD, $F = U\Sigma V^T$ 或可拆解成 $F = U^T\Sigma V$，為了後續證明需要採取後者。
則橢球可以表示為 $E = U^T\Sigma VB+c$
因為球旋轉後仍是球($VB=B$)$\Rightarrow E=U^T\Sigma B+c$
又$UB = B \Rightarrow E = U^T\Sigma UB+c$
所以對於同樣的橢球，可以取$F = U^T\Sigma U$
觀察到其對稱形式，利用此證明其半正定性質：
$\mathbf{v^T}F\mathbf{v}=\mathbf{v}^{T}U^{T}\Sigma U\mathbf{v}=\mathbf{v}^{T}U^{T} \sqrt{ \Sigma } \sqrt{ \Sigma }U\mathbf{v} = \|\sqrt{ \Sigma } U\mathbf{v}\|^{2}_{2}\geq 0$
1. 已知p=n (滿秩)，代表所有奇異值數量都大於0，所以特徵值必不為零。
2. 又從PSD知所有特徵值都大於等於0，即為PD。

## 直觀意義
若p=n，代表歐幾里德球體在所有維度都有被拉伸，所以若歐幾里德球體被一個正定矩陣affine mapping，則其不會有被降維的問題。
