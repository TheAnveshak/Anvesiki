A general second-order linear system is modeled by the ODE:

$$
a_2 \frac{d^2 y}{dt^2} + a_1 \frac{dy}{dt} + a_0 y = b f(t)
$$

We normalize it using the standard form:

$$
\tau^2 \frac{d^2 y}{dt^2} + 2 \xi \tau \frac{dy}{dt} + y = K_p f(t)
$$

###  Parameter Meaning and Physical Insights

- $\tau$ = time constant (s): characterizes how fast the system responds to input.
- $\xi$ = damping ratio (dimensionless): governs oscillatory behavior.
  - $\xi = 0$ → undamped (pure oscillation)
  - $0 < \xi < 1$ → underdamped (decaying oscillation)
  - $\xi = 1$ → critically damped (fastest return without oscillation)
  - $\xi > 1$ → overdamped (no oscillation, sluggish response)
- $K_p$ = process gain: steady-state gain of the system.

The Laplace transform of the above ODE is:

$$
G(s) = \frac{Y(s)}{F(s)} = \frac{K_p}{\tau^2 s^2 + 2 \xi \tau s + 1}
$$

Or,

$$
G(s) = \frac{K_p}{\tau^2 (s^2 + \frac{2 \xi}{\tau} s + \frac{1}{\tau^2})}
$$

We define:

$$
\omega_n = \frac{1}{\tau} \quad \text{(natural frequency)}
$$

Then:

$$
G(s) = \frac{K_p}{s^2 + 2 \xi \omega_n s + \omega_n^2}
$$

Consider a unit step input $f(t) = u(t) \Rightarrow F(s) = \frac{1}{s}$.

The output in Laplace domain:

$$
Y(s) = G(s) F(s) = \frac{K_p}{s(s - s_1)(s - s_2)}
$$

---
### Underdamped Case: $\xi < 1$
Where $s_1$ and $s_2$ are complex conjugate roots of the denominator:

$$
s_1 = \frac{-\xi + i\sqrt{\xi^2 - 1}}{\tau}, \quad s_2 = \frac{-\xi - i\sqrt{\xi^2 - 1}}{\tau}
$$
$$
s_{1,2} = -\xi \omega_n \pm i \omega_n \sqrt{1 - \xi^2}
$$
Decompose the transfer function as:

$$
\frac{1}{s(s - s_1)(s - s_2)} = \frac{A}{s} + \frac{B}{s - s_1} + \frac{C}{s - s_2}
$$

Where:

- $A = \frac{1}{2 \xi \tau + 1}$
- $B = \frac{A s_1}{s_2 - s_1}$
- $C = \frac{A s_2}{s_1 - s_2}$
So,
$$
Y(s) = K_p \left( \frac{A}{s} + \frac{B}{s - s_1} + \frac{C}{s - s_2} \right)
$$

Taking the inverse Laplace:

$$
y(t) = K_p A \left[ 1 + \frac{s_2 e^{s_2 t} - s_1 e^{s_1 t}}{s_2 - s_1} \right]
$$

For $\xi < 1$, define:

- $\omega_d = \frac{\sqrt{1 - \xi^2}}{\tau}$
- $s_{1,2} = -\frac{\xi}{\tau} \pm j \omega_d$

Then:

$$
y(t) = \frac{K_p}{1 + 2 \xi \tau} \left[ 1 + e^{- \xi \omega_n t} \left( \frac{\xi}{\sqrt{1 - \xi^2}} \sin(\omega_d t) - \cos(\omega_d t) \right) \right]
$$

Where:

- $\omega_d = \omega_n \sqrt{1 - \xi^2}$ is the damped natural frequency
- $\alpha = \omega_d t$

We simplify further using sine-phase identity:

$$
y(t) = \frac{K_p}{1 + 2 \xi \tau} \left[ 1 - \frac{1}{\sqrt{1 - \xi^2}} e^{- \xi \omega_n t} \sin(\omega_d t + \phi) \right]
$$

With phase:

$$
\phi = \tan^{-1} \left( \frac{\sqrt{1 - \xi^2}}{\xi} \right)
$$

The second-order system under unit step input, in the underdamped regime ($\xi < 1$), responds with an exponentially decaying oscillation governed by the damping ratio $\xi$ and the natural frequency $\omega_n$. The gain $K_p$ scales the output, while the time constant $\tau$ determines the response speed.

---
### Overdamped Case: $\xi > 1$

We start again with the standard second-order transfer function:

$$
G(s) = \frac{K_p}{\tau^2 s^2 + 2 \xi \tau s + 1}
$$

Define:

