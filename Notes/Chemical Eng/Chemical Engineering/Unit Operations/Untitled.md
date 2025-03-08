**$$
F\ =\ L\ +\ V
$$**
$Fz_f = Lx_L + Vy_V$ 

|              |               |               |          |          |
| ------------ | ------------- | ------------- | -------- | -------- |
| P_T          | 760           |               | z_F      | 0.7      |
|              |               |               |          |          |
| Material     | BP            | A             | B        | C        |
| Cyclopentane | 49.2          | 15.8602       | 2589.2   | 231.36   |
| Benzene      | 80            | 15.9037       | 2789.01  | 220.79   |
|              |               |               |          |          |
|              |               |               |          |          |
|              |               |               |          |          |
| Temp         | P_{Av} (mmHg) | P_{Bv} (mmHg) | x_A      | y_A      |
| 50           | 778.8004      | 271.5562      | 0.962936 | 0.986757 |
| 55           | 914.5521      | 327.3064      | 0.736819 | 0.886657 |
| 60           | 1068.06       | 391.8874      | 0.544406 | 0.765077 |
| 65           | 1240.821      | 466.2636      | 0.379231 | 0.619156 |
| 70           | 1434.372      | 551.4503      | 0.236204 | 0.445795 |
| 75           | 1650.288      | 648.5113      | 0.111291 | 0.241661 |
| 80           | 1890.174      | 758.5563      | 0.001276 | 0.003173 |

![[Pasted image 20241223113342.png]]

## Relative Volatility
Relative Volatility of a component $A$ in a mixture indicates the **Ease** of its **SEPARATION** from another component $B$.
$$
\alpha_{AB} = \frac{(\text{conentration of }A / \text{concentration of }B)_\text{vapour}}{(\text{conentration of }A / \text{concentration of }B)_\text{liquid}}
$$
$$
y = \frac{\alpha x}{1+(\alpha-1)x}
$$

![[Pasted image 20241223113324.png]]

## Equilibrium in Multicomponent Systems
$$
y_i = \frac{P_j}{P_T} = \frac{x_j P^V_j}{\sum^{i=n}_{i=n}}
$$

## $F = D + W$

Component A Balance:
$Fz_F = Dx_D + Wx_W$ 
$(D+W)z_F = Dx_D +Wx_W$ 
Enthalpy balance:
$FH_F + Q = DH_D + WH_W$
$$-\frac{W}{D} = \frac{x_{_D}-z_{_F}}{x_{_W}-z_{_F}} = \frac{H_D -[H_F+ \frac{Q}{F}]}{}$$


> [!Question] ?
> A liquid mixture containing 50 mol% each of Benzene and Toluene at 40C is to be continuously flash vaporize 60 mol% of the feed . The residual liquid product contains 35 mol% benzene. The enthalpies per mole of feed the liquid product and the vapor product  are 2, 5 and 30 kJ/mol resp. Calculate the energy to be supplied in kJ to the feed. Calculate the heat added in kJ per mole of vapour product.

Basis : 100gmol
Vapor : 60gmol - 15gmol B and 45gmol T
Liquid : 40gmol -35gmol B and 5gmol T
$100 \times 2 + Q = 60 \times 30 +40 \times 5$
$\therefore Q = 1800kJ$

## Steam Distillation
![[Pasted image 20250106114819.png]]

For an Ideal Binary Mixture: $y_A = P_A/P_T = x_AP_A^V/P_T$
- A and B are immiscible their mixture exerts a vapour Pressure = sum of vapour pressure of individual components
- Bubble Point of such mix < boiling point of A and B
- Separation of High Boiling materials 
- Separation and Purification Of Hazardous Materials 
### Separation OF Immiscible Substances A and B

$P =P_A^V +P^V_B \quad\ \quad\ \implies\ \quad\ P_B^V =P-P^V_A$
- if $m_A$ moles of A are volatilised and $m_B$ moles of B moles of steam, at equm,
- $\frac{m_A}{m_A} = \frac{P^V_A}{P-P_A^V} \implies m_A = m_B \frac{P_A^V}{P-P_A^V}$
- $P_A<P_A^V$ does not operate at equm
- A factor called 'Vaporization Efficiency - E' is defined as $P_A = EP_A^V$
- $\implies m_A =M_B \frac{EP_A^V}{P-P_A^V}$
- To estimate the steam requirement: $m_B=m_A\frac{P_B^V}{EP_A^V}$

> [!Question] Question
> Chlorobenzene is flammable liquid and is used as a common solvent . It is proposed to purify Chlorobenzene by steam distillation at 100C and at Atmospheric pressure. A small scale unit is charged with 1 liter od crude Chlorobenzene containing non-volatile impurities. Calculate the steam required assuming that Chlorobenzene is immiscible with Water.
 

| Compound  | BP(C)             | *A*               | *B*                 | *C*    |
| --------- | ----------------- | ----------------- | ------------------- | ------ |
| **CB**    | 131.5             | 16.4              | 3485.35             | 224.87 |
| **Water** | 100               | 18.5882           | 3984.92             | 233.43 |
|           |                   |                   |                     |        |
| ***T***   | ***$P_A^{sat}$*** | ***$P_B^{sat}$*** | ***$P-P_B^{sat}$*** |        |
| 50        | 41.26463          | 92.62632          | 667.3737            |        |
| 60        | 64.40047          | 149.5635          | 610.4365            |        |
| 70        | 97.51883          | 233.9919          | 526.0081            |        |
| 80        | 143.7032          | 355.7729          | 404.2271            |        |
| 90        | 206.6091          | 527.0992          | 232.9008            |        |
| 100       | 290.4858          | 762.7314          | -2.73135            |        |
![[Pasted image 20250106122254.png]]
The intersection is at $91\degree C$   
The density of CHLOROBENZENE $\rho = 1107 kg/m^3\ \ \ \therefore m=1.107kg \implies n_{CB} = 9.84$ 
$n_{water} = 9.84\times \frac{547.5}{214} \approx 25.17 gmol = 453.06g$
































































