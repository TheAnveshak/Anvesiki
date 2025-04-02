[[Conservation of Energy]]
[[Entropy]]
[[Will Name it Later...]]


> [!Info]  Blue Pill
> **What is life?**
> Just kidding, **AWP Sir** denied answering that (maybe is out of scope of this syllabus), so for now we will stick to modelling and formulating equation of State 
********

## Residual Function

The changes in enthalpy or entropy for real fluids can be determined by considering the corresponding changes for an ideal gas under identical conditions, while also accounting for deviations from ideal gas behavior.

### Departure of Enthalpy

![[Images/Pasted image 20241011144242.png]]

The change in enthalpy from State 1 to State 2 following the orange path is given by:

$$
H_2 - H_1 = \int_{P_1}^0 \left[V - T\left(\frac{\partial V}{\partial T}\right)_P\right]_{T_1} dP + \int_{T_1}^{T_2} c_P^{IG} dT + \int_0^{P_2} \left[V - T\left(\frac{\partial V}{\partial T}\right)_P\right]_{T_2} dP
$$

$$
H_2 - H_1 = -\Delta H^R_{T_1,P_1} + \Delta H^{IG} + \Delta H^R_{T_2,P_2}
$$

$$
H_2 - H_1 = (H_2^{IG} - H_1^{IG}) + (H_2^R - H_1^R)
$$

where $\Delta H^{IG}$ and $\Delta H^R$ represent the changes in enthalpy due to ideal gas behavior and residual enthalpy, respectively. This can be expressed as:

>$$H^R = (H - H^{IG})_{T,P} = \int_{T,P=0}^{T,P}\left[V - T \left(\frac{\partial V}{\partial T}\right)_P\right]_T dP$$


### Departure of Entropy
The change in entropy from State 1 to State 2 is given by:

$$
S_2 - S_1 = \int_{P_1}^{0} \left[ \frac{V - T \left( \frac{\partial V}{\partial T} \right)_P}{T} \right]_{T_1} dP + \int_{T_1}^{T_2} \frac{C_P^{IG}}{T} \, dT + \int_{0}^{P_2} \left[ \frac{V - T \left( \frac{\partial V}{\partial T} \right)_P}{T} \right]_{T_2} dP
$$


$$
S_2 - S_1 = \int_{P_1}^{0} \left[ \left(\frac{\partial V}{\partial T}\right)_P - \frac{R}{P} \right]_{T_1} dP + \int_{T_1}^{T_2} \frac{C_P^{IG}}{T} \, dT + \int_{0}^{P_2} \left[ \frac{\partial V}{\partial T} - \frac{R}{P} \right]_{T_2} dP
$$

$$
S_2 - S_1 = -\Delta S^R_{T_1, P_1} + \Delta S^{IG} + \Delta S^R_{T_2, P_2}
$$

where $\Delta S^{IG}$ and $\Delta S^R$ are the changes in entropy due to ideal gas behavior and residual entropy, respectively. This can be written as:

$$
S_2 - S_1 = (S_2^{IG} - S_1^{IG}) + (S_2^R - S_1^R)
$$

Considering the residual entropy $S^R$:

>$$S^R = (S - S^{IG})_{T, P} = - \int_{T,P=0}^{T,P}\left[ \left( \frac{\partial V}{\partial T} \right)_P - \frac{R}{P}\right] dP$$


>$$S^R = (S - S^{IG})_{T, V} = \int_{T,V=\infty}^{T,V}\left[ \left( \frac{\partial P}{\partial T} \right)_V - \frac{R}{V}\right] dV$$


## Van der Waals EOS (1873)

The van der Waals equation, named for its originator, the Dutch physicist Johannes Diderik van der Waals, extends the ideal gas law to account for the non-zero size of gas molecules and their interactions. This allows the equation to model phase changes, such as liquid $\leftrightarrow$ vapor, and provides analytic expressions for the properties of real substances.


>$$\boxed{P = \frac{RT}{V-b} - \frac{a}{V^2}}$$

Or equivalently,

$$\boxed{\left(P + \frac{a}{V^2}\right)(V-b) = RT}$$

Where $a$ and $b$ are defined as follows:

