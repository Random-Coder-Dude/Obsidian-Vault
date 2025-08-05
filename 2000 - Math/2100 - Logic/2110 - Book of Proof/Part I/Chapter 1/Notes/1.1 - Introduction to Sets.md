---
date: 2025-08-03T13:12
tags:
  - Logic
cssclasses:
  - default
---
All of math can be described in sets. This affect is more noticeable at higher levels of math. The language of sets is perfect in describing math

# Introduction to Sets
A **set** is a collection of things
Each of those things is called an **element** of the set
We are mainly concerned with sets whose elements are mathematical entities such as numbers, points and functions
A set is expressed in the following way $\set{2,4,6,8}$ this is called a **finite set** because it doesn't have infinite elements. Conversely a set that contains all integers would be a **infinite set** and would be written as $\set{...,-4,-3,-2,-1,0,1,2,3,4,...}$
Here the dots indicate a pattern which continues in both directions
Two sets are **equal** if they contain exactly the same elements. For example the sets $\set{2,4,6,8}=\set{2,4,8,6}$ are equal. Even if the order of elements are shifted. Similarly two sets would be **unequal** if all of their elements do not match. For example $\set{2,4,6,8}\ne\set{2,4,6,7}$ 
We usually call sets by a capital letter such as $A=\set{2,4,6,8}$ we can now $2\in A$ where it means 2 is a member of set A. The converse is also a symbol where $5\notin A$, meaning 5 is not a member of set A. This symbols can also be used as follows $2,4\in A$ as well as $5,7\notin A$ mean what you would expect them to mean.
Some sets are so important they have symbols reserved for them
$$\begin{align}
\mathbb{N}&=\set{1,2,3,4,5,6,7,...}\text{ The set of natural numbers} \\
\mathbb{Z}&=\set{...,-3,-2,-1,0,1,2,3,4,...}\text{ The set of integers} \\
\mathbb{R}&=\text{ The set of all real numbers}
\end{align}$$
One important note is that sets do not need to have numbers, a set can contain anything even other sets.
If $X$ is a finite set it has a property called **cardinality** which is a fancy word for size. It is denoted by $|X|$ Thus the set $A$ has a cardinality of 4 denoted as $|A|=4$. There is another special set which plays a bug role it is called the empty set and is defined as $\emptyset=\set{}$. This is the only set which has the property $|\emptyset|=0$. However be careful because $\set{\emptyset}\ne\emptyset$, the set $|\set{\emptyset}|=1$ in other words it is like an empty box vs a box with an empty box inside. Obviously different.
There is another notation for sets called **set-builder notation** it allows us to describe really big and complex sets easily. Here is an example $E=\set{2n:n\in\mathbb{Z}}$. This is the same thing as the infinite set of even integers, written normally as $\set{...,-6,-4,-2,0,2,4,6,...}$. We read the first brace as *the set of all thing of form* and the colon as *such that*. This leads to the expression for set $E$ meaning *E equals the set of all things of form $2n$, such that $n$ is an element of $\mathbb{Z}$*. In general the form for set-builder notation is $$X=\set{\text{expression}:\text{rule}}$$
As you get used to this notation it gets a lot easier to understand and follow here are some examples
$$\begin{align}
&1.\quad\set{n:n\text{ is a prime number}}=\set{2,3,5,7,11,13,17,...} \\
&2.\quad\set{n\in\mathbb{N}:n\text{ is prime}}=\set{2,3,5,7,11,13,17,...} \\
&3.\quad\set{n^2:n\in\mathbb{Z}}=\set{0,1,4,9,16,25,...} \\
&4.\quad\set{x\in\mathbb{R}:x^2-2=0}=\set{\sqrt{2},-\sqrt{2}} \\
&5.\quad\set{x\in\mathbb{Z}:x^2-2=0}=\emptyset \\
&6.\quad\set{x\in\mathbb{Z}:|x|\lt4}=\set{-3,-2,-1,0,1,2,3} \\
&7.\quad\set{2x:x\in\mathbb{Z},|x|\lt4}=\set{-6,-4,-2,0,2,4,6} \\
&8.\quad\set{x\in\mathbb{Z}:|2x|\lt4}=\set{-1,0,1} \\
\end{align}$$
Example 1.2
$A=\set{7a+3b:a,b\in\mathbb{Z}}$.
The set contains all of the numbers with form $7a+3b$ where $a$ and $b$ are integers. This means that if $n$ is any integer than $n=7n+3n(-2n)$ Aka $n=7n-6n$ so $n=7a+3b$ when $a=n$ and $b=-2n$. Therefore $n\in A$. Because $n$ is any integer $A=\mathbb{Z}$. 
To reiterate the special sets we have
$$\begin{align}
&\text{The empty set}&\emptyset&=\set{} \\
&\text{The natural numbers}&\mathbb{N}&=\set{1,2,3,4,5,...} \\
&\text{The integers}&\mathbb{Z}&=\set{...,-3,-2,-1,0,1,2,3,4,5,...} \\
&\text{The rational numbers}&\mathbb{Q}&=\set{x:x=m/n,\text{ where }m,n\in\mathbb{Z}\text{ and }n\ne0} \\
&\text{The real numbers}&\mathbb{R}
\end{align}$$
We visualize the set $\mathbb{R}$ as an infinitely long number line
Note: $\mathbb{Q}\ne\mathbb{R}$ because $\sqrt{2}\in\mathbb{R}\text{ but }\sqrt{2}\notin\mathbb{Q}$
Like $\mathbb{R}$, any 2 numbers $a,b\in\mathbb{R}$, with $a<b$ give rise to infinite sets which can be denoted on the number line as darkened segment between $a\text{ and }b$. A solid circle indicates a number is included in the interval and a hollow circle indicates its not
