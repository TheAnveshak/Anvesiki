1. Rectification Section: Above the feed section, more refined in volatile component. Flow Rates are $L$ for liquid and $V$ for Vapour.
2. Stripping Section: Below The Feed Section, enriched with lesser volatile component. Flow rates are $L'$ for liquid and $V'$ for vapour.

- $L_n$ & $V_N$ are molar liquid and vapour flow rate leaving the $n_{th}$ stage.
- $Q_C$ = heat removal from condenser.
- $Q_B$ = heat supply rate to boiler.
- F = feed rate tot column.
- D = rate of Distillate removal from reflux drum.
- W = rate of bottom product removal from reboiler.
- R = L/D = Reflux Ratio, Ratio of liquid flow rate L from the reflux drum to the flow rate of the Distillate.

##### MEBC for Envelope 1
$V = L + D$ 
$Vy = Lx + Dx_0$ 
$VH_V = LH_L + DH_0 + Q_C$ 

##### MEBC for Envelope 2
$D =- L_n + V_{n+1}$ 
$Dx_0 = -xL_n + yV_{n+1}\implies y_{n+1} = \frac{L/D}{V/D}\implies y_{n+1} = \frac{R}{R+1}x_n +\frac{1}{R+1}x_0$
$DH_0 = -L_nH_L + V_{n+1}H_V-Q_C$ 

##### MEBC for Envelope 3
$W + V'_{m+1} = L'_m$
$Wx_W + V'_{m+1}y_{m+1} = L'_mx_m \implies y_{n+1} = \frac{L'}{L'-w} x_n + \frac{W}{L'-W}x_w$ 
$WH_W+V'_{m+1}H_{y,m+1} = L'_mH_{L,m}$

##### MEBC for Envelope 4
$F=D+W$
$Fz_F = Dx_D+Wx_W$
$FH_F = Dh_D+WH_W+Q_C-Q_B$ 

##### Assumptions
1. Constant Molar Overflow of liquid and Vapour form one tray to another over any section of the distillation column
2. $L_1 = L_2 = \ldots = L_n=L$ for Rectifying Section
3. $L'_m=L'_{m+1} = \ldots=L'_N =L'$ for stripping Section
4. $V_1=V_2=\ldots=V_n = V$ for Rectifying Section
5. $V'_{m+1} = \ldots= V'_{N+1} = V'$ for Stripping Section
### Number of Trays : McCabe_Thiele Method
1. Define degree if Separation for a given feed flow compostion
2. Assume reflux ratio id not given
3. Calculate the top and bottom flow rates by overall material balance
4. Calculate $P^{sat}\ \ or\ \ P^V$ for each component using Antoine Equation
5. Calculate the equilibrium x-y data from $P^{sat}$ values using Rault's Law
6. Draw Equilibrium Curve using x-y data
7. Locate $z_F,x_D,x_W$ on the diagonal of the x-y curve
8. Calculate and Draw operating Lines for the rectifying and stripping section + feed line if required
9. Draw steps between equilibrium curve and operating lines to find out the number of Ideal Stages.
10. When feedline is crossed do changeover from one operating line to other: transition from rectification to stripping section











