$$
a = \frac{27R^2T_c^2}{64P_c}, \quad b = \frac{RT_c}{8P_c}
$$

This illustrates how the van der Waals equation fits experimental data.
Upon simplifying,

$$
PV^3 - (Pb + RT)V^2 + aV - ab = 0 \tag{7.2-2}
$$

The equation can also be expressed in the form:

$$
z^3 + a_1 z^2 + a_2 z + a_3 = 0
$$

where $z = \frac{V}{\frac{RT}{P}}$ is the compressibility factor. This substitution makes computations easier as it introduces dimensionless term.

Substituting for $V$ , we get:

$$
\frac{R^3 T^3_c}{P^2_c} z^3 - (Pb + RT) \frac{R^2 T_c^2}{P^2_c} z^2 + a \frac{RT_c}{P_c} z - ab = 0
$$

$$z^3 + \left(-1 - \frac{P_c b}{RT_c}\right) z^2 + \frac{a P_c}{R^2 T_c^2} z - \frac{P_c^2 ab}{R^3 T_c^3} = 0$$

>$$\boxed{\ \ 
z^3 + (-1-B) z^2 + A z - AB = 0} \ \ \ $$

where $A = \frac{a P_c}{R^2 T_c^2}$ and $B = \frac{P_c b}{RT_c}$.

For solving cubic equations of state in the form $z^3 + a_1 z^2 + a_2 z + a_3 = 0$, we need a generalized solution:


---

## Accentric Factor

The **acentric factor** ($\omega$) is a parameter introduced by **Pitzer (1955)** to account for the deviation of real gases from ideal behavior. This is particularly important for substances that do not conform to the **corresponding states theory**, which uses **critical temperature** ($T_c$), **critical pressure** ($P_c$), and **compressibility factor** ($Z_c$) as key parameters to describe gas behavior.

**Pitzer** observed that the **reduced vapor pressure**, defined as:
$$
P_{r}^{sat} = \frac{P^{sat}}{P_c}
$$
is a better indicator of gas behavior, especially at a reduced temperature $T_r = \frac{T}{T_c}$ of **0.7** for noble gases such as **neon** and **argon** (not helium haha... ). For these gases, the reduced vapor pressure is approximately **0.1** at $T_r = 0.7$. However, for other substances, deviations occur due to molecular interactions, and these deviations are captured by the **acentric factor**.

Pitzer defined the acentric factor as:

>$$\omega = -1 - \log_{10}\left(\frac{P_{r}^{sat}}{P_c}\right)_{T_r = 0.7}$$


This definition sets the acentric factor to **zero** for monatomic, inert gases like **Ne**, **Ar**, and **Kr**, where the behavior closely follows the corresponding states theory. For other substances, $\omega$ becomes non-zero, indicating deviations caused by molecular interactions.

- The **acentric factor** ($\omega$) is critical for describing the non-ideal behavior of gases, particularly those with complex molecular interactions.
- Experimentally, $\omega$ is relatively easy to determine using a single measurement of vapor pressure.
- **Acentric factor ($\omega$)**, improves the EOS’s flexibility in predicting the behavior of different substances. 
- The acentric factor adjusts for non-spherical molecular shapes and interactions, which enhances the accuracy of the equation for a wide range of fluids, particularly non-ideal substances and polar compounds.

For **water**, the acentric factor $\omega$ is calculated as **0.344**, which indicates significant deviation from the behavior of inert gases.


---

## Peng-Robinson EOS

The Peng-Robinson EOS is particularly good at predicting the behavior of **vapor-liquid equilibrium (VLE)**. It can be used to model non-ideal fluids, mixtures, and even gases near their critical points, where behavior can deviate significantly from ideal gas assumptions.

The **Peng-Robinson equation of state (PR EOS)** is:

$$P = \frac{RT}{V - b} - \frac{a(T)}{V^2 + 2bV - b^2}$$

Where:
- $P$ = Pressure
- $T$ = Temperature
- $V$ = Molar volume
- $R$ = Universal gas constant
- $a(T)$ = Attraction parameter (temperature-dependent)
- $b$ = Volume exclusion parameter

The attraction parameter $a(T)$ and $b$ are defined as follows:

