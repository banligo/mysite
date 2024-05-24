---
title: "Complex Variable Theory"
weight: 1
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
math: true
---

> conclusion, find proof in textbook. <br>
> typical problems answering

<!--more-->

- $C$ is in couterclockwise direction

# Theorems

### Cauchy-Riemann conditions

$$\frac{\partial u}{\partial x}=\frac{\partial v}{\partial y},\quad \frac{\partial u}{\partial y}=-\frac{\partial v}{\partial x}.$$

Proof: 

$$\lim_{\delta z\rightarrow 0}\frac{\delta f}{\delta z}=$$

### Cauchy's Theorem 

$$\oint_C f(z)dz=0$$

$$\oint_C(z-z_0)^ndz=\begin{cases}
    0, & n\neq 1,\\
    2\pi i, & n=-1.
\end{cases}$$

### Cauchy's integral formula

$$\frac{1}{2\pi i}\oint_C\frac{f(z)}{z-z_0}dz=\begin{cases}
    f(z_0), & z_0 \text{  within the contour},    \\
    0, & z_0 \text{ exterior to the contour}.
\end{cases}$$


### Residue Theorem

$$\oint_Cf(z)dz=2\pi i \sum \text{residues}$$

$$
  a_{-1}=\frac{1}{(n-1)!}\lim_{z\rightarrow z_0}\left[\frac{d^{n-1}}{dz^{n-1}}((z-z_0)^nf(z))\right]$$


## Evaluation of definite integrals


### Jordan's lemma
If $\lim_{R=\infty}f(z)=0$ for all $z=Re^{i\theta}$ in the range $0\leq\theta\leq\pi$, then 
$$\lim_{R\rightarrow\infty}\int_Ce^{iaz}f(z)dz=0,$$
where $z>0$ and $C$ is a semicircle of radius $R$ in the upper half-plane with center at the origin. 


#### 1. $(0,2\pi)$ 


 $$\begin{aligned} 
    I &=\int_0^{2\pi}f(\sin\theta,\cos\theta)d\theta =-i\oint f\left(\frac{z-z^{-1}}{2i},\frac{z+z^{-1}}{2i}\right)\frac{dz}{z}\\
     &=(-i)2\pi i\sum \text{residues} \end{aligned}$$

Note that use the redidues of $f/z$, and the the residues are in within the unit circle. 


#### 2. $(-\infty,\infty)$

$$I=\int_{-\infty}^{\infty}f(x)dx=\oint f(z)dz=2\pi i\sum \text{residues }\text{ (upper half-plane)}$$



#### 3. $e^{iax}$

$$I=\int_{-\infty}^{\infty}f(x)e^{-ax}dx=2\pi i\sum \text{residues of }e^{iaz}f(z) \text{ (upper half-plane)}$$



<br>

---
---


# Examples

not complete, just some steps

0. dfa 
1. da 
2. $$I=\int_0^\infty\frac{\sin x}{x}dx$$
   $\oint\frac{e^{iz}}{2iz}dz=I+\int_{C_r}\frac{e^{iz}}{2iz}dz+\int_{C_R}\frac{e^{iz}}{2iz}dz=0$
3. da  


<br>

---
---

Reference: <br>
[1] Mathematical Methods for Physcicists, Seventh Edition. 



Other chapter notes link: 