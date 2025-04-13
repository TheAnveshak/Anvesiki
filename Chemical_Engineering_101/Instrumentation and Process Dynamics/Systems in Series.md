## Non-Interacting Capacities in Series

Two tanks in series, where the second tank does **not** influence the dynamics of the first (i.e., no feedback from $h_2$ to tank 1).


              Fi(t)
               ↓
     +------------------+ 
     |                  |⎫
     |                  |⎬ h₁
     |     Tank 1       |⎭
     |                  |
     +--------+---------+ ------+
					              │
					              ▼  Flow (K₁√h₁)
					         ┌────┴────┐
					         │ Valve   │
					         └────┬────┘
					               │
					               +----------------+
					                                ▼
										     +------------------+     
										     |                  |⎫
										     |                  |⎬ h₂
										     |     Tank 2       |⎭
										     |                  |																			              +------------------+ ------+
													                       │
																		   ▼
															            Outlet



Let:
- $A_1$, $A_2$ = cross-sectional areas of Tank 1 and Tank 2  
- $K_1$, $K_2$ = flow resistance constants  
- $h_1$, $h_2$ = liquid heights

Equations:

1. **Tank 1:**
$$ A_1 \frac{dh_1}{dt} = F_i - K_1 \sqrt{h_1} $$
2. **Tank 2:** 
$$ A_2 \frac{dh_2}{dt} = K_1 \sqrt{h_1} - K_2 \sqrt{h_2} $$


Taking Laplace of deviation form after Taylor expansion:

$$
A_1 s \bar{H}_1(s) = \bar{F}_i(s) - \frac{K_1}{2 \sqrt{h_{1s}}} \bar{H}_1(s)
$$

- $R_1 = \frac{2 \sqrt{h_{1s}}}{K_1}$
- $\tau_1 = A_1 R_1$

$$
G_1(s) = \frac{\bar{H}_1(s)}{\bar{F}_i(s)} = \frac{K_p}{\tau_1 s + 1}
$$

Where:
- $K_p =$ Gain

Laplace domain linearized:

$$
A_2 s \bar{H}_2(s) = \frac{K_1}{2 \sqrt{h_{1s}}} \bar{H}_1(s) - \frac{K_2}{2 \sqrt{h_{2s}}} \bar{H}_2(s)
$$

Let:
- $R_2 = \frac{2 \sqrt{h_{2s}}}{K_2}$
- $\tau_2 = A_2 R_2$

Then:

$$
\bar{H}_2(s) = \frac{R_2}{R_1} \cdot \frac{1}{\tau_2 s + 1} \cdot \bar{H}_1(s)
$$

So,

$$
G_2(s) = \frac{\bar{H}_2(s)}{\bar{H}_1(s)} = \frac{R_2 / R_1}{\tau_2 s + 1}
$$

#### Overall Transfer Function

$$
G(s) = G_1(s) \cdot G_2(s) = \frac{1}{\tau_1 s + 1} \cdot \frac{R_2 / R_1}{\tau_2 s + 1}
$$



---
## Interacting Capacities

              Fi(t)
               ↓
     |                  |⎫                          |                  |⎫
     |                  |⎬ h₁                       |                  |⎬ h₁
     |     Tank 1       |⎭                          |     Tank 1       |⎭
     |                  |         ┌────┴────┐       |                  | 
     +--------+---------+ ------> │ Valve   │-----> +------------------+-+
							       	└────┬────┘                           |
															                ▼
															              Outlet




1. **Tank 1**:
$$
   A_1 \frac{dh_1}{dt} = F_i(t) - K_1 \sqrt{h_1 - h_2}
$$

2. **Tank 2**:
$$
   A_2 \frac{dh_2}{dt} = K_1 \sqrt{h_1 - h_2} - K_2 \sqrt{h_2}
$$

Use deviation variables and apply Taylor's expansion:
- $H_1(s), H_2(s)$ = Laplace transforms of $h_1'(t), h_2'(t)$
- $F(s)$ = Laplace transform of $f_i'(t)$

   $$
   \left( A_1 s + \frac{1}{R_1} \right) \bar H_1(s) = \bar F(s) + \frac{1}{R_1} \bar H_2(s)
   $$
   $$
   \left\{ A_2 R_2 s + \left(1 + \frac{R_2}{R_1} \right) \right\} \bar H_2(s) = \frac{R_2}{R_1} \bar H_1(s)
   $$

Here:
- $R_1 = \frac{1}{2 K_1 \sqrt{h_{1s} - h_{2s}}}$  
- $R_2 = \frac{1}{2 K_2 \sqrt{h_{2s}}}$


Solve for $G_p(s) = \frac{\bar H_2(s)}{\bar F(s)}$:

$$
G_p(s) = \frac{R_2}{(\tau_1 s + 1)(\tau_2 s + 1)}
$$

Where:
- $\tau_1 = A_1 R_1$, $\tau_2 = A_2 R_2 \left(1 + \frac{R_2}{R_1} \right)$

- The system behaves like a **second-order** system with **coupled dynamics**.
- Compared to non-interacting tanks, interacting systems are **slower** and more **coupled**, requiring more careful control.
