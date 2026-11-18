
:::titlepage
[[top]]
Physical and Colloid Chemistry — Lecture 2 Supplement

[[title]]
Addendum:
Partial Derivatives in Thermodynamics

[[subcaption]]
From Multivariable Surfaces to Equations of State, Response Functions, and Exact Differentials
:::

---

# Why Ordinary Derivatives Are Not Enough

:::matrix {cols="54/46"}
[[0,0]]
In introductory single-variable calculus, a function $y = f(x)$ has **only one input knob** $x$:
- Its graph is a **1D curve** in a plane.
- From any point on the curve, you can move along only **one axis** ($\pm x$).
- A single number — the ordinary derivative $\dfrac{dy}{dx}$ — completely describes the slope.
[[0,1]]
![](./lecture_02_basics_of_thermodynamics/images/addendum_1d_vs_2d.png){width=100% center}
:::

<br>

**In the real world (and in thermodynamics), almost nothing depends on a single variable:**
- The pressure of a pure gas depends on *both* temperature and volume: $P = f(T, V)$.
- The Gibbs free energy of a reaction mixture depends on temperature, pressure, and the amounts of every species: $G = G(T, P, n_1, n_2, \dots)$.
- Chemical reaction rates depend on $T$, $\text{pH}$, ionic strength, and concentrations.

<br>

**The Geometric Problem:**
A function of two variables $z = f(x, y)$ is a **2D surface in 3D space** — like a mountain range. If you stand at a point on a hillside and ask *"What is the slope here?"*, the question has **no answer** until you specify **which compass direction you walk**!


---

# Simple Derivative vs. Partial Derivative 

:::matrix {cols="50/50"}
[[0,0]]
| Feature | Ordinary Derivative $\dfrac{dy}{dx}$ | Partial Derivative $\left(\dfrac{\partial f}{\partial x}\right)_y$ |
|---|---|---|
| **Function** | Single variable: $y = f(x)$ | Multivariable: $z = f(x, y, \dots)$ |
| **Geometry** | Tangent slope of a **1D curve** | Tangent slope of a **1D slice** through a surface |
| **Other variables** | None exist | Explicitly **frozen** (held constant) |
| **Symbol** | Straight Roman $d$ (Leibniz, 1675) | Rounded $\partial$ ("curly d", Legendre & Jacobi, 1841) |
| **Subscript** | Never needed | **Mandatory in thermodynamics:** $(\dots)_y$ tells you which knob is locked |

### Total vs. Partial Derivative: The Weather-Balloon Analogy

Suppose atmospheric temperature $T(x, y, t)$ varies with position $(x, y)$ and time $t$:

[[0,1]]

1. **Fixed Weather Station (Partial Derivative $\dfrac{\partial T}{\partial t}$):**
   You bolt your thermometer to a fixed tower ($x = \text{const}, y = \text{const}$). You measure purely how fast the air warms up at that exact spot as the sun rises:
   $$
   \left(\frac{\partial T}{\partial t}\right)_{x,y} = \text{rate of change at fixed position.}
   $$

2. **Drifting Hot-Air Balloon (Total Derivative $\dfrac{dT}{dt}$):**
   Your balloon drifts with the wind at velocity $(v_x, v_y) = \left(\frac{dx}{dt}, \frac{dy}{dt}\right)$. Your thermometer reading changes *both* because the day is warming up **and** because you are flying into a warmer valley:
   $$
   \frac{dT}{dt} = \underbrace{\left(\frac{\partial T}{\partial t}\right)\_{x,y}}\_{\text{local warming}} + \underbrace{\left(\frac{\partial T}{\partial x}\right)\_{y,t}\frac{dx}{dt} + \left(\frac{\partial T}{\partial y}\right)\_{x,t}\frac{dy}{dt}}_{\text{motion across spatial gradients}}.
   $$
:::

---

# The Bigger Picture: Where Partial Derivatives Rule Science

The partial derivative $\partial$ is not just a bookkeeping trick for gases --- it is the foundational building block of modern mathematics, physics, and computational chemistry:

:::matrix {cols="56/44"}
[[0,0]]
1. **Vector Calculus, Gradients ($\nabla f$) & Modern AI:**
   Bundling all partial derivatives into a vector gives the **gradient** $\nabla f = \left(\frac{\partial f}{\partial x_1}, \dots, \frac{\partial f}{\partial x_n}\right)$, which always points up the direction of **steepest ascent**. Stepping in the opposite direction ($-\nabla f$, *Gradient Descent*) is how molecules relax to minimum-energy 3D geometries **and** how neural networks / LLMs train across billions of parameters!
2. **Partial Differential Equations (PDEs) — The Laws of Nature:**
   Whenever a physical field evolves in both space and time, its law is a PDE linking spatial and temporal partial derivatives:
   - **Fick's Diffusion / Heat Equation:** $\dfrac{\partial c}{\partial t} = D\,\dfrac{\partial^2 c}{\partial x^2}$
   - **Schrödinger's Quantum Wave Equation:** $i\hbar\dfrac{\partial \Psi}{\partial t} = -\dfrac{\hbar^2}{2m}\dfrac{\partial^2 \Psi}{\partial x^2} + V\Psi$
