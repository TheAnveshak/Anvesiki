# Second Order Processes
The general For 
$$
Y(s) = \frac{K_p}{\tau^2s^2+2\xi\tau s+1} U(s)
$$
$K_p :$ Process Steady state Gain
$\tau :$ Process time Constant
$\xi :$ Damping Coefficient

there are 3 case arising based on $\xi$
1. case A:
	$\xi>1$
$$
	x(t) =K_p\left[1 - e^{-\frac{\xi}{\tau}t}\left[\cosh\left(\frac{\sqrt{\xi^2 -1}}{\tau}t\right)+ \frac{\xi}{\sqrt{1-\xi^2}}\sinh\left(\frac{\sqrt{\xi^2 -1}}{\tau}t\right)\right]\right]
$$
1. case B:
	$\xi =1$
3. case C:
	$\xi<1$
$$
	\bar x(t) = K_p\left[1 - \frac{1}{\sqrt{1-\xi^2}}e^{\frac{-\xi}{\tau}t} \sin\left(\sqrt{1-\xi^2}\frac{t}{\tau} + \tan ^{-1} \frac{\sqrt{1-\xi^2}}{\xi}\right)\right]
$$

### Observations
- Responses exhibit overshoot $y(t) / K_m >1$ when $\xi<1$.
- Larger value of $\xi$ yield a slow sluggish response
- Systems with $\xi=1$ yield the fastest response without overshoot
- As 

![[Pasted image 20250128111253.png]]

$b/a =$ overshoot = $\exp(\frac{-\pi\xi}{\sqrt{1-\xi^2}})$
$c/b =$ decay ratio = overshoot$^2$ = $\exp(2\frac{-\pi\xi}{\sqrt{1-\xi^2}})$  $\sim 1/4$ recommended
$t_r =$ rise time
$t_s =$ Response time

## Standard Procedure
### First order System
$G(s) = \frac{1}{\tau s+1}$ 
$G(i\omega) = \frac{1}{\tau i\omega} = \frac{1-i\tau\omega}{1+\tau^2\omega^2} = \frac{1}{1+\tau^2\omega^2}+i \frac{-\tau\omega}{1+\tau^2\omega^2} = a+ib$
$AR = \frac{1}{\sqrt{1+\tau^2\omega^2}}$
$\phi = \tan^{-1}(-\tau\omega)$
$G(i\omega) = \frac{1}{\sqrt{1+\tau^2\omega^2}} e^{i\phi}$

### Second order System
$$
\begin{align*}
\frac{x(s)}{p(s)} = G(s) = G(j\omega) &= \frac{K_p}{\tau^2(j\omega)^2+2\xi\tau j\omega+1}\\
G(j\omega) &= K_p\frac{1-\tau^2\omega^2 - j2\xi\tau\omega}{(1-\tau^2\omega^2)^2 -(2\xi\tau\omega)^2}\\
G(j\omega) &= K_p\left(\frac{1-\tau^2\omega^2}{(1-\tau^2\omega^2)^2 -(2\xi\tau\omega)^2}-j\frac{ 2\xi\tau\omega}{(1-\tau^2\omega^2)^2 -(2\xi\tau\omega)^2}\right)\\
r(\omega) &= \frac{1}{\sqrt{(1-\tau^2\omega)^2 +(2\omega\xi\tau)^2 }}\\
\phi &= \tan{-1} \frac{-2\xi\tau\omega}{1-\tau^2\omega^2}
\end{align*}
$$


