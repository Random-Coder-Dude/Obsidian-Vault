---
date: 2025-10-22T15:36
tags:
  - Chemistry
cssclasses:
  - default
---
# Detailed Explanation of the 3s Orbital of Sulfur (Quantum Chemistry, No Approximations)

We want to find the **exact probability distribution** of an electron in the **3s orbital of sulfur**, including **reduced mass correction** and all physical constants. This will involve **quantum mechanics, math, and dimensional analysis**, explained in detail.

---

## Step 0: What is an orbital?

- Electrons are **tiny negatively charged particles** that orbit a nucleus (protons + neutrons) in an atom.
- We **cannot know exactly where an electron is** due to quantum mechanics. Instead, we describe **where it is likely to be** using a **wavefunction**, denoted ($\psi$).
- The **wavefunction** is a mathematical function of position, ($\psi(x,y,z)$) or ($\psi(r,\theta,\phi)$). Its **square** gives the **probability density** of finding the electron somewhere:

$$
|\psi|^2 = \text{probability density}
$$

- Units of \(|\psi|^2\) must make sense so that **integrating over all space gives 1**, meaning the electron must exist somewhere.

- The **3s orbital** is a “spherical shell” around the nucleus with **n = 3** energy level and **s-type (spherical) shape**.

---

## Step 1: Schrödinger Equation

The **Schrödinger equation** is the foundation of quantum mechanics. It’s like **Newton’s laws**, but for tiny particles:

$$
\hat{H} \psi = E \psi
$$

Where:

- \(\hat{H}\) = Hamiltonian = total energy operator (kinetic + potential energy)  
- \(\psi\) = wavefunction of the electron  
- \(E\) = total energy of the electron  

**Why this is important:** Solving this equation tells us **allowed energies and shapes of orbitals**.

---

### Step 1a: Hamiltonian for a hydrogen-like atom

For a single electron around a nucleus:

$$
\hat{H} = -\frac{\hbar^2}{2 \mu} \nabla^2 - \frac{Z e^2}{4 \pi \epsilon_0 r}
$$

Breakdown:

1. **Kinetic Energy Term:** \(-\frac{\hbar^2}{2 \mu} \nabla^2\)  

- \(\hbar\) = reduced Planck constant, a tiny number (\(1.0545718 \times 10^{-34}\ \mathrm{J\cdot s}\))  
- \(\nabla^2\) = Laplacian = second derivative in space (measures how the wavefunction curves)  
- \(\mu\) = reduced mass (explained below)  
- Units check: \(\hbar^2 / 2\mu \sim \mathrm{J \cdot m^2 / kg} = \mathrm{J}\), same as energy ✅  

2. **Potential Energy Term:** \(-\frac{Z e^2}{4 \pi \epsilon_0 r}\)  

- \(Z\) = number of protons (16 for sulfur)  
- \(e\) = elementary charge (\(1.602 \times 10^{-19}\ \mathrm{C}\))  
- \(\epsilon_0\) = permittivity of free space (\(8.854 \times 10^{-12} \mathrm{C^2/(N\cdot m^2)}\))  
- \(r\) = distance from nucleus (m)  
- Units check: \(e^2 / 4\pi\epsilon_0 r \sim \mathrm{J}\) ✅  

**Why the minus sign?** The electron is **attracted** to the nucleus, so potential energy is negative.

---

### Step 1b: Reduced mass \(\mu\)

- In real life, the nucleus is **not infinitely heavy**. Both electron and nucleus move slightly.  
- The **reduced mass** accounts for this:

$$
\mu = \frac{m_e M}{m_e + M}
$$

Where:

- \(m_e\) = electron mass (\(9.109 \times 10^{-31}\ \mathrm{kg}\))  
- \(M\) = sulfur nucleus mass (\(\approx 5.31 \times 10^{-26}\ \mathrm{kg}\))  

$$
\mu \approx 9.097 \times 10^{-31}\ \mathrm{kg}
$$

- Units: kg ✅  
- **Why important:** Gives slightly smaller Bohr radius → more accurate orbital.

---

## Step 2: Spherical coordinates

- The potential depends **only on distance \(r\)** from the nucleus.  
- Use **spherical coordinates**: \(r\) (radius), \(\theta\) (angle from z-axis), \(\phi\) (angle around z-axis).  
- Volume element in spherical coordinates:

$$
dV = r^2 \sin\theta \, dr \, d\theta \, d\phi
$$

- Probability of finding electron in shell of thickness \(dr\):

$$
dP = |\psi|^2 \, dV
$$

- **Why:** Integrals over volume must give total probability = 1.

---

## Step 3: Separate radial and angular parts

$$
\psi(r,\theta,\phi) = R(r) Y_\ell^m(\theta,\phi)
$$

- \(R(r)\) = radial function (how electron depends on distance)  
- \(Y_\ell^m(\theta,\phi)\) = angular part (shape)  