$$a(T) = a_c \left[1 + \kappa \left(1 - \sqrt{\frac{T}{T_c}}\right)\right]^2$$

$$b = 0.07780 \frac{RT_c}{P_c}$$

The critical constants $a_c$ and $\kappa$ are given by:

$$a_c = 0.45724 \frac{R^2 T_c^2}{P_c}$$

$$\kappa = 0.37464 + 1.54226 \omega - 0.26992 \omega^2$$

Where:
- $T_c$ = Critical temperature
- $P_c$ = Critical pressure
- $\omega$ = Acentric factor
The **Peng-Robinson equation of state (PREOS)** in terms of the compressibility factor $Z$ is:

$$Z^3 - (1 - B)Z^2 + (A - 3B^2 - 2B)Z - (AB - B^2 - B^3) = 0$$

Where:

- $Z = \frac{P V}{R T}$ is the compressibility factor.
- $A$ and $B$ are dimensionless parameters that depend on the critical temperature, critical pressure, and acentric factor:

$$
A = 0.45724 \frac{\alpha(T_r) P}{R^2 T^2}
$$

$$
B = 0.07780 \frac{P_c}{RT_c}
$$

$$
\alpha(T_r) = \left[1 + \kappa \left(1 - \sqrt{T_r}\right)\right]^2
$$

- $T_r = \frac{T}{T_c}$ is the reduced temperature.


---

## Virial EOS

One of the easiest ways to describe the relationship $V = f(T, P)$ for gases is to quantify the deviation from ideal behavior. For an ideal gas:

$$
\frac{PV}{RT} = 1
$$

The deviation from ideal behavior can be explained at a particular temperature 'T', using a polynomial expansion of the form:

$$
\frac{PV}{RT} = 1 + \frac{B}{V} + \frac{C}{V^2} + \frac{D}{V^3} + \cdots
$$

This equation is called the **Virial Equation of State (EOS)**. The constants **B**, **C**, **D**, and so on are called **Second Virial Coefficient**, **Third Virial Coefficient**, and so on. They are functions of **temperature (T)**. 

$$
Z = 1 + \frac{B(T)}{V} + \frac{C(T)}{V^2} + \frac{D(T)}{V^3} + \cdots
$$

It can also be written as a polynomial in **P** as:

$$
Z = 1 + B'P + C'P^2 + D'P^3 + \cdots
$$

$$
B' = \frac{B}{RT}, \quad C' = \frac{C - B^2}{R^2T^2}
$$

The **Virial Coefficients** $B$, $C$, etc., represent interactions between molecules and are temperature dependent. However, since higher-order terms are usually small, we often limit the Virial EoS to only two or three terms. This gives us a truncated form:

$$
Z = 1 + \frac{B(T)}{V} \quad \text{or} \quad Z = 1 + \frac{B(T)}{V} + \frac{C(T)}{V^2}
$$


#### Finding Virial Coefficients

The **Virial EOS** can also be written as:

$$
Z = 1 + \frac{B(T)\ P}{RT} + \frac{C(T) - B^2}{R^2T^2}P^2 + \cdots
$$

Remember that **Virial Coefficients** are functions of temperature only. This allows us to find the **Second Virial Coefficient (B)**:

$$
B = \lim_{P \to 0} \left( \frac{\partial Z}{\partial P} \right)_T
$$

Usually, the Virial EOS is truncated by keeping only the first term:

$$
Z = 1 + \frac{B(T)P}{RT}
$$

Rearrange as:

$$
V = B(T) + \frac{RT}{P}
$$


## Other EOS

### Redlich–Kwong EOS 

$$
P = \frac{RT}{V - b} - \frac{a}{V(V + b)\sqrt{T}}
$$

$$
a = \frac{0.42748 R^2 T_c^{2.5}}{P_c}
$$

$$
b = \frac{0.08664 R T_c}{P_c}
$$

$$
Z = 1 + \frac{B}{V} - \frac{A}{V(V + B)\sqrt{T_r}}
$$

$$
A = \frac{0.42748 \frac{P_c}{P} }{ \left( \frac{T}{T_c} \right)^{2.5} }
$$

$$
B = \frac{0.08664 \frac{P_c}{P} }{ \frac{T}{T_c} }
$$


