### We Know the $\textbf{Thermodynamic Functions}$
$$
dU = TdS - PdV + \hat{G}dM
$$
$$
dH = TdS + VdP
$$
$$
dG = -SdT + VdP
$$
$$
dA = -SdT - PdV
$$

Consider the equation $dG = -SdT + VdP$,
$$
\frac{\partial}{\partial T}\left(\frac{\partial G}{\partial P}\right)_T = \left(\frac{\partial V}{\partial T}\right)_P
$$
$$
\frac{\partial}{\partial P}\left(\frac{\partial G}{\partial T}\right)_P = -\left(\frac{\partial S}{\partial P}\right)_T
$$
Considering Schwarz's theorem, also called Clairaut's theorem or Young's theorem,
From Gibbs Free Energy $G(T, P)$:
$$
\left(\frac{\partial S}{\partial P}\right)_T = -\left(\frac{\partial V}{\partial T}\right)_P
$$
Similarly, from Internal Energy $U(S, V)$:
$$
\left(\frac{\partial T}{\partial V}\right)_S = -\left(\frac{\partial P}{\partial S}\right)_V
$$
From Enthalpy $H(S, P)$:
$$
\left(\frac{\partial V}{\partial T}\right)_P = -\left(\frac{\partial S}{\partial P}\right)_T
$$
From Helmholtz Free Energy $F(T, V)$:
$$
\left(\frac{\partial S}{\partial V}\right)_T = -\left(\frac{\partial P}{\partial T}\right)_V
$$

### All the other Coefficients
The Coefficient of Thermal Expansion $\alpha = \frac{1}{V}\left(\frac{\partial V}{\partial T}\right)_P$

### Enthalpy Changes in Substances:
$$
dH = \left(\frac{\partial H}{\partial T}\right)_P dT + \left(\frac{\partial H}{\partial P}\right)_T dP
$$
Since $c_P\ \text{is defined as}\ \frac{\partial H}{\partial T}\big|_P$ and
$$
\left(\frac{\partial H}{\partial P}\right)_T = T \left(\frac{\partial S}{\partial P}\right)_T + V
$$
$$
dH = c_P dT + \left[T \left(\frac{\partial S}{\partial P}\right)_T + V\right] dP
$$
From the previous relation we get,
$$
\boxed{dH = c_P dT + \left[V - T\left(\frac{\partial V}{\partial T}\right)_P\right]dP}
$$
For Ideal Gas $PV = RT \implies \left(\frac{\partial V}{\partial T}\right)_P = \frac{R}{P}$.
Furthermore, $T\left(\frac{\partial V}{\partial T}\right)_P = T \frac{R}{P} = V$
Hence
$$
dH = c_P dT
$$
Integrating the equation we get,
$$
\Delta H = c_P \Delta T
$$
For Liquid,
$$
dH = c_P dT + \left[V - T\alpha V\right] dP
$$
$$
\Delta H = c_P \Delta T\quad +\quad V \left[1 - T\alpha \right] \Delta P
$$

### Entropy Change in Substances:
Consider $dH = TdS + VdP$,
$$
\left(\frac{\partial H}{\partial T }\right)_P = T\left(\frac{\partial S}{\partial T}\right)_P + V\left(\frac{\partial P}{\partial T}\right)_P
$$
Assuming the changes in pressure with respect to temperature are negligible,
$$
\frac{1}{T}\left(\frac{\partial H}{\partial T}\right)_P = \left(\frac{\partial S}{\partial T}\right)_P \implies \left(\frac{\partial S}{\partial T}\right)_P = \frac{c_P}{T}
$$
$$
dS = \left(\frac{\partial S}{\partial T}\right)_P dT + \left(\frac{\partial S}{\partial P}\right)_T
$$
From the previous relation,
$$
\boxed{dS = \frac{c_P}{T}dT - \left(\frac{\partial V}{\partial T}\right)_P dP}
$$
For Ideal Gas $PV = RT \implies \left(\frac{\partial V}{\partial T}\right)_P = \frac{R}{P}$.
Hence entropy change for an Ideal Gas is given by,
$$
\boxed{dS = \frac{c_P}{T}dT - \frac{R}{P} dP}
$$
For liquids we consider,
The Coefficient of Thermal Expansion $\alpha = \frac{1}{V}\left(\frac{\partial V}{\partial T}\right)_P$
$$
dS = \frac{c_P}{T}dT - \frac{R}{P} dP
$$
Integrating the above equation we get,
$$
\Delta S = c_P \ln{\frac{T_2}{T_1}} - R \ln{\frac{P_2}{P_1}}
$$
$$
S_1 - S_2 = \ln{ \left(\frac{T_2}{T_1}\right)^{c_P}\left(\frac{P_1}{P_2}\right)^R}
$$
For Liquids,
$$
dS = \frac{c_P}{T}dT - \alpha V dP
$$