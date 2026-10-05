

# Statistical mechanics + Thermodynamics = POWER !!!

- Chemical thermodynamics
- Chemical kinetics
- Colloid and Surface Chemistry
- Materials Science and Solid-State Chemistry
- Quantum Chemistry and Molecular Modeling
- Enzymatic Catalysis
- Protein Thermodynamics
- Biomolecular Thermodynamics in the Cell
- Membrane Biophysics
- ...


---

# Statistical mechanics

:::matrix {cols="80/20"}
[[0,0]]
- assumes molecular (classical or quantum) composition of matter microstates
- uses probability distributions to cope with huge number equations of motion
- calculates measurable parameters as statistical / quantum mechanical averages

**Maxwell–Boltzmann distribution:**
$$
f(\mathbf{v}) \equiv \left[ \frac{2\pi k_{\text{B}} T}{m} \right]^{-3/2} \exp\left(-\frac{1}{2} \frac{m\mathbf{v}^2}{k_{\text{B}}T}\right).
$$
$$
\mathbb{E}[v] = \sqrt{\frac{8k_B T}{\pi m}} \qquad \mathbb{E}[v^2] = \frac{3k_B T}{m}
$$

**Brownian motion:**
$$
\rho(x,t) = \frac{N}{\sqrt{4\pi Dt}} \exp\left(-\frac{x^2}{4Dt}\right).
$$
$$
\mathbb{E}[x^2] = 2Dt.
$$
**Other results**: blackbody radiation, Fermi-Dirac statistics, Bose-Einstein statistics, Debye-Einstein heat capacity, etc.
[[0,1]]
![](./lecture_02_basics_of_thermodynamics/images/slide_3_img_1.png)
![](./lecture_02_basics_of_thermodynamics/images/slide_3_img_2.png) {width="70%"}
![](./lecture_02_basics_of_thermodynamics/images/slide_3_img_4.png) {width="70%"}
:::

---

# Thermodynamics

* largely phenomenological branch of science that ignores molecular (classical or quantum) composition of matter
* macrostates (thermodynamic states)
* uses state functions aka potentials - quantities that depend on the macrostate and independent on the path
* uses calculus to establish useful relations between the thermodynamic functions
* key concepts: isolated system, thermodynamic equilibrium, quasistatic process, reversible process

## 3 Laws of Thermodynamics

**Zeroth law:** If two systems are each in thermal equilibrium with a third, they are also in thermal equilibrium with each other.
$$
T \text{ is a state variable}
$$

**First law:** In a process without transfer of matter, the change in internal energy, $\Delta U$ of a thermodynamic system is equal to the energy gained as heat, Q minus the thermodynamic work A, done by the system on its surroundings.
$$
\Delta U = \Delta Q - A
$$

**Second law:** Heat does not spontaneously flow from a colder body to a hotter body.
$$
\text{For a reversible process:} \qquad dS = \frac{\delta Q}{T}
$$

**Third law:** As the temperature of a system approaches absolute zero, all processes cease and the entropy of the system approaches a minimum value.
$$
S(T = 0 \text{ K}) = 0
$$

---

# State variables / state functions
## (macro coordinates of the system / properties that don’t depend on the path)

:::matrix {cols="33/33/33"}
[[0,1::3]]
![](./lecture_02_basics_of_thermodynamics/images/slide_5_img_13.png)
[[0,0:2]]
- $\mathbf{P}$, $\mathbf{T}$, $\mathbf{V}$ --- pressure, temperature, volume
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
* **specific enthalpy** $h = H/m$<br>
* **standard molar enthalpy** $H^\circ = H/n$ at $p = 1 \text{ atm}$

$\mathbf{V, U, S, H, G, F}$ - extensive properties $\rightarrow$ $\mathbf{V^\circ, U^\circ, S^\circ, H^\circ, G^\circ, F^\circ}$
[[2,2]]
**Standard conditions** for Gibbs free energy are a temperature of $25^\circ$ C ($298$ K) and a pressure of $1$ atm (or $100$ kPa) for gases, with $1$ M concentration for all aqueous solutions. Designated with $^\circ$.

:::
---

# Explanation of Thermodynamic Quantities: $\Delta G^\circ = \Delta H^\circ - T\Delta S^\circ$

