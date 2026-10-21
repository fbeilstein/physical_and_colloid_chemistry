


# The perfect gas

The properties of gases were among the first to be established quantitatively (largely during the seventeenth and eighteenth centuries) when the technological requirements of travel in
balloons stimulated their investigation.

The **physical state** of a sample of a substance, its physical condition, is defined by its physical properties. Two samples of the same substance that have the same physical properties are said to be ‘in the same state’. The **variables of state**, the variables needed to specify the state of a system, are the amount of substance it contains, $n$; the volume it occupies, $V$; the pressure, $P$; and the temperature, $T$.

Suppose a sample is divided into smaller samples. If a property of the original sample has a value that is equal to the sum of its values in all the smaller samples, then it is said to be an
**extensive** property. If a property retains the same value as in the original sample for all the smaller samples, then it is said to be **intensive**. 

- Amount ($n$), mass ($m$), and volume ($V$) are examples of extensive properties.
- Temperature ($T$) and pressure ($P$) are examples of intensive properties. The value of a property $X$ divided by the amount $n$ gives the molar value of that property $X_m$: that is, $X_m = X/n$. All molar properties are intensive, whereas $X$ and $n$ are both extensive.
The mass density, $ρ = m/V$, is also intensive.

Although in principle the state of a pure substance is specified by giving the values of $n, V, p$, and $T$, it has been established experimentally that it is sufficient to specify only **three** of these variables because doing so fixes the value of the fourth variable. 
The general form of an **equation of state** is
$$
P = f(T, V, n).
$$

Each substance is described by its own equation of state, but the explicit form of the equation is known in only a few special cases. One very important example is the equation of state of a
**‘perfect gas’**, which has the form 
$$
P = nRT/V,
$$
where $R$ is a constant independent of the identity of the gas.

---

The equation of state of a perfect gas was established by combining a series of empirical laws that arose from experimental observations. These laws can be summarized as

| Law | Formula | Conditions |
|---|---|---|
| Boyle's law (Mariotte) | $pV = \text{constant}$ | at constant $n, T$ |
| Charles's law (Amonton / Gay-Lussac) | $V = \text{constant} \times T$ | at constant $n, p$ |
| Charles's law (Amonton / Gay-Lussac) | $p = \text{constant} \times T$ | at constant $n, V$ |
| Avogadro's principle | $V = \text{constant} \times n$ | at constant $p, T$ |

- Boyle’s and Charles’s laws are strictly true only in the limit that the pressure goes to zero ($p \to 0$): they are examples of a **limiting law**, a law that is strictly true only in a certain limit.
However, these laws are found to be reasonably reliable at normal pressures.
- Avogadro’s *principle* is so-called because it supposes that the system consists of molecules whereas a *law* is strictly a summary of observations and independent of any assumed model.
- The empirical observations summarized by Boyle’s and Charles’s laws and Avogadro’s principle can be combined into a single expression:
$$
p \\, V = \mathrm{constant} \times n T.
$$
The $\mathrm{constant}$ of proportionality, which is found experimentally to be the same for all gases, is denoted $R = 8.314 \\, \mathrm{J} / \mathrm{mol}\\, \mathrm{K})$ and called the (molar) **gas constant**.

---

![](./lecture_02_basics_of_thermodynamics/images/ideal_gas.png){width=100% center}

---

# Dalton’s law

When dealing with gaseous mixtures, it is often necessary to know the contribution that each component makes to the total pressure of the sample. The **partial pressure**, $P_J$, of a gas $J$ in a mixture (any gas, not just a perfect gas), is defined as
$$
P_J = x_j P,
$$
where $x_J$ is the **mole fraction** of the component $J$, the amount of $J$ expressed as a fraction of the total amount of molecules, $n$, in the sample:
$$
\begin{aligned}
x_j &= \frac{n_j}{n}, \\\\
\sum n_j = n \quad & \rightarrow \quad \sum x_j = 1, \\\\
\sum P_j &= P \sum x_j = P. \\\\
\end{aligned}
$$

![](./lecture_02_basics_of_thermodynamics/images/Dalton_law.png){float:right; width=30% center}

For both real and perfect gases **the sum of the partial pressures is equal to the total pressure.** 


When all the gases are perfect, the partial pressure as $P_J = x_j P$ is also the pressure that each gas would exert if it occupied the same container alone at the same temperature.
That identification was the basis of the original formulation of Dalton’s law:


**The pressure exerted by a mixture of gases is the sum of the pressures that each one would exert if it occupied the container alone.**

This law is valid only for mixtures of perfect gases, so it is **not** used to define partial pressure. 

---
**Example:**

The mass percentage composition of dry air at sea level is approximately $\ce{N2}: 75.5; \ce{O2}: 23.2; \ce{Ar}: 1.3$. What is the partial pressure of each component when the total pressure is $1.20 \\, \mathrm{atm}$?

**Solution:**

Partial pressures are defined by
$$
P_J = x_j P,
$$
To use the equation, first calculate the mole fractions of the components by using 
$$
x_j = \frac{n_j}{n}
$$
and the fact that the amount of atoms or molecules $J$ of molar mass $M_J$ in a sample of mass $m_J$ is $n_J = m_J/M_J$. The mole fractions are independent of the total mass of the sample, so choose the latter to be exactly $100 \\, \textrm{g}$ (which makes the conversion from mass percentages very straightforward). Thus, the mass of $\ce{N2}$ present is $75.5$ per cent of $100 \\, \textrm{g}$, which is $75.5 \\, \textrm{g}$.

The amounts of each type of atom or molecule present in $100  \\, \textrm{g}$ of air respectively, are
$$
\begin{align}
n(\mathrm{N_2}) &= \frac{75.5\ \mathrm{g}}{28.02\ \mathrm{g\\,mol^{-1}}} = \frac{75.5}{28.02}\ \mathrm{mol} = 2.69\ \mathrm{mol} \\\\
n(\mathrm{O_2}) &= \frac{23.2\ \mathrm{g}}{32.00\ \mathrm{g\\,mol^{-1}}} = \frac{23.2}{32.00}\ \mathrm{mol} = 0.725\ \mathrm{mol} \\\\
n(\mathrm{Ar})  &= \frac{1.3\ \mathrm{g}}{39.95\ \mathrm{g\\,mol^{-1}}} = \frac{1.3}{39.95}\ \mathrm{mol} = 0.033\ \mathrm{mol}
\end{align}
$$

---
The total is $3.45 \\, \mathrm{mol}$. The mole fractions are obtained by dividing each of the above amounts by $3.45 \\, \mathrm{mol}$ and the partial pressures are then obtained by multiplying the mole fraction by the total pressure ($1.20 \\, \mathrm{atm}$):

|  | $\mathrm{N_2}$ | $\mathrm{O_2}$ | $\mathrm{Ar}$ |
|---|---|---|---|
| Mole fraction | 0.780 | 0.210 | 0.0096 |
| Partial pressure/atm | 0.936 | 0.252 | 0.012 |

---
# Real gases

![](./lecture_02_basics_of_thermodynamics/images/interaction.png){float:right; width=40% center}


Real gases do not obey the perfect gas law exactly except in the limit of $p \to 0$. Deviations from the law are particularly significant at high pressures and low temperatures, especially when a gas is on the point of condensing to liquid.

Real gases show deviations from the perfect gas law because molecules interact with one another. 
- **Repulsive** forces are significant only when molecules are almost in contact; they are short-range interactions.
Therefore, repulsions can be expected to be important only when the average separation of the molecules is small (high pressure).
- **Attractive** intermolecular forces are effective over a longer range than repulsive forces: they are important when the molecules are moderately close together but not necessarily touching.

![](./lecture_02_basics_of_thermodynamics/images/co_state.png){float:right; width=40% center}

Consider experimental isotherms for carbon dioxide at several temperatures.
- At low pressures, when the sample occupies a large volume, the molecules are so far apart for most of the time that the intermolecular forces play no significant role, and the gas behaves virtually perfectly.
- At lower temperatures, such as $20^\circ \\, \mathrm{C}$, $\ce{CO2}$ behaves in a dramatically different way from a perfect gas. At $C$ the piston suddenly slides in without any further rise in pressure: this stage is represented by the horizontal line $CDE$. Examination of the contents of the vessel shows that just to the left of $C$ a liquid appears, and that there is a sharply defined surface separating the gas and liquid phases. 

---

The pressure corresponding when both liquid and vapour are present in equilibrium, is called **the vapour pressure** of the liquid at the temperature of the experiment.
- At $E$, the sample is entirely liquid and the piston rests on its surface. Any further reduction of volume requires the exertion of considerable pressure, as is indicated by the sharply rising line to the left of $E$. Even a small reduction of volume from $E$ to
$F$ requires a great increase in pressure. The liquid is much more incompressible than the gas.
- There is a temperature, called the **critical temperature**, $T_c$, which is the highest temperature at which condensation can take place. For $\ce{CO2}$ this temperature is $31.04^\circ \\, \textrm{C}$. At $T_c$ a surface separating two phases does not appear
and the two volumes have merged to a single point, the critical point of the gas. The pressure and molar volume at the critical point are called the critical pressure, $P_c$, and critical molar volume, $V_c$, of the substance. At and above $T_c$, the sample has a single phase which occupies the entire volume of the container (**supercritical ﬂuid**). The liquid phase of a substance does not form above the critical temperature. For example, because $T_c$
of oxygen is $155\\, \textrm{K}$ it follows that above this temperature it is impossible to produce liquid oxygen by compression alone. To liquefy oxygen the temperature must first be lowered to below $155 \\, \textrm{K}$; then isothermal compression will cause liquefaction.

:::matrix{cols="50/50"}
[[0,0]]
![youtube](GemthMqZ84s) {width="80%" left="10%"}

[[0,1]]
![](./lecture_02_basics_of_thermodynamics/images/co.png){width=80% center}

:::

---

![](./lecture_02_basics_of_thermodynamics/images/real_gases.png){float:right; width=40% center}


the compression factor, $Z$, the ratio of the measured
molar volume of a gas, $V_m = V/n$, to the molar volume of a perfect gas, $V^\circ_m$, at the same pressure and temperature:
$$
Z = \frac{V_m}{V^\circ_m}
$$
Because the molar volume of a perfect gas is equal to 
$$
V^\circ_m = \frac{RT}{P}
$$
we can write 
$$
PV_m = RTZ.
$$
Because for a perfect gas $Z = 1$ under all conditions, deviation of $Z$ from $1$ is a measure of departure from perfect behaviour.
- At very low pressures, all the gases shown have $Z \approx 1$ and behave
nearly perfectly.
- At high pressures, all the gases have $Z > 1$,
signifying that they have a larger molar volume than a perfect gas. Repulsive forces are now dominant.
- At intermediate
pressures, most gases have $Z < 1$, indicating that the attractive forces are reducing the molar volume relative to that of a
perfect gas.


At large molar volumes and high temperatures the real-gas isotherms do not diﬀer greatly from perfect-gas isotherms. The small differences suggest that the perfect gas law $PV_m = RT$ is in fact the first term of the expansion(**virial equation
of state**).

---

$$
\begin{aligned}
PV_m &= RT (1+B'p+C' p^2+\cdots) \\\\
PV_m &= RT \left(1+\frac{B}{V_m}+\frac{C}{V^2_m}+\cdots\right)
\end{aligned}
$$

The coefficients $B, C, \cdots$ the values of which *depend on the temperature*, are the second, third… **virial coefficients**.

