[[Material and Energy Balance Calculations]]
[[Basic Concepts and Definitions]]
## **The First Law of Thermodynamics** :
*Although energy assumes many forms, the total quantity of energy is constant, and when energy disappears in one form it appears simultaneously in other forms.*

The Sum of Internal, Kinetic and Potential Energy of the system is :
$$ 
\theta = U + M\left(\frac{v^2}{2} + \psi\right) 
$$

So, the rate at which the Total energy "$\theta$" of the System changes is given by:
$$ 
\frac{d}{dt} \left\{ U^t + M \left( \frac{v^2}{2} + \psi \right) \right\} = 
\left(
\begin{array}{c}
\text{Rate at which energy} \\
\text{enters the system}
\end{array}
\right)
-
\left(
\begin{array}{c}
\text{Rate at which energy} \\
\text{leaves the system}
\end{array}
\right) 
$$

Streams flowing into and out of the control volume have internal, potential, and kinetic forms of energy associated with them with respect to the System and the surroundings and all may contribute to the energy change of the system. 

Accounting for the **energy flow accompanying Mass flow** we get:
$$ 
\sum_{k=1}^{K}\dot{M}_k \left( \hat{U} + \frac{v^2}{2} + \psi\right) 

$$

Accounting for the **total rate of heat flow into the system** by both conduction and radiation, so that $\dot{Q}$ is positive if energy in the form of heat flows into the system and negative if heat flows from the system to its surroundings :
$$ 
\dot{Q} = \sum \dot{Q}_k 
$$

Rate of Energy associated with mechanical energy is divided into several parts. First is the mechanical energy flow that occurs without deforming the system boundary (control volume) and is given by $\dot{W}_s$. Conventionally, the $\dot{W}_s$ is positive if the work is done on the system by the surrounding and negative if the system does work on the surroundings. The second part is the Electrical Energy flow through the system.
$$ 
\dot{W}_s = \pm EI 
$$
Where $E$ is the Electrical Potential Difference applied across the system and $I$ is the Current flow through the system.

The third part is the work due to the deformation and movement of System Boundaries as a result of an external Force acting on the system.
$$ 
\dot{W} = -P_{ext}\frac{dV^t}{dt} 
$$

A negative sign arises as the Work done by the external Force or Pressure (force per unit area) is positive but the result of it, i.e. the change in volume $\frac{dV^t}{dt}$ is negative.

The fourth part is **the work of flowing Fluid against Pressure**: This energy flow arises from the fact that as an element of fluid moves, it works on the fluid ahead of it, and the fluid behind it works on it.
$$ 
\left(
\begin{array}{c}
\text{Net rate at which work is done on} \\
\text{the system due to pressure forces}\\
\text{acting on fluids moving into}\\
\text{and out of the system}
\end{array}
\right)
= \sum_{k=1}^K \dot{M}_k (P\hat{V})_k 
$$

Collecting all the terms we get,
$$ 
\frac{d}{dt} \left\{ U^t + M \left( \frac{v^2}{2} + \psi \right) \right\} = \sum_{k=1}^{K}\dot{M}_k \left( \hat{U} + \frac{v^2}{2} + \psi\right) 
+ \dot{Q} + \dot{W}_s - P_{ext}\frac{dV^t}{dt} + \sum_{k=1}^K \dot{M}_k (P\hat{V})_k 
$$

Hence after combining the 1st and last term on LHS, we get:
### The General Energy Balance Equation
$$
\begin{equation}
\boxed{
\frac{d}{dt} \left\{ U^t + M \left( \frac{v^2}{2} + \psi \right) \right\} = \sum_{k=1}^{K}\dot{M}_k \left( \hat{H} + \frac{v^2}{2} + \psi\right)
+ \dot{Q} + \dot{W}_s - P_{ext}\frac{dV^t}{dt} 
}
\end{equation}
$$
$$
\begin{equation}
\boxed{
\frac{d}{dt} \left\{ U^t + N \left( \frac{v^2}{2} + \psi \right) \right\} = \sum_{k=1}^{K}\dot{N}_k \left( \underline{H} + \frac{v^2}{2} + \psi\right)
+ \dot{Q} + \dot{W}_s - P_{ext}\frac{dV^t}{dt}
}
\end{equation}
$$
## Thermodynamic Properties of Matter

The temperature dependence of the internal energy and enthalpy of substances, beyond ideal gases, can be determined by measuring the temperature rise ($\Delta T$) that results from adding heat to a $\textit{closed}$, $\textit{stationary}$ system. For a small quantity of heat added, the temperature rise $\Delta T$ is linearly related to the heat added ($Q$) and inversely proportional to the number of moles ($N$):
$$
\frac{Q}{N} = C \Delta T = c \{T(t_2) - T(t_1)\}
$$
where $c$ is a parameter and $Q$ is the heat added at time $t_1$ and $t_2$.
$$
U(t_2) - U(t_1) = Q = N c_V \{T(t_2) - T(t_1)\}
$$
$$
c_V = \frac{U(t_2) - U(t_1)}{N \{T(t_2) - T(t_1)\}} = \frac{\underline{U}(t_2) - \underline{U}(t_1)}{T(t_2) - T(t_1)}
$$
where $c_V$ represents the constant volume heat capacity. For a very small temperature difference, $c_V$ is defined as:
$$
c_V(T,V) = \lim_{T(t_2) - T(t_1) \to 0} \frac{U(t_2) - U(t_1)}{T(t_2) - T(t_1)} = \left( \frac{\partial U}{\partial T} \right)_V = \left( \frac{\partial U(T,V)}{\partial T} \right)_V 
$$
The measured parameter $c_V$ for a constant volume equals the temperature derivative of the internal energy at constant volume. Similarly, when $c$ is determined at a constant pressure, the heat added ($Q$) relates to the change in internal energy and pressure volume work:
$$
Q = U(t_2) + P(t_2)V(t_2) - U(t_1) - P(t_1)V(t_1) = H(t_2) - H(t_1) = N c_P \{T(t_2) - T(t_1)\}
$$
where $H$ denotes enthalpy, and $c_P$ is the constant pressure heat capacity. Thus,
$$
c_P(T,P) = \left( \frac{\partial H}{\partial T} \right)_P = \left( \frac{\partial H(T,P)}{\partial T} \right)_P 
$$

For ideal gases, the $\textbf{enthalpy}$ and $\textbf{internal energy}$ are functions of temperature only. Hence,
$$
c^*_V(T) = \frac{dU}{dT} \quad c^*_P(T) = \frac{dH}{dT}
$$
The temperature dependence of the ideal gas heat capacity can be measured or, in some cases, computed using the methods of statistical mechanics and detailed information about molecular structure, bond lengths, vibrational frequencies, and so forth.
$$
c^*_P(T) = a + bT + cT^2 + dT^3 + \ldots
$$
$\underline{H} = \underline{U} + P\underline{V}$ and for ideal gas $P\underline{V} = RT$,
$$
c^*_P = \frac{d(\underline{U}+RT)}{dT} = C^*_V + R
$$
Hence similarly,
$$
c^*_V(T) = a - R + bT + cT^2 + dT^3 + \ldots
$$
$$
$$
