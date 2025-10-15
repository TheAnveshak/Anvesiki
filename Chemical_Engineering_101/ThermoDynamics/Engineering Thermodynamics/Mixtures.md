
[[Conservation of Energy]]
[[Entropy]]
[[Will Name it Later...]]
[[EOS]]
# Multicomponent Mixture Systems

## $\Delta M_{mix}$

We are studying the change in extensive properties (e.g., volume, internal energy, Gibbs free energy and entropy) during phase equilibrium processes at constant pressure and temperature, where entropy generation is zero. This is useful for several applications:
- **Chemical equilibrium**: Understanding the behavior of mixture components during reactions in various phases.
- **Separation processes**: These processes, like liquid-liquid extraction, crystallization, humidification, and distillation, often occur under phase equilibrium conditions.

In general, the property $M$ represents any **Extensive properties** like $V$, $U$, $G$, $S$ et al and the total property M will depend upon factor like Temperature, pressure etc.$$ M^t = f(T, P, n_i) \quad n = \Sigma n_i \quad M^t = nM \quad n_i = x_in $$ 
Where:
- $M^t$: Total extensive property of the system
- $n = \sum n_i$: Total number of moles
- $M^t = nM$: Total property as a function of per-mole properties
- $n_i = x_i n$: Moles of component $i$ related to mole fraction $x_i$

The partial molar property $\bar{M}_i$ is given by:

$$
\bar{M}_i = \left( \frac{\partial M^t}{\partial n_i} \right)_{P, T, n_{j \neq i}} 
$$
## Gibbs-Duhem Equation:
The total differential of any property $M^{tL}$ for a liquid component can be expressed as:
$$
dM^t = \frac{\partial M^t}{\partial P}\bigg|_{T, n} dP + \frac{\partial M^t}{T}\bigg|_{P, n} dT + \sum_i \frac{\partial M^t}{\partial n_i}\bigg|_{P, T, n_{j \neq i}} dn_i
$$
$$
d(n M^t) = \frac{\partial (n M^t)}{\partial P}\bigg|_{T, n} dP + \frac{\partial (n M^t)}{T}\bigg|_{P, n} dT + \sum_i \frac{\partial (n M^t)}{\partial n_i}\bigg|_{P, T, n_{j \neq i}} d(x_in)
$$
Rewriting in terms of mole fractions:
$$
d(n M^t) = \frac{\partial (n M^t)}{\partial P}\bigg|_{T, n} dP + \frac{\partial (n M^t)}{T}\bigg|_{P, n} dT + \sum_i \bar{M_i} d(x_in)
$$
$$
ndM + Mdn = n \frac{\partial M^t}{\partial P}\bigg|_{T} dP + n \frac{\partial M^t}{\partial T}\bigg|_{P} dT + \sum_i \bar{M_i} n dx_i + \sum_i \bar{M_i} x_i dn
$$
Hence from this we get,
$$
n\left[dM - \left(\frac{\partial M}{\partial T}\right)_{P,n} dT - \left(\frac{\partial M}{\partial P}\right)_{T, n} dP - \Sigma \bar{M_i} dx_i \right] + \left[M - \Sigma \bar{M_i} x_i\right] dn = 0
$$

We assume that the first term in the bracket is negligible, leading us to the expression $M = \Sigma \bar{M_i} x_i$. However, this assumption is not entirely accurate due to the presence of the mixing contribution $\Delta_{mix} M$.

### Final Form of Gibbs-Duhem Equation:

The Gibbs-Duhem equation is thus derived as:
$$
\boxed{
\left( \frac{\partial M}{\partial T} \right)_{P, n} dT + \left( \frac{\partial M}{\partial P} \right)_{T, n} dP - \sum_i x_i d\bar{M_i} = 0
}
$$

The Gibbs-Duhem Equation in Differential form is : 
$$
dG^{t} = \left( \frac{\partial G^{t}}{\partial P} \right)_{T, n} dP + \left( \frac{\partial G^{t}}{\partial T} \right)_{P, n} dT + \sum_i \left( \frac{\partial G^{t}}{\partial n_i} \right)_{P, T, n_{j \neq i}} dn_i
$$
Simplifying this:
$$ \boxed{
dG^{t} = V^{t} dP - S^{t} dT + \sum_{i=1}^n \left( \frac{\partial G^{t}}{\partial n_i} \right)_{P, T, n_{j \neq i}} dn_i}
$$

