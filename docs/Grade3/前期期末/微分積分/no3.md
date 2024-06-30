# 三角関数の積分
ここでは少し難しい三角関数を含んだ関数の積分について考察する。


## 三角関数に関する公式をもちいる

$$
\int \sin{5x} \cos{4x}dx
$$

ここでは三角関数の積を和に直す公式を用いる。

$$
\sin{(a+b)} = \sin{a}\cos{b} + \sin{b}\cos{a} \\
\sin{(a-b)} = \sin{a}\cos{b} - \sin{b}\cos{a} \\
$$

サインの加法定理には上の２つの式がある。そしてこれらの式を足すと以下のように公式を導出することができる。

$$
\begin{align}
\sin{(a+b)} + \sin{(a-b)} &= 2\sin{a}\cos{b} \\
\sin{a}\cos{b} &= \frac 1 2 (\sin{(a+b)} + \sin{(a-b)}) \\
\end{align}
$$

この公式を問題の式に適用する。

$$
\begin{align}
\int \sin{5x} \cos{4x}dx &= \int \frac{1}{2} (\sin{9x} + \sin{(x)}) dx \\
&= \frac{1}{2}\int  (\sin{9x} + \sin{(x)}) dx \\
&= \frac{1}{2} (-\frac{1}{9} \cos{9x} - \cos{x}) \\
&= - \frac{1}{18} \cos{9x} - \frac{1}{2} \cos{x} \\
\end{align}
$$

三角関数の公式を用いることによって積分を簡単な形にすることができた。
***このように解くために三角関数に関する公式の関係や導出などについて復習するべきだろう。***

## 置換積分法と組み合わせて解く
$$
\int \frac{dx}{\sin{x}}
$$

これはlogなどを用いることで意外となんとかなりそうではある。しかしここでは置換積分法も交えたアプローチで解いていく。

$$
\sin^2{x} = 1 - \cos^2{x}
$$

このような式があったことを覚えているだろうか。今回はこれを用いるために以下のように分母と分子に**sinｘ**をかけて解いていく

$$
\begin{align}
\int \frac{dx}{\sin{x}} &= \int \frac{\sin{x} dx}{\sin^2{x}} \\ 
&= \int \frac{\sin{x}}{1-\cos^2{x}} dx \\
\end{align}
$$

ここで置換積分法を適用する。今回は**t**を**cos x**とおいた。

$$
t = \cos{x}より \\
\frac{dt}{dx} = -\sin{x} \\
dx = \frac{dt}{-\sin{x}} \\
$$

これらを代入する

$$
\begin{align}
\int \frac{\sin{x}}{1-t^2} * \frac{dt}{-\sin{x}} &= -\int \frac{dt}{1-t^2} \\
&= \int \frac{dt}{t^2-1}
\end{align}
$$

P.111にある以下の公式を適用する
$$
\int \frac{dx}{x^2-a^2} = \frac{1}{2a} \log{\lvert \frac{x-a}{x+a}\rvert}
$$
これを用いると
$$
\frac{1}{2} \log{\lvert \frac{t-1}{t+1}\rvert} = \frac{1}{2} \log{\frac{1-\cos{x}}{1+\cos{x}}}
$$
しかしこれらの公式を覚えるのは難しい。そんな人にはこれを部分分数分解によって解くことをオススメする。

$$
\frac{1}{t^2-1} = \frac{1}{2} (\frac{1}{t-1} - \frac{1}{t+1})
$$
このようにするとそれぞれを積分するだけでよくなるので先程と同じような答えにたどり着けるだろう。