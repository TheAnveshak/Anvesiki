# Complexation Reaction

$$
A + E \ce{<=>[k_1][k_{-1}]} AE
$$
Complexing of Substrate should be higher thatn product
$$
AE \ce{->[k_2]} P +E
$$
here the decomplexation(desorption) rate of $[PE]$->$[P]+[E]$ is kinda assumed to be $\infty$ 
So at equilibrium,
$$k_1[A][E] = k_{-1}[AE]$$ 
$K_M = \frac{k_{-1}}{k_1} = \frac{[A][E]}{[AE]}$  Unlike in chemical engineering we are more concerned with the dissociation rate constant and hence from here we derive our constant known as Michaelis Menten Constant

$[AE] = \frac{[A][E]}{K_M}$

## Michaelis Menten Approach
By balancing the Enzyme,
$$
[E_0] = [E] + [AE] = [E]\bigg[1+\frac{[A0]}{K_M}\bigg]
$$
 free for enzyme is thus given by: $[E] = \bigg[\frac{[E_0]}{1+\frac{[A]}{K_M}}\bigg]$
hence the reating species is: $[AE] = \frac{[A][E_0]}{K_M+[A]}$
here we denote the rate constant as some form of velocity \[ $v$\] instead of regular chemical kinetics \[r\] 
$$
v =\frac{dP}{dt} = k_2[EA] = \frac{k_2[E_0][A]}{k_M + [A]}
$$
This is the Michaelis Menten form of Enzymatic Kinetics
Which is further abbreviated in form of maximum velocity or the the maximum rate:
$$
v = \frac{v_{max}[A]}{K_M+[A]}
$$

## Briggs Haldane Approach

$$
[A] + [E] \ce{<=>[k_1][k_{-1}]} AE \ce{-> [k_2]} P+E
$$
we assume a Quasi Steady State for this system,
$$
0 = \frac{d[EA]}{dt} = k_1[A][E] - k_{-1}[EA] - k_2[EA]
$$
$$
[EA]  = \frac{k_1[E][A]}{k_{-1}+k_2}
$$
here we use a modified MM constant $K_M = \frac{k_{-1}+k_2}{k_1}$

# Experiments and Plotting

## Linweaver Burk Plot  #TODOupdatelater
$$
\frac{1}{v}=\frac{K_M}{v_{max}} \bigg(\frac{1}{[S]}\bigg) + \frac{1}{v_{max}}
$$
## Eadie Hofsteed Plot

## Hanes Wolff Plot
