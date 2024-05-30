# 逆行列
$$
AA^{-1} = E
$$

ある行列Aがあったときに上の式を満たす行列が逆行列です。
また、逆行列が存在するときその行列は**正則**であるという。

##　逆行列の例

$$
A = 
\begin{bmatrix}
    2 & -1 \\
    -1 & 1
\end{bmatrix} \\
\\
X = 
\begin{bmatrix}
    1 & 1 \\
    1 & 2
\end{bmatrix}
$$
上のような行列があったときに
$$
AX = \begin{bmatrix}
    1 & 0 \\
    0 & 1
\end{bmatrix}
= E
$$
となるためAは正則である。また、Aの逆行列は以下のようになる。
$$
A^{-1}=
\begin{bmatrix}
    1 & 1 \\
    1 & 2
\end{bmatrix}
$$

## 逆行列を脳死で求める公式
導出過程はTeamsにあったと思うので脳死で公式Done

まず正方行列Aがあったときに以下の条件が守られているようにしてください
$$
A = 
\begin{bmatrix}
    a & b \\
    c & d
\end{bmatrix}\\
\\
ad - bc \neq 0
$$

上の条件式が守られているときAの逆行列は以下の通りになります。
$$
A^{-1} = \frac 1 {ad-bc} 
\begin{bmatrix}
    d & -b \\
    -c & a
\end{bmatrix}
$$

なるほど、さっきの条件式が守られてない場合は**１を０で割るという矛盾が発生してしまう**からだめだよっていうことなんですね。