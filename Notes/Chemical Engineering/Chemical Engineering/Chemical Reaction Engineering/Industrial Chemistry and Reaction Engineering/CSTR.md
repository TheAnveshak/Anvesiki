### Conversion of A

$$
\frac{V}{v} = \tau = \frac{C_A -C_{A0}}{r_A} = \frac{C_{A0}(1-x_A) - C_{A0}}{r_A}
$$
$$
\tau = \frac{-x_A C_{A0}}{k C_A^{n}}
$$


> [!Question] Question
> Consider the order of Reaction to be $n = -1$ and $r_A = 40C_A^{-1}$
> $F_{A0} = 30 gmol/s$ , $x_A = 0.3$, $F_A = 21 gmol/s$


hence,
$$
\begin{align*}
\tau &= \frac{(150 \times(1-0.3) - 150)\frac{gmol}{m^3}}{-40 (s^{-1})(\frac{gmol}{m^3})^2 \times 105^{-1}(\frac{gmol}{m^3})^{-1}}\\
&= \frac{-45 \times 105}{-40}\\
\therefore \tau &= 118.125 s
\end{align*}
$$
hence, $V = 23.6m^3$

For PFR,
$$
\begin{align*}
\frac{V}{v} &= \int^{C_A}_{C_{A0}} \frac{dC_A}{r_A} = \int^{C_A}_{C_{A0}} \frac{dC_A}{-k C_A^{-1}} \\
\frac{V}{0.2} = \int^{150}_{105} \frac{C_A dC_A}{40}\\
\therefore V &= \frac{0.2}{40} \left[\frac{150^2 - 105^2}{2}\right]\\
\therefore V &= 28.7 m^3
\end{align*}
$$
Hence, $V_{CSTR} < V_{PFR}$
So CSTR is better for $-ve$ order reactions.

For Power Law Model,
- For $0$ order reaction : CSTR and PFR both have same **volume.**
- For $-ve$ order reactions : $V_{CSTR} < V_{PFR}$ $\implies$ CSTR is better.
- For $+ve$ order reaction : $V_{CSTR} > V_{PFR}$ $\implies$ PFR is better.


> [!Question] Question continues 
> For $n=1$

$$
\begin{align*}
\tau &= \frac{(150 \times(1-0.3) - 150)\frac{gmol}{m^3}}{-40 (s^{-1})(\frac{gmol}{m^3})^2 \times 105^{0}(\frac{gmol}{m^3})^{-1}}\\
&= \frac{-45 }{-40}\\
\therefore \tau &= 1.125 s
\end{align*}
$$
hence, $V = 0.225m^3$
For PFR, $V = 0.225 m^3$

> [!TIP] Remember 
> "$0$" Order reactions cannot be "$0$" Order througout the range of $C_A$
> Rection order "$0$" increases so that $C_A$ only approaches "$0$"
> In extreme (Hypothetical) Case of "$0$" Order Reactions, $C_A =0$ at $\tau =\frac{C_{A0}}{k}$

Consider $A\xrightarrow{k}B$ ; $r_A = -kC_A^n$ in a CSTR

$$
\begin{align*}
\frac{C_A - C_{A0}}{r_A}  &=\tau \\
k \tau C_A^2 + C_A - C_{A0} &= 0 \\
\therefore C_A &= \frac{-1 \pm \sqrt{1^2 - k\tau (-C_{A0})}}{2k\tau}
\end{align*}
$$

$\tau = 1.02 \times 10^{-4} s$, $k = 40 s^{-1}(\frac{gmol}{m^3})^{-1}$, $C_{A0} = 150 \frac{gmol}{m^3}$
using the above equation, $C_A = 105 \frac{gmol}{m^3}$

## Limiting Reactant

When the reactions start with the stoichiometric coefficient of reactions the conversion of all reactants have to be same. 
However, amount of all the reactants reacted may not be the same.

