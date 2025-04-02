
Consider a cylindrical tank with CSA = $A$ and height =$h$ and Flowrates be $F_{in,\rho}$ and $F_{out, \rho}$ in $m^3/hr$ .
Since from Bernoulli's equation we know that, $v^2 = h$ (i.e. kinetic head is proportional to potential head)
$F_o = k\sqrt{h}$ 
Now Consider that the flow rate is the function of time.
At any time $t$ the mass inside the vessel = $V\rho$ = $Ah(t)\rho$ 
at time $t + \Delta t$ mass inside the vessel = $Ah(t+\Delta t)\rho$ 
$\therefore$ Accumulation = $Ah(t+\Delta t)\rho - Ah(t)\rho$ 
In time interval $\Delta t$,
mass Flow into the vessel = $F_{in}(t) \Delta t\rho$
mass Flow out of the vessel = $F_o(t)\Delta t \rho$
$\because$ Accumulation = input - output
$h(t) \to$ State Variable
$t \to$ independent variable

$$
\lim_{\Delta t \to 0} \frac{Ah(t+\Delta t)\rho - Ah(t)\rho}{\Delta t} = \lim_{\Delta t \to 0}\frac{F_{in}(t) \Delta t\rho-F_o(t)\Delta t \rho}{\Delta t}
$$
$$
\begin{align*}
A\frac{dh(t)}{dt} &= F_{in}(t) - k\sqrt{h(t)}\\
\frac{dh(t)}{dt} &= \frac{F_{in}}{A} - \frac{k}{A}\sqrt{h(t)}
\end{align*}
$$
$h_0 = 3$, $A=4$, $F_0=5$ 