### Soave-Redlich-Kwong Equation of State (SRK EOS)

The SRK EOS is given by:

$$ 
p = \frac{R T}{V - b} - \frac{a \alpha}{V (V + b)} 
$$

$$ a = \frac{\Omega_a R^2 T_c^2}{P_c} = \frac{0.42748 R^2 T_c^2}{P_c} $$

$$ b = \frac{\Omega_b R T_c}{P_c} = \frac{0.08664 R T_c}{P_c} $$

$$\alpha = \left( 1 + \left( 0.48508 + 1.55171 \omega - 0.15613 \omega^2 \right)(1 - T_r^{0.5}) \right)^2$$
$$T_r = \frac{T}{T_c}$$$$ \Omega_a \approx 0.42748 $$$$ \Omega_b \approx 0.08664 $$

By substituting into the reduced form:

$$
p_r = \frac{R T_r T_c}{P_c V_c (V_r - \frac{\Omega_b}{Z_c})} - \frac{\frac{\Omega_a}{Z_c^2} \alpha(\omega, T_r)}{V_r (V_r + \frac{\Omega_b}{Z_c})}
$$

The cubic equation in terms of the compressibility factor $Z$ is given by:

$$
0 = Z^3 - Z^2 + Z (A - B - B^2) - AB
$$
 
 $$ A = \frac{a \alpha P}{R^2 T^2} $$
 
 $$ B = \frac{b P}{RT} $$
 
### Patel-Teja EOS
 The Patel-Teja equation of state is given by: $$ P = \frac{RT}{V - b} - \frac{A(T)}{(V + c)(V - b)} - \frac{B}{V^2} $$
 
 $$ A(T) = \theta_{PT}(T) \cdot b \cdot (b + c) - cb $$

  $$ \theta_{PT}(T) = A + B T + C T^2 $$
  
 **$A, B, C$**: Empirical coefficients determined from experimental data.
 
### Ghoderao-Dalvi-Narayan (GDN) EOS

> [!Fact] Guess what?
> The Ghoderao-Dalvi-Narayan (GDN) EOS was developed at ICT Mumbai.

The GDN EOS excels in predicting the thermodynamic properties of 334 pure compounds, including saturated vapor pressure, liquid density, and heat capacities. It requires a limited set of parameters—critical temperature, critical pressure, Pitzer's acentric factor, critical compressibility factor, and two parameters for the alpha function—making it user-friendly. The EOS demonstrates high accuracy, particularly in predicting saturated liquid density, outperforming other models such as GDN1, Modified Peng-Robinson (MPR), and Patel-Teja (PT). Furthermore, its temperature-dependent covolume parameter $b$ effectively addresses thermodynamic inconsistencies at extreme conditions, enhancing its reliability. 
- **Comprehensive Property Prediction**: Accurately predicts multiple thermodynamic properties. 
- **Minimal Parameter Requirement**: Requires only critical and acentric factor data. - **High Accuracy**: Superior performance in saturated liquid density predictions. 
- **Thermodynamic Consistency**: Avoids inconsistencies at extreme temperatures and pressures.

The GDN EOS is expressed as:

$$
P = \frac{RT}{V - b} - \frac{a \alpha(T)}{V(V + d) + c(V - d)} 
$$

- **Constants**:
  - **$a$**, **$b$**, **$c$**, **$d$**: Parameters specific to the EOS.
- **$\alpha(T)$**: A temperature-dependent function that must satisfy the following properties:
  1. $\alpha(T) \geq 0$ and continuous.
  2. $\frac{d^2 \alpha(T)}{dT^2} \leq 0$ and continuous.
  3. $\frac{d^3 \alpha(T)}{dT^3} \geq 0$ and continuous.
  4. $\frac{d \alpha(T)}{dT} \leq 0$.

- The PREOS is derived by setting \( c = d = b \).
- The SRK EOS is derived by setting \( c = 0 \) and \( d = b \).
- The Patel-Teja (PT) EOS is recovered by setting \( d = b \).

To ensure an inflection in the $P-V$ curve at the critical point, the constants are given by:

