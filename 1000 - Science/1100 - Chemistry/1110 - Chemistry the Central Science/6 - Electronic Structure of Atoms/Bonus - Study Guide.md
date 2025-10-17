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
Eventually Planck solved both of these problems by saying energy is quantized and calculating the smallest "steps" energy. He then created a simple equation$$E=h\nu$$
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
Rydberg noticed this and formed his equation$$\Delta E(J)=\frac{R_H}{(m)}\left(\frac{1}{n_f^2}-\frac{1}{n_i^2}\right)$$
where $R_H$ is Rydberg's Constant
Also the energy $E$ can be modeled by $$E(J)=-h(J\cdot s)\cdot\frac{c(m)}{(s)}\cdot\frac{R_H}{(m)}\cdot\frac{1}{n^2}$$
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
De Broglie realized that electrons also behave like waves relating the two with his equation$$\lambda(m)=\frac{h(J\cdot s)}{m(g)\cdot\frac{v(m)}{s}}$$
where the bottom term $mv$ is the momentum of the object
Adding on to these ideas there is the uncertainty law$$\Delta x\cdot\Delta(mv)\ge\frac{h}{4\pi}$$ This equation tells us the maximum precision we could have based of either the $\Delta x$ precision or $\Delta(mv)$ precision
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