### Chemical Potential 

The **chemical potential** of a species is a measure of the change in the system's energy when the number of particles of that species is varied, particularly in processes like **chemical reactions** or **phase transitions**.
When **temperature** and **pressure** are held constant, the chemical potential $\mu_i$ is equivalent to the **partial molar Gibbs free energy for $i^{th}$ component**:
$$
\mu_i = \left( \frac{\partial G}{\partial n_i} \right)_{T, P, n_{j \neq i}}
$$
This relationship is fundamental to understanding **chemical equilibrium** and **phase equilibrium**. It acts as the driving force behind diffusion, phase changes, and reactions, linking **thermodynamics** with the behavior of individual components in a mixture.
- **In phase equilibrium**, the chemical potential of a component must be the same in all phases.
- **In chemical reactions**, equilibrium is achieved when the chemical potentials of reactants and products are balanced.
Chemical potential plays a key role in determining the direction and extent of reactions and phase transformations.
Hence,
$$
dG^{t} =  -\ S^{t} dT + V^{t} dP + \sum_{i=1}^n \mu_{i} dn_i
$$
### Enthalpy Relationship
The enthalpy can be expressed in terms of entropy (S) and pressure (P):
$$
dH = \left( \frac{\partial H}{\partial P} \right)_{S,N_i} dP + \left( \frac{\partial H}{\partial S} \right)_{P,N_i} dS + \sum_{i=1}^C \left( \frac{\partial H}{\partial N_i} \right)_{P,S,N_j} dN_i
$$
This leads us to:

$$
dH = V dP + T dS + \sum_{i=1}^C \left( \frac{\partial H}{\partial N_i} \right)_{P,S,N_j} dN_i
$$

The term $\left( \frac{\partial H}{\partial N_i} \right)_{P,S,N_j}$ is *not* the partial molar enthalpy, which is defined 
as $H_i = \left( \frac{\partial H}{\partial N_i} \right)_{T,P,N_j}$.

From the relation $H = G + TS$, we can derive:

$$
dH = dG + T dS + S dT = -S dT + V dP + \sum_{i=1}^c \bar{G_i} dN_i + T dS + S dT
$$
Simplifying leads to:

$$
dH = V dP + T dS + \sum_{i=1}^c \bar{G_i} dN_i 
$$

Comparing equations, we find:

$$
\left( \frac{\partial H}{\partial N_i} \right)_{P,S,N_j} = G_i = \left( \frac{\partial G}{\partial N_i} \right)_{T,P,N_j}
$$
Similarly, we can derive:

$$
dU = T dS - P dV + \sum_{i} G_i dN_i
$$

$$
dA = -P dV - S dT + \sum_{i} G_i dN_i
$$

$$
\bar{G}_i = \left( \frac{\partial U}{\partial N_i} \right)_{S,V,N_j} = \left( \frac{\partial A}{\partial N_i} \right)_{T,V,N_j}
$$

---

### Summability Relationship:

If the second term is zero, we get the **summability relationship**:

$$
M = \sum_i \bar{M_i} x_i
$$

Which states that the extensive property per mole of a mixture is the mole-fraction-weighted sum of the partial molar properties of the components.

However, note that in reality:
$$
M \neq \sum_i M_i x_i
$$
There exists a mixing term:

$$M = \Delta_{mix} M + \sum_i M_i x_i$$

---

## Redlich-Kister Expansion

$$
\Delta_{mix}M = \sum_{i=1}^n x_i(\bar{M_i} - M_i)
$$

For a binary mixture, the excess property due to mixing, $\Delta_{mix}M$, can be expressed as:

$$
\Delta_{mix}M = x_1(\bar{M_1} - M_1) + x_2(\bar{M_2} - M_2)
$$
Since $x_2 = 1 - x_1$:
$$
\Delta_{mix}M = x_1(\bar{M_1} - \bar{M_2} - (M_1 - M_2)) + \bar{M_2} - M_2
$$

Differentiating with respect to $x_1$:
$$
\frac{\partial \Delta_{mix}M}{\partial x_1} = (\bar{M_1} - \bar{M_2} - (M_1 - M_2))
$$

