---
date: 2025-10-16T21:44
tags:
  - Chemistry
  - "#StudyGuide"
cssclasses:
  - default
---
# 6.1
Light is a form of radiation
Light has two attributes its wavelength ($\lambda$) and its frequency ($\nu$)
Make sure you know $$c=\nu\lambda$$
$c$ is the speed of light
Also know the dimensional analysis shown below
## Example (6.11)
If a wave of light has a frequency of $6.01\cdot10^7s^{-1}$ what is its wavelength and which type of wave would this be most similar too?

First figure out what the question is asking
a) What is the wavelength ($\lambda$)
b) What type of radiation would this be

By applying the equation

$$c=\nu\lambda$$

Then plugging in values

$$\frac{3.00\cdot10^8(m)}{(s)}=\frac{6.01\cdot10^7}{s^{-1}}\cdot{\lambda(m)}$$

Then solving with basic algebra **You have bigger problems if you can't do this**

$$4.99(m)=\lambda(m)$$

**Remember Significant Figures**
You have solved part a, the wavelength is $4.99m$
Now to solve part b we look back at this image
![[Pasted image 20251012205244.png]]
Noticing where the wavelength and frequency line up on the graph we can conclude this radiation would be a radio wave

# 6.2
There were 3 big problems in chemistry at this time. 
1. Blackbody Problem
2. Photoelectric Effect
3. Emission Spectra

## Blackbody Problem
Basically scientists wanted to find an equation which related the temperature of a blackbody to the wavelength / frequency of the energy it emitted. 
However any attempts to do so always ended with an equation that asymptotes towards infinity (Not in the good way). It also didn't follow experimental results. 

## Photoelectric Effect
Scientists were looking to explain why bombarding a metal with light sometimes released electrons from the metal. It was an inequality where the metal would only release electrons if the frequency of the light was greater or lower than a value. 

## Planck's Constant
Eventually Planck solved both of these problems by saying energy is quantized and calculating the smallest "steps" energy. He then created a simple equation
$$E=h\nu$$

Where $h$ is Planck's constant. This law in conjunction with the relation between wavelength and frequency can be used to solve questions.

## Example (6.21)
If you had a metal that began to release electrons due to the photoelectric effect at $20kJ/mol$ of energy what would the minimum wavelength be required to trigger this effect?

First what are they asking
a) What is the wavelength of the radiation
Equation 1

$$\frac{c(m)}{(s)}=\lambda(m)\cdot\frac{\nu}{(s)}$$

Equation 2

$$E(J)=h(J\cdot s)\cdot\frac{\nu}{(s)}$$

Restructuring

$$\frac{c(m)}{s\lambda(m)}=\frac{\nu}{(s)}$$

Substitution

$$E(J)=h(J\cdot s)\cdot\frac{c(m)}{(s)\lambda(m)}$$

Plug in values

$$\frac{20kJ}{1mol}\cdot\frac{1000J}{1kJ}\cdot\frac{1mol}{6.02\cdot10^{23}photons}=6.63\cdot10^{-34}(J\cdot s)\cdot\frac{3.00\cdot10^8(m)}{(s)\lambda(m)}$$

Solve for $\lambda$
You should have gotten

$$6.0\cdot10^{-6}(m)=\lambda(m)$$

So our final answer is $6.0\cdot10^{-6}m$

# 6.3
## Emission Spectra
When looking at the gaseous state of an element through a spectrometer will form many colored bands in the view. Each one of these represent the wavelength of light the atom releases when it releases a photon due to moving to a lower energy state.
Rydberg noticed this and formed his equation
$$\Delta E(J)=\frac{R_H}{(m)}\left(\frac{1}{n_f^2}-\frac{1}{n_i^2}\right)$$

where $R_H$ is Rydberg's Constant
Also the energy $E$ can be modeled by 
$$E(J)=-h(J\cdot s)\cdot\frac{c(m)}{(s)}\cdot\frac{R_H}{(m)}\cdot\frac{1}{n^2}$$

Bohr this other scientist looked to improve the model of the atom.
Eventually he came up with Bohr's atomic theory which was wrong in certain aspects but eventually served as the base for idea to come.

## Bohr's 3 Postulates
1. Specific Orbits
	a. Electrons = ONLY orbits with certain radii and energies
2. Stable Energy States
	b. In an allowed orbit $\ce{->}$ electron DOES not lose energy or fall into the nucleus 
