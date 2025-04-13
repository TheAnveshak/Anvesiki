![[Screenshot_20250407_093537.png]]

Mass Into The vessel at any time $t = F(t) C_{A0}\big|_t$
Mass out of the vessel at any time $t+\Delta t = F(t) C_{A}\big|_{t+\Delta t}$
Accumulation in Tank in time period $\Delta t=V \frac{ C_A(t)\big|_{t+\Delta t} - C_A(t)\big|_t}{\Delta t}$
Moles of A reacted $= -kC_AV$
$\frac{F(t)C_{A0} \Delta t-F(t)C_A\Delta t}{ \Delta t}=\lim_{\Delta t\to0}V \frac{ C_A(t)\big|_{t+\Delta t} - C_A(t)\big|_t}{\Delta t} -\frac{kC_AV\Delta t}{\Delta t}$

$F(t)C_{A0} = V\frac{dC_A}{dt} -kC_AV+ F(t)C_A$
$\frac{dC_A}{dt} = \frac{F(t)}{V}C_{A0}-\frac{F(t)}{V}C_A  -kC_A$
$\frac{dC_A}{dt} = f(F,C_A,C_{A0})$
At steady state:
$0 = \frac{F_s(t)}{V}C_{A0s}-\frac{F_s(t)}{V}C_{As}  -kC_{As}$
$\frac{dC_A}{dt} = f_{ss}+\frac{\partial f}{dF}\bigg|_{ss}(F-F_s)+\frac{\partial f}{dC_{A0}}\bigg|_{ss}(C_{A0}-C_{A0s})+\frac{\partial f}{dC_{A}}\bigg|_{ss}(C_{A}-C_{As})$
$\frac{d\bar C_A}{dt} = \frac{C_{A0s}-C_{As}}{V}\bar F-\left(\frac{F_s}{V}+k\right)\bar C_A+\frac{F_s}{V}\bar C_{A0}$

Taking the Laplace Transform:
$s\bar C_A(s) = \frac{C_{A0s}-C_{As}}{V}\bar F(s)-\left(\frac{F_s}{V}+k\right)\bar C_A(s)+\frac{F_s}{V}\bar C_{A0}(s)$

$\bar C_A(s) = \frac{\frac{C_{A0s}-C_{As}}{V}}{\left(s+\frac{1}{\tau}+k\right)}\bar F(s)+\frac{\frac{F_s}{V}}{\left(s+\frac{1}{\tau}+k\right)}\bar C_{A0}$
$\tau = \frac{1}{\frac{F_s}{V}+k}$
$K_{p1} = \frac{C_{A0s}-C_{As}}{V}$
$K_{p2} = \frac{F_s}{V}$

$\bar C_A(s) = \frac{K_{p1}\tau}{\left(\tau s+1\right)}\bar F(s)+\frac{K_{p2}\tau}{\left(\tau s+1\right)}\bar C_{A0}$

![[Screenshot_20250407_094356.png]]


> [!Question]  Producing 200 Million Pounds per Year in a CSTR - Fogler
> Close to 16 billion pounds of ethylene glycol (EG) were produced in 2013. It previ-
ously ranked as the twenty-sixth most produced chemical in the nation on a total
pound basis. About one-half of the ethylene glycol is used for antifreeze, while the
other half is used in the manufacture of polyesters. In the polyester category, 88%
was used for fibers and 12% for the manufacture of bottles and films. The 2013 sell-
ing price for ethylene glycol was $0.60 per pound.
It is desired to produce 200 million pounds per year of EG. The reactor is to
be operated isothermally. A 16.1 mol/dm3 solution of ethylene oxide (EO) in water
is mixed (see Figure E5-2.1) with an equal volumetric solution of water containing
0.9 wt % of the catalyst H2SO4 and fed to a CSTR. The specific reaction-rate con-
stant is 0.311 min –1, as determined in Example 5-1. Practical guidelines for reactor
scale-up are given by Mukesh.1
(a) If 80% conversion is to be achieved, determine the necessary CSTR
volume.
(b) If two 800-gal reactors were arranged in parallel with the feed equally
divided, what would be the corresponding conversion?
(c) If two 800-gal reactors were arranged in series, what would be the cor-
responding conversion?

$F_C = 46.4 mol/s$
$C_{A0} = 16.1mol/L$
$F_{A0} = 46.4\times \frac{1}{0.8} = 58.0 mol/s = 3.625L/s$
$v = 5538L$

$G_p(s) = \frac{\frac{16.1-3.2}{3.625+5538\times5.2\times 10^{-3}}}{\frac{5538}{3.625+5538\times 0.0052}s+1}= \frac{0.398}{171s+1}$

$G_d(s) = \frac{\frac{3.625}{3.625+5538\times.0052}}{\frac{5538}{3.625+5538\times .0052}s+1} = \frac{0.112}{171s+1}$
Concentration/Composition Measurement is very very slow and will have a lag for simplicity we assume the slowest control loop to be 1.
Major dynamic lag is that of Control Valve.
Flow and Pressure measurement are very fast.
Using a Proportional Controller:
$\bar C(s)=\frac{G_pG_VG_C}{1+G_pG_VG_CH}\bar R(s) +\frac{G_L}{1+G_pG_VG_CH}\bar d(s)$
For regulatory:
$\frac{\bar C_A(s)}{\bar C_{A0}(s)} = \frac{G_L}{1+G_pG_VG_CH}$
$\frac{\bar C_A(s)}{\bar C_{A0}(s)} = \frac{G_L}{1+G_pG_VG_C} = \frac{\frac{0.112}{171s+1}}{1+\frac{0.398}{171s+1}\times K_c\left(1+\frac{1}{s}\right)\times 5\times 1}$
For Unit Step change,$\bar C_{A0}(s) = 1/s$
$\bar C_A(s) = \frac{\frac{0.112}{2K_c}}{\frac{171}{2K_c}s^2+\left(\frac{1}{2K_c}+1\right)s+1}$














