- For **s-orbitals**, \(\ell = 0\):  

$$
Y_0^0(\theta,\phi) = \frac{1}{\sqrt{4\pi}}
$$

- Dimensionless, just normalization.  

**Why:** Makes equation solvable. Now we focus on \(R(r)\).

---

## Step 4: Radial Schrödinger Equation

$$
-\frac{\hbar^2}{2\mu} \left( \frac{d^2 R}{dr^2} + \frac{2}{r} \frac{dR}{dr} \right) - \frac{Z e^2}{4 \pi \epsilon_0 r} R = E R
$$

- Units check: \(\hbar^2 / 2\mu \cdot d^2/dr^2 \sim J\) ✅  
- \(R(r)\) units: \(\mathrm{m^{-3/2}}\) to satisfy \(\int |\psi|^2 dV = 1\) ✅  

### Step 4a: Substitution \(u(r) = r R(r)\)

$$
-\frac{\hbar^2}{2\mu} \frac{d^2 u}{dr^2} - \frac{Z e^2}{4 \pi \epsilon_0 r} u = E u
$$

- \(u(r)\) units: \(\mathrm{m^{-1/2}}\) ✅  
- **Why:** Converts 3D radial equation to simpler 1D form.

---

## Step 5: Hydrogen-like solution

The **general solution** for hydrogen-like atoms:

$$
R_{n\ell}(r) = \sqrt{\left(\frac{2 Z}{n a_\mu}\right)^3 \frac{(n-\ell-1)!}{2n [(n+\ell)!]}} \, e^{-\rho/2} \, \rho^\ell \, L_{n-\ell-1}^{2\ell+1}(\rho)
$$

- \(\rho = \frac{2 Z r}{n a_\mu}\) dimensionless  
- \(a_\mu = \frac{4 \pi \epsilon_0 \hbar^2}{\mu e^2}\) = Bohr radius with reduced mass  

**Check units:**  

- \(a_\mu\) → meters ✅  
- \(R(r)\) → m^{-3/2} ✅  
- \(\rho\) → dimensionless ✅  

---

## Step 6: Bohr radius with reduced mass for sulfur

$$
a_\mu = \frac{4 \pi \epsilon_0 \hbar^2}{\mu e^2} \approx 5.315 \times 10^{-11}\ \mathrm{m}
$$

- Slightly smaller than the standard Bohr radius because nucleus moves slightly.

---

## Step 7: 3s orbital for sulfur

- \(n = 3, \ell = 0, Z = 16\)  

$$
\rho = \frac{2 Z r}{n a_\mu} = \frac{32 r}{3 a_\mu}
$$

$$
R_{3s}(r) = \frac{2}{81 \sqrt{3}} \left( \frac{16}{a_\mu} \right)^{3/2} \left( 27 - 18 \rho + 2 \rho^2 \right) e^{-\rho/2}
$$

Substitute \(\rho = 32 r / 3 a_\mu\):

$$
\boxed{
R_{3s}(r) = \frac{2}{81 \sqrt{3}} \left( \frac{16}{a_\mu} \right)^{3/2} \left( 27 - 192 \frac{r}{a_\mu} + \frac{2048}{9} \frac{r^2}{a_\mu^2} \right) e^{-16 r / 3 a_\mu}
}
$$

- Units: m^{-3/2} ✅  

---

## Step 8: Radial probability density

$$
P_{3s}(r) = r^2 |R_{3s}(r)|^2
$$

- Units: \(r^2 \sim m^2\), \(R^2 \sim m^{-3}\), so \(P(r) \sim m^{-1}\) ✅  
- Integral over all r: \(\int_0^\infty P_{3s}(r) dr = 1\) (electron must exist somewhere)  

Explicit formula:

$$
\boxed{
P_{3s}(r) = r^2 \left[ \frac{2}{81 \sqrt{3}} \left(\frac{16}{a_\mu}\right)^{3/2} \left( 27 - 192 \frac{r}{a_\mu} + \frac{2048}{9} \frac{r^2}{a_\mu^2} \right) e^{-16 r / 3 a_\mu} \right]^2
}
$$

---

## Step 9: Summary of all units (dimensional analysis)

| Quantity | Symbol | Units | Explanation |
|----------|--------|-------|-------------|
| Distance from nucleus | r | m | Radius |
| Reduced mass | μ | kg | μ = m_e M / (m_e + M) |
| Planck constant | ℏ | J·s | Kinetic energy factor |
| Electron charge | e | C | Potential energy factor |
| Permittivity | ε₀ | C²/(N·m²) | Coulomb law |
| Radial wavefunction | R(r) | m^{-3/2} | Normalization ensures total probability = 1 |
| Radial probability | P(r) | m^{-1} | Probability density for radial shell |
| Dimensionless radius | ρ | — | ρ = 2 Z r / n a_μ |
