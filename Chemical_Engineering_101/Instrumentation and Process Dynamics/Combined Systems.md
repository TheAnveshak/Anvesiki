## Consider 2 First order systems
### Noninteracting Independent units
$F_1 = k_1\sqrt{h_1}$ and $F_2 = k_2\sqrt{h_2}$ 

$F_1 - F_i =$ Accumulation
$k_1\sqrt{h_1} - F_i =$ Accumulation
$(F_1 - F_i )\rho \Delta t= A h_1 \rho$ 
$F_1 = \frac{A[h_1(t+\Delta t)-h_1(t)]}{\Delta t}+ F_i$  
$F_1 =A \frac{dh_1}{dt}+ F_i$ 
$A\frac{dh_1}{dt} = F_i-F_1 = F_i - k\sqrt{h_1} = f(F_i,h_1)$
$\ \ \ \ \ \ \ \ \ = f_{ss}^{\ \ ^{=0}}+\frac{\partial f}{\partial F_i}\bar F_i +\frac{\partial f}{gh_1}\bar h_i$ 

$\frac{h_1(s)}{F_i(s)} = \frac{\mathcal{R_1}}{\tau_1 s+1}$

Similarly,
$F_2 - F_1 = A\frac{h_2(t+\Delta t)-h_2(t)}{\Delta t}$
$F_2 = A\frac{dh_2(t)}{dt}+F_1 = A\frac{dh_2(t)}{dt} + A\frac{dh_1(t)}{dt}+ F_i$

$A_2\frac{d\bar h_2(t)}{dt} =$


$\frac{h_2{s}}{h_1{s}} = \frac{R_2/R_1}{\tau_2s+1}$ 
$\therefore \frac{h_2(s)}{F_i(s)} = \frac{\mathcal{R_2}}{(\tau_1s+1)(\tau_2s+1)}$


### Interacting Dependent Units
$F_1 = k_1\sqrt{h_1-h_2}$ and $F_2  = k_2\sqrt{h_2}$ 

$A\frac{dh_1}{dt} = F_i-F_1 = F_i - k\sqrt{h_1-h_2} = f(F_i,h_1,h_2)$
$\ \ \ \ \ \ \ \ \ = f_{ss}^{\ \ ^{=0}}+\frac{\partial f}{\partial F_i}\bar F_i +\frac{\partial f}{\partial h_1}\bar h_1+\frac{\partial f}{\partial h_2}\bar h_2$  
$\ \ \ \ \ \ \ = 0 + 0 + k_1\frac{\bar h_1 -\bar h_2}{2\sqrt{h_1-h_2}}$

$A \frac{\bar h_1(t)}{dt}= \frac{k_1}{2\sqrt{h_1-h_2}}\bar h_1 - \frac{k_1}{2\sqrt{h_1-h_2}}\bar h_2$
$A \frac{\bar h_1(t)}{dt}= \frac{\bar h_1}{R_1} - \frac{\bar h_2}{R_1}$






































































































