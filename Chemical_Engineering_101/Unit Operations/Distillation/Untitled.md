### Number of Trays: Tray by Tray Method
1. Define degree of separation for a given feed flow composition
2. Assume Reflux Ratio - Underwood equation
3. Calculate top and bottom flow rates by overall material balance
4. Start with the bottom mole fraction of liquid $x_W$ 
5. Assume some temperature value between boiling points of mixture
6. Calculate $P^{sat}$ for each component using Antoine Equation
7. Calculate the total pressure P, this pressure will be equal to the column pressure 
8. Use goal seek on MS-Excel and set the P to desired value
9. Calculate the activity coefficients $\gamma$ for non ideal mixtures using the suitable thermodynamic model
10. Calculate the mole fraction of vapour, y  in equilibrium with x for all components
11. Calculate the mole fraction of liquid x on the upper tray using the value of y and using material balance across the tray.
12. Start with this value of x and repeat the steps from 4 to 11 until the value of x matches with the defined degree of separation $x_D$ in distillate.

## Column Height and Diameter Estimation
Liquid_Vapour flow Parameter: $F_{LV} = \frac{m_L}{m_V}\sqrt{\frac{\rho_V}{\rho_L}}$ 
$K_1 = U_{fV,n}\sqrt{\frac{\rho_V}{\rho_L-\rho_V}}$ ; Flooding Vapour Velocity = $U_{fV,n}$
For liquid Surface Tension $\sigma$ = 20 dynes/cm
$K_1^{corrected} = K_1(\sigma/20)^{0.2}$

Tray Spacing : Typically $450<TS<750$ mm
- Higher tray spacing may be required to accommodate entrainment and frothing
- D > 1500 mm, TS > 600 mm
- D < 1200 mm, TS < 450 mm 
Column Height = Number of real trays $\times$ TS
\+ TS $\sim$ 1.5 time the regular TS or minimum 750 mm on feed entry or draw off trays
\+ 1500 mm above the upper tray
\+ 750 mm below tray
\+ 1200 mm for manholes , 1 manhole per 8-10 trays


> [!Question] why 
> A mixture of benzene, toluene and p-xylene is to be separated continuously in a tray tower. The top product should have more than 95 mole% of benzene resp. The feed in liquid is at boiling point.
> 1. Calculate the x-y data for non ideal mixture
> 2. Calculate the number of theoretical plates
> 3. Recommend column height and area for 50% efficiency

| Component | BP  | A       | B        | C       | MW  | Density |
| --------- | --- | ------- | -------- | ------- | --- | ------- |
| Benzene   | 80  | 4.72583 | 1660.652 | -1.461  | 78  | 878.7   |
| Toluene   | 110 | 4.23679 | 1426.448 | -45.957 | 92  | 863.6   |
| P-Xylene  | 129 | 4.14553 | 1474.403 | 55.377  | 106 | 860     |

$L = 1.014\ \ kg/hr$  $\rho_{L_{avg}feed} = 866.69\ kg /m^3$  $\rho_{L_{avg}top} = 877.94\ \ kg/m^3$



![[images/WhatsApp Image 2025-02-04 at 2.37.52 PM.jpeg]]






![[images/WhatsApp Image 2025-02-04 at 2.37.58 PM.jpeg]]










![[images/WhatsApp Image 2025-02-04 at 2.38.03 PM.jpeg]]

