$$
\begin{align*}
a &= \Omega_a \left(\frac{RT_c}{P_c}\right)^2 \\
b &= \Omega_b \frac{RT_c}{P_c} \\
c &= \Omega_c \frac{RT_c}{P_c} \\
d &= \Omega_d \frac{RT_c}{P_c}
\end{align*}
$$

Where $\Omega_a$, $\Omega_b$, $\Omega_c$, and $\Omega_d$ are proportionality constants.

The following conditions must be satisfied at the critical point:
1. $$ \left. \frac{\partial P}{\partial v} \right|_{T_c} = 0 $$
2. $$ \left. \frac{\partial^2 P}{\partial v^2} \right|_{T_c} = 0 $$
$$
Z^3 + A_Z Z^2 + B_Z Z + C_Z = 0
$$

Where is the compressibility factor. The coefficients $A_Z, B_Z, C_Z$ are defined as:

$$
\begin{align*}
A_Z &= \frac{P}{RT} \left(c + d - b\right) - 1 \\
B_Z &= \frac{P^2}{R^2 T^2} \left(\frac{a\alpha}{P} -bc -bd -cd\right) - \frac{P}{RT}(c+d)\\
C_Z &= \frac{P^3}{R^3 T^3} \left(bcd + \frac{RT}{P} cd - \frac{a \alpha b}{P} \right)
\end{align*}
$$

### Benedict-Webb-Rubin EOS
The BWR EOS is given by: $$ P = \frac{RT}{V - b} - \frac{a}{V^2} - \frac{c}{V^3} - \frac{d}{V^6} $$
- **$a$**: Attraction parameter 
- **$b$**: Volume occupied by molecules 
- **$c$**: Third virial coefficient 
- **$d$**: Fourth-order interactions
## Revisiting Departure Functions

> [!tip] Trust Me!
> I Bet they are more important then they seemed earlier.

### Residual Enthalpy

$$
H^R = \int_0^P \left[ V - \left(\frac{\partial V}{\partial T}\right)_P \right] dP
$$
$$
\because d(PV) = VdP + PdV
$$
$$
H^R = \int^P_0 d(PV) -\int^P_0 PdV - \int^P_0 T\left(\frac{\partial V}{\partial T}\right)_PdP
$$
$$
= \int^{PV}_{RT} d(PV) -\int^V_{\infty} PdV - \int^P_0 T\left(\frac{\partial V}{\partial T}\right)_PdP
$$
From the Triple Product Rule, we have:

$$
\left( \frac{\partial V}{\partial T} \right)_P \left( \frac{\partial P}{\partial V} \right)_T \left( \frac{\partial T}{\partial P} \right)_V = -1
$$

This simplifies to:

$$\left( \frac{\partial V}{\partial T} \right)_P \, dP = - \left( \frac{\partial P}{\partial T} \right)_V dV$$

Hence, re-substituting:

$$H^R = PV - RT -\int^V_{\infty} PdV + \int^P_0 T\left( \frac{\partial P}{\partial T} \right)_V dV$$
$$
H^R = PV - RT - \int^V_{\infty} \left(\frac{RT}{V-b}-\frac{a}{V^2}\right)dV + \int^P_0 \left(\frac{RT}{V-b}\right) dV
$$
$$
H^R = PV - RT - \frac{a}{V}
$$
Therefore, for Van der Waals EOS:

>$$\frac{H^R}{RT} = z - 1 - \frac{A}{z}$$

### Residual Entropy

$$
S^R = (S - S^{IG})_{T, P} = - \int_{T,P=0}^{T,P}\left[ \left( \frac{\partial V}{\partial T} \right)_P - \frac{R}{P}\right] dP
$$
$$
S^R =  \int_{T,P=0}^{T,P}\left[ \frac{R}{P} - \left( \frac{\partial V}{\partial T} \right)_P \right] dP
$$
$$
\because d(PV) = VdP + PdV
$$
$$
\frac{R}{P} dP = R \frac{d(PV)}{PV} - R \frac{dV}{V} = R\ d\ln(PV) - \frac{R}{V} dV
$$
$$
\therefore S^R = R \int^{PV(T,P)}_{PV = RT} d \ln(PV) - \int^{P=P(T,V)}_{P=0} \left[\left( \frac{\partial V}{\partial T} \right)_P + \frac{R}{V}dV\right]   
$$

