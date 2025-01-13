## Difference Equation 
The term difference equation some times refers to a specific type of recurrence relation. However difference equation is frequently used to refer to any recurrence relation.
Consider $u_n = cn - 3$ , where $c$ is any arbitrary constant

#### Tower of Hanoi
The **Tower of Hanoi** (also called **The problem of Benares Temple**[[1]](https://en.wikipedia.org/wiki/Tower_of_Hanoi#cite_note-oeis-1) or **Tower of Brahma** or **Lucas' Tower**[[2]](https://en.wikipedia.org/wiki/Tower_of_Hanoi#cite_note-2) and sometimes pluralized as **Towers**, or simply **pyramid puzzle**[[3]](https://en.wikipedia.org/wiki/Tower_of_Hanoi#cite_note-3)) is a [mathematical game](https://en.wikipedia.org/wiki/Mathematical_game "Mathematical game") or [puzzle](https://en.wikipedia.org/wiki/Puzzle "Puzzle") consisting of three rods and a number of disks of various [diameters](https://en.wikipedia.org/wiki/Diameter "Diameter"), which can slide onto any rod. The puzzle begins with the disks stacked on one rod in order of decreasing size, the smallest at the top, thus approximating a [conical](https://en.wikipedia.org/wiki/Conical "Conical") shape. The objective of the puzzle is to move the entire stack to one of the other rods, obeying the following rules:[[4]](https://en.wikipedia.org/wiki/Tower_of_Hanoi#cite_note-4)

1. Only one disk may be moved at a time.
2. Each move consists of taking the upper disk from one of the stacks and placing it on top of another stack or on an empty rod.
3. No disk may be placed on top of a disk that is smaller than it.

With three disks, the puzzle can be solved in seven moves. The minimal number of moves required to solve a Tower of Hanoi puzzle is $2^n − 1$, where _n_ is the number of disks.(reference: Wikipedia)

$H_n = 2H_{n-1} +1$ , where $H_i$ is the number of steps for $i$ disks
$H_n = \sum2^{n-i}H_{n-(n-i)}$ 
$H_n = 2^n -1$

$u_{n+1} = c(n+1)-3  = cn-3+c$
$\therefore u_{n+1} = u_n+c$
$\therefore c= \frac{u_n+3}{n}$
$u_{n+1} = \frac{n+1}{n}u_n + \frac{3}{n}$ 
$\therefore nu_{n+1} = (n+1)u_n+3$

## Linear Difference Equation with constant Coefficient
$$
c_0u_n + c_1u_{n-1} + c_2u_{n+2} = f(n) 
$$
If $f(n)= 0 \to$ is homogenous
with $f(n)= 0$ the above equation is called linear, homogenous, order-2 recurrence relation.

### Solution of Homogenous Equations
#### First Order:
$$
\begin{align*}
u_n &= ku_{n-1}\\
&= k\times k u_{n-2}\\
&\vdots\\
u_n&=k^n U_0
\end{align*}
$$
$u_n = ck^n$ where c is an arbitrary constant.
#### First order linear homogenous equation of the following form
$$
\begin{align*}
u_n&=au_{N-1} +b\\
&\ \ \ \ \ \vdots\\
&= a^i u_{n-i} + b\sum_{i} a^i \\
&\ \ \ \ \ \vdots \\
&= a^nu_0+\frac{a^n-1}{a-1}b \ \ \ \ \forall a>1\\
&= a^nu_0+\frac{1-a^n}{1-a}b \ \ \ \ \forall a<1\\
\end{align*}
$$

#### Consider second Order homogenous linear difference equation
$$
\begin{align*}
a_0 + a_1u_{n-1}+a_2u_{n-2} &= 0\\
u_n &= ck^n (c\neq 0)\ \ \ \text{               be a solution }\\
\therefore a_0k^2 + a_1k +a_2 &= 0\\
\end{align*}
$$
1. consider the equation has 2 distinct roots $m_1$ & $m_2$ 
	then, $u_n = c_1m_1^n + c_2m_2^n$ is the general solution of equation.
2. suppose $m_1=m_2=m$
	$u_n = (c_1+c_2n)m^2$ is the general solution where $c_1$&$c_2$ are arbitrary constants
3. suppose the roots are $\alpha = \pm \beta$ 
	Then, $u_n = \gamma^n(c_1\cos n\theta +c_2 \sin n\theta$
	where, $\gamma = \sqrt{\alpha^2+\beta^2}$ & $\theta = \tan^{-1}\left(\frac{\beta}{\alpha}\right)$
	& $c_1, c_2$ are arbitrary constant. 

$$
a^2
$$






















