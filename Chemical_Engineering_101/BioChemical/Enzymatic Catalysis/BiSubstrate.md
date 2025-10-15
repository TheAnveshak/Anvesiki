# Ternary
Hypothesized Reactions with respective dissociation rate constants
$$
[E]+[A] \ce{<-->[K_A]} [EA] \quad \quad \text{Enzyme Combines with Substrate A}
$$
$$
[E]+[B] \ce{<-->[K_B]} [EB] \quad \quad \text{Enzyme Combines with Substrate B}
$$
$$
[EA]+[B] \ce{<-->[K_AB]} [EAB] \quad \quad \text{Enzyme COmplex Combines with Substrate B}
$$
$$
[EB]+[A] \ce{<-->[K_BA]} [EBA] \quad \quad \text{Enzyme Complex Combines with Substrate A}
$$
Assumption: $K_A K_{AB} = K_B K_{BA}$ i.e. complex \[EAB\] is the same as \[EBA\].
$$
[EAB] \ce{->[k_2]}[P]+[E] \quad \quad \text{Enzyme-A-B complex forms product}
$$
Balancing the total Enzyme concentration give,
$$
[E_T] = [E] + [EA] + [EB] + [EAB]
$$
$$
[E] = \frac{[E_T]}{1+\frac{[A]}{K_A}+\frac{[B]}{K_B}+\frac{[A][B]}{K_{AB}K_A}}
$$
rate $= \frac{dP}{dt} = \frac{k_2[E][A][B]}{K_AK_{AB}} = k_2[EAB]$
$$
v = \frac{v_{max}[A][B]}{K_AK_{AB} + K_{AB}[A]+K_{BA}[B]+[A][B]}
$$
which in a special form turns out to be very handy(bring out the linearity in the velocity and subs conc relation) for model fitting,
$$
\frac{1}{v} = \bigg(\frac{K_AK_{AB}}{v_{max}}\frac{1}{[B]}+\frac{K_{BA}}{v_{max}}\bigg)\frac{1}{[A]}+\frac{K_{AB}}{v_{max}}\frac{1}{[B]}+\frac{1}{v_{max}}
$$

$$
W = \frac{a}{[A][B]} + \frac{b}{[B]}+\frac{c}{[A]}+d
$$
$$
W = aX + bY +cZ + d
$$
$$
\varepsilon = (W - aX -bY-cZ-d)
$$
For N experiments,
$$
SSE = E = \sum_N(W_i-aX_i-bY_i-cZ_i-d)^2
$$
for minimum, $\frac{\partial E}{\partial a} = \frac{\partial E}{\partial b} = \frac{\partial E}{\partial c} = \frac{\partial E}{\partial d} = 0$
The parameters a, b, c, d is as a solution to this system of linear equation of form $AX = b$
$$
\begin{bmatrix}
\sum X_i^2 & \sum X_iY_i & \sum X_iZ_i & \sum X_i \\
\sum Y_iX_i & \sum Y_i^2 & \sum Y_iZ_i & \sum Y_i \\
\sum Z_iX_i & \sum Z_iY_i & \sum Z_i^2 & \sum Z_i \\
\sum X_i & \sum Y_i & \sum Z_i & N \\
\end{bmatrix}
\begin{bmatrix}
a \\
b\\
c\\
d
\end{bmatrix}
=
\begin{bmatrix}
\sum W_iX_i\\
\sum W_i Y_i\\
\sum W_i Z_i\\
\sum W_i
\end{bmatrix}
$$
where,
$v_{max} = \frac{1}{d}$,  $K_{AB} = \frac{b}{d}$,  $K_{BA}=\frac{c}{d}$,  $K_A = \frac{a}{b}$



# Ping Pong Bi Bi
examples: Trasnminase, Nucleoside, Diphosphokinase
Here the same enzyme is found to be in different states/configuration(wrt eg: geometry, charge, etc) after every reaction and therefore facilitation different reactions in different configuration.
Hypothesized reaction:
$$
[E] +[A]\ce{<=>[K_A]}[EA]\ce{->[k_2]}[P]+[E^*]+[B]\ce{<=>[K_B]}[E^*B]\ce{->[k_4]}
[E]+[Q]$$
Further on i am dropping "\[\]" for denoting concentration(being a bit lazy; oops fast i mean),
$$
E + A \ce{<=>[K_A]}EA \quad \quad \text{enzyme E complexes with substrate A}
$$
$$
EA \ce{->[k_2]}P+E^* \quad \quad \text{The complex gives product P adn enzyme E*}
$$
$$
E^* + B \ce{<=>[K_B]}E^*B \quad \quad \text{enzyme E* complexes with substrate B}
$$
$$
E^*B \ce{->[k_4]}Q+E \quad \quad \text{The complex gives product Q and enzyme E}
$$

