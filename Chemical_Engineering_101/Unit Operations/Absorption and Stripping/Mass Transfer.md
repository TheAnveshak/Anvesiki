![[images/Screenshot_20250326_135354.png]]

$L_1y_1+L_2x_2 = G_2y_2+G_1x_1$
$Y = \frac{\text{moles of solute}}{\text{moles of non solute}} = \frac{y_{NH_3}}{y_{Air}} = \frac{y}{1-y}$
$X = \frac{x}{1-x}$
$G_S =$ Flow rate of solute free gas
$L_S =$ flow rate of solute free liquid

$G_SY = \frac{\text{moles of Solute}}{\text{time}}$
$G_sY_1+L_sX_2 = G_sY_2+L_sX_1$
$\frac{L_s}{G_s}=\frac{Y_1-Y_2}{X_1-X_2}$
$x = \frac{X}{1+X}$  $y = \frac{Y}{1+Y}$
$G_s = G_1(1-y_1)$
![[images/Screenshot_20250326_141254.png]]

- Obtain the equilibirium data and plot the X-Y curve
- From material Balance locate $X_1,Y_1,X_2,Y_2$ and join them to obtain operating line 
- Construct the number of stages starting from or bottom of the operating line

> [!question] Probelm
> It is required to remove 90% of the solute C from a solution of C in G by using pure solvent L in a counter current cascade. The feed containing 12% C in the mixture exters the column at the bottom at the rate of 6000kg/h. The solvent enters at the top at a rate of 7685 kg/h. The equilibrium relation is linear Y = 1.32X, where Y = kg per kg C-free G, and kg C per kg C_free L.
> Determine the number of trays required to perform the separation for 40% overall tray efficiency

G1 = 6000 kg/h
L2 = 7685 kg/h 
$L1$ = 76850+0.12 * 0.9 * 6000 = 8333kg/h
$Y_1 = 0.136$
$Y_2 = 0.01358$
$X_1 = 0.0842$
$X_2 = 0$
$G_S =G_1 (1-y) = 6000(1-0.12) = 5280$
$L_2 = \frac{G_S(Y_1-Y_2)}{X_1-X_2} = 7676.7$
Y = 1.32X

## Kremser-Brown-Souders
	 
For Adsorption
$$
N = \frac{\log\left[\left(\frac{Y_1-\alpha X_2}{Y_2-\alpha X_2}\right)\times \left(1-\frac{1}{A}\right)+\frac{1}A\right]}{\log A}
$$
A =  Absorption Factor = $\frac{L_s}{\alpha G_s}$
Equilibrium Relation  = $Y = \alpha X$


For Stripping
$$
N = \frac{\log\left[\left(\frac{X_1-\frac{Y_1}{\alpha}}{X_2-\frac{Y_1}{\alpha }}\right)\times \left(1-{A}\right)+A\right]}{\log A}
$$
S = Stripping Factor = $\frac{1}{A} = \frac{\alpha G_s}{L_s}$
Equilibrium Equation = $Y =\alpha X$


$-d(G_s'Y) = N_A\bar a dh$
$-YdG'_s - G'_sdY = K_Y(Y-Y')\bar a dh$
$\int^h_0 dh = \int^{Y_1}_{Y_2}\frac{G'_s}{K_Y \bar a}\frac{dY}{Y-Y^*}$
$h = \frac{G'_s}{K_Y \bar a}\int^{Y_1}_{Y_2}\frac{dY}{Y-Y^*} = HTU \times NTU$
For Dilute Solutions:
$h = \frac{G'_s}{K_Y \bar a}\int^{Y_1}_{Y_2}\frac{dY}{(1-Y)(Y-Y^*)}$


> [!question] Problem
> Solute A is to be absorbed from a binary mixture containing 7.5% of A with solvent B in a packed Tower. BAsed on flooding calculation, a tower diameter of 1.2m is selected. Total gas flow rateis 60kmol/h. The exit gas must not contain more than 0.2% of solute A. Free liquid B enters from top of the tower at 40 kmol/h. The gas phase and liqid phase mass transfer coefficients based on mole ratio unit are $k_X =2.05kmol/m^2h(\Delta X)$ and $k_Y=1.75kmol/m^2h(\Delta Y)$. The equilibrium line is Equation $Y = 0.63$. Specific interfacial area of gas liquid contact $\bar a$ is 71 $m^2/m^3$.
> a. Calculate packing height required for desired separation.


$G_s = 55.5 kmol/h$
$G_s' = \frac{4\times 55.5}{\pi 1.2^2} = 49.07 kmol/h.m^2$
$\frac{1}{K_Y} = \frac{1}{k_Y}+\frac{m}{k_X}$
$K_Y = 1.137kmol/m^2h$
$HTU = \frac{49.07}{1.137\times 71}=0.6m$


















































































[^1]: hi
