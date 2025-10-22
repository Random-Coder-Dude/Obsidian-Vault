---
date: 2025-10-22T15:36
tags:
  - Chemistry
cssclasses:
  - default
---
# Exact 3s Orbital Probability Density for Sulfur (Including Reduced Mass)

We want to calculate the **radial probability density** \(P_{3s}(r)\) of an electron in the **3s orbital of sulfur**. This is done using the **Schrödinger equation** with full **reduced-mass correction**, step by step.

---

## Step 0: What we are doing

- The electron is attracted to the nucleus by the **Coulomb force**.
- Quantum mechanics says we **cannot know the exact position**, instead we compute a **wavefunction** $\(\psi(r,\theta,\phi)\).
- The probability of finding the electron in a spherical shell of radius \(r\) and thickness \(dr\) is:

$$
dP = |\psi(r,\theta,\phi)|^2 \, dV
$$

where

$$
dV = r^2 \sin\theta \, dr \, d\theta \, d\phi.
$$

---

## Step 1: Schrödinger Equation

The **time-independent Schrödinger equation**:

$$
\hat{H} \psi = E \psi
$$

with Hamiltonian:

$$
\hat{H} = -\frac{\hbar^2}{2 \mu} \nabla^2 - \frac{Z e^2}{4 \pi \epsilon_0 r}
$$

- \(\hbar = 1.0545718 \times 10^{-34}\ \mathrm{J \, s}\)  
- \(\mu\) = reduced mass of electron-nucleus system  
- \(Z = 16\) for sulfur  
- \(e = 1.602176634 \times 10^{-19}\ \mathrm{C}\)  
- \(\epsilon_0 = 8.854187817 \times 10^{-12}\ \mathrm{C^2/(N \, m^2)}\)  
- \(r\) = distance from nucleus (\(\mathrm{m}\))  

### Step 1a: Reduced mass

$$
\mu = \frac{m_e M}{m_e + M}
$$

- \(m_e = 9.109 \times 10^{-31}\ \mathrm{kg}\)  
- \(M = 31.972 \times 1.66054 \times 10^{-27}\ \mathrm{kg} \approx 5.31 \times 10^{-26}\ \mathrm{kg}\)  

$$
\mu \approx \frac{9.109 \times 10^{-31} \cdot 5.31 \times 10^{-26}}{9.109 \times 10^{-31} + 5.31 \times 10^{-26}} \approx 9.097 \times 10^{-31}\ \mathrm{kg}
$$

**Dimensional check:** \([\mu] = \mathrm{kg}\) ✅

**Why?** The reduced mass accounts for the motion of the nucleus, giving more accurate energy levels.

---

## Step 2: Schrödinger Equation in Spherical Coordinates

Since the potential depends only on \(r\), use **spherical coordinates** \(r, \theta, \phi\):

$$
\nabla^2 = \frac{1}{r^2} \frac{\partial}{\partial r}\Big(r^2 \frac{\partial}{\partial r}\Big) + \frac{1}{r^2 \sin\theta} \frac{\partial}{\partial \theta} \Big(\sin\theta \frac{\partial}{\partial \theta}\Big) + \frac{1}{r^2 \sin^2\theta} \frac{\partial^2}{\partial \phi^2}
$$

Assume **separation of variables**:

$$
\psi(r,\theta,\phi) = R(r) \, Y_\ell^m(\theta,\phi)
$$

- \(R(r)\) = radial function  
- \(Y_\ell^m(\theta,\phi)\) = spherical harmonics (angular part)  

For **s-orbitals** (\(\ell = 0\)):

$$
Y_0^0(\theta,\phi) = \frac{1}{\sqrt{4 \pi}} \quad (\text{dimensionless})
$$

**Why?** Separation simplifies the 3D problem into radial and angular parts.

---

## Step 3: Radial Schrödinger Equation

$$
-\frac{\hbar^2}{2 \mu} \left( \frac{d^2 R}{dr^2} + \frac{2}{r} \frac{d R}{dr} \right) - \frac{Z e^2}{4 \pi \epsilon_0 r} R = E R
$$

- Units: \([R] = \mathrm{m^{-3/2}}\) to satisfy normalization: \(\int |\psi|^2 dV = 1\)

### Step 3a: Substitution \(u(r) = r R(r)\)