Conclusions may be drawn from the virial equations of state only by inserting specific values of the coefficients. It is often useful to have a broader, if less precise, view of all gases, such as that provided by an approximate equation of state. 

| Gas model | Equation |
|---|---|
| Perfect gas | $p = \dfrac{nRT}{V}$ |
| van der Waals | $p = \dfrac{nRT}{V - nb} - \dfrac{n^2 a}{V^2}$ |
| Berthelot | $p = \dfrac{nRT}{V - nb} - \dfrac{n^2 a}{T V^2}$ |
| Dieterici | $p = \dfrac{nRT\\,e^{-na/RTV}}{V - nb}$ |

The constant $a$ represents the strength of attractive interactions and
$b$ - the repulsive interactions.
They are characteristic of each gas and taken to be independent of the temperature. Although $a$ and $b$ are not precisely defined molecular properties, they correlate with 
physical properties that reﬂect the strength of intermolecular
interactions, such as critical temperature, vapour pressure, and
enthalpy of vaporization. 

---
# The kinetic theory of gases

![](./lecture_02_basics_of_thermodynamics/images/molecules.gif){float: right; width=20% center}


In the kinetic theory of gases (which is sometimes called the **kinetic-molecular theory**, KMT) it is assumed that the only contribution to the energy of the gas is from the kinetic energies of the molecules. 

- The gas consists of very small particles. This smallness of their size is such that the sum of the volume of the individual gas molecules is negligible compared to the volume of the container of the gas. This is equivalent to stating that the average distance separating the gas particles is large compared to their size, and that the elapsed time during a collision between particles and the container's wall is negligible when compared to the time between successive collisions.
- The number of particles is so large that a statistical treatment of the problem is well justified. This assumption is sometimes referred to as the **thermodynamic limit**.
- The rapidly moving particles constantly collide among themselves and with the walls of the container, and all these collisions are perfectly elastic.
- Interactions (i.e. collisions) between particles are strictly binary and uncorrelated, meaning that there are no three-body (or higher) interactions, and the particles have no memory.
Except during collisions, the interactions among molecules are negligible. They exert no other forces on one another.

As a simplifying assumption, the particles are usually assumed to have the same mass as one another; however, the theory can be generalized to a mass distribution, with each mass type contributing to the gas properties independently of one another. Many of the model's predictions are the same whether or not collisions between particles are included, so they are often neglected as a simplifying assumption in derivations.

---

# Fundamental equation of the kinetic theory of gases $pV=\frac{1}{3}nR\\, v_{\text{rms}}^2$
From the very economical assumptions of the kinetic model, it is possible to derive an expression that relates the pressure and volume of a gas to the mean speed with which the molecules are moving.

A molecule of mass $m$ hitting a wall perpendicular to the $x$-axis transfers momentum $2mv_x$, where $v_x$ is the $x$-component of the *mean speed*. In a cube of side $L$ it returns to the same wall after time $2L/v_x$, so the average force it exerts is $F=\frac{2mv_x}{2L/v_x}=\frac{mv_x^2}{L}$.
![](./lecture_02_basics_of_thermodynamics/images/gas_pressure.png){float: right; width: 450px; margin: 0 0 10px 15px;}

Summing over $N$ molecules and dividing by the wall area $L^2$:
$$
p = \frac{Nm\langle v_x^2 \rangle}{V}.
$$
By isotropy, $\langle v_x^2 \rangle=\frac{1}{3}\langle v^2 \rangle=\frac{1}{3}v_{\text{rms}}^2$, hence
$$
pV=\frac{1}{3}Nm\\, v_{\text{rms}}^2=\frac{1}{3}nR\\, v_{\text{rms}}^2,
$$
since the total mass is $Nm = nM$ ($M$ - molar mass, $n$ - amount of substance in moles).

This equation is one of the key results of the kinetic model. It will be shown that the right-hand side is equal to $nRT$, thus giving the perfect gas equation.

---
# Boltzmann distribution

The Boltzmann distribution gives the probability that a system in thermal equilibrium with a heat bath at temperature $T$ occupies a microstate $i$ with energy $\epsilon_i$:
$$
p_i=\frac{1}{Z}e^{-\epsilon_i/kT}=\frac{e^{-\epsilon_i/kT}}{\sum_{j=1}^M e^{-\epsilon_j/kT}}
$$
where $Z$ - canonical partition function. 

**Properties**
- Lower-energy states are exponentially favored. The relative population of two states depends only on their energy difference:
$$
\frac{N_i}{N_j}=\frac{p_i}{p_j}=e^{-(\epsilon_i-\epsilon_j)/kT}
$$
- For a classical ideal gas it yields the Maxwell–Boltzmann velocity distribution, and in a gravitational field it yields the barometric formula.
- As $T → 0$ only the ground state is occupied. As $T → ∞$ all accessible states become equally likely.
- Maximizes the entropy $S = −k \sum p_i \ln{p_i}$ subject to normalization and a fixed mean energy $\langle E\rangle$.
- Underlies Arrhenius reaction rates, population ratios in spectroscopy and lasers, semiconductor carrier statistics in the non-degenerate regime.

---
<iframe src="./lecture_02_basics_of_thermodynamics/demos/boltzmann.html" width="100%" height="850px" style="border:1px solid #ccc; border-radius: 8px;"></iframe>