For a general reaction,
$$
A\ +\ z\ B\ \longrightarrow \ p\ C\ +\ q\ D
$$
$z,\ p,\ q\ \geq\ 0$ .
$n_i$ = 1 + $z$  and  $n_f$ = $p + q$
Let, at time $t$ the conversion of component $A$ is $x_A$ ,
$x_B = \frac{\text{Intial } B - B\ \text{at }x_A\% \text{ conversion of }A}{\text{Initial } B}$
hence conversion of $B$ is $z \times x_A$ 
For products $C$ is $x_A \times p$ and $D$ is $x_A \times q$
hence, $n_t = (1 - x_A)(1+ z) + x_A (p + q)$
Hence at any time the total number of moles in Control Volume  is $n_i = \left[\min\{(1+z),(p+q)\}, \max\{(1+z),(p+q)\}\right]$ .

Let us consider the case when A is the Limiting Reagent
i.e. $\frac{n_{A\ 0}}{1} <\ \frac{n_{B\ 0}}{z}$ 
the number of moles of unreacted $B$ will be $(n_{B\ 0} - n_{A\ 0}\ z)$
hence, $n_t = n_{A\ 0}[(1 - x_A)(1+ z) + x_A (p + q)] +(n_{B\ 0} - n_{A\ 0}\ z)$ 

Let the initial mole ratio $= \frac{N_{B\ 0}}{N_{A\ 0}} =\ M\ =\ z\ \frac{x_A}{x_B}$ .

## Variable Volume 
	$$V = V_0\ (1+\epsilon\ x)$$
- $V_0$ = initial Volume 
- $V$ = Volume at time t
- $\epsilon$ = expansion factor
- $x$ = conversion rate

$$
\begin{align*}
N_A \bigg|_{t+\Delta t} - N_A \bigg|_t &= r_A V dt\\
\frac{dN_A}{dt} &= r_A V\\
\frac{dN_A}{dt} &= r_A\ V_0\ (\ 01+\varepsilon\ x_A\ )\\
\int^t_0 dt &= \int\frac{dN_A}{(1+\varepsilon x_A)r_A V_0} \\
\end{align*}
$$
for $A \xrightarrow{k} P\cdots$  (1st order reaction)
$$
\begin{align*}
\int^t_0 dt &= \int\frac{dN_A}{(1+\varepsilon x_A)\frac{-kN_A}{V} V_0} \\
t &= \frac{-1}{k}\int\frac{dN_A}{(1+\varepsilon x_A)N_A} \\
t &= \frac{-1}{k(1+\varepsilon x_A)}\bigg|\ln \frac{N_A}{N_{A0}}\bigg|\\
\end{align*}
$$
consider the Concentration changes,
$$
\begin{align*}
\int^t_0 dt &= \int\frac{dN_A}{(1+\varepsilon x_A)r_A V_0} \\
\end{align*}
$$

$$
\begin{align*}
x_A = \frac{N_{A0} - N_A}{N_{A0}} &\implies dx_A = \frac1{N_{A0}}\times (- dN_A)\\
t &= \int\frac{-N_A\ dx_A}{(1+\varepsilon\ x_A)\ r_A\ V_0} \\
t &= \int^{x_A}_0\frac{-C_{A0}\ dx_A}{r_A\ (1+ \varepsilon\ x_A)}\\
\end{align*}
$$

$$
\begin{align*}
C_A v - C_{A0} v_0 &= r_A V\\
C_A\ v_0\ (1+\varepsilon x_A) - C_{A0}v_0 &= r_A V\\
v_0\ [C_A\ (1+\varepsilon x_A) - C_{A0}] &= V
\end{align*}
$$


## CSTR : variable volume and limiting variable

$$
\frac{x_A}{x_B} = \frac{z}{M}
$$
$$
\frac{C_A}{C_{A0}} = \frac{1-x_A}{1+\varepsilon _A x_A} \quad\ ; \quad\ \frac{C_B}{C_{B0}} = \frac{1-x_B}{1-\varepsilon _B x_B}
$$
$$
{\varepsilon _B} = \frac{M}{z}\varepsilon _A
$$
For, $A + zB \to z_1P$ 
$$
\frac{C_P}{C_{A0}} = \frac{M + z_1 x_A}{1 + \varepsilon _A x_A}
$$
![[Pasted image 20241226090322.png]]
For, $x_A = 0$ $V = 100 + 200 + 100 = 400$
at, $x_A = 1$  $V = -100 + 600 + 100 = 600$
$\therefore\   \varepsilon_A = \frac{600-400}{400} =0.5$
$\varepsilon_B =\frac{\varepsilon_A C_{B0}}{zC_{A0}} = \frac{1}{3}$
$\frac{C_A}{C_{A0}} = \frac{1-x_A}{1+\varepsilon _A x_A} \implies \frac{40}{100} = \frac{1-x_A}{1+\frac{x_A}{2}} \implies x_A = 0.5$
$\therefore x_B =\frac{zC_{A0}x_A}{C_{B0}} =  0.75\ \ \implies C_B = 40$   

