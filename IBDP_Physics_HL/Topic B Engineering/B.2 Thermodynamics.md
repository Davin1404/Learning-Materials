# B.2 Thermodynamics

## B.2.1 Internal energy (U)

The internal energy $U$ of a system is the total of the potential ennergy and the random kinetic energy of all the particles making up the system.

$$
U=E_k +E_p\space
$$

For ideal gas that $E_p = 0$: ($k_B=6.02\times 10^{23}$)

$$
U=E_k=\frac{3}{2}Nk_BT=\frac{3}{2}nN_Ak_BT
$$

$$
(n=\frac{N}{N_A}=\frac{m(g)}{m(g\space mol^{-1})})
$$

$n =$ _amount of substance (mol)_

$$
\because k_B=\frac{R}{N_A}
$$

$R =$ _molar gas constant_

$$
\therefore U=\frac{3}{2}nN_A\frac{R}{N_A}T
$$

$$
U=\frac{3}{2}nRT
$$

> In most of the time $nR=\text{constant}$

#### Ideal gas law

$$
pV=nRT
$$

$$
\therefore \Delta p V + p\Delta V = nR\Delta T
$$

## B.2.2 The first law of thermodynamics

$$
Q=\Delta U+W
$$

$U=$ _the energy transferred from the surroundings to the system._
$\Delta U =$ _the increase in the internal energy of the system (this is not simply a change, it is an increase)_
$W=$ _the work done by the system as it expands and pushed back the surroundings._

| sign     | $Q$                                                         | $\Delta$U                       | $W$                        |
| -------- | ----------------------------------------------------------- | ------------------------------- | -------------------------- |
| Positive | Thermal energy is**added** to the system from surrounding   | **Increase** in internal energy | Work is done**by** the gas |
| Negative | Thermal energy is**removed** from the system to surrounding | **Decrease** in internal energy | Work is done**on** the gas |

##

### P-V diagrams and thermodynamic cycles

![ther-process](/IBDP_Physics_HL/Topic%20B%20Engineering/image/summary-of-Processes.png)

⚠️☝️🤓⚠️ The area of the $PV$ graph is the **_work done_** $W$ by the system as it expands or pushed back the surroudings.

##

### Isobaric change (in ideal gas)

$\Delta p=0$

#### The work done in an isobaric change

$$
W=p\Delta V
$$

#### The work done for a non-isobaric change

_Total energy = Area of the curve_

$$
W_t=\sum_n W_n=\sum_n p_n \Delta V_n
$$

#### Relationship between variables

$$
\because pV=nRT
$$

$$
\therefore V\frac{p}{nRT}=T
$$

$$
\because \Delta p = 0
$$

$$
\because \frac{p}{nRT}=\text{constant}
$$

$$
\therefore V\propto T
$$

#### Total thermal energy calculation (⚠️only in isobaric change⚠️)

$$
\because pV=nRT
$$

$$
\because \Delta p=0
$$

$$
\therefore \cancel{\Delta p V} + p\Delta V = nR\Delta T
$$

$$
\therefore p\Delta V = nR\Delta
$$

$$
\because Q=\Delta U+W
$$

$$
\because \Delta U=\frac{3}{2}nR\Delta T \text{;  }W=p \Delta V
$$

$$
\therefore Q = \frac{3}{2}nR\Delta T + nR\Delta T
$$

$$
\therefore Q =\frac{5}{2}nR\Delta T =\frac{5}{2}p\Delta V
$$

##

### Isothermal changes (in ideal gas)

No change in the temperature of the system, **_the internal energy_** $\Delta U$ **_of the system staying constant_**.

$$
\therefore \Delta T = 0 \space (T=\text{constant})
$$

$$
\therefore \Delta U = \frac{3}{2}nR\times \Delta T = 0
$$

$$
\therefore Q=0+W
$$

$$
\therefore pV=nRT=(\text{constant})
$$

$$
P=\frac{k}{V}=constant
$$

☝️🤓 The isothermal process **_would have to be conducted very slowly_**. (As the **_gradient_** of the isothermal process curve in $PV$ graph is not **_steep_**)

##

### Adiabatic changes (in ideal gas)

**_No_** thermal energy is **_transferred_** between the **_system_** and the **_surroundings_**

$$
Q=0
$$

$$
\therefore -\Delta U=W
$$

#### Adiabatic processes for monatomic gases

$$
pV^{\frac{5}{3}}=\text{constant}
$$

Substitude with $pV=nRT$

$$
\therefore nRTV^{\frac{2}{3}}=\text{constant}
$$

$$
\because nR=\text{constant}
$$

$$
\therefore TV^{\frac{2}{3}}=\text{constant}
$$

☝️🤓Although during an adiabatic process there is no thermal enery transfer with the surroudings, the temperature of the gas will change because **_work has been done_**. Furthermore, since an adiabatic process will only change the temperature of the gas, the curve of adiabatic process on PV diagram must be the steeper one.

