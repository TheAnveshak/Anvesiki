- Final Product is a Solid.
- An Operation in which liquid in a wet solid/suspension/solution is removed by vapourization to obtain relatively liquid free solid
- Transport of heat and mass:  
- Reasons: 
	- to reduce transportation costs- reduce volume
	- Remove moisture
	- Provide definite property
	- Make material more suitable for handling
- Transport movement Classification
	- Capillary Forces
	- Pressure induced transport
	- Liquid/molecular Diffusion
	- Vapour Diffusion

![[Pasted image 20250217111636.png]]                                    https://www.google.com/url?sa=i&url=https%3A%2F%2Flink.springer.com%2Fchapter%2F10.1007%2F978-981-16-7289-7_5&psig=AOvVaw3XMDH4F_D8ML8amTNNfONQ&ust=1739857545492000&source=images&cd=vfe&opi=89978449&ved=0CBYQjRxqFwoTCNCjxsqAyosDFQAAAAAdAAAAABAJ

## Types of Moisture
![[Pasted image 20250224105427.png]]https://media.springernature.com/lw685/springer-static/image/chp%3A10.1007%2F978-981-16-7289-7_5/MediaObjects/510562_1_En_5_Fig12_HTML.png
- Equilibrium Moisture Content - a function of the relative humidity of the gas, the temperature of the gas and the nature of the solid and the liquid
- Unbound Moisture - Moisture in excess of bound moisture, vapor pressure same as that of free water.
- Bound Moisture - it is moisture adsorbed on the surface of the solids or absorbed within the solids, exerts a vapor pressure less than that of free water.
- Free Moisture - water in excess of equilibrium moisture a a given temperature.

$\mathcal{H} = \frac{\text{mass of water vapor}}{\text{mass of dry air}}$
$\%\text{humidity} = \frac{\text{Humidity of Air}}{\text{Humidity of saturated Air}}\times 100$
$\mathcal{R} = \frac{\text{Partial Pressure of Water in Air}}{\text{Vapor pressure of Water}}$
Humidity Volume = Volume of Air + Volume of Water Vapor = $\frac{22.4}{29}\frac{T}{273}+\frac{22.4}{18}\frac{T}{273}\ \ \ \frac{m^3}{kg}$

![[Pasted image 20250224111456.png]]https://pub.mdpi-res.com/materials/materials-17-03334/article_deploy/html/images/materials-17-03334-g001-550.jpg?1720174873
The difference is due to the moisture that is retained by the solid

## The Drying Rate Curve
- Time required for drying can be determined from a knowledge of the drying rate under a given set of condition
- Drying Rate = $f$(T, Humidity, Flow Rate, Properties of Gas and Solid)
- Change of mass of the solid after drying
- Change of Humidity content of Gas.
- $N = -\frac{W_s}{a}\frac{dX}{dt} \approx -\frac{W_s}{a}\frac{\Delta X}{\Delta t}$

![[Pasted image 20250224112452.png]]https://www.researchgate.net/publication/311651620/figure/fig4/AS:668529099550720@1536401166037/Drying-Curve-Showing-Moisture-Content-as-a-Function-of-Time-of-a-crop-Source-34-35.png
- BC - Constant Rate Drying
- BC and CD - Non linear drop in drying rate
- Beyond E - Equilibrium Moisture content Reached
![[Pasted image 20250224112937.png]]https://www.researchgate.net/publication/324161313/figure/fig1/AS:685422900428802@1540428962513/Drying-rate-curve-as-a-function-of-moisture-content-A-B-initial-adjustment-period-B-C.png