![[Pasted image 20241226100210.png]]
 $\because$ constant pressure constant volume
1. $x_B = 0.4,\ C_A=20,\ C_B=120$ 
2. infeasible ig
3. $\varepsilon_A = \frac{-2}{3}$
4. infeasible solution
![[Pasted image 20241227105114.png]]
4.5. $\varepsilon_A = 0$ ; $\frac{C_A}{C_{A0}} = \frac{1-x_A}{1+\varepsilon_Ax_A} \frac{T_0P}{TP_0}$ $\implies \frac{20}{100} = \frac{1-x_A}{1}\frac{400 \times 3}{300 \times 4}\ \implies x_A= 0.8$
	$\implies x_B = \frac{z}{M}x_A = 0.4$ 
4.6. $\varepsilon_A = \frac{2}{3}$ ; $\frac{C_A}{C_{A0}} = \frac{1-x_A}{1+\varepsilon_Ax_A} \frac{T_0P}{TP_0}$ 
	$\implies \frac{20}{100} = \frac{1-x_A}{1+\frac{2}{3}x_A}\frac{1000 \times 5}{400 \times 4}\\ \implies x_A= 0.818\ \implies x_B = 0.409 \implies C_B =130$ 
4.7. *Commercial Popcorn Popping Popcorn Popper* :)  
	$28 = 1(1+\frac{31-1}{1}x_A) \implies x_A=0.9$ 90% of popcorn popped 

$$
aA +bB \to cC + dD
$$

| Initial <br>t = ==0== |                                      Change                                       |                                     Final<br>t = t                                     |
| :-------------------: | :-------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------: |
|       $N_{A0}$        |                                   $-N_{A0}x_A$                                    |                                   $N_{A0}-N_{A0}x_A$                                   |
|       $N_{B0}$        |                              $-\frac{b}{a}N_{A0}x_A$                              |                             $N_{A0}-\frac{b}{a}N_{A0}x_A$                              |
|       $N_{C0}$        |                              $\frac{c}{a}N_{A0}x_A$                               |                                 $\frac{c}{a}N_{A0}x_A$                                 |
|       $N_{D0}$        |                              $\frac{d}{a}N_{A0}x_D$                               |                                 $\frac{d}{a}N_{A0}x_A$                                 |
|       $N_{I0}$        |                                         -                                         |                                        $N_{I0}$                                        |
|       $N_{T0}$        | $-N_{A0}x_A$$-\frac{b}{a}N_{A0}x_A$+$\frac{c}{a}N_{A0}x_A$+$\frac{d}{a}N_{A0}x_A$ | $N_{T0} + N_{A0}x_A\left[\frac{c}{a} + \frac{d}{a}-1- \frac{b}{a}\right]_{_{=\delta}}$ |
$$
C_A = \frac{N_{A0}(1-x_A)}{V}\ ;\ C_B = \frac{N_{B0}-\frac{b}{a}N_{A0}x_A}{V}\ ;\ C_C = \frac{N_{C0}-\frac{c}{a}N_{0}x_A}{V}\ ;\ C_D = \frac{N_{D0}-\frac{d}{a}N_{A0}x_A}{V}\
$$

$$
\begin{align*}
\frac{N_T}{N_{T0}} &= \frac{N_{T0}+ \delta N_{A0}x_A}{N_{T0}}\\
\\
&= 1+ \delta \left(\frac{N_{A0}}{N_{T0}}\right)x_A\\
\\
\frac{N_T}{N_{T0}} &= 1 + \delta y_{A0} x_A\\
\\
&= 1+\varepsilon_Ax_A \\
\\
\therefore \varepsilon_A &= \frac{N_T -N_{T0}}{N_{T0}x_A}\\
\end{align*}
$$

![[Pasted image 20241227122126.png]]



