---
date: 2025-10-22T15:36
tags:
  - Chemistry
cssclasses:
  - default
---
# Quantum Mechanics Study Guide: Building Up to the Schrödinger Equation

## Part 0: Absolute Foundations — Concepts of Physics and Mathematics Needed

Before we even talk about electrons or wavefunctions, we need a firm foundation in **basic concepts**.

---

### 0.1 What is a Physical Quantity?

- A **physical quantity** is something measurable: e.g., length, mass, time, charge, energy.  
- Every physical quantity has a **unit**:

| Quantity | Symbol | SI Unit |
|----------|--------|---------|
| Length | $L$ | meter (m) |
| Mass | $M$ | kilogram (kg) |
| Time | $T$ | second (s) |
| Electric charge | $Q$ | coulomb (C) |
| Energy | $E$ | joule (J) |

**Dimensional analysis** allows us to check formulas: for example, energy $E$ has units of $ML^2T^{-2}$.

---

### 0.2 Vectors and Scalars

- **Scalars**: numbers with magnitude only (e.g., temperature, mass)  
- **Vectors**: numbers with magnitude **and direction** (e.g., position, velocity, force)  

- In 3D space, a vector $\mathbf{r}$ can be written as:

$$
\mathbf{r} = x \hat{i} + y \hat{j} + z \hat{k}
$$

- **Magnitude** of a vector:

$$
|\mathbf{r}| = \sqrt{x^2 + y^2 + z^2}
$$

- **Unit check:** Each component $x, y, z$ has units of meters → $|\mathbf{r}|$ also in meters ✅

**Why:** Electrons and other particles live in 3D space. We need vectors to describe their positions.

---

### 0.3 Motion in Space

- **Position vector:** $\mathbf{r}(t)$ describes where a particle is at time $t$  
- **Velocity:** $\mathbf{v} = \frac{d\mathbf{r}}{dt}$ → units m/s  
- **Acceleration:** $\mathbf{a} = \frac{d\mathbf{v}}{dt}$ → units m/s²  

- **Newton’s Second Law** (classical mechanics):

$$
\mathbf{F} = m \mathbf{a}
$$

- Units check: $[F] = kg \cdot m/s^2 = \text{newton (N)}$ ✅

**Why:** Before electrons, we understand classical particles — quantum particles generalize this.

---

### 0.4 Energy

- **Kinetic energy (motion):**

$$
KE = \frac{1}{2} m v^2
$$

- **Potential energy (position in a field):** depends on the force. Example: gravitational:

$$
PE = m g h
$$

- **Total energy:**

$$
E = KE + PE
$$

- Units: Joules (kg·m²/s²)

**Why:** In quantum mechanics, energy plays the same role, but it becomes an **operator**.

---

### 0.5 Waves

Electrons behave like **waves** as well as particles. To understand wavefunctions, we must first understand **waves mathematically**.

- **1D wave equation:**

$$
\frac{\partial^2 u}{\partial t^2} = c^2 \frac{\partial^2 u}{\partial x^2}
$$

Where:

- $u(x,t)$ = displacement at position $x$ and time $t$  
- $c$ = wave speed (m/s)  

- General solution:

$$
u(x,t) = f(x-ct) + g(x+ct)
$$

- Units check: $[u]$ = whatever the displacement unit is (e.g., meters) ✅  

**Conceptual note:** A wave carries energy and can interfere, like light, sound, or the quantum probability wave.

---

### 0.6 Complex Numbers

Quantum wavefunctions are **complex-valued**, meaning they involve $\mathbf{i} = \sqrt{-1}$.

- $z = a + i b$, $a, b$ real numbers  
- Magnitude: $|z| = \sqrt{a^2 + b^2}$  
- **Why:** Complex numbers allow **oscillations and phases** in quantum mechanics.

- **Euler’s formula:**

$$
e^{i \theta} = \cos\theta + i \sin\theta
$$

- Unit check: $\theta$ is dimensionless → $e^{i\theta}$ is dimensionless ✅

---

### 0.7 Partial Derivatives

- In multi-variable systems (like 3D space or space+time), we need **partial derivatives**:

$$
\frac{\partial f}{\partial x} \quad \text{means change in $f$ with $x$ keeping other variables constant}
$$

- Second derivative:

$$
\frac{\partial^2 f}{\partial x^2}
$$

- **Why:** Waves and quantum mechanics involve second derivatives in space and time (curvature of the wavefunction).

---

### 0.8 Introduction to Differential Equations

- Equations that involve derivatives are called **differential equations**.  

- Example: 1D wave equation:

$$
\frac{\partial^2 u}{\partial t^2} - c^2 \frac{\partial^2 u}{\partial x^2} = 0
$$

- **Why:** Schrödinger’s equation is a **partial differential equation (PDE)**.

---

### 0.9 Superposition Principle

- Waves can **add together**:

$$
u_{\text{total}} = u_1 + u_2
$$

- In quantum mechanics, **wavefunctions also obey superposition**:

$$
\psi_{\text{total}} = \psi_1 + \psi_2
$$

- Unit check: same as original wavefunction ✅

- **Why:** Key property for interference, which is fundamental in quantum mechanics.

---

### 0.10 Probability in Continuous Systems

- For a particle along a line (1D):

$$
\int_{-\infty}^{\infty} P(x) dx = 1
$$

- Probability density $P(x)$ units: m$^{-1}$ ✅  
- In 3D:

$$
\int |\psi(x,y,z)|^2 dV = 1
$$

- Units of $|\psi|^2$: m$^{-3}$ ✅

**Why:** Quantum mechanics deals with probabilities, not exact positions.

---

### Summary of Foundations (Part 0)

Before even writing Schrödinger’s equation, we have covered:

1. Basic units, dimensions, and physical quantities  
2. Scalars, vectors, and 3D space  
3. Motion, forces, and energy  
4. Waves, oscillations, and wave equations  
5. Complex numbers and Euler’s formula  
6. Partial derivatives and PDEs  
7. Superposition principle  
8. Probability densities and normalization  

**Next Step (Part 1):** We will start **connecting classical energy and wave concepts** to **quantum wavefunctions**, gradually building the Schrödinger equation from these foundations.