$$
s_{1,2} = \frac{-\xi \pm \sqrt{\xi^2 - 1}}{\tau}
$$

Decompose the transfer Function:
$$
\frac{K_p}{s(s - s_1)(s - s_2)} = K_p A \left( \frac{1}{s} + \frac{B}{s - s_1} + \frac{C}{s - s_2} \right)
$$

Where:

-  $A = \frac{1}{2 \xi \tau + 1}$
-  $B = \frac{A s_1}{s_2 - s_1}$
-  $C = \frac{A s_2}{s_1 - s_2}$

Thus,

$$
Y(s) = K_p A \left( \frac{1}{s} + \frac{B}{s - s_1} + \frac{C}{s - s_2} \right)
$$

Now, take inverse Laplace:

$$
y(t) = K_p A \left[ 1 - \frac{s_1 e^{s_1 t}}{s_2 - s_1} + \frac{s_2 e^{s_2 t}}{s_2 - s_1} \right]
$$

Factor and simplify:

$$
= K_p A \left[ 1 - e^{- \xi t / \tau} \left( \frac{e^{\alpha t} s_1 - e^{-\alpha t} s_2}{s_2 - s_1} \right) \right]
$$

Where:

$$
\alpha = \sqrt{\xi^2 - 1} / \tau
$$

Using hyperbolic identities:

- $\cosh(\alpha t) = \frac{e^{\alpha t} + e^{-\alpha t}}{2}$
- $\sinh(\alpha t) = \frac{e^{\alpha t} - e^{-\alpha t}}{2}$

We rewrite:

$$
y(t) = \frac{K_p}{1 + 2 \xi \tau} \left\{ 1 - e^{- \xi t / \tau} \left[ \cosh\left( \alpha t \right) + \frac{\xi}{\sqrt{\xi^2 - 1}} \sinh\left( \alpha t \right) \right] \right\}
$$

Or, putting everything neatly:

$$
y(t) = \frac{K_p}{1 + 2 \xi \tau} \left\{ 1 - e^{- \frac{\xi t}{\tau}} \left[ \cosh\left(\sqrt{\xi^2 - 1} \, \frac{ t}{\tau} \right) + \frac{\xi}{\sqrt{\xi^2 - 1}} \sinh\left(\sqrt{\xi^2 - 1} \, \frac{ t}{\tau} \right) \right] \right\}
$$


- The system has two **distinct negative real poles**.
- No oscillation — instead, the system shows a **slow, decaying exponential** behavior.
- The output rises slowly towards the steady state.
- Response time increases as $\xi$ increases.

---

###  Critical Damping: $\xi = 1$

For a critically damped system, the transfer function becomes:

$$
G(s) = \frac{K_p}{\tau^2 s^2 + 2 \tau s + 1}
$$

So the output in the Laplace domain is:

$$
Y(s) = \frac{K_p}{s(\tau^2 s^2 + 2 \tau s + 1)} = \frac{K_p}{s(\tau s + 1)^2}
$$

We now apply partial fractions:

$$
\frac{1}{s(\tau s + 1)^2} = \frac{A}{s} + \frac{B}{\tau s + 1} + \frac{C}{(\tau s + 1)^2}
$$

Solving gives:

- $A = K_p$
- $B = -K_p$
- $C = -K_p \tau$

So:

$$
Y(s) = K_p \left( \frac{1}{s} - \frac{1}{\tau s + 1} - \frac{\tau}{(\tau s + 1)^2} \right)
$$

Taking inverse Laplace:

$$
y(t) = K_p \left[ 1 - e^{-t/\tau} \left( 1 + \frac{t}{\tau} \right) \right]
$$


---

### No Damping: $\xi = 0$

For $\xi = 0$, the second-order system becomes purely oscillatory with no energy loss. The transfer function is:

$$
G(s) = \frac{K_p}{\tau^2 s^2 + 1}
$$

So the Laplace-domain output is:

$$
Y(s) = \frac{K_p}{s(\tau^2 s^2 + 1)}
$$

$$
\frac{1}{s(\tau^2 s^2 + 1)} = \frac{A}{s} + \frac{Bs + C}{\tau^2 s^2 + 1}
$$

So the expression becomes:

$$
\frac{1}{s(\tau^2 s^2 + 1)} = \frac{1}{s} - \frac{\tau^2 s}{\tau^2 s^2 + 1}
$$

$$
Y(s) = K_p \left( \frac{1}{s} - \frac{\tau^2 s}{\tau^2 s^2 + 1} \right)
$$

Therefore:

$$
y(t) = K_p \left[ 1 - \cos\left( \frac{t}{\tau} \right) \right]
$$