3. Energy Transitions
	c. Electrons emit or absorb photons when moving between orbits

Basically electrons only orbit around the nucleus in discrete orbitals. When they move between orbits they release of absorb photons. 

## Limitations
Major Limitations 
1. Fails for other atoms $\ce{->}$ cannot explain their spectra well
2. Avoids a key question: why doesn’t the electron fall into the nucleus?
3. Treats a electron like as a particle only 

# 6.4
De Broglie realized that electrons also behave like waves relating the two with his equation
$$\lambda(m)=\frac{h(J\cdot s)}{m(g)\cdot\frac{v(m)}{s}}$$

where the bottom term $mv$ is the momentum of the object
Adding on to these ideas there is the uncertainty law
$$\Delta x\cdot\Delta(mv)\ge\frac{h}{4\pi}$$
This equation tells us the maximum precision we could have based of either the $\Delta x$ precision or $\Delta(mv)$ precision
For small objects this matters (like an electron) but for larger objects the difference is small it doesn't matter.
Overall because we can't tell where an electron in an atom is the new atomic theory must explain where electrons are in the atom in terms of a probability cloud.

# 6.5
Welcome to quantum mechanics
Bohr assumes a circular or elliptical orbit around the atom however quantum mechanics represents electrons in terms of a cloud. 
There are electron shells 
And a principle quantum number ($n$)
Also there is angular momentum of the electron ($l$)
Also a magnetic quantum number ($m$)
The value of $n$ influences the possible values of $l$ and $m$ 

$$l(\# of)=n-1+1=n$$

Magnetic numbers

$$m(\#of)=-l\dots l=2n+1$$

Also values of $l$ represent different levels of orbitals

| $l$    | 0   | 1   | 2   | 3   |
| ------ | --- | --- | --- | --- |
| Letter | s   | p   | d   | f   |

The total number of orbitals in a shell is $n^2$ where $n$ corresponds to the energy level
Atom is in its ground state (Least energy state) vs Atom in an excited state (Any other state)

# 6.6
There are 4 types of orbitals dictated by the possible values of $l$ so use Aufbau Principle to fill in electrons and find an atoms ground state
![[Pasted image 20251017124941.png]]
Also make sure to know the shapes of all the orbitals
![[Pasted image 20251017125026.png]]
Higher energy orbitals are bigger in size.

# Misc. Parts
## PES (Photoelectron Spectroscopy)
**Photoelectron Spectroscopy** is a powerful technique which lets us find the relative energies of a electron in an atom
A PES spectrum looks something like this
![[Pasted image 20251018205437.png]]
Each peak in the image represents a subshell where the one with the highest binding energy is always the $1s$ orbital. By figuring out the relative numbers between the peaks we can experimentally figure out what atom the analyzed object is. In this case we can see 3 peaks which means 3 orbitals. 
Through Aufbau's principle we know it contains a $1s, 2s, 2p$ orbitals by seeing the relative heights we can clearly say that this atom has the electron config of $1s^22s^22p^4$ which is a spitting image of Oxygen
## eV (Electronvolt)
Just know the conversion factor for eV to J
$$1eV=1.602\cdot10^{-19}J$$
The nerdy explanation is that 1eV is equal to the amount of kinetic energy gained by a single electron when accelerating through an electrical potential difference of 1 volt in a vacuum

## Electron Spin (Box Notation)
Electrons can have 2 different types of spins
- $\frac{1}{2}$ 
- $-\frac{1}{2}$
Each orbital can hold a certain amount of positive spin electrons and a specific amount of negative spin electrons
Thankfully each orbital needs these pairs to be balanced
Now I will demonstrate how to do a box notation
Write the box notation for $O$ oxygen
First what is the electron config for oxygen
It is $1s^22s^22p^4$ now shorten this $[He]2s^22p^4$
So we need to draw boxes for the $2s^2$ and $2p^4$ orbitals
![[Pasted image 20251018211343.png]]
When drawing the boxes make sure to always draw all the up arrows first and then the down arrows (In each orbital). That way you follow Hund's rule
# Chapter 6 Practice Questions
## 6.1 — Light as a Form of Radiation

1. A beam of light has a frequency of $5.80 \times 10^{14}\,\mathrm{s^{-1}}$.  
   a) What is its wavelength?  
   b) What region of the electromagnetic spectrum does it belong to?  

2. A radio station broadcasts at $98.5\,\mathrm{MHz}$.  
   - Calculate the wavelength of the radio wave.  