Using the Triple Product Rule and simplifying :

$$
\therefore S^R = R \int^{PV(T,P)}_{PV = RT} d \ln(PV) + \int^{V=V(T,P)}_{V=\infty} \left[\left( \frac{\partial P}{\partial T} \right)_V - \frac{R}{V}\right] dV  
$$
$$
S^R = R \ln \left( \frac{PV}{RT} \right)+ \int^{V=V(T,P)}_{V=\infty} \left[\left( \frac{\partial P}{\partial T} \right)_V - \frac{R}{V}\right] dV
$$

Differentiating VDW EOS wrt T and resubstituting we get:

$$
S^R = R \ln Z + \int^{V=V(T,P)}_{V=\infty}\left[ \frac{R}{V - b} - \frac{R}{V}\right] dV
$$
$$
S^R = R\ln Z + R  \ln \left[\frac{V - b}{V}\right]^V_{V=\infty}
$$
$$
S^R = R\ln Z + R\ln \left[1 - \frac{b}{V}\right]
$$

and since, $z = \frac{PV}{RT} and B = \frac{Pb}{RT}$ we get:

$$
\frac{S^R}{R} = \ln \left[Z \left(1 - \frac{B}{Z}\right)\right]
$$

Therefore, for Residual function of Entropy Van der Waals EOS:

>$$\frac{S^R}{R} = \ln (Z - B)$$


### Residual Internal Energy

$$U^R = U - U^{IG} = \int_{V=\infty}^V \left[T \left(\frac{\partial P}{\partial T}\right)_V - P \right]dV$$
Similarly we can prove that:

$$\frac{U^R}{RT} = - \frac{A}{Z}$$

### Residual Volume

$$V^R = \frac{RT}{P}(Z - 1)$$

## For PR EOS:

### Residual Volume ($V^R$) 

$$ V^R = V - V^{\text{ig}} = V - \frac{RT}{P} = \frac{RT}{P} (Z - 1) $$

### Residual Enthalpy ($H^R$) 
$$ H^R = \int_0^P \left[V - T \left( \frac{\partial V}{\partial T} \right)_P \right] dP $$
>$$ \frac{H^R}{RT} = Z - 1 + \frac{T}{2\sqrt{2}bRT} \frac{da}{dT} \ln \left( \frac{Z + (1 + \sqrt{2})B}{Z + (1 - \sqrt{2})B} \right) $$

Where:
$$ \frac{da}{dT} = -0.45724 \frac{R^2 T_c^2}{P_c} \kappa \sqrt{\frac{\alpha}{T T_c}} $$

### Residual Entropy ($S^R$)
$$ S^R = \int_0^P \left[\left( \frac{\partial V}{\partial T} \right)_P - \frac{R}{P}\right] dP $$ Upon integration, we get: 

>$$\frac{S^R}{R} = \ln (Z - B) + \frac{\frac{da}{dT}}{2 \sqrt{2} b R T} \ln \left( \frac{Z + (1 + \sqrt{2})B}{Z + (1 - \sqrt{2})B} \right)$$

### Residual Internal Energy ($U^R$)

Residual internal energy is given by: 

$$
\frac{U^R}{RT} = \frac{T\frac{da}{dT} - a}{2 \sqrt{2} b R T} \ln \left( \frac{Z + (1 + \sqrt{2})B}{Z + (1 - \sqrt{2})B} \right) 
$$

### Residual Gibbs Energy ($G^R$)

$$\boxed{ \frac{G^R}{RT} = Z - 1 - \ln(Z - B) - \frac{A}{2 \sqrt{2} B} \ln \left( \frac{Z + (1 + \sqrt{2})B}{Z + (1 - \sqrt{2})B} \right) }$$ 
 - $a(T)$: Attraction parameter that depends on temperature through the function $\alpha(T_r)$. 
 - $b$: Volume exclusion parameter or co-volume.
## For Virial EOS:
### Residual Enthalpy

$$
 H^R = \int_0^P \left[V - T \left( \frac{\partial V}{\partial T} \right)_P \right] dP 
$$
$$
 H^R = \int_0^P \left[V - T \left( \frac{R}{P} - \frac{dB}{dT} \right) \right] dP 