---
# Experimental verification of the Boltzmann distribution
:::matrix{cols="85/15"}
[[0, 0]]
**Perrin (1908–1909).** A suspension of Brownian particles behaves like a gas in a gravitational field, so at equilibrium the particle concentration falls off with height as
$$
n(h) = n_0 \exp{\left(-\frac{m'gh}{kT}\right)}, \qquad m' = \frac{4}{3}\pi a^3 (\rho-\rho')
$$
where $m'$ is the buoyancy-corrected mass. Because the particles are about $10^{9}$ times heavier than gas molecules, this "atmosphere" is only about $0.1\\,\text{mm}$ thick and can be observed under a microscope.

**Method:** Perrin made uniform gamboge and mastic spheres by repeated fractional centrifugation. He measured their radius and density in several independent ways and counted particles at different depths with a microscope of shallow focus.

Result: The concentration fell off geometrically with height. From the slope he obtained $N_{A} \approx 6.8 \times 10^{23}\\,\text{mol}^{-1}$. The same $N_{A}$ came out when he varied particle size, material, liquid viscosity and temperature. It also agreed with Brownian displacements ($\langle x^{2}\rangle = 2Dt$),

**Svedberg's ultracentrifuge (1920s).** The same principle with centrifugal instead of gravitational force: at equilibrium 
$$
n(r) \propto \exp\\!\left(m^{*}\omega^{2}r^{2}/2kT\right).
$$

**Spectroscopy.** Line intensities follow the level populations $g_{J}\\,\mathrm{e}^{-E_{J}/kT}$. This tests the distribution over discrete levels directly.

[[0, 1]]
![](./lecture_02_basics_of_thermodynamics/images/perrin.png){width=100% center}


---


# The Maxwell distribution of speeds

In a gas the speeds of individual molecules span a wide range,
and the collisions in the gas ensure that their speeds are ceaselessly changing. Before a collision, a molecule may be travelling rapidly, but after a collision it may be accelerated to a higher speed, only to be slowed again by the next collision. 

**Don't get confused:**
$$
\begin{aligned}
&{\bf{v}} &&- \text{velocity},\\\\
&{\bf{v}} = (v_x, v_y, v_z) &&- \text{components of velocity}, \\\\
&v=|\bf{v}| &&- \text{speed = modulus of velocity}.
\end{aligned}
$$


The fraction of molecules that have speeds in the range $v$ to $v + dv$ is given by $f(v) dv $, where $f(v)$ is called the **distribution of speeds**. To do this we calculate the **distribution of velocities** $f({\bf{v}})$ first.

![](./lecture_02_basics_of_thermodynamics/images/velocity_space.png){float:right; width=25% center}

The Boltzmann distribution implies that the fraction of molecules with velocity components $v_x$, $v_y$, and $v_z$ is proportional to an exponential function of their kinetic energy $\epsilon$ : $f({\bf{v}})=Ke^{-\epsilon/kT}$, where $K$ is a constant of proportionality. The kinetic energy is simply the sum on the contributions from the motion along $x$, $y$, and $z$:
$$
\epsilon = \frac{1}{2}mv_x^2+\frac{1}{2}mv_y^2+\frac{1}{2}mv_z^2.
$$
$$
f({\bf{v}})=Ke^{-\epsilon/kT} = Ke^{-\left(\frac{1}{2}mv_x^2+\frac{1}{2}mv_y^2+\frac{1}{2}mv_z^2\right)/kT} = Ke^{-\frac{1}{2}mv_x^2/kT}e^{-\frac{1}{2}mv_y^2/kT}e^{-\frac{1}{2}mv_z^2/kT} = f(v_x)f(v_y)f(v_z)
$$
where $f(v_i)=K_ie^{-\frac{1}{2}mv_i^2/kT}$.

---
To evaluate the constant $K_x$, note that a molecule must have a
velocity component somewhere in the range $-\infty < v_x  \infty$, so
integration of the distribution over the full range of possible
values of $v_x$ must give a total probability of $1$:


$$
\begin{aligned}
\int_{-\infty}^{\infty} f(v_x)\\, dv_x &= 1 \qquad\rightarrow \qquad K_x = \left( \frac{m}{2 \pi kT} \right)^{1/2} \\\\
f(v_x) &= \left( \frac{m}{2 \pi kT}  \right)^{1/2} e^{-\frac{1}{2}mv_x^2/kT} \\\\
f({\bf{v}}) &= \left( \frac{m}{2 \pi kT} \right)^{3/2} e^{-\left(\frac{1}{2}mv_x^2+\frac{1}{2}mv_y^2+\frac{1}{2}mv_z^2\right)/kT} =
\left( \frac{m}{2 \pi kT} \right)^{3/2} e^{-\frac{1}{2}mv^2/kT}
\end{aligned}
$$


The probability that a molecule has a velocity in the range
$v_x$ to $v_x+dv_x$, $v_y$ to $v_y+dv_y$, $v_z$ to $v_z+dv_z$ is
$$
f({\bf{v}}) \\, dv_x dv_ydv_z = \left( \frac{m}{2 \pi kT} \right)^{3/2} e^{-\frac{1}{2}mv^2/kT} dv_xdv_ydv_z.
$$
![](./lecture_02_basics_of_thermodynamics/images/velocity_sphere.png){float: right; width=25% }

To evaluate the probability that a molecule has a speed in the range $v$ to $v + dv_x$ regardless of direction, think of the three
velocity components as defining three coordinates in ‘velocity
space’.
In ordinary space points that lie at a distance between $r$ and $r+dr$ from the centre are contained in a spherical shell of thickness $dr$ and radius $r$. The volume of this shell is the
product of its surface area, $4\pi r^2$, and its thickness $dr$, and is therefore $4πr^2 dr$. Similarly, the analogous volume in velocity space is the volume of a shell of radius $v$ and thickness $dv$, namely $4\pi v^2 dv$.
Because $f(v)$ depends only on $v^22$, and has the same value everywhere in a shell of radius $v$, the total probability of the molecules possessing a speed in the range $v$ to $v + dv$ is the product of the $f(v)$ and the volume of the shell of radius $v$ and thickness $dv$.
$$
f(v)=4 \pi v^2 \left( \frac{m}{2 \pi kT} \right)^{3/2} e^{-\frac{1}{2}mv^2/kT}=4 \pi \left( \frac{m}{2 \pi kT} \right)^{3/2} v^2 e^{-\frac{1}{2}mv^2/kT}.
$$

---

![](./lecture_02_basics_of_thermodynamics/images/slide_3_img_2.png) {float:right; ; width="25%"}


The molar gas constant $R$ is related to Boltzmann’s constant $k$ by $R = N_A k$, where $N_A$ is Avogadro’s constant. It follows that $m/k = mN_A/R = M/R$, where $M$ is the molar mass. 
$$
f(v)=4 \pi \left( \frac{M}{2 \pi RT} \right)^{3/2} v^2 e^{-\frac{1}{2}Mv^2/RT}.
$$

For students familiar with multivariable calculus, the switch from $f(\mathbf{v})$ to $f(v)$ can be viewed as a consequence of changing to spherical coordinates in velocity space and subsequent integration over angle variables.

$$
\begin{aligned}
(v_x, v_y, v_z) & \rightarrow (v, \phi, \theta),\\\\
dv_x \\, dv_y \\, d v_z &= \frac{\partial (v_x, v_y, v_z)}{\partial(v, \phi,\theta)} dv \\, d\phi \\, d\theta, \\\\
dv_x \\, dv_y \\, d v_z &= v^2 \sin{\theta} \\,dv \\, d\phi \\, d\theta, \\\\
f({\bf{v}})dv_x \\, dv_y \\, d v_z &= v^2 \\, \sin{\theta} \\, f\left({\bf{v}}(v, \phi, \theta)\right) \\, dv \\, d\phi \\, d\theta, \\\\
f(v)  &= \int_0^{2\pi} d\phi  \int_0^{\pi} \sin{\theta} \\, d\theta \\, v^2 \\, f(v, \phi, \theta), \\\\
f(v)  &= 4\pi \\, v^2 f(v, \phi, \theta). \\\\
\end{aligned}
$$


---

<iframe src="./lecture_02_basics_of_thermodynamics/demos/maxwell-speeds.html" width="100%" height="850px" style="border:1px solid #ccc; border-radius: 8px;"></iframe>

---

With speed distribution we can calculate mean value of any function of $v$. For example
$$
\begin{aligned}
\langle v\rangle &= \int vf(v)\\, dv \\\\
\langle v^2 \rangle &= \int v^2f(v)\\, dv  
\end{aligned}
$$
After integration we get

$$
\begin{array}{ll}
\text{Root-mean-square speed} &
  v_{\mathrm{rms}} = \sqrt{\langle v^2 \rangle} =  \left( 3RT/M \right)^{1/2} \cr
\text{Mean speed} &
  v_{\mathrm{mean}} = \langle v \rangle = \left( 8RT/\pi M \right)^{1/2} \cr
\end{array}
$$

By finding the argmaximum of the speed distribution function we get the most probable speed:

$$
\begin{array}{ll}
\text{Most probable speed} &
  v_{\mathrm{mp}} = \left( 2RT/M \right)^{1/2} \cr
\end{array}{ll}
$$

It's also possible calculate
$$
\begin{array}{ll}
\text{Mean relative speed} &
  v_{\mathrm{rel}} = \left( 8kT/\pi\mu \right)^{1/2}, \quad \mu = m_{\mathrm{A}} m_{\mathrm{B}} / (m_{\mathrm{A}} + m_{\mathrm{B}}) \cr
  \text{Collision frequency} &
  z=\sigma v_{\text{rel}} \\,  p/kT \cr
  \text{Mean free path} & 
  \lambda = kT/\sigma p
\end{array}
$$  
Under normal conditions, a typical gas molecule moves at about $500\\,\text{m/s}$ and undergoes about $10^{9}$–$10^{10}$ collisions per second, so its mean free path is of the order of $10^{-7}\\,\text{m}$ ($\sim 0.1\\,\mu\text{m}$).


---

<br><br><br>

![](./lecture_02_basics_of_thermodynamics/images/maxwell.gif) {width="75%"}

---
# Experimental verification of the Maxwell speed distribution
**Stern (1920)** A beam of silver atoms, evaporated from a heated platinum wire, was deposited on a rotating cylinder. Slower atoms were displaced further by the rotation, and the shift of the deposit gave the mean speed. The result agreed with kinetic theory, but the precision was too low to test the shape of the distribution.

**Lammert (1929)** Lammert worked in Stern's lab (Hamburg). The first mechanical velocity selector: two toothed discs on a common shaft, offset by a small angle, transmitted only atoms with a given speed. Varying the rotation rate, Lammert measured the speed distribution of a mercury beam and found qualitative agreement with Maxwell's law.

**Zartman and Ko (1930–1931)** Zartman (at Berkeley) used a technique similar to Stern's, but with higher resolution and with bismuth atoms.

**Miller and Kusch (1955)** A rotating cylinder with helical grooves acted as a high-resolution velocity selector. Measurements on potassium and thallium beams confirmed the Maxwell distribution to within about $1\\%$.

:::matrix{cols=25/25/25/25}
[[0, 0]] 
![](./lecture_02_basics_of_thermodynamics/images/stern_experiment.png){width=100%}
[[0, 1]] 
![](./lecture_02_basics_of_thermodynamics/images/lammert.png){width=100%}
[[0, 2]]
![](./lecture_02_basics_of_thermodynamics/images/miller_kusch.png){width=100%}
[[0, 3]]
![](./lecture_02_basics_of_thermodynamics/images/miller_kusch_result.png){width=100%}

:::

---

# Brownian motion

![](./lecture_02_basics_of_thermodynamics/images/slide_3_img_4.png){float: right; width: 250px; margin: 0 0 10px 15px;}
     
**1827, Robert Brown.** Observed the incessant irregular motion of small particles from pollen grains suspended in water. He found the same motion with inorganic particles, showing that it is not a property of living matter. Jan Ingenhousz had seen similar motion earlier (1785, coal dust on alcohol).

**1860s–1880s.** Several authors (Wiener, Delsaulx, Carbonelle) attributed the motion to collisions with liquid molecules. Gouy (1888) showed that it does not depend on external influences and grows with temperature and with decreasing viscosity.


**1905, Einstein.** Gave the quantitative theory: the mean square displacement grows linearly in time,
$$
\langle x^{2} \rangle = 2Dt, \qquad D = \frac{RT}{N_{A}}\\,\frac{1}{6\pi\eta a},
$$
where $a$ is the particle radius and $\eta$ the viscosity. Observing the motion thus gives a way to measure Avogadro's number $N_{A}$.


**1908, Langevin.** Wrote the stochastic equation of motion with a random force,
$$
m\ddot{x} = -6\pi\eta a\\,\dot{x} + F(t),
$$
the starting point of the theory of stochastic differential equations.

**1908–1909, Perrin.** Confirmed Einstein's theory experimentally with gamboge particles and determined $N_{A}$, convincing the remaining sceptics of the reality of atoms. Nobel Prize, 1926.

**1923, Wiener.** Gave the rigorous mathematical construction of Brownian motion as a stochastic process (the Wiener process).

**2010, Raizen's group.** Measured the instantaneous velocity of a Brownian particle (a glass bead in an optical trap) and verified the Maxwell velocity distribution for it, a measurement Einstein had considered practically impossible.


---
# Pollen Grains in Water - Brownian Motion

![youtube](R5t-oA796to) {width="80%" left="10%" start=13}

---
# Thermodynamics



* largely phenomenological branch of science that ignores molecular (classical or quantum) composition of matter
* the first results were obtained within the caloric theory (1824, Carnot), and the main results were formulated before the existence of atoms was established
* proved to be remarkably universal, with applications ranging from physics and chemistry to biology:
 >*It is the only physical theory of universal content concerning which I am convinced that, within the framework of the applicability of its basic concepts, it will never be overthrown. (Albert Einstein: Philosopher-Scientist, 1949)*
>
>*Nothing in life is certain except death, taxes and the second law of thermodynamics.(Seth Lloyd, Nature, 2004).*

* uses macrostates (thermodynamic states) to describe the systems
* uses state functions aka potentials - quantities that depend on the macrostate and independent on the path that led to it
* uses multivariable calculus to establish useful relations between the thermodynamic functions
* key concepts: isolated system, thermodynamic equilibrium, quasistatic process, reversible process



---
# State variables / state functions
## (macro coordinates of the system / properties that don’t depend on the path)

:::matrix {cols="33/33/33"}
[[0,1::3]]
![](./lecture_02_basics_of_thermodynamics/images/slide_5_img_13.png)
[[0,0:2]]
- $\mathbf{P}$, $\mathbf{T}$, $\mathbf{V}$ - pressure, temperature, volume
- $\mathbf{U}$ --- internal energy
- $\mathbf{S}$ --- entropy
- $\mathbf{H}$ --- enthalpy
- $\mathbf{G}$ --- Gibbs free energy
- $\mathbf{F}$ --- Helmholtz free energy

$ \color{red}{\xcancel{\color{black}{Q}}}$ Heat is not a state function (no *heat fluid*)
[[1,0:3]]
You don’t need all of them: for a homogeneous system in thermodynamic equilibrium you can pick any 2 of them (the rest are called state functions dependent on the chosen state variables).

When property is **extensive** (proportional to the size of the homogeneous system) we can define specific or molar quantity. 
[[2,0:2]]
Ex:<br>
* **specific enthalpy** $H_m = H/m$<br>
* **standard molar enthalpy** $H^\circ = H/n$ at $p = 1 \text{ atm}$

$\mathbf{V, U, S, H, G, F}$ - extensive properties $\rightarrow$ $\mathbf{V^\circ, U^\circ, S^\circ, H^\circ, G^\circ, F^\circ}$
[[2,2]]
**Standard conditions** for Gibbs free energy are a temperature of $25^\circ \\, \mathrm{C}$  ($298\\, \mathrm{K}$) and a pressure of $1$ atm (or $100\\, \mathrm{kPa}$) for gases, with $1 \\, \mathrm{M}$ concentration for all aqueous solutions. Designated with $^\circ$.
:::

---
# Systems
In thermodynamics, the universe is divided into two parts:
the system (reaction vessel, an engine, an electrochemical cell, a biological cell) and its surroundings.

**Classification of thermodynamic systems by the permeability of the boundary to matter and energy.**
- An **open** system has a boundary through which matter
can be transferred.

- A **closed** system has a boundary through which matter
cannot be transferred.

- An **isolated** system can exchange neither energy nor
matter with its surroundings.

| System type | Matter transfer | Energy transfer |
|-------------|-----------------|-----------------|
| Open        | Yes             | Yes             |
| Closed      | No              | Yes             |
| Isolated    | No              | No              |

![](./lecture_02_basics_of_thermodynamics/images/systems_class.png){width=40% center}

---
**Classification of thermodynamic systems by the number of phases.**
- A **homogeneous system** consists of a single phase. Its intensive properties (density, composition, etc.) are uniform throughout, or vary continuously, with no internal boundaries.
-  A **heterogeneous system** consists of two or more phases separated by phase boundaries (interfaces), across which properties change abruptly. Example: ice in water.
| System type   | Number of phases | Internal phase boundaries |
|---------------|------------------|---------------------------|
| Homogeneous   | One              | No                        |
| Heterogeneous | Two or more      | Yes                       |


**Classification of thermodynamic systems by the number of independent components.**
- A **one-component (single-component) system** contains only one independent chemical species. Example: pure water, even as ice + liquid + vapour.
- A **multicomponent system** contains two or more independent chemical species. Example: a salt solution. The number of components is the minimum number of independent species needed to specify the composition of every phase. It can be smaller than the number of species present when they are linked by chemical reactions.
  
| System type     | Number of components | Example                  |
|-----------------|----------------------|--------------------------|
| One-component   | One                  | Pure water (ice + liquid)|
| Multicomponent  | Two or more          | Aqueous salt solution    |

---

**Classification of thermodynamic systems by their state with respect to equilibrium.**
- A system is in **thermodynamic equilibrium** when its macroscopic properties do not change with time and there are no net flows of matter or energy within it or across its boundary. This means it is simultaneously in thermal, mechanical, and chemical (material) equilibrium.
- A **non-equilibrium system** has macroscopic properties that change with time, or sustains internal gradients and flows. Examples: a gas expanding into a vacuum, a rod with a temperature gradient.
| System type     | State variables         | Net fluxes / gradients | Example                          |
|-----------------|-------------------------|------------------------|----------------------------------|
| Equilibrium     | Constant in time        | None                   | Gas in a sealed vessel at rest   |
| Non-equilibrium | Change in time, or not  | Present                | Rod with a temperature gradient  |

![](./lecture_02_basics_of_thermodynamics/images/non_equilibrium.png){float: right; width=18%; margin: 0 0 10px 15px;}

<br><br><br><br>

**Non-equilibrium thermodynamics** is a branch of thermodynamics that deals with physical systems that are not in thermodynamic equilibrium but can be described in terms of macroscopic quantities (non-equilibrium state variables) that represent an extrapolation of the variables used to specify the system in thermodynamic equilibrium. Non-equilibrium thermodynamics is concerned with **transport processes** and with **the rates of chemical reactions**.


---
# Walls
**Thermal contact (heat)**

- A **diathermal (diathermic) wall** allows heat to flow through it. Two systems separated by a diathermal wall eventually reach the same temperature.
- An **adiabatic wall** does not allow heat to flow. Energy can cross it only as work.

**Mechanical contact (work)**

- A **movable (flexible) wall** can be displaced, so the system can do or receive work of expansion/compression, p dV.
- A **rigid (fixed) wall** cannot be displaced, so no $p \\, dV$ work is exchanged.

**Material contact (matter)**

- A **permeable wall** allows all chemical species to pass.
- An **impermeable** wall allows no matter to pass.
- A **semipermeable** wall allows only certain species to pass. Example: an osmotic membrane passing water but not solute.

:::matrix{cols="50/50"}
[[0, 0]]
![](./lecture_02_basics_of_thermodynamics/images/vacuum_flask.png){width=25% center}
[[0, 1]]
![](./lecture_02_basics_of_thermodynamics/images/palladium.png){width=80% center}
:::

---
# Zeroth Law of Thermodynamics 


**If system $A$ is in thermal equilibrium with $C$, and $B$ is also in equilibrium with $C$, then $A$ and $B$ are in equilibrium with each other.**
or as J.C. Maxwell has put it in his book *Theory Of Heat* (1909):
![](./lecture_02_basics_of_thermodynamics/images/maxwell_temperature.png){width=50% center}

It was formulated (named by R. Fowler, 1930s) after the first and second laws. It was then recognized as logically prior to them, since both implicitly assume that temperature exists.

- The law states that thermal equilibrium is transitive, which makes it an equivalence relation.
- Its equivalence classes (isotherms) are labeled by a state function, the empirical temperature $\theta$, with equilibrium $\iff$ $\theta_A = \theta_B$.
- $\theta$ is defined only up to a monotonic reparametrization. The absolute scale $T$ comes from the Second Law of Thermodynamics.
- The Zeroth Law underlies thermometry: two bodies can be compared in temperature by bringing each into thermal equilibrium with a third system — the thermometer — which serves as a reference.
- The Law postulates the *thermodynamic* temperature as a state variable. 

**Limitations.**

The Zeroth Law fails for *non-additive systems* 
$$
E \neq E_A + E_B
$$
(long-range interactions, self-gravitating systems with negative heat capacity) and becomes ambiguous for small systems.

---

:::matrix {cols="33/33/33"}
[[0,0]]
![](./lecture_02_basics_of_thermodynamics/images/termoscope_1.png){width=50%}

Principle of operation of a
thermoscope.

[[0,1]]
![](./lecture_02_basics_of_thermodynamics/images/Galileo_thermo.png){width=55% center}

Thermoscope, 
non-sealed

[[0,2]]
![](./lecture_02_basics_of_thermodynamics/images/florentce_thermo.png){width=60% center}

Thermometer,
sealed, thermometric liquid - alcohol.
:::

:::matrix {cols="33/33/33"}
[[0,0]]
![Pasted Image](./lecture_02_basics_of_thermodynamics/images/air_thermometer.png){width=35% }

Gas thermometer by Amonton, unsealed design (1690) 

[[0,1]]
![Pasted Image](./lecture_02_basics_of_thermodynamics/images/multi_scale_thermo.png){width=55%}

Thermometer with 18 scales (1754) 


[[0,2]]
![](./lecture_02_basics_of_thermodynamics/images/pt_thermometer.png){width=55%}

Sensing element of a modern standard platinum resistance thermometer
:::

---

![](./lecture_02_basics_of_thermodynamics/images/T-scales.png){float:right; width=25% }

**The Fahrenheit scale.** Daniel Fahrenheit (1686–1736) was born in Danzig but lived mainly in the Netherlands and worked as an instrument maker. He used mercury as his thermometric liquid. His scale (he claimed) had three fixed points: human body temperature (which he defined as $96^\circ$), an intermediate point (a mixture of ice and water) at $32^\circ$ ($96-32=64=2^6$) and a lower point which he obscurely defined as the temperature of a solution of brine made from equal parts of ice, water and salt (sea-salt or ammonium chloride) defined as $0^\circ$. However, it is unlikely that the lower point was in any way reliable and only the first two points were usable fixed points. 

After Fahrenheit’s death, the scale was redefined in terms of two reproducible fixed points: the melting point of ice ($32^\circ\mathrm{F}$) and the boiling point of water ($212^\circ \\, \mathrm{F}$), separated by $180$ degrees. The relation to the Celsius scale is
$$
t_{\mathrm{F}} = \frac{9}{5}t_{\mathrm{C}}+32.
$$

**The Réaumur scale.** René-Antoine Réaumur (1683–1757) was a French scientist. His original thermometers used alcohol “spirit of wine” as the thermometric liquid. He proposed a scale, the lower fixed point being the freezing point of water at $0^\circ\\, \mathrm{Ré}$. The upper fixed point description was very confused, but most people believed that he was saying that $80^\circ\\, \mathrm{Ré}$ was the boiling point of water. He took the volume of the alcohol at the freezing point of water as $1000$ units, with each degree corresponding to an expansion of one thousandth of that volume. His alcohol (diluted with water) expanded to about $1080$ units at the upper point, hence $80^\circ$.

$$
t_{\mathrm{Ré}} = \frac{4}{5} t_C.
$$

**The Celsius (Centigrade) scale.** Anders Celsius was a Swedish astronomer. He used mercury in his thermometers. He used two fixed points and an inverted scale with the melting point of ice (snow) set to be $100^\circ{\mathrm{C}}$ and boiling water set to be $0^\circ{\mathrm{C}}$ ⁰C. This scale was reversed quite early on –reputedly by Swedish botanist Carolus Linnaeus. 



---

# A gas thermometer

![](./lecture_02_basics_of_thermodynamics/images/gas_thermometer.png){float:right; width=20% center}

A gas thermometer is a bulb of gas at constant volume whose pressure is proportional to $T$. The non-ideality of the gas is removed by extrapolating to zero pressure, after which the reading no longer depends on the choice of gas and coincides with thermodynamic temperature.

For an ideal gas,
$$
PV = nRT.
$$

If the volume is kept constant and the amount of gas $n$ does not change, then
$$
P \propto T.
$$

The pressure is directly proportional to the absolute temperature. This is the basis of the constant-volume gas thermometer, the most common type. A constant-pressure version ($V \propto T$) is also possible, but volume is harder to measure accurately, so it is used less often.

Since 1954 the **Kelvin scale** has been defined by a single fixed point, the triple point of water, $T_\text{tp} = 273.15$ K. (Since 2019 the kelvin has been defined through the Boltzmann constant, but numerically the scale is the same.)

Place the bulb in a water triple-point cell and measure the pressure $P_\text{tp}$.
Place the bulb in the system of interest and measure the pressure $P$.
Since $P \propto T$,
$$T = 273.15\ \mathrm{K}\cdot\frac{P}{P_\text{tp}}.$$

---

The main subtlety: a real gas is not ideal. A real gas obeys the virial equation:

$$PV_m = RT\left(1 + \frac{B(T)}{V_m} + \frac{C(T)}{V_m^2} + \dots\right),$$

where $B(T)$, the second virial coefficient, accounts for interactions between pairs of molecules. As a result, thermometers filled with different gases ($\ce{He, N2, H2}$), or with different amounts of gas, give slightly different values of $T$.

**The solution:** reduce the amount of gas. Repeat the measurement at progressively lower $P_\text{tp}$ (by pumping gas out) and plot “measured $T$ versus $P_\text{tp}$”. The points lie on straight lines, and on extrapolation to $P_\text{tp} \to 0$ all gases converge to a single point:

$$T = 273.15\ \mathrm{K}\cdot\lim_{P_\text{tp}\to 0}\frac{P}{P_\text{tp}}.$$

In the limit of infinite dilution every gas becomes ideal, so the result does not depend on the substance. This ideal-gas temperature scale coincides with the thermodynamic Kelvin scale (as can be proved with a Carnot cycle using an ideal gas as the working substance).


**Historical role**
- **Amontons (around 1700)**: the pressure of air increases with temperature. By extrapolating to zero pressure he made the first estimate of “absolute cold”.
- **Charles, Gay-Lussac (around 1800)**: all gases have the same expansion coefficient, about $1/273$ per degree.
- **Regnault (1840s)**: precision gas thermometers; he showed small differences between gases.
- **Kelvin (1848)**: defined the absolute scale thermodynamically and showed that the gas scale agrees closely with it.


---

# First Law of Thermodynamics


In thermodynamics, the total energy of a system is called its internal energy, $U$. The internal energy is the total kinetic and potential energy of the constituents (the atoms, ions, or molecules) of the system. It does not include the kinetic energy arising from the motion of the system as a whole, such as its kinetic energy as it accompanies the Earth on its orbit around the Sun.

It has been found experimentally that:
- the internal energy of a closed system may be changed either by doing work on the system or by heating it.
- if a system is isolated from its surroundings, meaning that it can exchange neither matter nor energy with its surroundings, then no change in internal energy takes place. This is now known as the
First Law of thermodynamics:
 **The internal energy of an isolated system is constant.**

If $A$ is the work done *on a system* (acquisitive convention), $Q$ is the energy transferred as heat to a system, and $\Delta U$ is the resulting change in internal energy, then
$$
\Delta U = Q+A.
$$
This equation 
- summarizes the equivalence of heat and work for
bringing about changes in the internal energy of a closed system.
- embodies the fact that in an isolated system, for which $Q = 0$ and $A = 0$, the internal energy is constant.
- states that the change in internal energy of a closed system is equal to the energy that passes through its boundary as heat or work.
The differential form:
$$
d U = \delta Q+\delta A.
$$
The notation emphasizes that $dU$ is an exact differential, since $U$ is a state function, whereas $\delta Q$ and $\delta A$ are inexact: heat and work are not state functions, and their integrals depend on the path, although their sum does not.

---
# Experiments that showed that heat and work are modes of energy transfer

**Rumford’s cannon-boring experiments (1798)** Benjamin Thompson, Count Rumford, supervised the arsenal in Munich and noticed that boring cannon barrels produced large amounts of heat. In a test, a blunt borer driven by horses was turned inside a barrel immersed in water. After about two and a half hours the water boiled, with no fire involved. His key conclusion was that heat could be produced without limit as long as the mechanical work continued. If heat were a substance (caloric) stored in a finite amount in the metal, it should eventually run out. Heat, therefore, had to be a form of motion generated by work.

**Mayer (1842).** Julius Robert Mayer, a ship’s physician, formulated the principle of energy conservation and was the first to calculate the mechanical equivalent of heat. He used the difference between the specific heats of a gas, $c_P - c_V$: when a gas is heated at constant pressure, part of the heat goes into the work of expansion. He performed no experiments himself, but obtained a value of about $3.6 \\, \text{J}/\text{cal}$.

**Joule’s paddle-wheel experiment (1840s).** Falling weights, connected through pulleys, turned a paddle wheel in a water-filled calorimeter, and the friction of the paddles warmed the water. Joule measured the work done and the temperature rise. He found about  $4.15 \\, \text{J}/\text{cal}$ (the modern value is $4.184$). Crucially, he showed that the same ratio holds for different ways of converting work into heat: friction in water and mercury, compression of gases, and electric current in a conductor. This established the mechanical equivalent of heat, and the unit of energy is named after him.

**Hirn’s steam-engine measurements (1850s–60s).** Gustave Adolphe Hirn tested the reverse direction. He measured that a steam engine delivers less heat to the condenser than it receives from the boiler, and the difference corresponds to the work done. Heat is therefore not simply carried through the engine, like water through a mill wheel, as Carnot had assumed within the caloric theory. Part of it is consumed and converted into work.

---
:::matrix {cols="33/33/33" rows="50/50"}
[[0,0]]
![](./lecture_02_basics_of_thermodynamics/images/rumbord.png){width=60% center}
[[0,1]]
![](./lecture_02_basics_of_thermodynamics/images/mayer.png){width=80% center}
[[0,2]]
From the 1842 paper *Remarks on the Forces of Inanimate Nature*  by J.R. Mayer in the *Annalen der Chemie und Pharmacie*:
 - “forces” (energy) are indestructible and can be converted into one another (causa aequat effectum, “the cause equals the effect”);
- an estimate of the mechanical equivalent of heat from $c_P - c_V$: a weight falling from a height of about $365 \\, \text{m}$ corresponds to heating the same mass of water by $1 °\text{C}$.

[[1,0]]
![](./lecture_02_basics_of_thermodynamics/images/joule_paddle_scheme.png){width=60% center}
[[1,1]]
![](./lecture_02_basics_of_thermodynamics/images/joule_paddle.png){width=60% center}
[[1,2]]
![](./lecture_02_basics_of_thermodynamics/images/joules_tombstone.png){width=55% center}
foot-pounds ($1.36 \\, \text{J}$) to raise the temperature of pound of water by $1 \text{F}$ (BTU)


---

# Calorimetry

Calorimetry is the study of the transfer of energy as heat during a physical or chemical process.

:::matrix {cols="80/20"}
[[0,0]]


A **calorimeter** is a device for measuring energy transferred as heat. The most common device for measuring $q_V$ (and therefore $\Delta U$) is an adiabatic bomb calorimeter. The process to be studied which may be a chemical reaction is initiated inside a constant-volume container, the ‘bomb’. The bomb is immersed in a stirred water bath, and the whole device is the calorimeter.

The calorimeter is also immersed in an outer water bath. The temperature of the water in the calorimeter and of the outer bath are both monitored and that of the outer bath is adjusted
to keep it the same as the water in the calorimeter. This arrangement ensures that there is no net loss of heat from the
calorimeter to the surroundings (the bath) and hence that the
calorimeter is adiabatic.
The change in temperature, $\Delta T$, of the calorimeter is commonly found to be proportional to the energy that the reaction releases or absorbs as heat:
$$
q = C \Delta T
$$
where $C$ - is the **calorimeter constant**. The value of this empirical constant can be found by measuring $\Delta T$ for a process of known heat output. One possibility is to use electrical heating  and relation 
$$
q = It\Delta \phi
$$
where constant current $I$ from a source of known potential defference $\Delta \phi$, passes through a heater for a known period of time $t$.

[[0,1]]

![](./lecture_02_basics_of_thermodynamics/images/bomb_calorimeter.png){width: 350px; margin: 0 0 10px 15px;}
![](./lecture_02_basics_of_thermodynamics/images/maxwell_calorimeter.png){width: 350px; margin: 0 0 10px 15px;}
The Ice calorimeter described by J.C. Maxwell
:::

---
# Bomb calorimetry 

![youtube](RJXq92dzAWA) {width="80%" left="10%"}

---

# Enthalpy ($H$)

The change in internal energy is not equal to the energy transferred as heat when the system is free to change its volume,
such as when it is able to expand or contract under conditions
of constant pressure. Under these circumstances, some of the
energy supplied as heat to the system is returned to the surroundings as expansion work, so $dU$ is less than $\delta Q$.
In this case, the energy supplied as heat at constant pressure is
equal to the change in another thermodynamic property of the
system, the **enthalpy**.

![](./lecture_02_basics_of_thermodynamics/images/entalpy.png)
{float: right; width=18%; margin: 0 0 10px 15px;}

$$
H = U + PV
$$

If the system is under constant pressure, $dp = 0$, the increase in enthalpy of the system is equal to the heat added
$$
\begin{aligned}
    dH &= dU + d(PV) \\\\
    dH &= \underbrace{dU + PdV}\_{\delta Q} + VdP \\\\
    dH &= \delta Q + VdP \\\\
    dH &= \delta Q \quad \text{if} \quad P = \text{const}
\end{aligned}
$$

This equation states that, provided there is no additional (nonexpansion) work done, and the system and surroundings are in
mechanical equilibrium, *the change in enthalpy is equal to the
energy supplied as heat at constant pressure*.

---
# Heat capacity
**Heat capacity** or **thermal capacity** is a physical property of matter, defined as the amount of heat that must be supplied to an object to produce a unit change in its temperature:

$$
C=\lim_{\Delta T \to 0} \frac{Q}{\Delta T} = \frac{\delta Q}{dT}.
$$

At constant volume $\delta Q = dU$, at constant pressure $\delta Q = dH$:

$$
C_V = \left(\frac{\partial U}{\partial T}\right)_V, \\qquad C_P=\left( \frac{\partial H}{\partial T}  \right)_P. 
$$
For $1$ mole ideal *monoatomic* gas ($3$ degrees of freedom):

$$
\begin{aligned}
U_m(T)  &= \frac{3}{2}RT \quad \longrightarrow \quad
&&C_{V,m} = \frac{\partial}{\partial T} \left( \frac{3}{2} RT \right) = \frac{3}{2} R\\\\
PV &= RT \quad \longrightarrow \quad
&&C_{P,m} = \left( \frac{\partial (U+PV)}{\partial T}  \right)_P = \frac{3}{2}R+R .
\end{aligned}
$$

Relation between heat capacities:

$$
\begin{aligned}
C_{P,m} - C_{V,m} &= R \qquad \text{Mayer's relation}\\\\
\frac{C_{P,m}}{C_{V,m}} &= \frac{5}{2}
\end{aligned}
$$

---

For more general homogeneous substances (not just ideal gases), the difference takes the form:

$$
C_{P,m} - C_{V,m} = V_m T \frac{\alpha_V^2}{\kappa_T}, \qquad \alpha_V=\frac{1}{V}\left( \frac{\partial V}{\partial T} \right)_P \qquad \kappa_T=-\frac{1}{V} \left( \frac{\partial V}{\partial P} \right)_T.
$$

where $V_m$ is the *molar volume*, $\alpha_V$
is the *thermal expansion coefficient* and $\kappa_T$ is the *isothermal compressibility*.


|              | $\alpha/(10^{-4}\,\mathrm{K}^{-1})$ | $\kappa_T/(10^{-6}\,\mathrm{bar}^{-1})$ |
|:-------------|------:|------:|
| *Liquids:*   |       |       |
| Benzene      | 12.4  | 92.1  |
| Water        | 2.1   | 49.6  |
| *Solids:*    |       |       |
| Diamond      | 0.030 | 0.187 |
| Lead         | 0.861 | 2.21  |


Since $\beta_T$  is positive for nearly all phases, and the square of thermal expansion coefficient $\alpha_V$ is always either a positive quantity or zero:

$$
C_{P,m} >C_{V,m}.
$$

Because expansion coefficients α of liquids and solids are small, it is tempting to deduce  that for them $C_P \approx C_V$.
But this is not always so, because the compressibility $\kappa_T$ might
also be small, so $\alpha_V^2/\kappa_T$ might be large (example: lead). That is, although pushing back the atmosphere requires only a little work, a great deal of work may have to be done to pull atoms apart from one another as the solid expands.

---

![](./lecture_02_basics_of_thermodynamics/images/entalpy_plot.png){float:left; width=40% center}
<br><br><br>
The enthalpy of a substance increases as its temperature is
raised. The reason is the same as for the internal energy: molecules are excited to states of higher energy so their total energy increases.


The constant-pressure heat capacity at a particular temperature is the slope of the tangent to a curve of the enthalpy 
of a system plotted against temperature (at constant pressure). For most substances, at a given temperature the slope of enthalpy versus temperature is steeper than that of internal energy versus


<br><br>
![](./lecture_02_basics_of_thermodynamics/images/C_P_coeffs.png){float: right; width=30% center}

The variation of heat capacity with temperature can sometimes be ignored if the temperature range is small; this is an excellent approximation for a monatomic perfect gas (for
instance, one of the noble gases at low pressure). However, when it is necessary to take the variation into account for other substances, a convenient approximate empirical
expression is:

$$
\begin{aligned}
C_{P,m} &= a+b\\, T+\frac{c}{T^2}, \\\\
\Delta H &= \int_{T_1}^{T_2} C_{P,m} \\, dT = \int_{T_1}^{T_2} a+b\\, T+\frac{c}{T^2} \\, dT = a (T_2-T_1)+\frac{1}{2}(T_2^2-T_1^2)-c\left(\frac{1}{T_2}-\frac{1}{T_1}\right).
\end{aligned}
$$



---
The heat capacity at constant pressure relates the change in
enthalpy to a change in temperature. For infinitesimal changes
of temperature

$$
dH = C_p \\, dT \quad \text{at constant pressure}.
$$

If the heat capacity is constant over the range of temperatures of
interest, then for a measurable increase in temperature 

$$
\Delta H=\int_{T_1}^{T_2} C_P \\, dT = C_P \Delta T.
$$

Because a change in enthalpy can be equated to the energy
supplied as heat at constant pressure, the practical form of this
equation is

$$
Q_P = C_P \\, \Delta T.
$$

A process that releases energy as
heat is called **exothermic**, and one that absorbs energy - **endothermic**. Because the release of energy as heat into the surroundings at constant pressure signifies a
decrease in the enthalpy of a system, it follows that 
- an exothermic process at constant pressure is one for which $ΔH < 0$; such
a process is **exenthalpic**.
- an absorption of heat from the surroundings at constant pressure results in an
increase in enthalpy, an endothermic process at constant pressure has $\Delta H > 0$; such a process is **endenthalpic**.

:::matrix {cols="30/30/30"}
[[0:1]]
$$
\ce{Ba(OH)2 * 8H2O + NH4SCN}
$$
[[0:2]]
![](./lecture_02_basics_of_thermodynamics/images/slide_8_img_16.png){width=95%}
[[0:3]]
$$
\ce{Fe2O3 + Al2O3} 
$$
:::


---
# Strong endothermic reaction

![youtube](kb6-xzFr4nk){width=90}

---
# Standard enthalpy of transition

![](./lecture_02_basics_of_thermodynamics/images/plimsoll.png){float: right; width=20% center}

Changes in enthalpy are normally reported for processes taking place under a set of standard conditions. The standard enthalpy change, $\Delta H^\ominus$ ($\ominus$ - [Plimsoll](https://en.wikipedia.org/wiki/Load_line_(watercraft)) line symbol) is the change in enthalpy for a process in which the initial and final substances are in their standard states:

**The standard state of a substance at a specified temperature is its pure form at $1 \text{bar}$.**

For example, the standard state of liquid ethanol at $298 \text{K}$ is pure liquid ethanol at $298 \text{K}$ and $1 \text{bar}$. 

The standard enthalpy change for a reaction or a physical process is the diﬀerence in enthalpy between the products in their standard states and the reactants in their standard states, all at the same specified temperature.

$$
\Delta H^\ominus = H_{\text{products}}^\ominus-H_{\text{reactans}}^\ominus
$$

The standard molar enthalpy change that accompanies a change of physical state is called the standard enthalpy of transition and is denoted $\Delta_{\text{trs}}H^\ominus$. For example,

- standard enthalpy of vaporization $\Delta_{\text{vap}}H^\ominus$. 

$$
\ce{H2O(l) \longrightarrow H2O(l)(g)} \qquad \Delta_{\text{vap}} H^\ominus (373 \text{K})=+40.66 \\, \text{kJ}\\,\text{mol}^{-1}
$$

- standard enthalpy of fusion $\Delta_{\text{fus}} H^\ominus$:

$$
\ce{H2O(s) \longrightarrow H2O(l)(g)} \qquad \Delta_{\text{fus}} H^\ominus (373 \text{K})=+6.01 \\, \text{kJ}\\,\text{mol}^{-1}
$$

The different types of enthalpy changes encountered in thermochemistry are summarized in the Table.

---

| Transition | Process | Symbol |
|:--|:--|:--|
| Transition | Phase $\alpha \to$ phase $\beta$ | $\Delta_{\text{trs}}H$ |
| Fusion | $\text{s} \to \text{l}$ | $\Delta_{\text{fus}}H$ |
| Vaporization | $\text{l} \to \text{g}$ | $\Delta_{\text{vap}}H$ |
| Sublimation | $\text{s} \to \text{g}$ | $\Delta_{\text{sub}}H$ |
| Mixing | Pure $\to$ mixture | $\Delta_{\text{mix}}H$ |
| Solution | Solute $\to$ solution | $\Delta_{\text{sol}}H$ |
| Hydration | $\text{X}^{\pm}(\text{g}) \to \text{X}^{\pm}(\text{aq})$ | $\Delta_{\text{hyd}}H$ |
| Atomization | Species(s, l, g) $\to$ atoms(g) | $\Delta_{\text{at}}H$ |
| Ionization | $\text{X}(\text{g}) \to \text{X}^{+}(\text{g}) + \text{e}^{-}(\text{g})$ | $\Delta_{\text{ion}}H$ |
| Electron gain | $\text{X}(\text{g}) + \text{e}^{-}(\text{g}) \to \text{X}^{-}(\text{g})$ | $\Delta_{\text{eg}}H$ |
| Reaction | Reactants $\to$ products | $\Delta_{\text{r}}H$ |
| Combustion | Compound(s, l, g) $+ \text{O}_2(\text{g}) \to \text{CO}_2(\text{g}) + \text{H}_2\text{O}(\text{l, g})$ | $\Delta_{\text{c}}H$ |
| Formation | Elements $\to$ compound | $\Delta_{\text{f}}H$ |
| Activation | Reactants $\to$ activated complex | $\Delta^{\ddagger}H$ |

---

Because enthalpy is a state function, a change in enthalpy is independent of the path between the two states. This feature is of great importance in thermochemistry, because it implies that the same value of $H^\ominus$ will be obtained however the change is brought about between specified initial and final states. For example, the conversion of a solid to a vapour can be pictured either as occurring by sublimation (the direct conversion from solid to vapour)

$$
\ce{H2O(s)\longrightarrow H2O(g)} \qquad \Delta_{\text{sub}}H^\ominus
$$

or as occurring in two steps, first fusion (melting) and then vaporization of the resulting liquid:

![](./lecture_02_basics_of_thermodynamics/images/entalpy_subl.png){float: right; width=25% center}

$$
\begin{aligned}
\ce{H2O(s)\longrightarrow H2O(l)} & \qquad \Delta_{\text{fus}}H^\ominus \\\\
\ce{H2O(l)\longrightarrow H2O(g)} & \qquad \Delta_{\text{vap}}H^\ominus \\\\
\text{Overall: } \ce{H2O(s)\longrightarrow H2O(g)} & \qquad \Delta_{\text{fus}}H^\ominus+\Delta_{\text{vap}}H^\ominus.
\end{aligned}
$$



Because the overall result of the indirect path is the same as that
of the direct path, the overall enthalpy change is the same in each
case, and (for processes occurring at the same temperature)

$$
\Delta_{\text{sub}}H^\ominus = \Delta_{\text{fus}}H^\ominus+\Delta_{\text{vap}}H^\ominus.
$$

It follows that, because all enthalpies of fusion are positive, the enthalpy of sublimation of a substance is greater than its enthalpy of vaporization (at a given temperature).

![](./lecture_02_basics_of_thermodynamics/images/enthalpy_reverse.png){float: right; width=28% center}

Another consequence of $H$ being a state function is that the
standard enthalpy change of a forward process is the negative of
its reverse

$$
\Delta H^\ominus (A \rightarrow B) = - \Delta H^\ominus (A \leftarrow B)
$$

For instance, because the enthalpy of vaporization of water is
$+44 \\, \text{kJ} \\, \text{mol}^{−1}$ at $298 K$, the enthalpy of condensation of water vapour at that temperature is $−44 \\, \text{kJ} \\, \text{mol}^{−1}$.

---

There are two ways of reporting the change in enthalpy that
accompanies a chemical reaction. One is to write the **thermochemical equation**, a combination of a chemical equation and
the corresponding change in standard enthalpy:

$$
\ce{CH4(g) + 2O2(g)\longrightarrow CO2(g) + 2 H2O(l)} \qquad \Delta H^\ominus =-890 \\, \text{kJ}
$$

where $\Delta H^\ominus$ is the change in enthalpy when reactants in their standard states change to products in their standard states:

$$
\text{Pure, separate reactants in their standard states} \longrightarrow \text{pure, separate products in their standard states}.
$$

Except in the case of ionic reactions in solution, the enthalpy changes accompanying mixing and separation are insignifcant in comparison with the contribution from the reaction itself.
For the combustion of methane, the standard value refers to the reaction in which $1 \\, \text{mol} \\, \ce{CH4}$ in the form of pure methane gas at $1 \\, \text{bar}$ reacts completely with $2\ \\, \text{mol} \\, \ce{O2}$ in the form of pure oxygen gas to produce $1 \\, \text{mol} \\, \ce{CO2}$ as pure carbon dioxide at $1 \\, \text{bar}$ and $2 \\, \text{mol} \\, \ce{H2O}$ as pure liquid water at $1 \\, \text{bar}$; the numerical value quoted is for the reaction at $298.15 \\, \text{K}$.

Alternatively, the chemical equation is written and the **standard reaction enthalpy**, $\Delta_r H^\ominus$ (or ‘standard enthalpy of reaction’) reported. Thus, for the combustion of methane at $298 \\, \text{K}$, write

$$
\ce{CH4(g) + 2O2(g)\longrightarrow CO2(g) + 2 H2O(l)} \qquad \Delta_r H^\ominus =-890 \\, \text{kJ} \\, \text{mol}^{-1}.
$$

In general

$$
\Delta_r H^\ominus = \sum_{\text{Products}} \nu H_m^\ominus - \sum_{\text{Reactants}} \nu H_m^\ominus
$$

where in each case the molar enthalpies of the species are multiplied by their (dimensionless and positive) stoichiometric coefficients, $\nu$.


---
# Hess's law

Standard reaction enthalpies can be combined to obtain the value for another reaction. This application of the First Law is called **Hess’s law**:
**The standard reaction enthalpy is the sum of the values for the individual reactions into which the overall reaction may be divided.**
The individual steps need not be realizable in practice: they may be ‘hypothetical’ reactions, the only requirement being that their chemical equations should balance. The thermodynamic basis of the law is the path-independence of the value of $\Delta_r H^\ominus$. The importance of Hess’s law is that information about a reaction of interest, which may be difficult to determine directly, can be assembled from information on other reactions.

**Example:**

The standard reaction enthalpy for the hydrogenation of propene,

$$
\ce{CH2=CHCH3 (g) + H2 (g)} \longrightarrow \ce{CH3CH2CH3 (g)}
$$
is $-124 \\, \text{kJ} \\, \text{mol}^{-1}$. The standard reaction enthalpy for the combustion of propane 

$$
\ce{CH3CH2CH3 (g) + 5 O2 (g)} \longrightarrow \ce{3CO2 (g) + 4H2O (l)}
$$
is $-2220 \\, \text{kJ} \\, \text{mol}^{-1}$. The standard reaction enthalpy for the formation of water,

$$
\ce{H2 (g) + \frac{1}{2} O2 (g) \longrightarrow H2O (l)}
$$
is $-286 \\, \text{kJ} \\, \text{mol}^{-1}$. Calculate the standard enthalpy of combustion of propene.


---

| Reaction | $\Delta_\text{r}H^\ominus/(\text{kJ mol}^{-1})$ |
|:--|--:|
| $\text{C}_3\text{H}_6(\text{g}) + \text{H}_2(\text{g}) \to \text{C}_3\text{H}_8(\text{g})$ | $-124$ |
| $\text{C}_3\text{H}_8(\text{g}) + 5\\,\text{O}_2(\text{g}) \to 3\\,\text{CO}_2(\text{g}) + 4\\,\text{H}_2\text{O}(\text{l})$ | $-2220$ |
| $\text{H}_2\text{O}(\text{l}) \to \text{H}_2(\text{g}) + \tfrac{1}{2}\\,\text{O}_2(\text{g})$ | $+286$ |
| $\text{C}_3\text{H}_6(\text{g}) + \tfrac{9}{2}\\,\text{O}_2(\text{g}) \to 3\\,\text{CO}_2(\text{g}) + 3\\,\text{H}_2\text{O}(\text{l})$ | $-2058$ |

$$
\begin{aligned}
\ce{C3H6 + H2} &\ce{-> C3H8} \\\\
\ce{C3H8 + 5 O2} &\ce{-> 3 CO2 + 4 H2O} \\\\
\ce{H2O} &\ce{-> H2 + 1/2 O2} \\\\
\hline
\ce{C3H6 + H2 + C3H8 + 5 O2 + H2O} &\ce{-> C3H8 + 3 CO2 + 4 H2O + H2 + 1/2 O2} \\\\
\ce{C3H6 + 9/2 O2} &\ce{-> 3 CO2 + 3 H2O}
\end{aligned}
$$

---

# Enthalpy and Alkenes

:::matrix {cols="40/60"}
[[0,0]]
Part of the explanation for this trend lies in the **hyperconjugative and polarization effects of alkyl groups**.
The traditional explanation invokes an electron-releasing inductive effect of alkyl groups, 
but <a src="https://pubs.acs.org/jceda8/article/102/11/4666/3694550/Rethinking-Organic-Chemistry-The-Dual-Electronic">recent analyses</a> suggest that this is misleading: 
relative to hydrogen, alkyl groups are weakly electron-withdrawing through the $\sigma$-bond framework.
In an alkene, however, $\sigma$(C–H) orbitals of the alkyl substituents can interact with the $\pi^*$ orbital of the double bond ($\sigma \rightarrow \pi^\*$ hyperconjugation), 
while polarization of the $\pi$ system also contributes. 
These effects stabilize increasingly alkyl-substituted alkenes and help explain the observed trend in hydrogenation enthalpies.
[[0,1]]
![](./lecture_02_basics_of_thermodynamics/images/slide_12_img_24.png)
[[1,0:2]]
![](./lecture_02_basics_of_thermodynamics/images/slide_12_img_25.png)
:::

---
# Problem

Using Hess's Law find enthalpy of Chlorine monofluoride reacting with fluorine to form chlorine trifluoride:

$$
\begin{array}{rll}
(i) & \ce{ClF(g) + F2(g) -> ClF3(g)} & \Delta H = ? \\\\[1em]
(ii) & \ce{2OF2(g) -> O2(g) + 2F2(g)} & \Delta H_{(ii)} = -49.4 \text{ kJ} \\\\[1em]
(iii) & \ce{2ClF(g) + O2(g) -> Cl2O(g) + OF2(g)} & \Delta H_{(iii)} = +205.6 \text{ kJ} \\\\[1em]
(iv) & \ce{ClF3(g) + O2(g) -> \frac{1}{2}Cl2O(g) + \frac{3}{2}OF2(g)} & \Delta H_{(iv)} = +266.7 \text{ kJ}
\end{array}
$$

# Solution

$$
\begin{array}{ll}
\ce{ClF(g) + \frac{1}{2}O2(g) -> \frac{1}{2}Cl2O(g) + \frac{1}{2}OF2(g)} & \Delta H = +102.8 \text{ kJ} \\\\[1em]
\ce{\frac{1}{2}O2(g) + F2(g) -> OF2(g)} & \Delta H = +24.7 \text{ kJ} \\\\[1em]
\ce{\frac{1}{2}Cl2O(g) + \frac{3}{2}OF2(g) -> ClF3(g) + O2(g)} & \Delta H = -266.7 \text{ kJ} \\\\[0.5em]
\hline \\\\[-0.8em]
\ce{ClF(g) + F2 -> ClF3(g)} & \Delta H = -139.2 \text{ kJ}
\end{array}
$$

---
# Differential scanning calorimeter

![](./lecture_02_basics_of_thermodynamics/images/DSC.png){float: right; width=25% center}


A **differential scanning calorimeter** (DSC) measures the energy transferred as heat to or from a sample at constant pressure during a physical or chemical change. The term ‘differential’ refers to the fact that measurements on a sample are compared to those on a reference material that does not undergo a physical or chemical change during the analysis.
The term ‘scanning’ refers to the fact that the temperatures of the sample and reference material are increased, or scanned, during the analysis.


A DSC consists of two small compartments that are heated electrically at a constant rate:
$$
T = T_0 + \alpha t,
$$
where $\alpha$ is *scan rate*. A computer controls the electrical power supply that maintains the same temperature in the sample and reference compartments throughout the analysis.

If no physical or chemical change occurs in the sample at temperature $T$, the heat transferred to the sample is written as 
$$
Q_P = C_P \Delta T
$$
where $\Delta T = \alpha \Delta t$.
If a chemical or physical process takes place, the energy required to be transferred as heat to attain the same change in temperature of the sample as the control is $Q_P + Q_{P, \mathrm{ex}}$.
The quantity $Q\_{P,\mathrm{ex}}$ is interpreted in terms of an apparent change in the heat capacity at constant pressure, from $C\_P$ to $C\_P+C\_{P,\mathrm{ex}}$ of the sample during the temperature scan:
$$
C_{P,\text{ex}} = \frac{Q\_{P,\mathrm{ex}}}{\Delta T} = \frac{Q\_{P,\mathrm{ex}}}{\alpha t} = \frac{\mathcal{P}\_{\mathrm{ex}}}{\alpha}
$$
where $\mathcal{P}\_{\mathrm{ex}}=Q\_{P,\mathrm{ex}}/t$ is the excess electrical power necessary to
equalize the temperature of the sample and reference compartments. A DSC trace, also called a thermogram, consists of a
plot of $C\_{P,\mathrm{ex}}$ against $T$.

---
:::matrix{cols=50/50 width="100%"}
[[0, 0]]
![](./lecture_02_basics_of_thermodynamics/images/DSC_ubi.png){width="100%"}

[[1, 0]] 
A thermogram for the protein ubiquitin at $\mathrm{pH} = 2.45$. The protein retains its native structure up to about $45^\circ\mathrm{C}$ and then undergoes an endothermic conformational change.

[[0, 1]]
![youtube](Y2Nb0LVYykE) {width="100%"}
DSC of the solid sample under an inert $\ce{N2}$ atmosphere.
:::

The enthalpy change associated with the process is 
$$
\Delta H = \int_{T_1}^{T_2} C\_{P,\mathrm{ex}} \\, dT
$$
where $T_1$ and $T_2$ are, respectively, the temperatures at which the process begins and ends. This relation shows that the enthalpy
change is equal to the area under the plot of $C\_{P,\mathrm{ex}}$ against $T$.



---
# Entropy ($S$)

:::matrix { cols="70/30" }
[[0,0]]
* State function that is the measure of the number of possible microscopic arrangements or states of individual atoms and molecules of a system that comply with the macroscopic condition of the system.
* Thermodynamics (for reversible process! '$>$' for irreversible):
$$ 
\Delta S = \frac{\Delta Q}{T} 
$$
* Statistical mechanics:
$$ 
S = k \ln W 
$$
[[1,0]]
![](./lecture_02_basics_of_thermodynamics/images/slide_14_img_29.png)
[[0,1]]
![](./lecture_02_basics_of_thermodynamics/images/slide_14_img_33.png) {width=80}
[[1,1]]
![](./lecture_02_basics_of_thermodynamics/images/slide_14_img_32.png) {width=80}
:::

---
# Examples

:::matrix{cols="80/20"}
[[0,0]]
$$ \Delta S^\circ = \sum nS^\circ(\text{products}) - \sum mS^\circ(\text{reactants}) $$

**Example:** 
$$
\ce{N2(g) + 3H2(g) -> 2NH3(g)}
$$
$$
\begin{aligned}
\Delta S^\circ &= 2S^\circ(\ce{NH3}) - [S^\circ(\ce{N2}) + 3S^\circ(\ce{H2})] \\\\
\Delta S^\circ &= (2 \text{ mol})(192.5 \text{ J/mol-K}) - [(1 \text{ mol})(191.5 \text{ J/mol-K}) + (3 \text{ mol})(130.6 \text{ J/mol-K})] \\\\
&= -198.3 \text{ J/K}
\end{aligned}
$$
$$
\Delta S\_{\text{univ}} = \Delta S\_{\text{sys}} + \Delta S\_{\text{surr}} 
$$

[[0:2,1]]{.smaller-table .dense}
| **Substance** | **$S^\circ$ (J/mol-K)** |
| :--- | :--- |
| $\require{mhchem} \ce{H2(g)}$ | 130.6 |
| $\ce{N2(g)}$ | 191.5 |
| $\ce{O2(g)}$ | 205.0 |
| $\ce{H2O(g)}$ | 188.8 |
| $\ce{NH3(g)}$ | 192.5 |
| $\ce{CH3OH(g)}$ | 237.6 |
| $\ce{C6H6(g)}$ | 269.2 |
| $\ce{H2O(l)}$ | 69.9 |
| $\ce{CH3OH(l)}$ | 126.8 |
| $\ce{C6H6(l)}$ | 172.8 |
| $\ce{Li(s)}$ | 29.1 |
| $\ce{Na(s)}$ | 51.4 |
| $\ce{K(s)}$ | 64.7 |
| $\ce{Fe(s)}$ | 27.23 |
| $\ce{FeCl3(s)}$ | 142.3 |
| $\ce{NaCl(s)}$ | 72.3 |
[[1,0:2]]
**Example:** Consider $1$ mol of ice melting at $T = 310\text{ K}$.
$$ 
\Delta S\_{\text{sys}} = \frac{q_{\text{rev}}}{T} = \frac{(1 \text{ mol})(6.01 \times 10^3 \text{ J/mol})}{273 \text{ K}} = 22.0 \text{ J/K} 
\qquad\qquad
\Delta S\_{\text{surr}} = \frac{q_{\text{rev}}}{T} = \frac{(1 \text{ mol})(-6.01 \times 10^3 \text{ J/mol})}{310 \text{ K}} = -19.4 \text{ J/K} 
$$
$$ 
\Delta S\_{\text{univ}} = \Delta S_{\text{sys}} + \Delta S_{\text{surr}} = (22.0 \text{ J/K}) + (-19.4 \text{ J/K}) = 2.6 \text{ J/K} 
$$
$$
\begin{aligned}
\textit{Reversible Process:} \quad & \Delta S_{\text{univ}} = \Delta S_{\text{sys}} + \Delta S_{\text{surr}} = 0 \\\\
\textit{Irreversible Process:} \quad & \Delta S_{\text{univ}} = \Delta S_{\text{sys}} + \Delta S_{\text{surr}} > 0
\end{aligned}
$$
**The entropy of the universe increases in any spontaneous process.**
:::

---
# Gibbs free energy ($G$)

* $G = H - TS$
* The change in free energy for a process, $\Delta G$, equals the maximum useful work that can be done by the system on its surroundings in a spontaneous process occurring at constant temperature and pressure.
* The sign of G tells us whether the reaction is spontaneous at constant **pressure** and **temperature**:

$$
\begin{array}{c}
\Delta G = \Delta H - T\Delta S \\\\[0.5em]
\Delta S\_{\text{univ}} = \Delta S\_{\text{sys}} + \Delta S\_{\text{surr}} = \Delta S\_{\text{sys}} + \left( -\frac{\Delta H_{\text{sys}}}{T} \right) \\\\[0.5em]
-T\Delta S\_{\text{univ}} = -T\Delta S\_{\text{sys}} + \Delta H_{\text{sys}} = \Delta G \\\\[0.5em]
\Delta S_{\text{univ}} {\color{#009900}\Large\uparrow} \qquad \Delta G {\color{red}\Large\downarrow}
\end{array}
$$

* If $\Delta G < 0$, the reaction is spontaneous in the forward direction.
* If $\Delta G = 0$, the reaction is at equilibrium.
* If $\Delta G > 0$, the reaction in the forward direction is nonspontaneous (work must be done to make it occur) but the reverse reaction is spontaneous.

---
# Equilibrium

:::matrix{ cols="70/30" }
[[0,0]]
$$
G = H - TS = U + PV - TS
$$
$$
dG = \underline{dU + PdV} + VdP - \underline{TdS} - SdT
$$
$$
dG = VdP - SdT; \qquad
dG\_{\text{mol}} = V\_{\text{mol}}dP - S_{\text{mol}}dT
$$
$$
\color{pink}{\boldsymbol{\downarrow}}
$$
$$
\left( \frac{\partial G\_{\text{mol}}}{\partial P} \right)\_T = \underline{V_{\text{mol}}}
$$
$$
\text{at constant } T \quad 
\left[ 
\begin{aligned} 
  & G_{\text{mol}} - G^{\circ} = \int_{P_0}^{P} \frac{RT}{P} dP \\\\ 
  & G_{\text{mol}} - G^{\circ} = RT \ln \frac{P}{P_0} 
\end{aligned} 
\right.
$$
For a mix of ideal gases of reactants and products:
$$
\alpha \mathbf{A} + \beta \mathbf{B} \rightleftharpoons \rho \mathbf{R} + \sigma \mathbf{S}
$$
$$
\Delta G\_{\text{mol}} - \Delta G^{\circ} = RT \ln Q \hspace{2cm} Q = \frac{P\_{\mathbf{R}}^\rho P\_{\mathbf{S}}^\sigma}{P\_{\mathbf{A}}^\alpha P\_{\mathbf{B}}^\beta}
$$
[[0,1]]
$$
\bbox[#FCAECA, 20px, border-radius: 15px]{
\begin{array}{c}
\text{The First Law of} \\\\
\text{Thermodynamics} \\\\[1em]
TdS = dU + PdV
\end{array}
}
$$
$$
\bbox[#FCAECA, 20px, border-radius: 15px]{
\begin{array}{c}
\text{For ideal gas} \\\\[0.5em]
PV = NRT \\\\[0.5em]
V_{\text{mol}} = \frac{RT}{P}
\end{array}
}
$$
'mol' - per 1 mole
:::

---
# Reaction Equilibrium

:::matrix {cols="70/30"}
[[0,0]]
$$
\begin{array}{rl}
\Delta G = \Delta G^\circ + RT \ln Q & \color{#2C5485}{\longleftarrow \text{reaction quotient}} \\\\
0 = \Delta G^\circ + RT \ln K & \color{#2C5485}{\longleftarrow \text{equilibrium constant}} \\\\
\Delta G^\circ = -RT \ln K & \\\\
\ln K = \frac{\Delta G^\circ}{-RT} & \\\\
K = e^{-\Delta G^\circ / RT} &
\end{array}
$$
In determining the value of Q, the concentrations of gases are always expressed as **partial pressures** in atmospheres and solutes are expressed as their concentrations in **molarities**.
$$ 
\alpha \mathbf{A} + \beta \mathbf{B} \rightleftharpoons \rho \mathbf{R} + \sigma \mathbf{S} 
$$
$$ 
Q = \frac{\{\mathbf{R}\}^\rho \{\mathbf{S}\}^\sigma}{\{\mathbf{A}\}^\alpha \{\mathbf{B}\}^\beta} \qquad \color{#2C5485}{\longleftarrow \text{activities}} 
$$

*   If $Q < K$, then the reaction will **move to the right**.
*   If $Q > K$, then the reaction will **move to the left**.
*   If $Q = K$, then the reaction is at equilibrium
[[0,1]]
![](./lecture_02_basics_of_thermodynamics/images/slide_18_img_47.png){ width=80 }
![](./lecture_02_basics_of_thermodynamics/images/slide_18_img_51.png){ width=80 }
:::

---
# Dynamic Equilibrium

:::matrix{cols="70/30"}
[[0,0]]
**Thermodynamic equilibrium** is the state of a system in which all macroscopic flows of energy and matter cease, all types of equilibrium (mechanical, thermal, and chemical) are satisfied, and the system's macroscopic properties remain constant in time.
[[1,0]]
**Dynamic equilibrium** is the microscopic realization of thermodynamic equilibrium: opposing processes occur simultaneously at equal rates, so that no net macroscopic change takes place.
[[2,0]]
:::matrix{cols="10/50/40"}
[[0,0]]
**Examples:**
[[0,1]] 
* evaporation $\leftrightarrow$ condensation, 
* dissolution $\leftrightarrow$ recrystallization,
* dissociation $\leftrightarrow$ recombination,
* reversible chemical reactions, 
* etc
[[0,2]]
**Generalization of mechanical equilibrium**
:::
[[3,0:2]]
**Relation:** Dynamic equilibrium is the **microscopic mechanism** that sustains thermodynamic equilibrium.
[[0,1]]
**WHAT HAPPENS**<br>
**Perspective of thermodynamics**
[[1,1]]
**HOW IT HAPPENS**<br>
**Perspective of Stat.mechanics**
[[2,1]]
![](./lecture_02_basics_of_thermodynamics/images/slide_19_img_54.png){width=60}
:::
:::matrix{cols="50/50"}
[[0,0]]
**evaporation ↔ condensation**
![](./lecture_02_basics_of_thermodynamics/images/slide_19_img_52.png){width="40%"}
[[0,1]]
**reversible chemical reactions**
![](./lecture_02_basics_of_thermodynamics/images/slide_19_img_53.png){width="70%"}
:::
![rect](40 32 60 25){color=red width=4px}

---
# Dynamic Equilibrium Model

![youtube](bDtkv8q-YGQ){width=90}

---
# Predicting Reaction Spontaneity

| $\Delta H$ | $\Delta S$ | $-T\Delta S$ | $\Delta G = \Delta H - T\Delta S$ | Reaction Characteristics | Example |
| :--- | :--- | :--- | :--- | :--- | :--- |
| $-$ | $+$ | $-$ | $-$ | Spontaneous at all temperatures | $\require{mhchem} \ce{2O3(g) -> 3O2(g)}$ |
| $+$ | $-$ | $+$ | $+$ | Nonspontaneous at all temperatures | $\ce{3O2(g) -> 2O3(g)}$ |
| $-$ | $-$ | $+$ | $+$ or $-$ | Spontaneous at low $T$; nonspontaneous at high $T$ | $\ce{H2O(l) -> H2O(s)}$ |
| $+$ | $+$ | $-$ | $+$ or $-$ | Spontaneous at high $T$; nonspontaneous at low $T$ | $\ce{H2O(s) -> H2O(l)}$ |


$\Delta H$ and $\Delta S$ often change little with temperature. 
The value of $T$ directly affects the magnitude of $-T \Delta S$.

**Example:**
$$
\ce{N2(g) + 3H2(g) <=> 2NH3(g)} \qquad\leftarrow\qquad \bbox[border: 1px solid #777, 10px]{\text{Haber process}}
$$

How $\Delta G$ changes with temperature?

We expect $\Delta S$ for this reaction to be negative because the number of molecules of gas is smaller in the products. 
As a result, $\Delta G$ becomes less negative (or more positive) with increasing temperature. 
Thus, the driving force for the production of $\ce{NH3}$ becomes smaller with increasing temperature.

---
# Le Châtelier’s principle

## (Le Chatelier–Braun principle, equilibrium law)

:::matrix {cols="50/50" gap="30px"}
[[0,0]]
If the equilibrium of a system is disturbed by a change in one or more of the determining factors (as temperature, pressure, or concentration) the system tends to adjust itself to a new equilibrium by **counteracting** as far as possible the effect of the change.
![](./lecture_02_basics_of_thermodynamics/images/slide_22_img_58.png)
[[0,1]]
Discovered in 1884 by extending the reasoning from the **Van't Hoff relation**:
$$
\begin{aligned}
\Delta G^\circ &= -RT \ln K \\\\[0.5em]
\Delta H^\circ - T\Delta S^\circ &= -RT \ln K \\\\[0.5em]
\frac{\Delta H^\circ}{RT} - \frac{\Delta S^\circ}{R} &= -\ln K
\end{aligned}
$$
Differentiate by $T$,<br>
assuming $\Delta H^\circ, \Delta S^\circ$ do not depend on $T$
$$
\frac{\Delta H^\circ}{RT^2} = \frac{d\ln K}{dT} \qquad\qquad \bbox[#FFB6D9, 15px, border-radius: 10px]{\text{Van 't Hoff equation}}
$$
$$
\begin{array}{c|c}
\text{exothermic: } \Delta H^\circ < 0 \quad & \quad \text{endothermic: } \Delta H^\circ > 0 \\\\[1.5em]
T {\color{#4CAF50}\Large\uparrow} \quad K {\color{#F44336}\Large\downarrow} \quad & \quad T {\color{#4CAF50}\Large\uparrow} \quad K {\color{#4CAF50}\Large\uparrow} \\\\[1.5em]
\text{reaction shifts left} \quad & \quad \text{reaction shifts right}
\end{array}
$$
:::

---
# Concentration and Le Châtelier's Principle.
 
![](./lecture_02_basics_of_thermodynamics/images/slide_23_img_60.png) {width=80}
![](./lecture_02_basics_of_thermodynamics/images/slide_23_img_59.png) {width=60}

---
# Removing Products and Le Châtelier's Principle

![](./lecture_02_basics_of_thermodynamics/images/slide_24_img_61.png) {width=80}

---
# Temperature and Le Châtelier's principle

![](./lecture_02_basics_of_thermodynamics/images/slide_25_img_63.png) {width=80}
![](./lecture_02_basics_of_thermodynamics/images/slide_25_img_62.png) {width=50}

---
# Previously, in Lecture 3:

![](./lecture_02_basics_of_thermodynamics/images/slide_26_img_64.png) {width=80}

![text](80 10 "Le Châtelier's principle"){color=red bg=white padding=5px border="1px solid black" radius=4px}
![arrow](80 12 -> 60 25)

---
# Temperature and Le Châtelier's principle

![youtube](z_iLK7gm_fo){width=90}

---
# Pressure and Le Châtelier's principle

![](./lecture_02_basics_of_thermodynamics/images/slide_28_img_66.png) {width=90}
![](./lecture_02_basics_of_thermodynamics/images/slide_28_img_65.png) {width=70}

---
:::titlepage
[[title]]
HOMEWORK
:::

---
**Problem 1.** Calculate $\Delta H$ for the process 
$$
\ce{N2(g) + 2O2(g) -> 2NO2(g)}
$$
given the following information:
$$
\ce{N2(g) + O2(g) -> 2NO(g)} \quad \Delta H = 180.5 \text{ kJ}
$$
$$
\ce{NO(g) + \frac{1}{2}O2(g) -> NO2(g)} \quad \Delta H = -57.06 \text{ kJ}
$$

**Problem 2.** Calculate the lattice enthalpy of $\ce{CaO}$ from the following data:

|  | $\Delta H/(\text{kJ mol}^{-1})$ |
| --- | --- |
| Sublimation of $\ce{Ca(s)}$ | $+178$ |
| Ionization of $\ce{Ca(g)}$ to $\ce{Ca^{2+}(g)}$ | $+1735$ |
| Dissociation of $\ce{\frac{1}{2}O2(g)}$ | $+249$ |
| Electron attachment to $\ce{O(g)}$ | $-141$ |
| Electron attachment to $\ce{O^-(g)}$| $+844$ |
| Formation of $\ce{CaO(s)}$ from $\ce{Ca(s)}$ and $\ce{\frac{1}{2}O2(g)}$ | $-635$ |

