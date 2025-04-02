
# Robust Design and Control of Extractive Distillation Processes under Feed Disturbances
Hesam Ahmadian Behrooz*
Chemical Engineering Faculty, Sahand University of Technology, Tabriz, Iran

	Mixtures forming azeotropes cannot be separated with the
desired purity using a conventional distillation process because
of the existence of distillation boundaries in the residue curve
map of these systems.2 In the case of azeotropic mixtures, the
desired separation is performed using other methods such as
extractive or azeotropic distillation,3 reactive distillation,4
pressure swing distillation,5 membrane pervaporation,6 and
molecular sieves.
	Extractive distillation and azeotropic distillation are based on
the addition of a third component to the original binary mixture
in order to change the relative volatility of the components. In
some cases, extractive distillation represents a more energy
efficient solution than azeotropic distillation.
	In an extractive distillation process, a higher boiling point
solvent is fed near the top of the extraction column above the
binary feed mixture. The lighter component of the azeotropic
feed is withdrawn at the top of the extractive distillation column
and the mixture of the solvent and the heavier component of
the azeotropic feed is sent to the recovery column. In the
recovery column, the almost pure solvent leaves the bottom of
the column and it is recycled to the extractive distillation
column while the other component leaves the recovery column
as the distillate product.
	The extractive distillation process has been studied from
various points of views, including solvent selection, synthesis of
the separation sequence, and controllability issues. The main
variables affecting the economics of the extractive distillation
process are the type of the solvent and its flow rate, reflux ratio
of the columns, number of stages, azeotropic feed location,
solvent tray, and recovery column feed stage. This leads to a
large number of degrees of freedom to cope with using the
shortcut methods8 and needs to be dealt with using systematic
procedures.
	3.2. Objective Function. For the simultaneous optimization
of the design and operation of the benzene/acetonitrile
extractive distillation process, the objective is the minimization
of the total annual cost (TAC) of the plant. TAC is calculated
as the sum of the operating costs (i.e., utility costs) and annual
capital investment (i.e., investment for column shell and heat exchangers) as shown in eq 2, where the annual capital
investment is defined as the capital cost divided by a three year
payback period with an operating time of 8000 h per year.
TAC($/yr) = +
capital cost
payback period
annual operating cost
(2)
The sizing relationships, utility costs and the capital cost of the
equipment (including columns and heat exchangers) which
depends on the tray number, the column diameters and heat
exchanger areas are summarized in Table S1 based on the cost
models given by Luyben (Luyben, 2013). The height of a
distillation column with N trays considering 0.61 m spacing
between the trays plus 20% extra length is calculated as L = N ×
0.61 × 1.2.
3.3. Mathematical Formulation. Defining x̲= [N1 N2 N3
N4 N5 IDC1 IDC2 S/F RRC1 QR
C2 mB1
A ] as the vector of the
decision variables, the mathematical formulation of the MINLP
problem for the optimal synthesis of the configuration and
operation of the extractive distillation of benzene/acetonitrile
can be stated as
![](Images/Pasted image 20241228124831.png)
It is also worth mentioning that the optimization framework is
implemented in Matlab and the required communications
between the optimizer (i.e., Matlab) and the simulator (i.e.,
Aspen Plus) are provided through Microsoft Excel.
3.4. Optimization Results for Various Feed Compositions.
The main target of this work is to find a control
structure which can maintain the specified purity levels in both
product streams when changes in feed composition occur. As
the first step, the temperature, pressure, and mass flow rate of
the azeotropic feed stream are assumed to be constant and
through the proposed MINLP deterministic optimization
framework in section 3.3, different plants are designed for a
range of feed compositions including: 55, 60, 65, 70, and 75 wt
% benzene. The optimization problem is solved for
deterministic cases and both design and operating conditions
are summarized in Table S2for various values of the benzene wt
% in the feed mixture. It is worth mentioning that the run time
of each deterministic optimization problem on an Intel Core i7-
4770 PC, 3.40 GHz, and 8 GB RAM is about 20 min
corresponding to approximately 3000 to 3500 simulation runs.
The operating pressure of the columns leads to approximate
reflux drum temperatures of 328 and 323 K in C1 and C2,
respectively, and cooling water can be used in the condensers.
In column C1, as the bottom temperature is in the range of
385−405 K, low-pressure steam is used in the reboiler while
medium-pressure steam is required in the reboiler of the C2 due
to a higher temperature (∼428 K).
Optimization of the steady-state economics of the plants,
while satisfying the desired purities, requires extractive columns
with different numbers of trays and different reflux ratios, and
also the variations of the feed composition alter the
composition profile of the columns leading to the change of
the optimal feed trays. The investigation of the results obtained
using the steady-state model of the plant can reveal some
guidelines in the design of the control structure. The results of
the feed sensitivity analysis21 are given in Table 2 where the
reflux ratio (RR), reflux-to-feed ratio (R/F) and % change from
their corresponding nominal values are compared for each feed
composition.
In a “single-temperature control” structure, the most effective
alternative among the two commonly used control structures22
including (1) a constant reflux ratio or (2) a constant reflux-tofeed
ratio, should be selected. This selection can be made
considering the variations of the reflux ratio and reflux-to-feed
ratio with feed composition. Accordingly, as the changes in the
reflux-to-feed ratio are smaller than those of the reflux ratio,
maintaining a constant reflux-to-feed ratio is the preferred
choice to bring the product purities closer to their specified
values under both feed composition and feed flow rate
disturbances. However, both reflux ratio and reflux-to-feed
ratio show significant changes which indicates the inefficiency
of the “single-end control” and that a “two-end control” scheme
is required for efficient disturbance handling.21
In conclusion, it can be stated that a “single-temperature”
control scheme with fixed reflux-to-feed ratio can generate
better regulatory control performances compared to the fixed
reflux ratio while a “two-temperature control” scheme outperforms
both of the “single-temperature” structures. Despite the
fact that these conclusions are made using a steady-state feed
sensitivity analysis, they are validated in the work of Yang et al.1
where the performance of the three mentioned control
structures are compared in the face of feed composition and
feed flow rate disturbances.