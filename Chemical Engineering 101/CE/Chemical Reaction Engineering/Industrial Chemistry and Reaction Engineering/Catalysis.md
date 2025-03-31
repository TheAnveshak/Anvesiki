Rate of Attachment  $=k_AP_{CO}C_V$ 
Rate of Desorption   = $k_{-A}C_{CO.S}$
$$
\begin{align*}
r_{ADsorption} &= k_AP_{CO}
\end{align*}
$$

Show that the adsorption isotherm of A in the presence of another Absorbate B is given by relationship,
$$
C_{A.S} = \frac{K_AP_AC_t}{1+K_AP_A+K_BP_B}   
$$

## Haber Bosch Process
$H_2 +2S \leftrightarrow 2H.S$
$N_2 +2S \leftrightarrow 2N.S$  Rate Limiting step
$N.S+H.S \leftrightarrow HN.S+S$
$HN.S+H.S \leftrightarrow H_2N.S+S$
$H_2N.S+H.S \leftrightarrow H_3N.S +S$
$H_3N.S \leftrightarrow H_3N+S$

- Rapid
CO + S ←→ CO ⋅ S
NO + S ←→ NO ⋅ S
- Rate-limiting
NO.S+CO.S ←→ $CO_2$ +N.S+S
- Rapid
N ⋅ S + N ⋅ S ←→ $N_2$⋅S 
$N_2$ ⋅ S → $N_2$ + S

At equilibrium,
$r_{ADe} = k_A\left(P_{Ceq}-\frac{K_BP_{B eq} P_{Peq}}{K_SK_C}C_v\right) = 0$
$P_{Ceq} = \frac{K_BP_{Beq}P_{Peq}}{K_SK_C}\implies \frac{P_{Beq}P_{Peq}}{P_{Ceq}} = \frac{K_sK_C}{K_B}$
$\therefore  K_P = \frac{K_SK_C}{K_B}$

$r_{AD} = \frac{K_A\left(P_C-\frac{P_BP_P}{K_P}\right)C_t}{\left(1+\frac{K_BP_BP_P}{K_S}+K_BP_B\right)}$
$r'_{C0}\approx C_tk_AP_{C0}$


$r_S = k_S\left[C_{C.S}-\frac{P_PC_{B.S}}{K_S}\right]$


## Single Catalyst Pore Model - Wheeler
- Chemical Reaction on Catalyst Surface
- One end of the pore is closed
- Diffusion and Reaction Simultaneously

Boundary COnditions,
- at $x=0,\ C_A =C_{AS}$
- at $x =L,\ C_A =C_{AL}$
- at $x=L,\ \frac{dC_A}{dx}=0$
Rate of A OUT at x+dx - Rate of A IN at x = 'A' reacted on the differential surface between '$x$' & '$x+dx$'

$-D_A\frac{dC_A}{dx}\bigg|_{x+dx} + D_A\frac{dC_A}{dx}\bigg|_x =r_A dV$ 
$\frac{\pi d^2}{4}\left(-D_A\frac{dC_A}{dx}\bigg|_{x+dx} + D_A\frac{dC_A}{dx}\bigg|_x\right) =-k_{SR}C_A \pi d.dx$ 
$D_{Ae} \frac{d^2C_A}{dx^2} = 4\frac{k_{SR}C_A}{d}$
$C_A = A e^{mx} + B e^{-mx}$
$\frac{C_A}{C_{AS}} = \frac{e^{-2mL}e^{mx}}{1+e^{-2mL}}+\frac{e^{-mx}}{1+e^{-2mL}}$
$\frac{C_A}{C_{AS}} = \frac{e^{m(x-L)}+e^{m(L-x)}}{e^{mL}+e^{-mL}}$
$\frac{C_A}{C_{AS}} = \frac{\cosh(m(L-x))}{\cosh(mL)}$
$\frac{dC_A}{dx}\big|_{x=0}= -C_{AS}\tanh(mL)$
$\frac{dC_A}{dx}\big|_{x=0} = m(A-B)$
Flux$\big|_{x=0}  -D_A\frac{dC_A}{dx}\big|_{x=0} = -D_A m(A-B)$
Flux$\big|_{x=0} = -D_AC_{AS}m\left[\frac{e^{mL}-e^{-mL}}{e^{mL}+e^{-mL}}\right]$
Flux$\big|_{x=0} = -D_AC_{AS}m\left[\tanh{mL}\right]$
Rate = $\frac{\pi}{4}d^2C_{AS} D_A m \tanh(mL)$

Consider the Hypothetical condition where the complete catalytic surface of the pore is exposed to max concentration i.e. $C_{AS}$ 

$\text{Rate}_{\text{kinetic}} = k_{SR} C_{AS} \pi d .L$

$\frac{\text{Rate}_{\text{actual}}}{\text{Rate}_{\text{kinetic}}} = \frac{dD_A\sqrt{\frac{4k_{SR}}{dD_{Ae}}}\tanh(L){\sqrt{\frac{4k_{SR}}{dD_{Ae}}}}}$
$\frac{\text{Rate}_{\text{actual}}}{\text{Rate}_{\text{kinetic}}} = \frac{dD_A \sqrt{\frac{4k_{SR}}{dD_{Ae}}} \tanh(L)}{\sqrt{\frac{4k_{SR}}{dD_{Ae}}}}$

$\frac{\text{Rate}_{\text{actual}}}{\text{Rate}_{\text{kinetic}}} = dD_A \tanh(L)$


##  

$\left[D_{Ae}\frac{dC_A\rho_c}{dr}4\pi r^2\right]_r- \left[D_{Ae}\frac{dC_A \rho_c}{dr}4\pi r^2\right]_{r+dr}= r_A \rho_c4 \pi r^2dr$
$\frac{D_{Ae}}{r^2}\frac{d}{dr}\left(r^2\frac{dC_A}{dr}\right) = kC_A$
$\frac{1}{r^2}\frac{d}{dr}\left(r^2\frac{dC_A}{dr}\right) = \frac{k}{D_{Ae}}C_A= \alpha^2C_A$
$y = C_A.r\implies \frac{dy}{dr} = r\frac{dC_A}{dr}+C_A\implies \frac{dC_A}{dr} = \frac{1}{r}\frac{dy}{dr}-\frac{y}{r^2}$
$\frac{1}{r^2}\frac{d}{dr}\left(r^2\frac{1}{r}\frac{dy}{dr}-r^2\frac{y}{r^2}\right) = \alpha^2\frac{y}{r}$
$\frac{d^2y}{dr^2} = \alpha^2y$


#### Interpretation of Thiele Modulus
$\Phi = L \sqrt{\frac{k}{D_A}} = \frac{R}{3} \sqrt{\frac{k}{D_A}}$
$\Phi^2 = \frac{kC_{AS}\rho_c \frac{4}{3}\pi R^3}{D_A.\frac{C_{AS}-0}{R/3}}$

$\Phi^2 = \frac{\text{kinetic Rate of reaction}}{\text{maximum diffusion rate}}$
$\eta = \frac{\text{actual rate of reaction}}{\text{kinetic rate of reaction}}$
$\Phi^2\eta =\Phi_W= \frac{\text{actual rate of reaction}}{\text{maximum rate of diffusion}}$
$\eta = \frac{1}{\Phi}\left[\frac{1}{\tanh(3\Phi)} - \frac{1}{3\Phi}\right]$
Rate $=4\pi R^2C_{AS}\sqrt{D_Ak}\left[\frac{1}{\tanh(3\Phi)}-\frac{1}{3\Phi}\right]$












































































