
Assume the true model 
$$
y = f(x) +\epsilon
$$
$f(x) \to$ systematic component (true function)
$\ \ \epsilon\ \ \ \ \to$ random component (irreducible error)
Goal: develop techniques to know $f$ .
If someone say that the given below is a correct model or claims so
$$
f \equiv f_1(x) = b_0 + b_1 x
$$
We never would now if it is correct, we can assume and make a good guess (just as in STEM), there are no correct models but just better and better guesses; our job is to take a educated guess
$f \equiv f_2(x) = b_0 + b_1 x + b_2 x^2$                The model complexity increases 
$f \equiv f_3(x) = b_0 + b_1 x + b_2 x^2 + b_3 x^3$   as we go on increasing it s flexibility
$f \equiv f_p(x) = b_0 + b_1 x + \ldots + b_px^p$

We assume("typical common assumption"):
$$\epsilon \sim \mathcal{N}(0, \sigma^2)$$
General: $\epsilon$ is random component with $E(\epsilon) = 0$ and Var$(\epsilon) = \sigma^2$ 

### How to estimate "$f$ " ?
1. Choose/assume a functional form of $f$ :
	1. Guided by Domain Knowledge
	2. Purely Data Driven
2. Estimate $f$ by minimizing the loss function 
$$
\min_f\sum_{i=1}^n\left(y_i - f(x_i)\right)^2 \ \ \ \implies \ \ \hat f(x)
$$
Example:
$$
\begin{align*}
& \min_{b_0,\ldots,b_p}\sum_{i=1}^n\left[y_i - b_0 - b_1x_i - \ldots - b_px_i^p\right]^2\\
=& \min_{b_0,\ldots,b_p} \mathcal{S}(b_0, b_1, \ldots, b_p)\\
0 = \frac{\partial \mathcal{S}}{\partial b_0} =& 2 \sum_{i=1}^n\left[y_i - b_0 - b_1x_i - \ldots - b_px_i^p\right]. (-1)\\
0 = \frac{\partial \mathcal{S}}{\partial b_1} =& 2 \sum_{i=1}^n\left[y_i - b_0 - b_1x_i - \ldots - b_px_i^p\right]. (-x_i)\\
\vdots & \\
0 = \frac{\partial \mathcal{S}}{\partial b_p} =& 2 \sum_{i=1}^n\left[y_i - b_0 - b_1x_i - \ldots - b_px_i^p\right]. (-x_i^p)\\
\end{align*}
$$
After simplifying the above set of equation we get a system of "$p+1$" equation in           "$p+1$" variables

$$
\begin{align*}
n b_0 + b_1 \sum x_i + \ldots + b_p\sum x_i^p &= \sum y_i \\
b_0 \sum x_i+ b_1 \sum x_i^2 + \ldots + b_p\sum x_i^{p+1} &= \sum y_ix_i \\
b_0 \sum x_i^2+ b_1 \sum x_i^3 + \ldots + b_p\sum x_i^{p+2} &= \sum y_ix_i^2 \\
\vdots &\\
b_0 \sum x_i^p+ b_1 \sum x_i^{p+1} + \ldots + b_p\sum x_i^{2p} &= \sum y_ix_i^p \\
\end{align*}
$$
writing this in matrix form; which will obvio make it easier for further computations,
We formulate what is known as **Design Matrix**,
$$
\textbf{X} = 
\begin{bmatrix}
1 & x_1 & \ldots &x_1^p \\
1 & x_2 & \ldots & x_2^p \\
\vdots&\vdots&\ddots&\vdots\\
1 & x_n&\ldots& x_n^p
\end{bmatrix}
$$

from here we can get,
$$
\textbf{X}^T\textbf{X} = 
\begin{bmatrix}
1 & x_1 & \ldots &x_1^p \\
1 & x_2 & \ldots & x_2^p \\
\vdots&\vdots&\ddots&\vdots\\
1 & x_n&\ldots& x_n^p
\end{bmatrix}
\begin{bmatrix}
1 & 1 & \ldots &1 \\
x_1 & x_2 & \ldots & x_n \\
\vdots&\vdots&\ddots&\vdots\\
x_1 & x_2^p&\ldots& x_n^p
\end{bmatrix}
=
\begin{bmatrix}
n & \sum x_i & \ldots &\sum x_i^p \\
1 & x_2 & \ldots & x_2^p \\
\vdots&\vdots&\ddots&\vdots\\
1 & x_n&\ldots& x_n^p
\end{bmatrix}
$$

$$
(X'X)\ \underset{\sim}{b} = X^T y
$$
$$
\underset{\sim}{\hat b} = (X^TX)^{-1}X'y
$$
provided $|X'X| \neq 0 \ \ \implies$ not ill-conditioned

$\underset{\sim}{\hat b}$  is referred as an estimate of $\underset{\sim}{b}$
 
Prediction of $y$
$$
\hat y = X \ \ \underset{\sim}{\hat b}
$$
"^" is used to understand the fact that this value is subject to sampling variation 
and it can be,
characterized by probabilioty distribution called **Sampling Distribution** 