3. **Differential Geometry & Curved Manifolds:**
   The equilibrium states of a substance form a smooth curved surface (**Gibbs' thermodynamic manifold**). At any state $p$, the partial derivative operators $\left\\{\frac{\partial}{\partial T}, \frac{\partial}{\partial V}\right\\}$ span the local **tangent plane** $T_p\mathcal{M}$ — the exact same geometric apparatus used in Einstein's General Relativity.

[[0,1]]
4. **Differential Forms & Topology ($df$ vs. $\delta A$):**
   Distinguishing path-independent state functions ($dU, dS$) from path-dependent integrals ($\delta Q, \delta A$) is the gateway to **exterior calculus** ($1$-forms $\omega = M\,dx + N\,dy$), Stokes' theorem, and cohomology.
![](./lecture_02_basics_of_thermodynamics/images/addendum_math_connections.png){width=71}
:::

---
# From Hamiltonian $\mathcal{H}$ to Macrostate: Collapsing $10^{24}$ Variables

Why can $1\text{ mol}$ of gas ($N \approx 6\times 10^{23}$ molecules, $6N \approx 3.6\times 10^{24}$ positions and momenta) be described by just **2 or 3 macroscopic variables**?

1. **The Microscopic Hamiltonian ($\mathcal{H} = \sum \mathbf{p}_i\cdot\dot{\mathbf{r}}_i - \mathcal{L}$):**
   In classical mechanics, the microstate is a point $(\mathbf{r}_1, \dots, \mathbf{r}_N, \mathbf{p}_1, \dots, \mathbf{p}_N) \in \mathbb{R}^{6N}$ governed by the Hamiltonian:
   $$
   \mathcal{H}\bigl(\underbrace{\mathbf{r}\_1, \dots, \mathbf{r}\_N,\; \mathbf{p}\_1, \dots, \mathbf{p}\_N}\_{6N \text{ fast internal coordinates}};\\; \underbrace{V, N}\_{\text{external parameters}}\bigr) = \sum\_{i=1}^{N} \frac{\mathbf{p}\_i^2}{2m} + \sum\_{i < j} u\_{\text{pair}}(|\mathbf{r}\_i - \mathbf{r}\_j|) + \sum\_{i=1}^{N} U\_{\text{wall}}(\mathbf{r}\_i;\\, V).
   $$
2. **The Phase-Space Integral Collapse (Boltzmann Partition Function $Z$):**
   Just as a 1D definite integral $\int_0^L f(x;\, \alpha)\,dx = F(\alpha, L)$ **integrates out the dummy variable $x$** and leaves a function only of $\alpha$ and $L$, thermal equilibrium integrates $e^{-\mathcal{H}/k_B T}$ over all $6N$ microscopic coordinates:
   $$
   Z({\color{#d9480f}T}, {\color{#1971c2}V}, {\color{#0f766e}N}) = \frac{1}{{\color{#0f766e}N!}\\,h^{3{\color{#0f766e}N}}} \underbrace{\int_{\color{#1971c2}V} d^3\mathbf{r}\_1 \cdots \int_{\color{#1971c2}V} d^3\mathbf{r}\_N \int_{-\infty}^{+\infty} d^3\mathbf{p}\_1 \cdots \int_{-\infty}^{+\infty} d^3\mathbf{p}_N}\_{\text{All } 6N \approx 10^{24} \text{ microscopic coordinates }(\mathbf{r}_i, \mathbf{p}_i)\text{ are INTEGRATED OUT!}} \\, \exp\\!\left(-\frac{\mathcal{H}(\mathbf{r}_1, \dots, \mathbf{p}_N;\\, {\color{#1971c2}V}, {\color{#0f766e}N})}{k_B {\color{#d9480f}T}}\right).
   $$

---
# From Hamiltonian $\mathcal{H}$ to Macrostate: Collapsing $10^{24}$ Variables

**What survives the integral?** Only the un-integrated parameters: ${\color{#d9480f}T}$ (from the Boltzmann factor), ${\color{#1971c2}V}$ (from the spatial integral bounds), and ${\color{#0f766e}N}$ (particle count)! The phase-space integral collapses $10^{24}$ coordinates into **one master generating function** — the Helmholtz free energy $F({\color{#d9480f}T}, {\color{#1971c2}V}, {\color{#0f766e}N}) = -k_B T\ln Z({\color{#d9480f}T}, {\color{#1971c2}V}, {\color{#0f766e}N})$.

![](./lecture_02_basics_of_thermodynamics/images/addendum_hamiltonian_collapse.png){width=100% center}

---
# Why Partial Derivatives? Differentiating Under the Integral Sign

Wait — the **integral** collapsed $6N$ coordinates into $Z(T, V, N)$. So **why do we then take 1st and 2nd partial derivatives of $\ln Z$ (or $F = -k_B T\ln Z$) to get $U, P, S, C_V$?**
Because $\mathcal{H}$ sits inside the exponential $e^{-\mathcal{H}/k_B T}$ under the integral! 

:::matrix {cols="50/50" gap=20px}
[[0,0]]
Differentiating $\ln Z$ with respect to an external parameter ($T$ or $V$) pulls the conjugate physical quantity down from the exponent and automatically computes its Boltzmann ensemble average $\langle \cdots \rangle$:
### 1. How a Partial Derivative Computes an Average
- **Differentiate $\ln Z$ wrt ${\color{#d9480f}T}$** $\left(\text{using }\frac{\partial}{\partial T}\left(-\frac{\mathcal{H}}{k_B T}\right) = +\frac{\mathcal{H}}{k_B T^2}\right)$:
  $$
  \\!\\!\\!\\!\left(\frac{\partial \ln Z}{\partial T}\right)\_{V,N}\\!\\!\\! = \frac{1}{Z}\frac{\partial Z}{\partial T} = \frac{1}{k_B T^2}\int \mathcal{H}\\,\underbrace{\frac{e^{-\mathcal{H}/k_B T}}{Z}}\_{\rho(\mathbf{r},\mathbf{p})} d^{3N}r\\,d^{3N}p =
  $$
  $$
  = \frac{\langle \mathcal{H} \rangle}{k_B T^2} \Longrightarrow \quad \mathbf{U = \langle \mathcal{H} \rangle = k_B T^2\left(\frac{\partial \ln Z}{\partial T}\right)_{V,N}}.
  $$
- **Differentiate $\ln Z$ wrt ${\color{#1971c2}V}$** $\left(-\frac{\partial \mathcal{H}}{\partial V}\text{ is the wall force/area}\right)$:
  $$
  \mathbf{P = -\left\langle \frac{\partial \mathcal{H}}{\partial V}\right\rangle = k_B T\left(\frac{\partial \ln Z}{\partial V}\right)\_{T,N} = -\left(\frac{\partial F}{\partial V}\right)\_{T,N}}.
  $$

[[0,1]]
### 2. The Complete Hierarchy: 0th, 1st & 2nd Derivatives

| Order | Mathematical Object | Physical Role |
|:---:|:---|:---|
| **0th** *(Function)* | $F(T,V,N) = -k_B T\ln Z$<br>*(plus $G = F + PV$, $H = U + PV$)* | **Thermodynamic Potentials**<br>(master generating functions) |
| **1st** *(Slopes)* | $S = -\left(\dfrac{\partial F}{\partial T}\right)\_{V,N}$<br>$P = -\left(\dfrac{\partial F}{\partial V}\right)\_{T,N}$<br>$\mu = +\left(\dfrac{\partial F}{\partial N}\right)\_{T,V}$ | **Equations of State**<br>(ensemble mean values $\langle \cdots \rangle$) |
| **2nd** *(Curvatures)* | $C_V = -T\left(\dfrac{\partial^2 F}{\partial T^2}\right)\_{V,N} = \dfrac{\operatorname{Var}(\mathcal{H})}{k_B T^2}$<br>$\dfrac{1}{V\kappa_T} = \left(\dfrac{\partial^2 F}{\partial V^2}\right)\_{T,N}$ | **Response Functions & Fluctuations**<br>(variances $\langle \mathcal{H}^2\rangle - \langle\mathcal{H}\rangle^2$) |
:::


---
# Counting Degrees of Freedom & The 1–2–3 Variable Rule

:::matrix {cols="52/48" gap=20px}
[[0,0]]
### 1. Why 2 Variables for a Closed Pure Phase?
- For a pure substance ($c=1$), **3 parameters** survive the phase-space integral: $(T, V, N)$ — giving our Equation of State $P = f(T, V, n)$.
- Because a homogeneous phase is **extensive (scale-invariant)**, fixing the amount $n = 1\text{ mol}$ (or dividing by $n$ to use molar quantities $V_m = V/n, U_m = U/n$) eliminates the size knob $n$, leaving a **2D Equilibrium State Surface $\mathcal{M}$** ($\dim \mathcal{M} = 2$).

### 2. When Does the Dimensionality Change?
- **Mix $c$ chemical species:** $\mathcal{H}$ has $c$ distinct species sums with particle counts $N_1, \dots, N_c$ that all survive the integral $\implies Z(T, V, N_1, \dots, N_c)$ ($\mathbf{c + 1}$ intensive variables: $T, P, x_1, \dots, x_{c-1}$).
- **Turn on external fields ($\mathbf{B}, \mathbf{E}$) or colloidal surface area $A_{\text{surf}}$:** New un-integrated parameters inside $\mathcal{H}(\dots; V, N, \mathbf{B}, A_{\text{surf}})$ survive into $Z$ ($\mathbf{+1}$ dimension per external field/interface!).
- **Coexisting phases ($\phi \ge 2$):** Phase equilibrium ($T^{(1)}=T^{(2)}, P^{(1)}=P^{(2)}, \mu^{(1)}=\mu^{(2)}$) imposes constraints that *remove* $\phi - 1$ degrees of freedom (**Gibbs' Phase Rule:** $F = c - \phi + 2$).

[[0,1]]
### 3. The 1–2–3 Rule on the 2D State Surface $\mathcal{M}$
For $1\text{ mol}$ of a pure single-phase substance ($\dim \mathcal{M} = 2$), we can measure many scalar observables ($P, V_m, T, U_m, H_m, S_m, G_m, F_m$):

1. **Pick 1 variable (e.g. $T = T_0$):**
   Carves out a **1D curve** on the 2D surface (an isotherm, isobar, isochore, or adiabat). *1 degree of freedom remains.*

2. **Pick 2 independent variables (e.g. $(T, V_m)$ or $(T, P)$):**
   Forms a **2D coordinate chart (grid)** on $\mathcal{M}$. You can vary both knobs independently, and every pair $(T, V_m)$ uniquely pins down the state.

3. **Pick ANY 3 variables $(x, y, z)$ (e.g. $(P, V_m, T)$ or $(T, P, H_m)$):**
   Mapping a **2D surface into 3D space** $\mathbb{R}^3$ means the 3 variables **cannot** be independent — they are forced to obey **one implicit constraint equation**:
   $$
   \bbox[#eef6ff, 10px, border-radius: 8px]{
   f(x, y, z) = 0 \quad \text{(An Equation of State!)}
   }
   $$
   And any triple $(x, y, z)$ linked by $f(x, y, z) = 0$ automatically obeys the **Cyclic Rule**!
:::

---

# Slicing a Surface: What $\left({\partial P}/{\partial V}\right)_T$ Means Geometrically

:::matrix {cols="48/52"}
[[0,0]]
How do we turn a 3D surface $P = f(T, V)$ back into a 1D curve that we already know how to differentiate? **We slice it with a flat plane!**
- **Isochore Slice (Blue Plane, $V = V_0 = \text{const}$):**
  Lock the volume in a rigid container and vary temperature $T$. The intersection of the surface with the plane $V = V_0$ is a 1D curve $P(T)$, and its tangent slope is:
  $$
  {\color{#1971c2}\left(\frac{\partial P}{\partial T}\right)\_V} = \lim_{\Delta T \to 0} \frac{P(T + \Delta T,\\, V_0) - P(T,\\, V_0)}{\Delta T}.
  $$
- **Isotherm Slice (Red Plane, $T = T_0 = \text{const}$):**
  Immerse the cylinder in a constant-temperature bath and vary volume $V$. The intersection with the plane $T = T_0$ is an **isotherm** $P(V)$, and its tangent slope is:
  $$
  {\color{#d9480f}\left(\frac{\partial P}{\partial V}\right)\_T} = \lim_{\Delta V \to 0} \frac{P(T_0,\\, V + \Delta V) - P(T_0,\\, V)}{\Delta V}.
  $$
- **Isobar Slice (Horizontal Plane, $P = P_0 = \text{const}$):**
  Let a weighted piston keep pressure constant and measure how volume expands with temperature: slope $= \left(\dfrac{\partial V}{\partial T}\right)_P$.

[[0,1]]
![](./lecture_02_basics_of_thermodynamics/images/addendum_surface_slices.png){width=100% center}
:::

---

<iframe src="./lecture_02_basics_of_thermodynamics/demos/partial-slicer.html" width="100%" height="850px" style="border:1px solid #ccc; border-radius: 8px;"></iframe>

---

# How to Compute a Partial Derivative: "The Freeze Rule"

To compute $\left(\dfrac{\partial f}{\partial {\color{#d9480f}x}}\right)_{\color{#1971c2}y}$ algebraically, **pretend that every variable in the subscript (${\color{#1971c2}y}$) is a fixed number like $5$ or $\pi$**, and apply ordinary 1D differentiation rules to the active variable (${\color{#d9480f}x}$):

:::matrix {cols="33/33/34"}
[[0,0]]
### 1. Polynomial Warmup
Let $f(x, y) = 3x^2 y + y^3 - 5x$.

**Differentiate wrt ${\color{#d9480f}x}$ at constant ${\color{#1971c2}y}$:**
$$
\begin{aligned}
\left(\frac{\partial f}{\partial {\color{#d9480f}x}}\right)_{\color{#1971c2}y} &= \frac{\partial}{\partial {\color{#d9480f}x}}\left(3{\color{#1971c2}y}\cdot {\color{#d9480f}x}^2 + {\color{#1971c2}y^3} - 5{\color{#d9480f}x}\right) \\\\
&= 3{\color{#1971c2}y}\cdot (2{\color{#d9480f}x}) + 0 - 5 \\\\
&= 6xy - 5.
\end{aligned}
$$
*(Notice ${\color{#1971c2}y^3}$ has no $x$ in it, so its derivative wrt $x$ is $0$!)*

**Differentiate wrt ${\color{#d9480f}y}$ at constant ${\color{#1971c2}x}$:**
$$
\begin{aligned}
\left(\frac{\partial f}{\partial {\color{#d9480f}y}}\right)_{\color{#1971c2}x} &= \frac{\partial}{\partial {\color{#d9480f}y}}\left(3{\color{#1971c2}x^2}\cdot {\color{#d9480f}y} + {\color{#d9480f}y}^3 - {\color{#1971c2}5x}\right) \\\\
&= 3x^2 + 3y^2 - 0.
\end{aligned}
$$

[[0,1]]
### 2. Perfect Gas Law
$$
P(T, V) = \frac{nRT}{V}
$$

**Isochore slope ($\text{freeze } {\color{#1971c2}V, n}$, vary ${\color{#d9480f}T}$):**
$$
\begin{aligned}
\left(\frac{\partial P}{\partial {\color{#d9480f}T}}\right)_{{\color{#1971c2}V,n}} &= {\color{#1971c2}\frac{nR}{V}} \cdot \frac{d}{d{\color{#d9480f}T}}({\color{#d9480f}T}) \\\\
&= +\frac{nR}{V} > 0.
\end{aligned}
$$

**Isotherm slope ($\text{freeze } {\color{#1971c2}T, n}$, vary ${\color{#d9480f}V}$):**
$$
\begin{aligned}
\left(\frac{\partial P}{\partial {\color{#d9480f}V}}\right)_{{\color{#1971c2}T,n}} &= {\color{#1971c2}nRT} \cdot \frac{d}{d{\color{#d9480f}V}}\left({\color{#d9480f}V^{-1}}\right) \\\\
&= -\frac{nRT}{V^2} < 0.
\end{aligned}
$$

[[0,2]]
### 3. van der Waals Equation
$$
P(T, V) = \frac{nRT}{V - nb} - \frac{n^2 a}{V^2}
$$

**Differentiate wrt ${\color{#d9480f}T}$ at constant ${\color{#1971c2}V}$:**
$$
\begin{aligned}
\left(\frac{\partial P}{\partial {\color{#d9480f}T}}\right)\_{\color{#1971c2}V} &= \frac{\partial}{\partial {\color{#d9480f}T}}\left({\color{#1971c2}\frac{nR}{V - nb}}\\,{\color{#d9480f}T} - \underbrace{\color{#1971c2}\frac{n^2 a}{V^2}}\_{\text{constant!}}\right) \\\\
&= \frac{nR}{V - nb} - 0.
\end{aligned}
$$
**Differentiate wrt ${\color{#d9480f}V}$ at constant ${\color{#1971c2}T}$:**
$$
\left(\frac{\partial P}{\partial {\color{#d9480f}V}}\right)_{\color{#1971c2}T} = -\frac{nRT}{(V - nb)^2} + \frac{2n^2 a}{V^3}.
$$
:::

---
# Mathematicians Drop the Subscript, but Chemists NEVER Can

In a pure math textbook, a function $f(x, y)$ has only one canonical set of variables, so writing $\dfrac{\partial f}{\partial x}$ unambiguously means *"hold $y$ constant"*. 

### 1. Pure Math Demonstration
Suppose $z = x^2 + xy$.
- If our independent variables are $(x, y)$, holding $y$ constant gives:
  $$
  \left(\frac{\partial z}{\partial x}\right)_y = 2x + y.
  $$
- Now define a new variable $u = x + y$ (so $y = u - x$) and express the **exact same quantity** $z$ in terms of $(x, u)$:
  $$
  z = x^2 + x(u - x) = xu.
  $$
- Differentiating $z$ with respect to $x$ while holding $u$ constant gives:
  $$
  \left(\frac{\partial z}{\partial x}\right)_u = u = x + y \\;\neq\\; \left(\frac{\partial z}{\partial x}\right)_y = 2x + y!
  $$
Changing *which partner variable is frozen* changes the geometric slice direction and gives a **completely different derivative**!

---
# Mathematicians Drop the Subscript, but Chemists NEVER Can

**In thermodynamics, state variables $(P, V, T, U, H, S, G)$ are linked by equations of state**, so writing $\dfrac{\partial U}{\partial T}$ without a subscript is mathematically incomplete!

### 2. Thermodynamic Reality: Constant $V$ vs. Constant $P$
Consider the enthalpy $H = U + PV$ of $1\text{ mol}$ of a monatomic ideal gas ($U_m = \frac{3}{2}RT$, $PV_m = RT$). How fast does energy rise with temperature $T$?
- **Hold Volume $V$ Constant (Rigid Bomb Calorimeter):**
  No expansion work is done ($dV = 0$), so all heat goes into internal energy:
  $$
  C_{V,m} = \left(\frac{\partial U_m}{\partial T}\right)_V = \frac{\partial}{\partial T}\left(\frac{3}{2}RT\right)_V = \frac{3}{2}R \approx 12.47\,\mathrm{J/(mol\,K)}.
  $$
- **Hold Pressure $P$ Constant (Open Piston Cylinder):**
  As temperature rises, the gas must expand ($\left(\frac{\partial V_m}{\partial T}\right)\_P = \frac{R}{P}$) and push back the atmosphere, requiring extra energy $P\,dV_m = R\,dT$:
  $$
  \begin{aligned}
  C_{P,m} = \left(\frac{\partial H_m}{\partial T}\right)_P = \left(\frac{\partial (U_m + PV_m)}{\partial T}\right)_P = \frac{3}{2}R + R = \frac{5}{2}R \approx 20.79\,\mathrm{J/(mol\,K)}.
  \end{aligned}
  $$

---
# Changing the Frozen Variable: The Subscript Bridge Formula

Geometrically, why is $\left(\dfrac{\partial F}{\partial x}\right)_y$ different from $\left(\dfrac{\partial F}{\partial x}\right)_z$? Because on the 2D state surface $\mathcal{M}$, the coordinate curves $y = \text{const}$ (e.g. blue isochores $V = \text{const}$) and $z = \text{const}$ (e.g. green isobars $P = \text{const}$) **intersect at an angle**!
Walking along $P = \text{const}$ while increasing $T$ by $1\,\mathrm{K}$ means you are stepping in a **different direction on the 2D surface** than walking along $V = \text{const}$.

:::matrix {cols="52/48"}
[[0,0]]

### 1-Line Derivation of the Subscript Bridge Rule:
Start with the total differential of any state function $F(x, y)$:
$$
dF = \left(\frac{\partial F}{\partial x}\right)_y dx + \left(\frac{\partial F}{\partial y}\right)_x dy.
$$
Now divide through by $dx$ while holding a **new variable $z$ constant**:
$$
\bbox[#eef6ff, 12px, border-radius: 10px]{
\left(\frac{\partial F}{\partial x}\right)_z = \left(\frac{\partial F}{\partial x}\right)_y + \left(\frac{\partial F}{\partial y}\right)_x \left(\frac{\partial y}{\partial x}\right)_z
}
$$
**Thermodynamic Example — Heating $U(T, V)$ at Constant $P$ vs. Constant $V$:**
Set $F = U$, $x = T$, $y = V$, and new constraint $z = P$:
$$
\left(\frac{\partial U}{\partial T}\right)\_P = \underbrace{\left(\frac{\partial U}{\partial T}\right)\_V}\_{C_V} + \underbrace{\left(\frac{\partial U}{\partial V}\right)_T}\_{\text{internal pressure } \pi_T} \underbrace{\left(\frac{\partial V}{\partial T}\right)\_P}\_{V\alpha_V}.
$$

[[0,1]]
![](./lecture_02_basics_of_thermodynamics/images/addendum_coordinate_grids.png){width=95% center}
:::

---
# Anatomy of Response Functions: $\alpha_V$ and $\kappa_T$

$$
\bbox[#eef6ff, 14px, border-radius: 10px]{
\alpha_V = \frac{1}{V}\left(\frac{\partial V}{\partial T}\right)_P \quad \text{(isobaric thermal expansion coefficient)}
}
\qquad
\bbox[#fff3ee, 14px, border-radius: 10px]{
\kappa_T = -\frac{1}{V}\left(\frac{\partial V}{\partial P}\right)_T \quad \text{(isothermal compressibility)}
}
$$

:::matrix {cols="50/50"}
[[0,0]]
### Why Are They Defined This Way?

1. **Why divide by $V$ in front of the derivative?**
   - Volume $V$ is **extensive**: a $10\\,\mathrm{L}$ tank of water expands $10\times$ more in $\mathrm{cm^3/K}$ than a $1\\,\mathrm{L}$ beaker ($\left(\frac{\partial V}{\partial T}\right)_P$ depends on sample size).
   - Dividing by $V$ gives the **fractional (relative) change per unit $\Delta T$ or $\Delta P$**, making $\alpha_V$ ($\mathrm{K^{-1}}$) and $\kappa_T$ ($\mathrm{bar^{-1}}$) **intensive material properties**!
   *(Recall from 1D calculus: $\frac{1}{V}\frac{\partial V}{\partial x} = \frac{\partial \ln V}{\partial x}$.)*

2. **Why the minus sign in $\kappa_T$?**
   - Squeezing any mechanically stable substance increases $P$ and *decreases* $V$, so the raw slope $\left(\frac{\partial V}{\partial P}\right)_T$ is always **negative**.
   - Putting a minus sign in front ensures tabulated compressibilities $\kappa_T > 0$ are convenient positive numbers.

[[0,1]]
### Worked Example: $\alpha_V$ and $\kappa_T$ of an Ideal Gas

Start with the equation of state solved for volume:
$$
V(T, P) = \frac{nRT}{P}.
$$

1. **Thermal Expansion Coefficient $\alpha_V$:**
   Freeze $P$ and $n$, differentiate wrt $T$:
   $$
   \left(\frac{\partial V}{\partial T}\right)_P = \frac{nR}{P} \quad \Longrightarrow \quad \alpha_V = \frac{1}{V}\left(\frac{nR}{P}\right) = \frac{nR}{PV} = \mathbf{\frac{1}{T}}.
   $$

2. **Isothermal Compressibility $\kappa_T$:**
   Freeze $T$ and $n$, differentiate wrt $P$:
   $$
   \left(\frac{\partial V}{\partial P}\right)_T = -\frac{nRT}{P^2} \quad \Longrightarrow \quad \kappa_T = -\frac{1}{V}\left(-\frac{nRT}{P^2}\right) = \mathbf{\frac{1}{P}}.
   $$
:::

---

# Heat Capacities & Gibbs Free Energy

Partial derivatives also govern how thermodynamic potentials ($U, H, S, G$) respond to changes in temperature and pressure:

:::matrix {cols="50/50"}
[[0,0]]
### 1. Heat Capacities as Tangent Slopes
$$
C_V = \left(\frac{\partial U}{\partial T}\right)_V, \qquad C_P = \left(\frac{\partial H}{\partial T}\right)_P
$$
![](./lecture_02_basics_of_thermodynamics/images/entalpy_plot.png){width=60% center}
- Geometrically, $C_P(T)$ is the **instantaneous slope of the tangent line** to the $H$ vs. $T$ isobar at temperature $T$.
- Because $C_P = \left(\frac{\partial H}{\partial T}\right)_P$, reversing the derivative (integrating at constant $P$) recovers the enthalpy change:
  $$
  \Delta H = \int\_{T_1}^{T_2} \left(\frac{\partial H}{\partial T}\right)\_P dT = \int\_{T_1}^{T_2} C_P(T)\,dT.
  $$

[[0,1]]
### 2. Gibbs Free Energy Slopes ($dG = V\,dP - S\,dT$)
We derived the fundamental differential of molar Gibbs energy: $dG_m = V_m\\,dP - S_m\\,dT.$
Reading off the two partial slopes immediately tells us how chemical stability shifts with $P$ and $T$:
1. **Pressure Slope at Constant $T$:** Set $dT = 0$:
:::matrix{cols=45/55}
[[0,0]]
$$
 \left(\frac{\partial G_m}{\partial P}\right)\_T = +V_m > 0.
$$
[[0,1]]
Since molar volume $V_m$ is always positive, $G_m$ always increases with pressure (steeply for gases with large $V_m$, gently for condensed phases).
:::
   For an ideal gas, $V_m = \frac{RT}{P}$, so integrating along an isotherm gives:
   $$
   G_m(P) - G_m^\circ = \int\_{P^\circ}^P \left(\frac{\partial G_m}{\partial P'}\right)\_T dP' = \int_{P^\circ}^P \frac{RT}{P'}dP' = RT\ln\frac{P}{P^\circ}.
   $$
3. **Temperature Slope at Constant $P$:** Set $dP = 0$:
:::matrix{cols=50/50}
[[0,0]]
   $$
   \left(\frac{\partial G_m}{\partial T}\right)_P = -S_m < 0.
   $$
[[0,1]]
   Since absolute entropy $S_m > 0$, $G_m$ always decreases with increasing $T$!
:::
:::

---

# Moving in Both Directions at Once: The Total Differential ($df$)

What if **both** independent variables change simultaneously by small amounts $(dx, dy)$ — for example, you heat a liquid by $dT$ *and* compress it by $dP$ at the same time?

Geometrically, for any smooth surface $f(x, y)$, a small patch around $(x_0, y_0)$ looks flat and can be approximated by its **tangent plane**. The total height change on the tangent plane is the sum of the two partial steps:

:::matrix {cols="60/40"}
[[0,0]]
$$
\bbox[#fff8e6, 12px, border-radius: 10px]{
df = \left(\frac{\partial f}{\partial x}\right)_y dx + \left(\frac{\partial f}{\partial y}\right)_x dy
}
$$

### Application to Volume $V(T, P)$:
Writing the total differential of $V(T, P)$ and substituting $\alpha_V$ and $\kappa_T$:
$$
\begin{aligned}
dV &= \left(\frac{\partial V}{\partial T}\right)_P dT + \left(\frac{\partial V}{\partial P}\right)_T dP \\\\
dV &= V\alpha_V\\,dT - V\kappa_T\\,dP \quad \Longrightarrow \quad \mathbf{\frac{dV}{V} = \alpha_V\\,dT - \kappa_T\\,dP}.
\end{aligned}
$$
**Quick Numerical Example (Liquid Water at $298\,\mathrm{K}$):**
$\alpha_V = 2.1\times 10^{-4}\\,\mathrm{K^{-1}}$, $\kappa_T = 49.6\times 10^{-6}\\,\mathrm{bar^{-1}}$, if water is heated by $\Delta T = +20\\,\mathrm{K}$ and compressed by $\Delta P = +100\\,\mathrm{bar}$:
$$
{\Delta V}/{V} \approx (2.1\times 10^{-4})(20) - (49.6\times 10^{-6})(100) = +0.42\% - 0.50\% = -0.08\%.
$$

[[0,1]]
![](./lecture_02_basics_of_thermodynamics/images/addendum_tangent_plane.png){width=100% center}
:::

---

# The Three Golden Rules of Partial Derivative Manipulation

In thermodynamics we constantly need to express a derivative that is **hard or impossible to measure** in terms of derivatives that are **easy to measure**. Three algebraic identities do all the heavy lifting:

:::matrix {cols="50/50"}
[[0,0]]
### 1. The Inversion (Reciprocal) Rule
You can flip a partial derivative upside down **if and only if the exact same variable $z$ is held constant**:
$$
\left(\frac{\partial x}{\partial y}\right)_z = \frac{1}{\left(\dfrac{\partial y}{\partial x}\right)_z}.
$$
*Geometrically: the both derivatives lie in the exact same 2D plane $z = \text{const}$, where $dx/dy = 1/(dy/dx)$.*

<br>

### 2. The Same-Subscript Chain Rule
To insert an intermediate variable $y$ while keeping $z$ fixed throughout:
$$
\left(\frac{\partial w}{\partial x}\right)_z = \left(\frac{\partial w}{\partial y}\right)_z \left(\frac{\partial y}{\partial x}\right)_z.
$$
*Example:* How does internal energy change with volume at constant $T$ if we know $U(P)$? $\left(\frac{\partial U}{\partial V}\right)_T = \left(\frac{\partial U}{\partial P}\right)_T \left(\frac{\partial P}{\partial V}\right)_T$.

[[0,1]]
### 3. The Cyclic (Triple Product) Rule
When three variables $(x, y, z)$ are linked by an equation of state $f(x, y, z) = 0$:
$$
\bbox[#ffeef0, 14px, border-radius: 10px]{
\left(\frac{\partial x}{\partial y}\right)_z \left(\frac{\partial y}{\partial z}\right)_x \left(\frac{\partial z}{\partial x}\right)_y = \mathbf{-1} \quad \color{#d9480f}{\Longleftarrow \text{NEVER } +1\text{!}}
}
$$

**2-Line Proof (Where Does the Minus Sign Come From?):**

From $df = f_x dx + f_y dy + f_z dz = 0$, holding one variable constant at a time gives:
$$
\left(\frac{\partial x}{\partial y}\right)_z = -\frac{f_y}{f_x}, \qquad \left(\frac{\partial y}{\partial z}\right)_x = -\frac{f_z}{f_y}, \qquad \left(\frac{\partial z}{\partial x}\right)_y = -\frac{f_x}{f_z}.
$$
Multiply all three together; the derivatives cancel, leaving $(-1)^3 = \mathbf{-1}$.
:::

---
# Payoff of the Cyclic Rule: Sealed Vessels

### 1. Measuring the Unmeasurable in Solids & Liquids
Suppose you want to know $\left(\dfrac{\partial P}{\partial T}\right)_V$ for **solid lead** or **liquid water** — how much pressure builds up per Kelvin if the sample is heated at strictly constant volume.
- **Direct measurement is nearly impossible:** If you heat lead inside a steel bomb, the steel container *also* expands and stretches!
- **The Cyclic Rule solution:** Measure $\alpha_V$ at constant atmospheric pressure and $\kappa_T$ at constant temperature, then divide them:
  $$
  \left(\frac{\partial P}{\partial T}\right)_V = -\frac{(\partial V/\partial T)_P}{(\partial V/\partial P)_T} = \frac{V\alpha_V}{V\kappa_T} = \frac{\alpha_V}{\kappa_T}.
  $$

### 2. Why Thermometer Bulbs & Sealed Bombs Explode
Using the table for **liquid water** ($\alpha_V = 2.1\times 10^{-4}\,\mathrm{K^{-1}}$, $\kappa_T = 49.6\times 10^{-6}\,\mathrm{bar^{-1}}$):
$$
\left(\frac{\partial P}{\partial T}\right)_V = \frac{2.1\times 10^{-4}\,\mathrm{K^{-1}}}{49.6\times 10^{-6}\,\mathrm{bar^{-1}}} \approx \mathbf{4.23\,\mathrm{bar/K}}.
$$
Heating a completely filled, rigid sealed vessel of water by just $\Delta T = +10\,\mathrm{K}$ generates $\Delta P \approx \mathbf{42.3\,\mathrm{bar}}$ ($\sim 42\,\mathrm{atm}$) of pressure! For **solid lead**, $\alpha_V/\kappa_T = 0.861\times 10^{-4} / 2.21\times 10^{-6} \approx \mathbf{39.0\,\mathrm{bar/K}}$!

---
# Payoff of the Cyclic Rule: $C_{P,m} - C_{V,m}$

### 3. Origin of Mayer's General Relation
We stated that for *any* homogeneous substance:
$$
C_{P,m} - C_{V,m} = V_m T \frac{\alpha_V^2}{\kappa_T}.
$$
Where does $\alpha_V^2 / \kappa_T$ come from? From multivariable calculus, the difference between heating at constant $P$ vs. constant $V$ is:
$$
C_{P,m} - C_{V,m} = T \underbrace{\left(\frac{\partial P}{\partial T}\right)\_V}_{\alpha_V / \kappa_T} \underbrace{\left(\frac{\partial V_m}{\partial T}\right)_P}\_{V_m \alpha_V} = V_m T \frac{\alpha_V^2}{\kappa_T}.
$$

| Substance | $\alpha_V / (10^{-4}\mathrm{K^{-1}})$ | $\kappa_T / (10^{-6}\mathrm{bar^{-1}})$ | $(\partial P/\partial T)\_V$ ($\mathrm{bar/K}$) | $C_{P,m} - C_{V,m}$ ($\mathrm{J/mol\\,K}$) |
|:---|---:|---:|---:|---:|
| **Benzene (l)** | $12.4$ | $92.1$ | $13.5$ | $44.5$ |
| **Water (l)** | $2.1$ | $49.6$ | $4.23$ | $0.48$ |
| **Lead (s)** | $0.861$ | $2.21$ | $39.0$ | $1.82$ |
| **Diamond (s)** | $0.030$ | $0.187$ | $1.60$ | $0.005$ |

---

# The Cyclic Rule Works on ANY Triple of State Functions

Because the equilibrium state surface of $1\text{ mol}$ of a pure phase is **2-dimensional**, *any* three state functions $(x, y, z)$ chosen from $\{P, V, T, U, H, S, G, F\}$ are linked by a constraint $f(x, y, z) = 0$ and obey $\left(\frac{\partial x}{\partial y}\right)_z\left(\frac{\partial y}{\partial z}\right)_x\left(\frac{\partial z}{\partial x}\right)_y = -1$:

| Physical Process | Triple $(x, y, z)$ | State Relation $f(x,y,z)=0$ | Cyclic-Rule Identity & Physical Meaning |
|:---|:---:|:---|:---|
| **1. Sealed-Vessel Heating** | $(P, V, T)$ | Mechanical EoS $P = P(T, V)$ | $\left(\dfrac{\partial P}{\partial T}\right)_V = -\dfrac{(\partial V/\partial T)_P}{(\partial V/\partial P)_T} = \dfrac{\alpha_V}{\kappa_T}$ *(thermal pressure spike)* |
| **2. Joule–Thomson Throttling** *(Gas Liquefaction)* | $(T, P, H)$ | Enthalpy surface $H = H(T, P)$ | $\mu_{\mathrm{JT}} = \left(\dfrac{\partial T}{\partial P}\right)_H = -\dfrac{(\partial H/\partial P)_T}{(\partial H/\partial T)_P} = -\dfrac{1}{C_P}\left(\dfrac{\partial H}{\partial P}\right)_T$ |
| **3. Joule Free Expansion** *(Into Vacuum, $U=\text{const}$)* | $(T, V, U)$ | Caloric EoS $U = U(T, V)$ | $\mu_{\mathrm{J}} = \left(\dfrac{\partial T}{\partial V}\right)_U = -\dfrac{(\partial U/\partial V)_T}{(\partial U/\partial T)_V} = -\dfrac{1}{C_V}\left(\dfrac{\partial U}{\partial V}\right)_T$ |
| **4. Acoustics & Sound Speed** | $(P, V, S)$ | Adiabatic EoS $P = P(V, S)$ | $\kappa_S = -\dfrac{1}{V}\left(\dfrac{\partial V}{\partial P}\right)_S = \dfrac{1}{V}\dfrac{(\partial S/\partial P)_V}{(\partial S/\partial V)_P}$ *(adiabatic compressibility)* |
| **5. Adiabatic Compression** *(Fire Syringe / Diesel)* | $(T, P, S)$ | Entropy surface $S = S(T, P)$ | $\left(\dfrac{\partial T}{\partial P}\right)_S = -\dfrac{(\partial S/\partial P)_T}{(\partial S/\partial T)_P} = \dfrac{TV\alpha_V}{C_P}$ *(temp. rise per bar)* |

---

<iframe src="./lecture_02_basics_of_thermodynamics/demos/cyclic-rule-pvt.html" width="100%" height="850px" style="border:1px solid #ccc; border-radius: 8px;"></iframe>

---

# Second Partial Derivatives & Critical Point Inflection

Just as in 1D calculus, differentiating a second time measures **curvature** (concavity). In a function of two variables $f(x, y)$, there are **two pure second derivatives** and **two mixed second derivatives**:

$$
\frac{\partial^2 f}{\partial x^2} = \left(\frac{\partial}{\partial x}\left(\frac{\partial f}{\partial x}\right)_y\right)_y, \qquad
\frac{\partial^2 f}{\partial y^2} = \left(\frac{\partial}{\partial y}\left(\frac{\partial f}{\partial y}\right)_x\right)_x, \qquad
\frac{\partial^2 f}{\partial y\\,\partial x} = \left(\frac{\partial}{\partial y}\left(\frac{\partial f}{\partial x}\right)_y\right)_x.
$$

:::matrix {cols="50/52"}
[[0,0]]
### Finding the Critical Point $(T_c, P_c, V_c)$ of a Real Gas
In Lecture 2 (Real Gases), we saw that below the critical temperature $T_c$, a van der Waals isotherm $P(V_m) = \frac{RT}{V_m - b} - \frac{a}{V_m^2}$ has an unphysical loop with a local minimum and local maximum where $\left(\frac{\partial P}{\partial V_m}\right)_T = 0$.

As $T \to T_c$, the minimum and maximum coalesce into a **horizontal inflection point**, where **both the first and second partial derivatives wrt $V_m$ vanish simultaneously**:
$$
\begin{aligned}
\left(\frac{\partial P}{\partial V_m}\right)\_{T_c} &= -\frac{RT_c}{(V_c - b)^2} + \frac{2a}{V_c^3} = 0, \\\\
\left(\frac{\partial^2 P}{\partial V_m^2}\right)_{T_c} &= +\frac{2RT_c}{(V_c - b)^3} - \frac{6a}{V_c^4} = 0.
\end{aligned}
$$

[[0,1]]
![](./lecture_02_basics_of_thermodynamics/images/addendum_vdw_critical.png){width=80% center}
Solving this $2\times 2$ algebraic system immediately yields:
$$
\mathbf{V_c = 3b, \qquad T_c = \frac{8a}{27Rb}, \qquad P_c = \frac{a}{27b^2}}.
$$
:::

---
# Mixed Partials & Exact ($dU$) vs. Inexact ($\delta Q, \delta A$) Differentials

Why did we write the First Law  as $dU = \delta Q + \delta A$ with a straight **$d$** for internal energy but a Greek **$\delta$** for heat and work?

:::matrix {cols="52/48"}
[[0,0]]
### Schwarz's Theorem & Euler's Exactness Test
For any smooth state function $f(x, y)$, **the order of mixed partial differentiation does not matter**:
$$
\frac{\partial}{\partial y}\left(\frac{\partial f}{\partial x}\right)_y = \frac{\partial}{\partial x}\left(\frac{\partial f}{\partial y}\right)_x.
$$
Consequently, a differential form $\omega = M(x, y)\\,dx + N(x, y)\\,dy$ is an **exact differential** $df$ of a path-independent state function $f$ if and only if its cross-derivatives match:
$$
\bbox[#e8f8f5, 10px, border-radius: 8px]{
\text{Exact } (df): \quad \left(\frac{\partial M}{\partial y}\right)_x = \left(\frac{\partial N}{\partial x}\right)_y \quad \Longleftrightarrow \quad \int_A^B df = f(B) - f(A)
}
$$

### Proof that Expansion Work $\delta A$ is Inexact:
Write reversible work for $1\text{ mol}$ of ideal gas in $(V, T)$ coordinates:
$$
\delta A = -P\\,dV + 0\\,dT = \underbrace{-\frac{RT}{V}}\_{M(V,T)} dV + \underbrace{0}\_{N(V,T)} dT.
$$

[[0,1]]
Test the cross-derivatives:
$$
\left(\frac{\partial M}{\partial T}\right)\_V = -\frac{R}{V} \neq 0 = \left(\frac{\partial N}{\partial V}\right)\_T \Longrightarrow \mathbf{\delta A \text{ is INEXACT!}}
$$
*(Bonus: Dividing $\delta Q_{\mathrm{rev}} = C_V dT + \frac{RT}{V}dV$ by the **integrating factor** $T$ makes cross-derivatives equal: $\frac{\partial (C_V/T)}{\partial V} = \frac{\partial (R/V)}{\partial T} = 0$, creating the state function **Entropy** $dS = \frac{\delta Q_{\mathrm{rev}}}{T}$!)*

![](./lecture_02_basics_of_thermodynamics/images/addendum_exact_vs_inexact.png){width=100% center}

:::

---

<iframe src="./lecture_02_basics_of_thermodynamics/demos/state-vs-path.html" width="100%" height="850px" style="border:1px solid #ccc; border-radius: 8px;"></iframe>

---
# Master Cheat Sheet: Core Rules of Manipulation

|#|Rule|Equation|
|---|---|---|
1.| **Freeze Rule:**| In $\left({\partial f}/{\partial x}\right)_y$, treat $y$ as a constant number.|
|2.|**Total Differential (Tangent Plane):**|$$ df = \left({\partial f}/{\partial x}\right)_y dx + \left({\partial f}/{\partial y}\right)_x dy $$|
|3.| **Inversion (Reciprocal) Rule** *(same subscript $z$!)*:|$$ \left(\frac{\partial x}{\partial y}\right)_z = \frac{1}{\left(\partial y/\partial x\right)_z} $$|
|4.| **Same-Subscript Chain Rule:**|$$    \left(\frac{\partial w}{\partial x}\right)_z = \left(\frac{\partial w}{\partial y}\right)_z \left(\frac{\partial y}{\partial x}\right)_z $$| 
|5.|**Cyclic (Triple Product) Rule** *(note the minus sign!)*:|$$ \left(\frac{\partial x}{\partial y}\right)_z \left(\frac{\partial y}{\partial z}\right)_x \left(\frac{\partial z}{\partial x}\right)_y = -1 \implies \left(\frac{\partial P}{\partial T}\right)_V = -\frac{(\partial V/\partial T)_P}{(\partial V/\partial P)_T} $$|
|6.| **Euler's Exactness & Maxwell Symmetry:**|$$ df = M\\,dx + N\\,dy \text{ is exact} \iff \left(\frac{\partial M}{\partial y}\right)_x = \left(\frac{\partial N}{\partial x}\right)_y $$|
   
---
# Key Partial Derivatives in Our Lectures

| Quantity | Definition | Ideal Gas Value |
|---|---|---|
| **Isobaric expansion $\alpha_V$** | $\dfrac{1}{V}\left(\dfrac{\partial V}{\partial T}\right)_P$ | $\dfrac{1}{T}$ |
| **Isothermal compressibility $\kappa_T$** | $-\dfrac{1}{V}\left(\dfrac{\partial V}{\partial P}\right)_T$ | $\dfrac{1}{P}$ |
| **Thermal pressure coeff. $\beta$** | $\left(\dfrac{\partial P}{\partial T}\right)_V = \dfrac{\alpha_V}{\kappa_T}$ | $\dfrac{P}{T} = \dfrac{nR}{V}$ |
| **Heat capacity at const. $V$** | $C_V = \left(\dfrac{\partial U}{\partial T}\right)_V$ | $\dfrac{3}{2}nR$ (monatomic) |
| **Heat capacity at const. $P$** | $C_P = \left(\dfrac{\partial H}{\partial T}\right)_P$ | $\dfrac{5}{2}nR$ (monatomic) |
| **Molar Gibbs pressure slope** | $\left(\dfrac{\partial G_m}{\partial P}\right)_T$ | $V_m = \dfrac{RT}{P} > 0$ |
| **Molar Gibbs temp. slope** | $\left(\dfrac{\partial G_m}{\partial T}\right)_P$ | $-S_m < 0$ |


---

# Down the Rabbit Hole I: Differential Topology

In modern **Differential Topology**, expressions like $dU$, $\delta Q$, and $\delta A$ are not "infinitesimally small numbers" — they are geometric objects called **Differential $1$-Forms** living in the **cotangent bundle** $T^*\mathcal{M}$:

:::matrix {cols="50/50"}
[[0,0]]
### 1. The Exterior Derivative $d$ and Why $d^2 = 0$
In exterior calculus, the operator $d$ turns a scalar field ($0$-form $f$) into a $1$-form $df = \frac{\partial f}{\partial x}dx + \frac{\partial f}{\partial y}dy$, and turns a $1$-form into an oriented **area $2$-form** using the antisymmetric **wedge product** ($dx \wedge dy = -dy \wedge dx$, $dx \wedge dx = 0$).

Apply $d$ **twice** to any smooth state function $U(T, V)$:
$$
d(dU) = \left(\frac{\partial^2 U}{\partial V\\,\partial T} - \frac{\partial^2 U}{\partial T\\,\partial V}\right) dV \wedge dT = 0 \Longleftrightarrow \mathbf{d^2 = 0!}
$$
- **Schwarz's symmetry of mixed partials** and **Euler's exactness test** are compressed into the single topological equation $\mathbf{d^2 = 0}$!
- By contrast, for an **inexact $1$-form** like reversible work $\delta A = -P\,dV$ or heat $\delta Q = T\,dS$, the exterior derivative does **not** vanish:
  $$
  d(\delta A) = -dP \wedge dV \neq 0, \qquad d(\delta Q) = dT \wedge dS \neq 0.
  $$

[[0,1]]
### 2. Generalized Stokes' Theorem on Manifolds
The fundamental theorem of calculus, Green's, Gauss's divergence, and Kelvin–Stokes' curl theorems are all special cases of one master equation for a $k$-form $\omega$ on a manifold $\Sigma$ with boundary $\partial \Sigma$:
$$
\bbox[#fff8e6, 12px, border-radius: 10px]{
\int_{\partial \Sigma} \omega = \int_{\Sigma} d\omega
}
$$
Apply Stokes' theorem to a thermodynamic heat-engine cycle $\mathcal{C} = \partial \Sigma$ bounding a 2D patch $\Sigma \subset \mathcal{M}$:
1. **First Law ($\omega = dU$):** $\oint_{\partial \Sigma} dU = \iint_{\Sigma} d^2 U = 0$.
2. **Carnot Area Invariance ($dU = T\,dS - P\,dV \implies d^2 U = dT\wedge dS - dP\wedge dV = 0$):**
   $$
   \oint_{\partial \Sigma} \delta Q_{\mathrm{rev}} = \iint_{\Sigma} dT \wedge dS = \iint_{\Sigma} dP \wedge dV = -\oint_{\partial \Sigma} \delta A_{\mathrm{rev}}.
   $$
   *The oriented area enclosed by ANY cycle in the $(S, T)$ plane is strictly equal to the area enclosed in the $(V, P)$ plane!*
:::

---
# Down the Rabbit Hole II: Differential Topology

Where else does this mathematical rabbit hole lead if you keep exploring?

:::matrix {cols="50/50"}
[[0,0]]
### 2. Contact Geometry ($\dim = 2n + 1$)
Why do thermodynamic variables always come in **conjugate pairs** $(T, S)$, $(-P, V)$, $(\mu_i, N_i)$ plus one energy $U$ — making full thermodynamic phase space **odd-dimensional** ($2n + 1 = 5$ for $(U, S, V, T, P)$)?
- In differential topology, the First & Second Laws define the **Gibbs contact $1$-form**:
  $$
  \theta = dU - T\,dS + P\,dV = 0.
  $$
- Because $\theta \wedge (d\theta)^2 \neq 0$, thermodynamic phase space is a **Contact Manifold** (the odd-dimensional cousin of Hamiltonian symplectic manifolds!).
- An equilibrium state surface $\mathcal{M}$ is a $2\mathrm{D}$ **Legendrian submanifold** on which $\theta|_{\mathcal{M}} = 0$, and switching from $U(S,V)$ to $G(T,P) = U - TS + PV$ is a **Legendre transformation** between contact charts!

[[0,1]]
### 3. Thermodynamic Riemannian Curvature
Can you define **distance** and **curvature** on a thermodynamic state surface?
- In fluctuation theory (Weinhold & Ruppeiner geometry), the matrix of **second partial derivatives** of entropy defines a **Riemannian metric tensor** $ds^2 = g_{ij}\,dX^i dX^j$:
  $$
  g_{ij} = -\frac{1}{k_B}\frac{\partial^2 S}{\partial X^i\,\partial X^j}.
  $$
- For an **ideal gas** (no intermolecular forces), the Riemann scalar curvature of state space is identically **$R = 0$ (flat Euclidean space!)**.
- For a **real interacting gas**, $R \neq 0$ measures intermolecular attractions vs. repulsions — and **$R$ diverges to $-\infty$ right at the Critical Point $(T_c, P_c, V_c)$**, just like spacetime curvature near a black hole singularity!
:::

---
1. For Dieterici's gas $P = \frac{nRT\,e^{-na/RTV}}{V-nb}$, what is $\left(\frac{\partial P}{\partial T}\right)_V$?
2. Why does $\oint dU = 0$ around a Carnot cycle while $\oint \delta A \neq 0$?
3. Using the Cyclic Rule, prove that $\left(\frac{\partial T}{\partial P}\right)_H = -\frac{1}{C_P}\left(\frac{\partial H}{\partial P}\right)_T$ (the Joule–Thomson coefficient!).