##

### Isovolumetric changes

$$
\because V=\text{constant}\text{; }\Delta V=0
$$

**_No_** work can be **_done_** by or on the system

$$
\therefore W=p\Delta V=0
$$

$$
\therefore Q=\Delta U
$$

The equation of state for an isovolumetric change is:

$$
\frac{P}{T}=constant
$$

#### Total thermal energy calculation (⚠️only in isovolumetric change⚠️)

$$
\because pV=nRT
$$

$$
\because \Delta V=0
$$

$$
\therefore \Delta p V + \cancel{p\Delta V} = nR\Delta T
$$

$$
\therefore Q =\Delta U=\frac{3}{2}nR\Delta T =\frac{3}{2}p\Delta V
$$

## B.2.3 Cycles and Engines

### The Carnot Cycle: the Principle of heat engine

Take in energy at a high temperature, reject energy at a low temperature and use the remainder of the energy to do work on the system.

$$
\text{useful work done}=W=Q_1-Q_2
$$

**_Net thermal energy flow_** is:

$$
Q_{in}-Q_{out}(Q_{out} \text{ refers to "waste heat"})
$$

Since no temperaure change (⚠️because there is only **_isothermal_** and **_adiabatic_** change in the Carnot Cycle⚠️), thus $\Delta T =0$, $\Delta U=0$.

$$
\therefore \Delta Q = \Delta W = Q_{in}-Q_{out}
$$

- ⚠️The first law of thermodynamics **_does not forbid_** $Q_{out}=0$⚠️
- ☝️🤓A Carnot cycle is of **little** use for a partical heat engine since the isothermal process **_would have to be conducted very slowly_**.

##

### The Carnot cycle Graph

The area **_enclosed_** by the curve is the **_net work done_** by the gas on the surroundings in one cycle.

![CarnotCycle](/IBDP_Physics_HL/Topic%20B%20Engineering/image/CarnotCycle.png)

##

### Efficiency

$$
\eta =\frac{\text{useful work done}}{\text{energy input}}=\frac{W}{Q_1}=\frac{Q_1-Q_2}{Q_1}
$$

$$
\therefore \eta_{\text{Carnot}} = 1-\frac{Q_2}{Q_1}=1-\frac{T_{\text{cold}}(\text{K})}{T_{\text{hot}}(\text{K})}
$$

$$
\eta = \text{The efficiency}
$$

⚠️The Carnot efficiency is the **maximum** possible! ⚠️
☝️🤓 In real life, energy **_losses_** to surroudings (friction, heat losses, sound energy)

## B.2.4 The Second Law of Thermodynamics

### The Clausius version of the second law

It is impossible to transfer energy from a body at a lower temperature to one at higher temperature without doing work on the system.

### The Kelvin (or Kelvin-Planck) version

It is impossible to extract energy from a hot reservoir and transfer this entirely into work.

That means **_NO_** power plant can cover **_100%_** of $Q_{in}$ into work.

### Entropy

A third version of the second law of thermodynamics involves the concept of entropy $S$.

$$
\Delta S=\frac{\Delta Q}{T}
$$

$$
\Delta S = \text{the increase in entropy}
$$

$$
\Delta Q = \text{is the energy absorbed by the system}
$$

$$
T = \text{the temperature in kelvin at which this occurs}
$$

Entropy is a **_scalar quantity_** and has units of **joule per kelvin** ( $\text{J K}^{-1}$ )

- When energy is absorbed by a system, $\Delta Q>0$, a positive change in entropy-increase;
- When energy is rejected by the system, $\Delta Q<0$, the entropy will decrease;

⚠️The total entropy of the universe **INCREASES**.⚠️😡

##

State abd explain at which point in the cycle ABCA the entropy of the gas is the largest.
![shapeOfTheCurve](/IBDP_Physics_HL/Topic%20B%20Engineering/image/cycle%20ABCA.png)

Entropy is largest at B, entorpy increases from A to B because $T=\text{constant}$, but volume increases, so more **_disorder_**.

$\Delta S = \frac{\Delta Q}{T}$, $\Delta Q>0$, $\therefore \Delta S>0$

##

### Entropy as a measure of disorder

Entropy is a measure of the disorder of a system or energy unavailable to do work.

Increase in entropy means when the entropy increases, there is an increase in the degree of disorder of the system.

![shapeOfTheCurve](/IBDP_Physics_HL/Topic%20B%20Engineering/image/16-enigmatic-facts-about-entropy-1694212091.jpg)

> When a chicken develops inside an egg, the entropy of the egg and its contents decreases. Explain how this observation is consistent with the second law of thermodynamics.
>
> Entropy of the surroundings must increase more than the decrease of entropy in the developing egg. The energy generated by the biochemical process within the egg becomes more spread out as a consequence of some passing into the surroundings.

$$


$$