$$
-\frac{\hbar^2}{2 \mu} \frac{d^2 u}{dr^2} - \frac{Z e^2}{4 \pi \epsilon_0 r} u = E u
$$

- \(u(r)\) units: \(\mathrm{m^{-1/2}}\) ✅  
- **Why?** Converts to a 1D-like problem, easier to solve analytically.

---

## Step 4: Hydrogen-like Solution (with Reduced Mass)

$$
R_{n\ell}(r) = \sqrt{\left(\frac{2 Z}{n a_\mu}\right)^3 \frac{(n-\ell-1)!}{2 n [(n+\ell)!]}} \, e^{-\rho/2} \, \rho^\ell \, L_{n-\ell-1}^{2\ell+1}(\rho)
$$

- \(\rho = \frac{2 Z r}{n a_\mu}\) – dimensionless  
- \(a_\mu = \frac{4 \pi \epsilon_0 \hbar^2}{\mu e^2}\) – Bohr radius with reduced mass  
- \(L_{n-\ell-1}^{2\ell+1}(\rho)\) – associated Laguerre polynomial (dimensionless)  

Units:

- \(a_\mu\): meters ✅  
- \(R(r)\): \(\mathrm{m^{-3/2}}\) ✅  
- \(\rho\): dimensionless ✅  

---

## Step 5: Reduced-mass Bohr Radius for Sulfur

$$
a_\mu = \frac{4 \pi \epsilon_0 \hbar^2}{\mu e^2} \approx 5.315 \times 10^{-11}\ \mathrm{m}
$$

- Slightly smaller than \(a_0 = 0.529177 \times 10^{-10}\ \mathrm{m}\)  
- Includes **nuclear motion**  

---

## Step 6: 3s Orbital for Sulfur

- \(n = 3\), \(\ell = 0\), \(Z = 16\)  

$$
\rho = \frac{2 Z r}{n a_\mu} = \frac{32 r}{3 a_\mu}
$$

$$
R_{3s}(r) = \frac{2}{81 \sqrt{3}} \left(\frac{16}{a_\mu}\right)^{3/2} \left( 27 - 18 \rho + 2 \rho^2 \right) e^{-\rho/2}
$$

Substitute \(\rho = 32 r / 3 a_\mu\):

$$
\boxed{
R_{3s}(r) = \frac{2}{81 \sqrt{3}} \left(\frac{16}{a_\mu}\right)^{3/2} \left( 27 - 192 \frac{r}{a_\mu} + \frac{2048}{9} \frac{r^2}{a_\mu^2} \right) e^{-16 r / 3 a_\mu}
}
$$

- Units check: \(R_{3s} \sim \mathrm{m^{-3/2}}\) ✅  

---

## Step 7: Radial Probability Density

$$
P_{3s}(r) = r^2 |R_{3s}(r)|^2
$$

- Units: \(r^2: \mathrm{m^2}\), \(R^2: \mathrm{m^{-3}}\), so \(P_{3s} \sim \mathrm{m^{-1}}\) ✅  
- Normalization: \(\int_0^\infty P_{3s}(r) dr = 1\)

---

## Step 8: Explicit Radial Probability Density for Sulfur 3s

$$
\boxed{
P_{3s}(r) = r^2 \left[ \frac{2}{81 \sqrt{3}} \left(\frac{16}{a_\mu}\right)^{3/2} \left( 27 - 192 \frac{r}{a_\mu} + \frac{2048}{9} \frac{r^2}{a_\mu^2} \right) e^{-16 r / 3 a_\mu} \right]^2
}
$$

- Fully exact **including reduced mass**  
- Units: \(\mathrm{m^{-1}}\)  
- Can be plotted to show the radial distribution of the electron in the 3s orbital.

---

## Step 9: Dimensional Summary

| Quantity | Symbol | Units | Notes |
|----------|--------|-------|-------|
| Radial distance | r | m | distance from nucleus |
| Reduced mass | μ | kg | μ = m_e M / (m_e + M) |
| Planck constant | ℏ | J·s | kinetic term |
| Elementary charge | e | C | potential term |
| Permittivity | ε₀ | C²/(N·m²) | Coulomb law |
| Radial wavefunction | R(r) | m^{-3/2} | normalized |
| Radial probability density | P(r) | m^{-1} | ∫ P(r) dr = 1 |
| Dimensionless radius | ρ | — | ρ = 2 Z r / n a_μ |