| Term | Name | Explanation |
| :--- | :--- | :--- |
| $\color{#279B61}{\Delta G^\circ}$ | <span style="color: #279B61; font-weight: bold;">Gibbs free-energy change</span> | Represents the difference in energy between products and reactants. A negative $\Delta G^\circ$ indicates an **exergonic** reaction that proceeds spontaneously with a favorable equilibrium constant. Conversely, a positive $\Delta G^\circ$ denotes an **endergonic** reaction, which is nonspontaneous and has an unfavorable equilibrium constant. |
| $\color{#D91E76}{\Delta H^\circ}$ | <span style="color: #D91E76; font-weight: bold;">Enthalpy change</span> | The overall heat associated with a reaction, reflecting the net difference in bond strengths between newly formed bonds and those broken. A negative $\Delta H^\circ$ signifies an **exothermic** process where heat is released. A positive $\Delta H^\circ$ signifies an **endothermic** process where heat is absorbed. |
| $\color{#2B8CBE}{\Delta S^\circ}$ | <span style="color: #2B8CBE; font-weight: bold;">Entropy change</span> | The shift in the system's molecular disorder or randomness resulting from a reaction. A negative $\Delta S^\circ$ means the system becomes less random; a positive $\Delta S^\circ$ indicates an increase in molecular randomness. |

---

# Enthalpy (H)

![text](20 10 <i>work that would be required to "make room" for the system if the pressure of the environment remained constant.</i>)
![arrow](20 12 -> 13 13)

:::matrix {cols="30/30/40"}
[[0,0:2]]
* $H = U + pV$
* If the system is under constant pressure, $dp = 0$ the increase in enthalpy of the system is equal to the heat added
[[1,0]]
$$
\begin{aligned}
    dH &= dU + d(pV) \\\\
    dH &= \underbrace{dU + pdV}\_{\delta Q} + Vdp \\\\
    dH &= \delta Q + Vdp \\\\
    dH &= \delta Q \quad \text{if} \quad p = \text{const}
\end{aligned}
$$
[[1,1]]
$$
\bbox[#F4E5F7, 20px, border-radius: 15px]{
\begin{array}{l}
\text{The First Law of} \\\\
\text{Thermodynamics:} \\\\
\\\\
\delta Q = dU + pdV
\end{array}
}
$$
[[0:3,2]]
$$
\begin{aligned}
& \\\\
\Delta H > 0 \quad &\textbf{endothermic} \text{ reaction} \\\\
\Delta H < 0 \quad &\textbf{exothermic} \text{ reaction}
\end{aligned}
$$
![](./lecture_02_basics_of_thermodynamics/images/slide_8_img_16.png){width=85%}
$$\ce{Ba(OH)2 * 8H2O + NH4SCN} \qquad  \ce{Fe2O3 + Al2O3} $$
[[2,0:2]]
We have an analog of "heat fluid" but at **constant pressure only**

There are a lot of "different" enthalpies that refer to the enthalpy change in various processes:
$$
\Delta H = H\_\text{products} - H\_\text{reactants}
$$
[[3,0:3]]
:::matrix{cols="20/20/20/20/20"}
[[0,0]]
* mean bond enthalpy
* enthalpy of reaction
* enthalpy of formation
[[0,1]]
* enthalpy of combustion
* enthalpy of neutralisation
* enthalpy of fusion 
[[0,2]]
* enthalpy of vaporisation 
* enthalpy of sublimation
* enthalpy of solution
[[0,3]]
* enthalpy of hydration
* enthalpy of atomisation
* lattice formation enthalpy
[[0,4]]
* lattice dissociation enthalpy
* first ionisation energy
* second ionisation energy
:::

:::

---

# Strong endothermic reaction

![youtube](kb6-xzFr4nk){width=90}

---

# Hess's law

If a reaction is carried out in a series of steps, $\Delta H$ for the overall reaction equals the **sum** of the enthalpy changes for the **individual steps**. 
The overall enthalpy change for the process is independent of the number of steps and independent of the path by which the reaction is carried out.

This law is a consequence of the fact that enthalpy is a state function. 
We can therefore calculate $\Delta H$ for any process as long as we find a route for which $\Delta H$ is known for each step. 
This means that a relatively small number of experimental measurements can be used to calculate $\Delta H$ for a vast number of reactions.

**Example:**

:::matrix {cols="50/25/25"}
[[0,0]] {font-size: 80%;}
$$
\begin{array}{lrcll}
& \ce{CH4(g) + 2O2(g)} & \longrightarrow & \ce{CO2(g) + 2H2O(g)} & \Delta H = -802 \text{ kJ} \\\\
\text{(Add)} & \ce{2H2O(g)} & \longrightarrow & \ce{2H2O(l)} & \Delta H = -88 \text{ kJ} \\\\
\hline
& \ce{CH4(g) + 2O2(g) + 2H2O(g)} & \longrightarrow & \ce{CO2(g) + 2H2O(l) + 2H2O(g)} & \\\\
& & & & \Delta H = -890 \text{ kJ}
\end{array}
$$

The net equation is
$$
\ce{CH4(g) + 2O2(g) -> CO2(g) + 2H2O(l)} \qquad \Delta H = -890 \text{ kJ}
$$
[[0,1]]
![](./lecture_02_basics_of_thermodynamics/images/slide_10_img_21.png)
[[0,2]]
![](./lecture_02_basics_of_thermodynamics/images/slide_10_img_22.png)
:::


Hess's law provides a useful means of **calculating** energy changes that are difficult to **measure** directly.

---

# Hess's law

The formation of $\ce{CO2(g)}$ from its elements can be thought of as occurring in two steps, which sum to the overall reaction, as described by Hess's law. 
The horizontal blue lines represent enthalpies. 
For an exothermic process, the products are at lower enthalpy than are the reactants.

![](./lecture_02_basics_of_thermodynamics/images/slide_11_img_23.png)

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
dG = VdP - SdT
$$
$$
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

