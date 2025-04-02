
## First Order System
$$
G_p(s) = \frac{k_p}{\tau s+1}
$$

$$
\begin{align*}
Y(s) &= \frac{K_p}{\tau s+1}\frac{M}{s}\\
Y(s) &= MK_p {(1-e^{\frac{-t}\tau})}\\
\frac{dY}{dt} &= \frac{M}{\tau}K_p e^{\frac{-t}{\tau}}\\

\end{align*}
$$
![](Images/Pasted image 20241231112422.png)
for, $k=10,\ \tau=1.5$ 
When t=$1\times \tau$ $\frac{C(t)}{K_pM} = 1- e^{-1} = 0.632$  
the system gives $63.2\%$ response for a 1st order System.

**For a Thermometer** in a system which is being heated from $30\degree C$ to $50\degree C$
$mc_P T |_{t+\Delta t}-mc_PT|_t = hA(T_0-T)$
$\frac{dT}{dt} = \frac{hA}{mc_p} (T_0-T)$
Taking Laplace transform,
$s\bar{T}(s) - \bar T(0) = k\bar T_0(s) - k\bar T(s)$   
$\frac{\bar T(S)}{\bar T_0(S)} = \frac{k}{k+s} = \frac{1}{\frac{1}{k}s +1}$ 
$\therefore \tau = \frac{1}{k} = \frac{mc_p}{hA}$ (m,$c_p$,A of the bulb or the material in the bulb are constant, hence we can change the time constant by changing )
![](Images/Pasted image 20241231114545.png)
#### Impulse Response of 1st Order Reaction
$R(s) = \delta(s) = 1$
$C(s) = \frac{K}{\tau s+1}$
$C(s) = \frac{K/\tau}{s+1/\tau}$ 
$$
C(t) = \frac{K}{\tau}e^{-t/\tau}
$$
#### Relation Between Step and Impulse Response
$\frac{dc(t)}{dt} = \frac{d()}{}$

#### Ramp Function
$R(t) = kt \implies R(s) = \frac{k}{s^2}\implies C(s) = \frac{kK_p}{s^2 (\tau s +1)}$
$C(s) = \frac{kK_p}{s^2(\tau s +1)} = \frac{kK_p}\tau \times \left[\frac{-\tau^2}{s}+\frac{\tau}{s^2}+\frac{\tau^2}{s+\frac{1}{\tau}}\right]$ 
$C(t) = \frac{kK_p}\tau (-\tau^2 + \tau t + \tau^2 e^{-t/\tau})$ 
$C(t) = kK_p(-\tau +t+\tau e^{-t/\tau})$  
![](Images/Pasted image 20241231120647.png)
#### First Order - Sinosoidal 
$x(t) = A\sin (\omega t) \implies x(t) = A \frac{\omega}{s^2+\omega^2}$
$Y(t) = \frac{K_p}{\tau s +1} x(s) \implies Y(s) =$
$Y(s) = \frac{K_p A\omega}{\tau}\left[\frac{\frac{\tau^2}{1+\omega^2\tau^2}}{s+\frac{1}{\tau}} +\frac{s\frac{-\tau^2}{1+\omega^2\tau^2}}{s^2+\omega^2}+ \frac{\frac{\tau}{1+\omega^2\tau^2}}{s^2+\omega^2}\right]$ 
$Y(t) = \frac{K_p A\omega}{\tau(1+\omega^2\tau^2)}\left[\frac{{\tau^2}}{s+\frac{1}{\tau}} -\frac{s{\tau^2}}{s^2+\omega^2}+ \frac{{\tau}}{s^2+\omega^2}\right]$  
$Y(t) =  \frac{K_p A}{(1+\omega^2\tau^2)}(\tau e^{-t/\tau} -\tau \omega\cos \omega t+  \sin \omega t)$  
$Y(t) =  {K_p A}({\frac{\tau e^{-t/\tau}}{(1+\omega^2\tau^2)}} +\frac{1}{\sqrt{1+\omega^2\tau^2}} \sin (\omega \tau +\phi))$  
$y(t)\bigg|_{t \to \infty} = \frac{A}{\sqrt{1+\omega^2\tau^2}}K_p \sin (\omega \tau + \phi)$   $\phi = \tan^{-1}\left(\frac{\omega^2\tau^2}{1}\right)$
Noise is just a sine wave with a very high frequency
