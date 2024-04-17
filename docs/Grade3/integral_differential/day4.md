# Day 4
2024/4/16

# Easy way to solve definite integrals
Definite integrals can be easily solved without using formulas like the one from the other day.

It can be found by calculating the primitive function of a given function and subtracting the result when the lower end number is entered into the function from the result when the upper end number is entered into the function.

$$ \int_{a}^{b}f(x) dx = F(b) - F(a)$$

For example, Question6(P.93)

$$
\begin{align}
\int_{0}^{\frac \pi 2} cosx dx &= [sinx]^{\frac \pi 2}_0 \\
&= 1 - 0 \\
&= 0
\end{align}
$$

# Properties of definite integral
These are some properties in **Definite Integral** like a below.

**c is constant value.**

$$ (I) \int_{a}^{b} cdx = c(b - a)$$
$$(II) \int_{a}^{b} cf(x)dx = c \int_{a}^{b} f(x)dx $$

$$(III) \int_{a}^{b} (f(x)+g(x))dx = \int_{a}^{b}f(x)dx + \int_{a}^{b} g(x)dx \\
\int_{a}^{b} (f(x)-g(x))dx = \int_{a}^{b}f(x)dx - \int_{a}^{b} g(x)dx \\
$$

$$
(IV) \int_{a}^{b} f(x)dx = \int_{a}^{c} f(x)dx + \int_{c}^{b} f(x)dx
$$