Multiplying by $x_1$ and rearranging, we get:
$$
\bar{M_2} - M_2 = \Delta_{mix}M - x_1 \frac{\partial \Delta_{mix}M}{\partial x_1}
$$

Similarly:
$$
\bar{M_1} - M_1 = \Delta_{mix}M + x_2 \frac{\partial \Delta_{mix}M}{\partial x_1}
$$

### General Property Change Due to Mixing:

For any property change due to mixing, we can use a polynomial expansion, namely the **Redlich-Kister expansion**:

$$
\Delta_{mix}M = x_1x_2 \left[ A + B(x_1 - x_2) + C(x_1 - x_2)^2 + D(x_1 - x_2)^3 + \dots \right]
$$

For a binary mixture, often a second-degree polynomial is sufficient:
$$
\Delta_{mix}M = x_1x_2 \left[ A + B(x_1 - x_2) \right]
$$
Substituting $x_2 = 1 - x_1$:
$$
\Delta_{mix}M = x_1(1 - x_1) \left[ A + B(2x_1 - 1) \right]
$$
### Differentiating with Respect to $x_1$:

$$
\frac{\partial \Delta_{mix}M}{\partial x_1} = 2B(x_1 - x_1^2) + (1-2x_1) \left[ (A - B) + 2x_1B \right]
$$

From this, we can express the partial molar properties:
$$
\bar{M_1} - M_1 = (A + 3B)x_2^2 - 4Bx_2^3
$$
Similarly:
$$
\bar{M_2} - M_2 = (A - 3B)x_1^2 - 4Bx_1^3
$$

---

### Infinite Dilution Properties

The concentration does not change on adding more solvent at infinite dilution.
For infinite dilution conditions, we define the partial molar properties at infinite dilution:

$$
\lim_{x_1 \to 0} (\bar{M_1} - M_1) = \bar{M_1}^\infty - M_1
$$
$$
\lim_{x_2 \to 0} (\bar{M_2} - M_2) = \bar{M_2}^\infty - M_2
$$
Here, $\bar{M_1}^\infty$ and $\bar{M_2}^\infty$ are called **infinite dilution partial molar properties**.

---

### The Differential Form of the Equations of Change for a Multicomponent System

#### Species Balance

$$
\frac{dN_i}{dt} = \sum_{k=1}^{K} (\dot{N}_i)_k + \sum_{j=1}^{M} \nu_{ij} \dot{X}_j 
$$
#### Mass Balance

$$
\frac{dN}{dt} = \sum_{k=1}^{K} \dot{N}_k + \sum_{i=1}^{C} \sum_{j=1}^{M} \nu_{ij} \dot{X}_j
$$
#### Energy Balance

$$
\frac{dU}{dt} = \sum_{k=1}^{K} (\dot{N} H)_k + \dot{Q} + \dot{W_s} - P \frac{dV}{dt} 
$$

#### Entropy Balance

$$
\frac{dS}{dt} = \sum_{k=1}^{K} (N \dot{S})_k + \frac{\dot{Q}}{T} + \dot{S}_{\text{gen}} 
$$

Where:
$$
\dot{N}_k = \sum_{i=1}^{C} (\dot{N}_i)_k, \quad (\dot{N} H)_k = \sum_{i=1}^{C} (\dot{N}_i H_i)_k, \quad (\dot{N} S)_k = \sum_{i=1}^{C} (\dot{N}_i S_i)_k
$$


---

## Chemical Potential at Equilibrium between Phases

For a Control Volume, the Gibbs-Duhem Equation is given by:
$$
dG^{CV} = -\ S^{CV} dT + V^{CV} dP + \sum_{i=1}^n \left( \frac{\partial G^{tV}}{\partial n_i} \right)_{P, T, n_{j \neq i}} dn_i^V + \sum_{i=1}^n \left( \frac{\partial G^{tL}}{\partial n_i} \right)_{P, T, n_{j \neq i}} dn_i^L
$$
But we know that for any Control Volume at Equilibrium,
$$
dG^{CV} = -\ S^{CV} dT + V^{CV} dP
$$
Thus,
$$\sum \bar{G_i}^L dn_i^L + \sum \bar{G}_i^L dn_i^V = 0$$
and  $dn_i^L  =  -dn_i^V$, hence:
$$\therefore \bar{G}_i^L = \bar{G}_i^V$$
Hence the Chemical Potential for a component is same at **Phase Equilibrium**.

