# 巡回行列
## 定義
以下の形で表されるような $n\times n$ 行列を巡回行列という．

$$C=
\begin{bmatrix}
c_0 & c_1 & \ldots & c_{n-2} & c_{n-1}\\
c_{n-1} & c_0 & \ldots & c_{n-3} & c_{n-2} \\
&&\vdots\\
c_1 & c_2 & \ldots & c_{n-1} & c_0
\end{bmatrix}
$$

つまり任意の行がその上の行の右シフトになっている行列である．
(左シフトも巡回行列だが，ここでは右シフトのみを考えることとする．)

## 固有値・固有ベクトル
上記の行列Cの固有値とそれに対応する固有ベクトルは， $\zeta=\exp\left(\frac{2\pi i}{n}\right)$ とすると，以下の形で表せる．

$$
\text{固有値：}\lambda_k=\sum_{j=0}^{n-1}c_j(\zeta ^k)^j\hspace{5em}(k=0,1,\ldots,n-1)
$$

$$
\text{固有ベクトル：}\mathbf{e}_k=[1\ \zeta^k\ \ (\zeta^k)^2\ \ldots\ (\zeta^k)^{n-1}]
$$

## 性質
巡回行列同士の積は可換で，同時対角化可能

$P=[\mathbf{e}_0\ \mathbf{e}_1\ \ldots\ \mathbf{e}_n-1]$ とすると， $P^{-1}=\frac{1}{n}[\mathbf{e}_0\ \mathbf{e}_n-1\ \ldots\ \mathbf{e}_1]$

$A\subset \lbrace 0,1,\ldots,n-1\rbrace$ とすると， $|\sum_{a\in A}\zeta^a|\leq |1+\zeta+\ldots+\zeta^{|A|-1}|$