$$
$$
H^R = \int_0^P \left[T \frac{dB}{dT} + B \right] dP 
$$
$$
H^R = BP - PT\frac{dB}{dT}
$$
### Residual Entropy

$$
 S^R = \int_0^P \left[\left( \frac{\partial V}{\partial T} \right)_P - \frac{R}{P}\right] dP 
$$
$$
 S^R = \int_0^P \left[\frac{R}{P} - \frac{dB}{dT} - \frac{R}{P}\right] dP 
$$
$$
S^R = -P  \frac{dB}{dT}
$$

## Clausius-Clapeyron Relation 

Consider the equation:
$$
dG = VdP - SdT
$$
$$
V^V dP - S^V\, dT = V^L dP - S^L\, dT
$$
$$(V^V - V^L)\,dP = (S^V - S^L)\,dT$$
$\Delta G$ across $G^L \longleftrightarrow G^V$ transition is $0$:
$$
\Delta G = 0 = \Delta H - T\Delta S 
$$
$$
\frac{\Delta H_{vap}}{T} = \Delta S
$$
Very far away from the critical point (i.e., at lower pressure), the substance behaves like an ideal gas:
$$
(V^V - V^L) \, dP = \left(\frac{H^V - H^L}{T}\right) \, dT 
$$
$$
V^V \, dP \approx \left(\frac{H^V - H^L}{T}\right) \, dT 
$$
$$
\frac{RT}{P^{sat}} \, dP^{sat} = \frac{\Delta H_{vap}}{T} \, dT 
$$
$$
d(\ln P^{sat}) = \frac{\Delta H_{vap}}{RT^2} \, dT
$$
This is the Clausius-Clapeyron Relation; it is only valid when pressure is low, $V^V >> V^L$, and vapor behaves as an Ideal Gas.
$$
\ln \frac{P_2}{P_1} = - \frac{\Delta H}{R} \left[\frac{1}{T_2} - \frac{1}{T_1}\right]
$$
This relation helps us understand the temperature dependence of vapor pressure and is crucial for phase transitions.
### Poynting Correction Factor
The Poynting correction factor accounts for the non-ideal behavior of gases when they are under pressure, particularly in situations where gas phase interactions become significant. 
$$
d\left(\frac{G}{RT}\right) = \frac{V\,dP - S\,dT}{RT} - \frac{H - TS}{RT^2}\,dT 
$$
$$
d\left(\frac{G}{RT}\right) = \left(\frac{V}{RT}\right)\,dP - \left(\frac{S}{RT}\right) -\left(\frac{H}{RT^2}\right)\, dT + \left(\frac{S}{RT}\right)dT
$$
$$
\frac{\partial \left(\frac{G^R}{RT}\right)}{\partial P}\bigg|_T = \frac{V^R}{RT} 
$$
$$
\frac{\partial}{\partial P} \left(\ln \frac{f}{P}\right) = \frac{V^R}{RT} = \frac{V - V^{IG}}{RT} = \frac{V}{RT} - \frac{1}{P} 
$$
Integrating both the sides we get,
$$
\int_{f^{L_{sat}}}^{f^L} d\left(\ln \frac{f}{P}\right) = \int_{P^{sat}}^{P} \left[\frac{V}{RT} - \frac{1}{P}\right] dP 
$$
$$
\ln \frac{f^L}{f^{L_{sat}}} = \frac{V^L}{RT} (P - P^{sat}) - \ln P 
$$
$$
\ln \frac{f^L}{f^{L_{sat}}} = \frac{V^L}{RT} (P - P^{sat}) 
$$
Hence we get the **Poynting Correction Factor.**
$$\boxed{
f^L = f^{L_{sat}} \exp\left[\frac{V^L (P - P^{sat})}{RT}\right]}
$$
The Poynting factor reflects how the chemical potential of a gas deviates from ideal behavior due to intermolecular forces. As pressure increases, the assumption of an ideal gas becomes less valid, necessitating corrections to accurately predict vapor-liquid equilibria.

## Third Law of Thermodynamics

> [!Quote] The 3rd Law
> The entropy of all substances in the perfect crystalline state (for solids) or the perfect liquid state (for example, for helium) is zero at the absolute zero of temperature (0 K).