$t = -\frac{W_s}{a}\int^{X_f}_{X_i}\frac{dX}{N}=\frac{W_s}{a}\int^{X_i}_{X_c}\frac{dX}{N}+\frac{W_s}{a}\int^{X_c}_{X_f}\frac{dX}{N}$
$t = \frac{W_s(X_i-X_c)}{aN_c}+\frac{W_s}{a}\int^{X_c}_{X_f}\frac{dX}{pX+q}$
$t = \frac{W_s(X_i-X_c)}{aN_c} +\frac{W_s}{ap} \ln\frac{pX_c+q}{pX_f+q}=\frac{W_s(X_i-X_c)}{aN_c} +\frac{W_s}{ap} \ln\frac{N_c}{N_f}$
$t=\frac{W_s(X_i-X_c)}{aN_c} +\frac{W_s}{a}\frac{X_c-X_f}{N_c-N_f} \ln\frac{N_c}{N_f} = t_c+t_f$
$N = px+q$
At equilibrium , $0 = px+q \implies -q = px$
$\frac{x_c-x_f}{N_c-N_f} = \frac{x_c - x^*}{N_c-0}\implies  = \frac{N_c}{N_f} = \frac{px_c+q}{px_f+q}=\frac{x_c-x^*}{x_f-x^*}$
$t = t_c+t_f = \frac{W_s}{aN_c}(x_i-x_c)+\frac{W_s}{a}\frac{x_c-x^*}{N_c}\ln\frac{x_c-x^*}{x_f-x^*}$


> [!Question] Problem
> A batch of 120 kg wet saw dust with initial moisture content of 0.2 kg water/kg dry saw dust was fed to a Shelf Dryer. The exposed are for drying is 0.05 $m^2/kg$ dry saw dust. For how long the drying of this batch of saw dust should be carried out to achieve a moisture content of 0.1 kg water / kg dry saw dust.




> [!Question] Problem
> A batch of 120 kg wet saw dust with initial moisture content of 0.4 kg water/kg dry saw dust was fed to a Shelf Dryer. The exposed are for drying is 0.05 $m^2/kg$ dry saw dust. For how long the drying of this batch of saw dust should be carried out to achieve a moisture content of 0.1 kg water / kg dry saw dust.

$t _1= t_c+t_f = \frac{85.7}{0.05\times 85.7\times1.5}(0.4 - 0.25)+0$
$t_2 = t_c+t_f =0+\frac{85.7}{0.05\times 85.7}\frac{0.25-0.02}{1.5}\ln\frac{0.25-0.02}{0.1-0.02}$
$t = t_1+t_2 = 5.23\ hr$

For quadratic Relation between $N$ and $x$
$N = \beta x^2$
$\therefore t_f = \frac{W_s}{a}\int^{x_c}_{x_f}\frac{dx}{N} = \frac{W_s}{a\beta}\left[\frac{1}{x_f}-\frac{1}{x_c}\right] = \frac{W_s x_c^2}{aN_c}\left[\frac{1}{x_f}-\frac{1}{x_c}\right]$
 $t = t_c+t_f = \frac{85.7}{0.05\times 85.7\times1.5}(0.4 - 0.25) + \frac{85.7 0.25^2}{0.05\times85.7\times 1.5}\left[\frac{1}{0.1}-\frac{1}{0.25}\right]$
$t = 7\ hr$

$t = t_c + \sum_i t_{f_{i, linear}} +\sum_j t_{f_{j,power}}$


> [!Question] Question
> A $25 cm \times 25 cm \times 1 cm$ flat sheet wrighting 1.2kg intially was dried from both sides under constant drying rate conditions in a lab scale dryer. It took 1500 s for weight of the sheet to reduce to 1.05 kg.
> Another $1m\times1m\times1m$ flat sheet of the same material is to be dried in a tray dryer from one side only. Under the same constant drying rate conditions, calculate the time required for drying from its initial weight of 19.2kg to 17.6 kg

Answer : 2000 s


> [!Question] Question
> A chocolate sponge cake with a critical moisture content of 0.4kg/kg dry solid is dried from an initial moisture content of 0.6 kg/kg dry spolid to a final moisture content of 0.1 kg/kg dry soild in 5 hrs. The equilibrium moistyure content is 0. The drying rate regime is $2 kg/m^2h$
> 1. If the falling rate is linear function of the moisture content, calculate the mass of dry solid per unit area.
> 2. If the falling rate is proportional to the square of the moisture content, calculate the mass of the dry solid per unit area 

1. 13.25 $kg/m^2$ -  for a 100kg/hr prod facility a 37.7 $m^2$ area dryer required
2. 7.14 $kg/m^2$ - for a 100 kg/hr prod facility a 70 $m^2$ area dryer required

























































