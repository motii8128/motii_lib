# 様々な行列

##　零行列
以下のように含まれる成分がすべて０である行列は零行列よ呼ばれる。

$$
\begin{bmatrix}
    0\quad 0\quad 0 \\
    0\quad 0\quad 0 \\
    0\quad 0\quad 0 \\
\end{bmatrix}
$$

## 行ベクトル
下のように行が１つしかないときにその行列は行ベクトルと呼ばれる

$$
\begin{bmatrix}
    a\quad b\quad c \\
\end{bmatrix}
$$

## 列ベクトル
行ベクトルの列バージョン

$$
\begin{bmatrix}
    x \\
    y \\
    z \\
\end{bmatrix}
$$

## 正方行列
行の数と列の数が等しい行列のことを正方行列と呼ぶ

$$
\begin{bmatrix}
    2a-3b \quad c-d \\
    a+2b \quad 3c+5d
\end{bmatrix}
=
\begin{bmatrix}
    -5\quad 5 \\
    8\quad -17
\end{bmatrix}
$$

上式を解くと**a = 2, b = 3, c = 1, d = -4**となります。
また、上の行列を変換すると以下のような４つの式に展開できます。

$$
\begin{array}{}
2a-3b = -5 \\
a+2b = 8 \\
c - d = 5 \\
3c+5d = -17
\end{array}
$$

## 対角行列と単位行列
左上から右下にむかっての並びを**対角成分**という。そしてその対角成分以外がすべて０である行列は対角行列と言われる。

$$
\begin{bmatrix}
    4\quad 0\quad 0 \\
    0\quad 0\quad 0 \\
    0\quad 0\quad 2
\end{bmatrix}
$$

そして対角成分がすべて１である行列は単位行列と呼ばれ**E**で表す。

$$
\begin{bmatrix}
    1\quad 0\quad 0 \\
    0\quad 1\quad 0 \\
    0\quad 0\quad 1
\end{bmatrix}
$$

$$
\begin{bmatrix}
    1\quad 0 \\ 
    0\quad 1
\end{bmatrix}
$$