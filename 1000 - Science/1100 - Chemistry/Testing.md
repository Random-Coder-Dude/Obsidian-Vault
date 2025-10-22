---
date: 2025-10-22T15:36
tags:
  - Chemistry
cssclasses:
  - default
---
# Quantum Wavefunctions: Complete Conceptual Study Guide

## Preface

This guide explains **quantum wavefunctions** from scratch, assuming **no prior knowledge** of physics, chemistry, or advanced mathematics.  
- Includes **units, reasoning, and step-by-step derivations**.  
- Designed to help you **conceptually understand and derive any wavefunction**.

---

# Part 1: Foundations

## 1.1 What is a wavefunction?

- A **wavefunction** $\psi(\mathbf{r}, t)$ is a mathematical function that describes the **quantum state** of a particle, such as an electron.  
- The **square of its magnitude** gives the **probability density** of finding the particle in space:

$$
|\psi|^2 = \text{probability density}
$$

- **Units**: In 3D space, $|\psi|^2$ has units of $\mathrm{m^{-3}}$ so that

$$
\int_{\text{all space}} |\psi|^2 dV = 1
$$

**Why:** The particle must exist somewhere, so the total probability is 1.

---

## 1.2 Time-Independent Schrödinger Equation (TISE)

For stationary states (time-independent systems):

$$
\hat{H} \psi = E \psi
$$

Where:

- $\hat{H}$ = Hamiltonian = total energy operator (kinetic + potential)  
- $E$ = energy eigenvalue  
- $\psi$ = wavefunction of stationary state  

**Conceptual Note:** Solving this equation gives **allowed energies** and **shapes of orbitals**.

---

### 1.2.1 Hamiltonian for a single particle

$$
\hat{H} = -\frac{\hbar^2}{2 m} \nabla^2 + V(\mathbf{r})
$$

- **Kinetic energy**: $-\frac{\hbar^2}{2 m} \nabla^2$  
- **Potential energy**: $V(\mathbf{r})$  

**Units check:**  
- $\hbar^2 / 2 m \sim \mathrm{J \cdot m^2 / kg} = \mathrm{J}$ ✅  

**Why:** The kinetic term measures how the wavefunction “curves” in space; the potential term depends on position.

---

## 1.3 Probability and Normalization

- Probability of finding particle in a volume $dV$:

$$
dP = |\psi(\mathbf{r})|^2 dV
$$

- Normalization condition:

$$
\int_{\text{all space}} |\psi|^2 dV = 1
$$

**Why:** Ensures the total probability of finding the particle somewhere in space is 1.

---

## 1.4 Dimensional Analysis

| Quantity | Symbol | Units | Explanation |
|----------|--------|-------|-------------|
| Wavefunction | $\psi$ | m$^{-3/2}$ | Normalized in 3D |
| Probability density | $|\psi|^2$ | m$^{-3}$ | Integrates to 1 |
| Position | $r$ | m | Distance from reference |
| Momentum | $p$ | kg·m/s | Mass × velocity |
| Energy | $E$ | J | Kinetic + potential energy |

---

# Part 2: Solving Wavefunctions in One Dimension

## 2.1 Infinite Square Well (1D Box)

- Particle confined between $x = 0$ and $x = L$  
- Potential:

$$
V(x) =
\begin{cases}
0 & 0 < x < L \\
\infty & \text{otherwise}
\end{cases}
$$

- Schrödinger equation:

$$
-\frac{\hbar^2}{2 m} \frac{d^2 \psi}{dx^2} = E \psi
$$

- Boundary conditions: $\psi(0) = \psi(L) = 0$  

**Solution**:

$$
\psi_n(x) = \sqrt{\frac{2}{L}} \sin\left(\frac{n \pi x}{L}\right), \quad n = 1,2,3,...
$$

- Energy levels:

$$
E_n = \frac{n^2 \pi^2 \hbar^2}{2 m L^2}
$$

**Why:** The wavefunction must vanish at infinite walls → sine solutions.

---

## 2.2 Free Particle

- Potential $V(x) = 0$ everywhere  
- Schrödinger equation:

$$
-\frac{\hbar^2}{2 m} \frac{d^2 \psi}{dx^2} = E \psi
$$

- Solution: plane waves  

$$
\psi(x) = A e^{ikx} + B e^{-ikx}, \quad k = \frac{\sqrt{2 m E}}{\hbar}
$$

- Concept: The particle is **completely delocalized**, uniform probability over space.

---

## 2.3 Harmonic Oscillator (1D)

- Potential:

$$
V(x) = \frac{1}{2} m \omega^2 x^2
$$

- Solutions involve **Hermite polynomials** $H_n(x)$:

$$
\psi_n(x) = \left(\frac{m \omega}{\pi \hbar}\right)^{1/4} \frac{1}{\sqrt{2^n n!}} H_n\left(\sqrt{\frac{m \omega}{\hbar}} x\right) e^{-m \omega x^2 / 2 \hbar}
$$

- Energy levels:  

$$
E_n = \hbar \omega \left(n + \frac{1}{2}\right)
$$

**Conceptual note:** Harmonic oscillator wavefunctions are **Gaussian-like shapes** modulated by polynomials.

---

# Part 3: Three-Dimensional Central Potentials

## 3.1 Spherical Coordinates

- Many systems are **radially symmetric**, e.g., atoms  
- Coordinates: $r$ (radius), $\theta$ (polar), $\phi$ (azimuthal)  

$$
dV = r^2 \sin\theta \, dr \, d\theta \, d\phi
$$

- Laplacian in spherical coordinates:

$$
\nabla^2 = \frac{1}{r^2} \frac{\partial}{\partial r} \left( r^2 \frac{\partial}{\partial r} \right) + \frac{1}{r^2 \sin\theta} \frac{\partial}{\partial \theta} \left( \sin\theta \frac{\partial}{\partial \theta} \right) + \frac{1}{r^2 \sin^2\theta} \frac{\partial^2}{\partial \phi^2}
$$

---

## 3.2 Hydrogen-like Atom

- Potential:

$$
V(r) = -\frac{Z e^2}{4 \pi \epsilon_0 r}
$$

- Separate variables:  

$$
\psi(r, \theta, \phi) = R(r) Y_\ell^m(\theta, \phi)
$$

- Radial equation:

$$
-\frac{\hbar^2}{2 \mu} \left( \frac{d^2 R}{dr^2} + \frac{2}{r} \frac{dR}{dr} - \frac{\ell(\ell+1)}{r^2} R \right) - \frac{Z e^2}{4 \pi \epsilon_0 r} R = E R
$$

- Angular part: **Spherical harmonics** $Y_\ell^m$  
- **Quantum numbers:** $n$, $\ell$, $m$  

---

## 3.3 Steps to Solve Any Orbital

1. Determine **$Z$**, the nuclear charge  
2. Include **reduced mass**:

$$
\mu = \frac{m_e M}{m_e + M}
$$

3. Solve **radial Schrödinger equation**  
4. Solve **angular Schrödinger equation** → $Y_\ell^m$  
5. Combine radial and angular parts:

$$
\psi_{n\ell m}(r, \theta, \phi) = R_{n\ell}(r) Y_\ell^m(\theta, \phi)
$$

6. Normalize the wavefunction:

$$
\int_0^\infty \int_0^\pi \int_0^{2\pi} |\psi_{n\ell m}(r,\theta,\phi)|^2 r^2 \sin\theta \, dr \, d\theta \, d\phi = 1
$$
