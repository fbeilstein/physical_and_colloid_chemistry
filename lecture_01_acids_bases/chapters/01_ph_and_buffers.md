
# Solvation

The power of solvation
$$
\ce{HCl (aq) <=> H+ (aq) + Cl- (aq)} \quad \Delta G^\circ_{298\text{K}} = -40 \text{ kJ mol}^{-1}
$$
Gibbs free energy may not tell you much at this point (we'll get to that), but this means $\ce{HCl}$ (hydrochloric acid) completely dissociates in aqueous solution
$$
\ce{HCl (g) <=> H+ (g) + Cl- (g)} \quad \Delta G^\circ_{298\text{K}} = +1347 \text{ kJ mol}^{-1}
$$
No dissociation at all in gas phase (1 molecule in $10^{240}$, in later lectures we'll get how to calculate that)


:::matrix{cols="70/30"}
[[0,0]]
In the gas phase we would have to form an isolated proton ($\ce{H+}$, hydrogen ion) and chloride ion and this is energetically very unfavourable. 
In contrast, in aqueous solution the proton is strongly attached to a water molecule to give the very stable hydronium ion, $\ce{H3O+}$, and the ions are **no longer isolated but solvated**.

By an IUPAC definition, **solvation** is an interaction of a **solute** with the **solvent**, which leads to **stabilization** of the solute species in the solution. 
In the solvated state, an ion or molecule in a solution is surrounded or complexed by solvent molecules. 
Solvated species can often be described by coordination number, and the complex stability constants. 
The concept of the solvation interaction can also be applied to an insoluble material, for example, solvation of functional groups on a surface of ion-exchange resin.
[[0,1]]
![](./lecture_01_acids_bases/images/slide_3_img_3.png)

In case of water can be called **hydration**
:::

---

# Solvation

:::matrix{cols="33/33/33"}
[[0,0:2]]
Proton is solvated as well in form of hydronium ion, $\ce{H3O+ (aq)}$
![](./lecture_01_acids_bases/images/slide_4_img_4.png){width=70}
[[1,0]]
![](./lecture_01_acids_bases/images/slide_4_img_7.png){width=70}
[[1,1]]
![](./lecture_01_acids_bases/images/slide_4_img_5.png){width=70}
[[0:2,2]]
![](./lecture_01_acids_bases/images/slide_4_img_6.png){width=80}
:::

---

# Grotthuss mechanism

:::matrix{cols="33/33/33"}
[[0,0]]
| **Cation** | **Electrical mobility** <br><br> $(\text{cm}^2 \text{ s}^{-1} \text{ V}^{-1})$ |
| --- | --- |
| $\ce{Na+}$ | $0.519 \times 10^{-3}$ |
| $\ce{K+}$ | $0.762 \times 10^{-3}$ |
| $\ce{NH4+}$ | $0.763 \times 10^{-3}$ |
| $\ce{H+}$ | $3.62 \times 10^{-3}$ |

![](./lecture_01_acids_bases/images/slide_5_img_10.png) 
[[0,1]]
![](./lecture_01_acids_bases/images/slide_5_img_9.png){width=80}
[[0,2]]
![](./lecture_01_acids_bases/images/slide_5_img_8.png){width=80}
:::


**Proton hopping (Grotthuss mechanism)** 
Short "hops" of protons between a series of hydrogen-bonded water molecules result in an extremely rapid net movement of a proton over a long distance. 
As a hydronium ion gives up a proton, a water molecule some distance away acquires one, becoming a hydronium ion. 
Proton hopping is much faster than true diffusion and explains the remarkably high ionic mobility of $\ce{H+}$ ions compared with other monovalent cations such as $\ce{Na+}$ and $\ce{K+}$.

---

# Definition of pH

:::matrix{cols="70/30"}
[[0,0]]
## Protons' properties
* Protons are highly reactive: In fact, an isolated proton is so reactive that it will even add on to a molecule of methane in the gas phase to give $\ce{CH5+}$ in a strongly exothermic reaction (can be seen during mass-spectroscopy)
* Protons solvate
* Protons can rapidly move in water
* We will characterize solutions by the concentration of $[\ce{H+}]$


Thus we will be concerned with their fate as they can significantly influence the chemistry of the processes

**Note:** Different books use interchangeably $[\ce{H+}]$ and $[\ce{H3O+}]$, we will do the same.

## pH

The measure of proton concentration is pH. Note that $[\ce{H3O+}]$ is measured in mol/L often designated M. Logarithm taken is base 10, **NOT** natural.
$$
\text{pH} = -\log[\ce{H3O+}]
$$
[[0,1]]
![](./lecture_01_acids_bases/images/slide_7_img_11.png){width=90}

---

# Autoprotolysis of Water

$$
\ce{H2O + H2O <=> H3O+ (aq) + OH- (aq)}
$$

:::matrix{cols="50/50"}
[[0,0]]
![](./lecture_01_acids_bases/images/slide_8_img_13.png){width=70}
[[0,1]]
![](./lecture_01_acids_bases/images/slide_8_img_16.png){width=50}

## Dynamic equilibrium:

Law of mass action:
$$
k\_1 \cdot [\ce{H2O}] \cdot [\ce{H2O}] = k\_2 \cdot [\ce{H3O+}] \cdot [\ce{OH-}]
$$
$$
k = \frac{k\_1}{k\_2} = \frac{[\ce{H3O+}] \cdot [\ce{OH-}]}{\underbrace{[\ce{H2O}] \cdot [\ce{H2O}]}_{\textbf{approximate constant}}}
$$
::: 

$$
K_{\text{W}} = [\ce{H3O+}][\ce{OH-}] = 10^{-14} \text{ mol}^2 \text{ dm}^{-6} \text{ at } 25~^\circ\text{C}
$$

---

# Autoprotolysis of Water

:::matrix{cols="50/50"}
[[0,0]]
$$
\ce{H2O + H2O <=> H3O+ (aq) + OH- (aq)}
$$
In this reaction, one molecule of water is acting as a base, receiving a proton from the other, which in turn is acting as an acid by donating a proton. From the equation we see that, for every hydronium ion formed, we must also form a hydroxide ion and so in pure water the concentrations of hydroxide and hydronium ions are equal.
$$
[\ce{H3O+}] = [\ce{OH-}] = 10^{-7} \text{ mol dm}^{-3}
$$
The product of these two concentrations is known as the ionization constant of water, $K\_{\text{W}}$ 
(or as the ionic product of water, or maybe sometimes as the autoprotolysis constant, $K\_{\text{AP}}$)
$$
K_{\text{W}} = [\ce{H3O+}][\ce{OH-}] = 10^{-14} \text{ mol}^2 \text{ dm}^{-6} \text{ at } 25~^\circ\text{C}
$$
This is a constant in aqueous solutions, albeit a very, very small one. 
This means that, if we know the hydronium ion concentration, we also know the hydroxide concentration and vice versa since the product of the two concentrations always equals $10^{-14}$.

**NOTE:**<br> 
$\text{p}K\_{\text{w}} = -\log(K\_{\text{w}}) = \text{pH} + \text{pOH}$<br>
$\text{pH} + \text{pOH} = 14$

[[0,1]]
![](./lecture_01_acids_bases/images/slide_11_img_20.png)
:::
---

# Water Dissociation and Temperature


$$
\ce{H2O + H2O <=> H3O+ (aq) + OH- (aq)}
$$

:::matrix{cols="50/50"}
[[0,0]]
### Relationships among $[\ce{H+}]$, $[\ce{OH-}]$, and pH at $25~^\circ\text{C}$
| Solution Type | $[\ce{H+}] (\text{M})$ | $[\ce{OH-}] (\text{M})$ | pH |
| --- | --- | --- | --- |
| Acidic | $> 1.0 \times 10^{-7}$ | $< 1.0 \times 10^{-7}$ | $< 7.00$ |
| Neutral | $1.0 \times 10^{-7}$ | $1.0 \times 10^{-7}$ | $7.00$ |
| Basic | $< 1.0 \times 10^{-7}$ | $> 1.0 \times 10^{-7}$ | $> 7.00$ |

![](./lecture_01_acids_bases/images/slide_14_img_27.png)
[[0,1]]
Water dissociation occurs **endothermically** (due to electric field fluctuations between neighboring molecules). 
Thus **increase** in temperature shifts equilibrium to the **right**.
![](./lecture_01_acids_bases/images/slide_10_img_19.png)
:::

---

# What is Acid

* A **Brønsted–Lowry acid** is a substance that donates a proton ($\ce{H+}$), and
* a **Brønsted–Lowry base** is a substance that accepts a proton.

:::matrix{cols="60/40"}
[[0,0]]
![](./lecture_01_acids_bases/images/slide_12_img_21.png)
[[0,1]]{justify-content: center;}
The transfer of a proton always involves both an acid (donor) and a base (acceptor).
In other words, a substance can function as an acid only if another substance simultaneously behaves as a base.
:::
:::matrix{cols="30/50/20"}
[[0,0]]{justify-content: center;}
Definition is valid not only in liquid phase (though that is the most interesting case)
[[0,1]]
![](./lecture_01_acids_bases/images/slide_12_img_22.png)
[[0,2]]
![](./lecture_01_acids_bases/images/slide_12_img_23.png){width=80}
:::

---

# Arbitrary Acid or Base

> 🔴 For any acid and any base
$$
{\ce{AH + B <=> BH+ + A-}}
$$
where $\ce{AH}$ is an acid and $\ce{A-}$ is its conjugate base and $\ce{B}$ is a base and $\ce{BH+}$ is its conjugate acid, that is, *every acid has a conjugate base associated with it and every base has a conjugate acid associated with it.*

:::matrix{cols="50/50"}
[[0,0]]
![](./lecture_01_acids_bases/images/slide_13_img_25.png){width=70}
[[0,1]]
![](./lecture_01_acids_bases/images/slide_13_img_26.png){width=70}
:::

* Water can act both as acid and base
* We will always suppose water as a solvent (concentration much greater)
* $[\ce{H3O+}]$ and $[\ce{H+}]$ will be used interchangeably
* pH-meter measures concentration of $\ce{H+}$
* NOTE: $[\ce{H+}][\ce{OH-}] = 10^{-14}$

---

# Acid Strengths

Acid may not fully dissociate. 
Depending on the dissociation level we  call acids strong, week, or negligible (not acids). 
Strong acids fully dissociate, not acids do not dissociate.

We need a way to quantify this
$$
\ce{AH + H2O <=> H3O+ (aq) + A- (aq)}
$$
:::matrix{cols="30/70"}
[[0,0]]
$$
K_{\text{eq}} = \frac{[\ce{H3O+}][\ce{A-}]}{[\ce{AH}][\ce{H2O}]}
$$
[[0,1]]
The position of equilibrium is measured by the equilibrium constant for this reaction
[[1,0]]
$$
K_{\text{a}} = \frac{[\ce{H3O+}][\ce{A-}]}{[\ce{AH}]}
$$
[[1,1]]
The concentration of **water** remains essentially **constant** (at $55.56 \text{mol}/\text{dm}^3$) with **dilute** solutions. 
Thus we define the **acidity constant**.
[[2,0:2]]
> 🔴 $\text{p}K\_{\text{a}} = -\log K\_{\text{a}}$
Because of the minus sign in this definition, the lower the $\text{p}K\_{\text{a}}$, the larger the equilibrium constant, $K\_{\text{a}}$, is and hence the stronger the acid. 
*The $pK\_a$ of the acid is the pH where it is exactly half dissociated.* 
At pHs above the $\text{p}K\_{\text{a}}$, the acid $\ce{HA}$ exists as $\ce{A-}$ in water; 
at pHs below the $\text{p}K_{\text{a}}$, it exists as undissociated $\ce{HA}$.
:::


---

# Wilhelm Ostwald's Laws of dilution

$$
\ce{AH (aq) + H2O (l) <=> H3O+ (aq) + A- (aq)}
$$

:::matrix{cols="20/20/60"}
[[0,0]]
For weak **acids**:
$$
{\color{red}[\ce{H+}] = \sqrt{K_a[\ce{HA}]}}
$$
[[0:2,1]]
$$ 
\begin{array}{l} 
\text{let } x = [\ce{H3O+}] = [\ce{A-}] \\\\ 
[\ce{HA}]\_{eq} = [\ce{HA}] - x 
\end{array} 
$$
$$ 
K\_a = \frac{[\ce{H3O+}][\ce{A-}]}{[\ce{HA}]_{eq}} 
     = \frac{x \cdot x}{[\ce{HA}] - \color{red}{\cancel{\color{black}{x}}}}
$$
$$
x = [\ce{H+}] = \sqrt{K_a[\ce{HA}]}
$$
[[1,0]]
Likewise for weak **bases**:
$$
{\color{red}[\ce{OH-}] = \sqrt{K_b[\ce{B}]}}
$$
[[2,0: 2]]
![](./lecture_01_acids_bases/images/slide_17_img_37.png)
[[0:3,2]]
![](./lecture_01_acids_bases/images/slide_19_img_39.png)
:::


---

# Acids and Water

1. A **strong acid** completely transfers its protons to water, leaving essentially no undissociated molecules in solution.
2. A **weak acid** only partially dissociates in aqueous solution and therefore exists in the solution as a mixture of the undissociated acid and its conjugate base. 
3. A substance with **negligible acidity** contains hydrogen but does not demonstrate any acidic behavior in water.


![](./lecture_01_acids_bases/images/slide_18_img_38.png)

> 🔴 The strongest base in aqueous solution is $\ce{OH-}$ and the strongest acid in aqueous solution is $\ce{H3O+}$. 
>
> Remember that:
>* Addition of stronger bases than $\ce{OH-}$ just gives more $\ce{OH-}$ by the deprotonation of water
>* Addition of stronger acids than $\ce{H3O+}$ just gives more $\ce{H3O+}$ by protonation of water
>
> Also remember that:
>* The pH of pure water at $25~^\circ\text{C}$ is $7.00$ (not the $\text{p}K_{\text{a}}$)
>* The $\text{p}K_{\text{a}}$ of $\ce{H2O}$ is $15.74$
>* The $\text{p}K_{\text{a}}$ of $\ce{H3O+}$ is $-1.74$

**Reminder:**
* Strong acid $\rightarrow$ negligible conjugate base;
* Weak acid $\rightarrow$ weak conjugate base;
* Negligible acidity $\rightarrow$ strong conjugate base;

---

:::matrix{cols="50/50" gap="30px"}
[[0,0]]
# Example: Strong Acid

$$
\ce{HNO3 (aq) + H2O (l) -> H3O+ (aq) + NO3- (aq)}
$$
**Note:** Strong acid = complete ionization. 
So for every mole of the monoprotic acid we'll get mole of $\ce{H+}$ ions and a mole of conjugated base. 
Situation may be a bit more complicated for diprotic acids.


In a $0.20 \text{ M}$ solution of $\ce{HNO3 (aq)}$, $[\ce{H+}] = [\ce{NO3-}] = 0.20 \text{ M}$.


**Note:** we neglect autoionization of water, for pure water $[\ce{H+}] \sim 10^{-7} \text{ M}$. 
If the concentration of acid will be $10^{-6} \text{ M}$ or less, it would be preferable to consider water autoionization as well.
$$
\text{pH} = -\log\_{10}([\ce{H+}]) = -\log\_{10}(0.2) \approx 0.7
$$

[[0,1]]
# Example: Strong Base 
## (negligible acid)

$$
\ce{Ca(OH)2 (aq) -> Ca^2+(aq) + 2 OH- (aq)}
$$
**Note:** Strong base = complete ionization.
In a $0.0011 \text{ M}$ solution of $\ce{Ca(OH)2 (aq)}$, $[\ce{OH-}] = 2[\ce{Ca^2+}] = 0.0022 \text{ M}$.


**Note:** we neglect $\ce{OH-}$ from autoionization of water since for pure water $[\ce{OH-}] \sim 10^{-7} \text{ M}$. 
If the concentration of the base will be $10^{-6} \text{ M}$ or less, it would be preferable to consider water autoionization as well.

We suppose there is much more water $[\ce{H2O}] = 56 \text{ M}$, thus $[\ce{H+}][\ce{OH-}] = 10^{-14}$. 
So we have
$$
[\ce{H+}] = \frac{10^{-14}}{0.0022} = 4.55 \times 10^{-12}.
$$
As a result
$$
\text{pH} = -\log_{10}(4.55 \times 10^{-12}) \approx 11.34
$$
:::

---

# Example: Weak acid

## Problem
Find $pH$ of $0.1\text{ M}$ solution of formic acid.

## Solution

![](./lecture_01_acids_bases/images/slide_22_img_42.png)

Here we do not know how many molecules dissociated. 
Let's write what we know.
$$
K_a = \frac{[\ce{HCOO-}][\ce{H+}]}{[\ce{HCOOH}]}
$$
We neglect $\ce{H+}$ from autoionization of water since for pure water $K_W = 10^{-14}$ and use chemical equation to get $[\ce{HCOO-}] = [\ce{H+}]$
$$
0.1 \text{ M} = [\ce{HCOOH}] + [\ce{H+}] = [\ce{HCOOH}] + [\ce{HCOO-}]
$$
This yields
$$
[\ce{H+}]^2 = K_a[\ce{HCOOH}] = K_a(0.1 - [\ce{H+}]) \approx 0.1K_a
$$
Thus
$$
[\ce{H+}] = 1.8 \times 10^{-5}; \quad pH = 2.37
$$

---

# Polyprotic Acids

It is always easier to remove the first proton from a polyprotic acid than to remove the second. 
Similarly, for an acid with three ionizable protons, it is easier to remove the second proton than the third.

### Acid-Dissociation Constants of Some Common Polyprotic Acids

| Name | Formula | $K\_{a1}$ | $K\_{a2}$ | $K\_{a3}$ |
| --- | --- | --- | --- | --- |
| Ascorbic | $\ce{H2C6H6O6}$ | $8.0 \times 10^{-5}$ | $1.6 \times 10^{-12}$ |  |
| Carbonic | $\ce{H2CO3}$ | $4.3 \times 10^{-7}$ | $5.6 \times 10^{-11}$ |  |
| Citric | $\ce{H3C6H5O7}$ | $7.4 \times 10^{-4}$ | $1.7 \times 10^{-5}$ | $4.0 \times 10^{-7}$ |
| Oxalic | $\ce{HOOC-COOH}$ | $5.9 \times 10^{-2}$ | $6.4 \times 10^{-5}$ |  |
| Phosphoric | $\ce{H3PO4}$ | $7.5 \times 10^{-3}$ | $6.2 \times 10^{-8}$ | $4.2 \times 10^{-13}$ |
| Sulfurous | $\ce{H2SO3}$ | $1.7 \times 10^{-2}$ | $6.4 \times 10^{-8}$ |  |
| Sulfuric | $\ce{H2SO4}$ | Large | $1.2 \times 10^{-2}$ |  |
| Tartaric | $\ce{C2H2O2(COOH)2}$ | $1.0 \times 10^{-3}$ | $4.6 \times 10^{-5}$ |  |

---

# Henderson-Hasselbalch equation

:::matrix{cols="50/50"}
[[0,0]]
For chemical reaction
$$
\ce{HA <=> H+ + A-}
$$
we write
$$
K_a = \frac{[\ce{H+}][\ce{A-}]}{[\ce{HA}]}
$$
Solve for $[\ce{H+}]$
$$
[\ce{H+}] = K_a \frac{[\ce{HA}]}{[\ce{A-}]}
$$
On both sides, take the negative logarithm:
$$
-\log[\ce{H+}] = -\log K_a - \log \frac{[\ce{HA}]}{[\ce{A-}]}
$$
[[0,1]]
$\text{pH} = -\log[\ce{H+}]$, while $\text{p}K\_a = -\log K_a$ by definition. 
We get
$$
\text{pH} = \text{p}K_a - \log \frac{[\ce{HA}]}{[\ce{A-}]}
$$
Inversion of $-\log \frac{[\ce{HA}]}{[\ce{A-}]}$ by changing its sign, provides the **Henderson-Hasselbalch equation**
$$
\text{pH} = \text{p}K_a + \log \frac{[\ce{A-}]}{[\ce{HA}]}
$$


**Note:** equation is still true if $\ce{A-}$ is a common ion.
:::
---

# Titration of Weak Acid with Strong Base / Creating Buffer


![](./lecture_01_acids_bases/images/slide_25_img_45.png)

Henderson-Hasselbalch equation still applies. 
$pH = pK_a + \log \textcolor{#7EA6FF}{\rule[-0.2em]{2em}{1.2em}} / \textcolor{#FF7E82}{\rule[-0.2em]{1.5em}{1.2em}}$

**Note:** we can get the final situation by mixing weak acid and salt, say CH3COONa


---

# Buffers in Action

:::matrix{cols="70/30"}
[[0:2,0]]
* Most cases weak acid and a salt are used. 
* Most practical cases salt is considered as fully dissociated, $[\ce{H+}]$ from water and $[\ce{A-}]$ from acid neglected
![](./lecture_01_acids_bases/images/slide_26_img_46.png){width=90}
[[0,1]]
![](./lecture_01_acids_bases/images/slide_26_img_47.png){width=80}
[[1,1]]
![](./lecture_01_acids_bases/images/slide_26_img_48.png){width=150}
:::

---

# Titration Curve Form

$$
\ce{HA <=> H+ + A-}
$$
Henderson-Hasselbalch equation
$$
pH = pK_a + \log \frac{[\ce{A-}]}{[\ce{HA}]}
$$
If equilibrium is shifted to the left or to the right, the decrease or increase in $[\ce{A-}]$ is compensated by $[\ce{HA}]$
$$
pH = pK_a + \log \frac{[\ce{A-}] - x}{[\ce{HA}] + x}
$$
Here’s a plot of $\ln\left(\frac{1-x}{1+x}\right)$ to get the idea of possible curves


![](./lecture_01_acids_bases/images/slide_27_img_50.png)


---

# Notable buffers in human body

1. **Bicarbonate buffer** ($\ce{H2CO3 / HCO3-}$)
   * Most important extracellular buffer, especially in blood plasma.
   * Works with the lungs (exhaling $\ce{CO2}$) and kidneys (adjusting $\ce{HCO3-}$) for rapid and long-term control.
   * Maintains blood pH near 7.4.
2. **Phosphate buffer** ($\ce{H2PO4- / HPO4^2-}$)
   * Important in intracellular fluid and renal tubules.
   * Has a $\text{p}K_a \approx 6.8$, close to physiological pH, so it is effective inside cells.
3. **Protein buffer systems**
   * Proteins act as buffers via ionizable side chains (e.g., histidine imidazole group).
   * Very important inside cells and in plasma (albumin is a major buffer in blood).
4. **Hemoglobin buffer**
   * A subset of the protein buffer system but often mentioned separately.
   * Hemoglobin binds both protons ($\ce{H+}$) and $\ce{CO2}$ (as carbamino groups).
   * Works in tandem with the bicarbonate system (Bohr effect, Haldane effect).
   * Crucial for pH regulation during gas transport in blood.

---

# Mixing Two Acids

:::matrix{cols="50/50"}
[[0,0]]
For chemical reactions
$$
\ce{HA1 + H2O <=> H3O+ + A1-}, \quad K_1 = \frac{[\ce{H3O+}][\ce{A1-}]}{[\ce{HA1}]}
$$
$$
\ce{HA2 + H2O <=> H3O+ + A2-}, \quad K_2 = \frac{[\ce{H3O+}][\ce{A2-}]}{[\ce{HA2}]}
$$
mass balance (molar concentrations before dissociation are $C\_1$ and $C\_2$)
$$
C\_1 = [\ce{HA1}] + [\ce{A1-}]; \qquad C\_2 = [\ce{HA2}] + [\ce{A2-}]
$$
charge balance (I neglect autodissociation of water, but it can be included with appropriate equations)
$$
[\ce{H3O+}] = [\ce{A1-}] + [\ce{A2-}]
$$
Express
$$
[\ce{HA1}] = C\_1 - [\ce{A1-}] = \frac{[\ce{H3O+}][\ce{A1-}]}{K\_1} \rightarrow [\ce{A1-}] = \frac{C\_1K\_1}{[\ce{H3O+}] + K_1}
$$
[[0,1]]
Same for $\ce{A2-}$, thus
$$
[\ce{H3O+}] = \frac{C\_1K\_1}{[\ce{H3O+}] + K\_1} + \frac{C\_2K\_2}{[\ce{H3O+}] + K_2}
$$
We can make a $3$-rd order equation on $[\ce{H3O+}]$ from this (4-th order if we include autodissociation of water), solve it numerically and find $pH$


**Another aspect:** acid protonates acid.
$$
K = \frac{K\_1}{K\_2} = \frac{[\ce{A1-}][\ce{HA2}]}{[\ce{HA1}][\ce{A2-}]}, \quad \ce{HA1 + A2- <=> A1- + HA2}
$$
![rect](-2 40 100 20){color=red width=4px}
:::