3. If a certain ultraviolet ray has a wavelength of $2.40 \times 10^{-7}\,\mathrm{m}$, what is its frequency?  

4. As wavelength increases, what happens to frequency and energy? Explain why using the equation $c = \lambda \nu$.  

5. Which type of radiation has the shortest wavelength: infrared, visible, or ultraviolet?  

---

## 6.2 — Blackbody Problem, Photoelectric Effect, Planck’s Constant

6. Why did early blackbody radiation equations fail to match experimental data?  

7. What observation about the photoelectric effect could not be explained by classical physics?  

8. If a photon has a frequency of $7.25 \times 10^{14}\,\mathrm{s^{-1}}$, calculate its energy in joules.  

9. A metal requires a minimum energy of $3.00 \times 10^{-19}\,\mathrm{J}$ to eject an electron.  
   a) What is the threshold frequency?  
   b) What is the corresponding wavelength?  

10. Explain how Planck’s idea of quantized energy changed our understanding of light and matter.  

---

## 6.3 — Emission Spectra & Bohr Model

11. What causes the bright lines in an emission spectrum?  

12. Using Rydberg’s equation, calculate the energy difference when an electron in hydrogen moves from $n_i = 3$ to $n_f = 2$.  

13. Which Bohr postulate explains why electrons do not spiral into the nucleus?  

14. When an electron jumps from $n = 5$ to $n = 2$ in hydrogen, does it absorb or emit a photon? Explain.  

15. Name two major limitations of Bohr’s atomic model.  

---

## 6.4 — De Broglie & Heisenberg

16. Calculate the wavelength of an electron moving at $2.50 \times 10^6\,\mathrm{m/s}$ (electron mass $m_e = 9.11 \times 10^{-31}\,\mathrm{kg}$).  

17. Explain why the wave–particle duality of electrons was important in modern physics.  

18. What does the Heisenberg Uncertainty Principle say about measuring an electron’s position and momentum simultaneously?  

19. Why does uncertainty matter for electrons but not for macroscopic objects like baseballs?  

20. What does a “probability cloud” represent in quantum mechanics?  

---

## 6.5 — Quantum Numbers and Orbitals

21. List the four quantum numbers and what each represents.  

22. For $n = 3$,  
   a) What are the possible values of $l$?  
   b) What are the possible values of $m$ for each $l$?  

23. What shape corresponds to the $p$ orbital? To the $d$ orbital?  

24. How many orbitals exist in the $n = 4$ shell?  

25. Describe the difference between an atom in its ground state and one in an excited state.  

---

## 6.6 — Aufbau Principle and Orbital Filling

26. Write the electron configuration for:  
   a) Nitrogen (N)  
   b) Calcium (Ca)  
   c) Iron (Fe)  

27. Use the Aufbau principle to determine the ground-state configuration of phosphorus.  

28. Draw the box notation for carbon and label the spin of each electron.  

29. What rule tells you to fill each orbital with one electron before pairing them?  

30. Which orbital ($2p$ or $3s$) has higher energy? Explain.  

---

## Miscellaneous Topics

31. What information does a PES (Photoelectron Spectroscopy) spectrum give about an atom?  

32. In a PES spectrum, which orbital always appears at the highest binding energy?  

33. The conversion factor between joules and electronvolts is $1\,\mathrm{eV} = 1.602 \times 10^{-19}\,\mathrm{J}$.  
   a) Convert $5.00 \times 10^{-19}\,\mathrm{J}$ into eV.  
   b) Convert $12.0\,\mathrm{eV}$ into joules.  

34. Define electron spin and explain why each orbital can hold only two electrons.  

35. Based on the PES spectrum showing peaks for $1s$, $2s$, and $2p$ orbitals, which element could it represent?  

---

## Challenge Problems

36. A photon has a wavelength of $4.50 \times 10^{-7}\,\mathrm{m}$.  
   - Find its frequency and energy.  

37. Using the Rydberg equation, calculate the wavelength of light emitted when an electron in hydrogen moves from $n = 4$ to $n = 2$.  

38. The work function of a certain metal is $2.20\,\mathrm{eV}$. What wavelength of light is just sufficient to eject electrons from the surface?  

39. Determine all possible sets of quantum numbers $(n, l, m)$ for the $3p$ subshell.  

40. Explain how the ideas of Planck, Einstein, Bohr, De Broglie, and Heisenberg each contributed to quantum theory.  

---

# Answer Key

### 6.1
1. $\lambda = \frac{c}{\nu} = \frac{3.00 \times 10^8}{5.80 \times 10^{14}} \approx 5.17 \times 10^{-7}\,\mathrm{m}$ → Visible  
2. $\lambda = \frac{c}{\nu} = \frac{3.00 \times 10^8}{9.85 \times 10^7} \approx 3.05\,\mathrm{m}$ → Radio  
3. $\nu = \frac{c}{\lambda} = \frac{3.00 \times 10^8}{2.40 \times 10^{-7}} \approx 1.25 \times 10^{15}\,\mathrm{s^{-1}}$ → Ultraviolet  
4. As $\lambda$ increases, $\nu$ decreases, so $E = h\nu$ decreases.  
5. Ultraviolet  

### 6.2
6. Classical blackbody radiation predicted infinite energy at short wavelengths (“ultraviolet catastrophe”).  
7. Photoelectric effect occurs only above a threshold frequency; classical theory predicted intensity mattered, not frequency.  
8. $E = h\nu = (6.63 \times 10^{-34})(7.25 \times 10^{14}) \approx 4.80 \times 10^{-19}\,\mathrm{J}$  
9. $\nu_\text{threshold} = \frac{E}{h} \approx 4.53 \times 10^{14}\,\mathrm{s^{-1}}$, $\lambda_\text{threshold} = \frac{c}{\nu} \approx 6.62 \times 10^{-7}\,\mathrm{m}$  
10. Energy is quantized; light interacts as photons, solving blackbody and photoelectric problems.  

### 6.3
11. Electrons dropping to lower energy levels emit photons at specific wavelengths.  
12. $\Delta E = R_H \left(\frac{1}{2^2} - \frac{1}{3^2}\right) hc \approx 1.89 \times 10^{-18}\,\mathrm{J}$  
13. Bohr’s 2nd postulate (Stable Energy States)  
14. Emit photon  
15. Fails for multi-electron atoms; does not explain why electrons don’t collapse  

### 6.4
16. $\lambda = \frac{h}{mv} \approx 2.90 \times 10^{-10}\,\mathrm{m}$  
17. Electrons behave as both particles and waves → quantum mechanics  
18. $\Delta x \cdot \Delta p \ge \frac{h}{4\pi}$  
19. Large mass → $\Delta p$ negligible, macroscopic objects unaffected  
20. Probability distribution of electron positions  

### 6.5
21. $n$ = principal, $l$ = angular, $m$ = magnetic, $s$ = spin  
22. a) $l = 0,1,2$ b) $m = -l,\dots,+l$  
23. $p$ → dumbbell, $d$ → clover  
24. $n^2 = 16$ orbitals  
25. Ground = lowest energy, Excited = higher energy  

### 6.6
26. a) $1s^2 2s^2 2p^3$ b) $[Ar]4s^2$ c) $[Ar]4s^2 3d^6$  
27. $[Ne]3s^2 3p^3$  
28. Box notation: $1s \uparrow\downarrow, 2s \uparrow\downarrow, 2p \uparrow \uparrow \uparrow$  
29. Hund’s rule  
30. $3s$ higher than $2p$ → higher principal quantum number  

### Misc
31. Binding energies of electrons/subshells  
32. $1s$ orbital  
33. a) $5.00\times10^{-19}\,\mathrm{J}/1.602\times10^{-19}\approx3.12\,\mathrm{eV}$  
    b) $12\,\mathrm{eV}\times1.602\times10^{-19}\approx1.92\times10^{-18}\,\mathrm{J}$  
34. Spin = $\pm \frac{1}{2}$; 2 electrons per orbital (Pauli exclusion)  
35. Oxygen ($[He]2s^2 2p^4$)  

### Challenge
36. $\nu = c/\lambda \approx 6.67 \times 10^{14}\,\mathrm{s^{-1}}, E = h\nu \approx 4.42 \times 10^{-19}\,\mathrm{J}$  
37. $\lambda \approx 486\,\mathrm{nm}$  
38. $\lambda = \frac{hc}{E} \approx 564\,\mathrm{nm}$  
39. $n=3, l=1 \Rightarrow m=-1,0,1$ → 3 orbitals → 6 electrons possible  
40. Planck: quantized energy; Einstein: photons; Bohr: energy levels; De Broglie: matter waves; Heisenberg: uncertainty  