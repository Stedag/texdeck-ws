---
id: GPgIY1P3Zf3fH0J3PY4sN
title: Lec08
desc: ''
updated: 1637530120234
created: 1637530120234
---
\section{III.C The Bogoliubov-Born-Green-Kirkwood-Yvon Hierarchy}

The full phase space density contains much more information than necessary for description of equilibrium properties. For example, knowledge of the one particle distribution is sufficient for computing the pressure of a gas. A one particle density refers to the expectation value of finding any of the $N$ particles at location $\vec{q}$, with momentum $\vec{p}$, at time $t$, which is computed from the full density $\rho$ as

$$
\begin{aligned}
f_{1}(\vec{p}, \vec{q}, t) &=\left\langle\sum_{i=1}^{N} \delta^{3}\left(\vec{p}-\vec{p}_{i}\right) \delta^{3}\left(\vec{q}-\vec{q}_{i}\right)\right\rangle \\
&=N \int \prod_{i=2}^{N} d^{3} \vec{p}_{i} d^{3} \vec{q}_{i} \rho\left(\vec{p}_{1}=\vec{p}, \vec{q}_{1}=\vec{q}, \vec{p}_{2}, \vec{q}_{2}, \cdots, \vec{p}_{N}, \vec{q}_{N}, t\right)
\end{aligned}
$$

To obtain the second identity above, we used the first pair of delta functions to perform one set of integrals, and then assumed that the density is symmetric with respect to permuting the particles. Similarly, a two particle density can be computed from

$$
f_{2}\left(\vec{p}_{1}, \vec{q}_{1}, \vec{p}_{2}, \vec{q}_{2}, t\right)=N(N-1) \int \prod_{i=3}^{N} d V_{i} \rho\left(\vec{p}_{1}, \vec{q}_{1}, \vec{p}_{2}, \vec{q}_{2}, \cdots, \vec{p}_{N}, \vec{q}_{N}, t\right)
$$

where $d V_{i}=d^{3} \vec{p}_{i} d^{3} \vec{q}_{i}$ is the contribution of particle $i$ to phase space volume. The general $s$ -particle density is defined by

$$
f_{s}\left(\vec{p}_{1}, \cdots, \vec{q}_{s}, t\right)=\frac{N !}{(N-s) !} \int \prod_{i=s+1}^{N} d V_{i} \rho(\mathbf{p}, \mathbf{q}, t)=\frac{N !}{(N-s) !} \rho_{s}\left(\vec{p}_{1}, \cdots, \vec{q}_{s}, t\right)
$$

where $\rho_{s}$ is a standard unconditional $P D F$ for the coordinates of $s$ particles, and $\rho_{N} \equiv \rho$ While $\rho_{s}$ is properly normalized to unity when integrated over all its variables, the $s$ particle density has a normalization of $N ! /(N-s) ! . \quad$ We shall use the two quantities interchangeably.

The evolution of the few-body densities is governed by the BBGKY hierarchy of equations attributed to Bogoliubov, Born, Green, Kirkwood, and Yvon. The simplest non-trivial Hamiltonian studied in kinetic theory is

$$
\mathcal{H}(\mathbf{p}, \mathbf{q})=\sum_{i=1}^{N}\left[\frac{\vec{p}_{i}{ }^{2}}{2 m}+U\left(\vec{q}_{i}\right)\right]+\frac{1}{2} \sum_{(i, j)=1}^{N} \mathcal{V}\left(\vec{q}_{i}-\vec{q}_{j}\right)
$$

This Hamiltonian provides an adequate description of a weakly interacting gas. In addition to the classical kinetic energy of particles of mass $m$, it contains an external potential $U$, and a two-body interaction $\mathcal{V}$, between the particles. In principle, three and higher body interactions should also be included for a realistic description, but they are not very important in the dilute gas (nearly ideal) limit.

For evaluating the time evolution of $f_{s}$, it is convenient to divide the Hamiltonian into

$$
\mathcal{H}=\mathcal{H}_{s}+\mathcal{H}_{N-s}+\mathcal{H}^{\prime}
$$

where $\mathcal{H}_{s}$ and $\mathcal{H}_{N-s}$ include only interactions among each group of particles,

$$
\begin{gathered}
\mathcal{H}_{s}=\sum_{n=1}^{s}\left[\frac{\vec{p}_{n}^{2}}{2 m}+U\left(\vec{q}_{n}\right)\right]+\frac{1}{2} \sum_{(n, m)=1}^{s} \mathcal{V}\left(\vec{q}_{n}-\vec{q}_{m}\right) \\
\mathcal{H}_{N-s}=\sum_{i=s+1}^{N}\left[\frac{\vec{p}_{i}^{2}}{2 m}+U\left(\vec{q}_{i}\right)\right]+\frac{1}{2} \sum_{(i, j)=s+1}^{N} \mathcal{V}\left(\vec{q}_{i}-\vec{q}_{j}\right)
\end{gathered}
$$

while the interparticle interactions are contained in

$$
\mathcal{H}^{\prime}=\sum_{n=1}^{s} \sum_{i=s+1}^{N} \mathcal{V}\left(\vec{q}_{n}-\vec{q}_{i}\right)
$$

From eq.(III.18), the time evolution of $f_{s}\left(\right.$ or $\left.\rho_{s}\right)$ is obtained as

$$
\frac{\partial \rho_{s}}{\partial t}=\int \prod_{i=s+1}^{N} d V_{i} \frac{\partial \rho}{\partial t}=-\int \prod_{i=s+1}^{N} d V_{i}\left\{\rho, \mathcal{H}_{s}+\mathcal{H}_{N-s}+\mathcal{H}^{\prime}\right\}
$$

where eq.(III.9) is used for the evolution of $\rho$. The three Poisson brackets in eq.(III.23) will now be evaluated in turn. Since the first $s$ coordinates are not integrated, the order of integrations and differentiations for the Poisson bracket may be reversed, and

$$
\int \prod_{i=s+1}^{N} d V_{i}\left\{\rho, \mathcal{H}_{s}\right\}=\left\{\left(\int \prod_{i=s+1}^{N} d V_{i} \rho\right), \mathcal{H}_{s}\right\}=\left\{\rho_{s}, \mathcal{H}_{s}\right\}
$$

Writing the Poisson brackets explicitly, the second term of eq.(III.23) takes the form

$$
-\int \prod_{i=s+1}^{N} d V_{i}\left\{\rho, \mathcal{H}_{N-s}\right\}=\int \prod_{i=s+1}^{N} d V_{i} \sum_{j=1}^{N}\left[\frac{\partial \rho}{\partial \vec{p}_{j}} \cdot \frac{\partial \mathcal{H}_{N-s}}{\partial \vec{q}_{j}}-\frac{\partial \rho}{\partial \vec{q}_{j}} \cdot \frac{\partial \mathcal{H}_{N-s}}{\partial \vec{p}_{j}}\right]
$$

(using eq.(III.21))

$$
=\int \prod_{i=s+1}^{N} d V_{i} \sum_{j=s+1}^{N}\left[\frac{\partial \rho}{\partial \vec{p}_{j}} \cdot\left(\frac{\partial U}{\partial \vec{q}_{j}}+\frac{1}{2} \sum_{k=s+1}^{N} \frac{\partial \mathcal{V}\left(\vec{q}_{j}-\vec{q}_{k}\right)}{\partial \vec{q}_{j}}\right)-\frac{\partial \rho}{\partial \vec{q}_{j}} \cdot \frac{\vec{p}_{j}}{m}\right]=0
$$

The last equality is obtained after performing the integrations by part: The term multiplying $\partial \rho / \partial \vec{p}_{j}$ has no dependence on $\vec{p}_{j}$, while $\vec{p}_{j} / m$ does not depend on $\vec{q}_{j}$. The final term in eq.(III.23), involving the Poisson bracket with $\mathcal{H}^{\prime}$, is

$$
\begin{aligned}
& \int \prod_{i=s+1}^{N} d V_{i} \sum_{j=1}^{N}\left[\frac{\partial \rho}{\partial \vec{p}_{j}} \cdot \frac{\partial \mathcal{H}^{\prime}}{\partial \vec{q}_{j}}-\frac{\partial \rho}{\partial \vec{q}_{j}} \cdot \frac{\partial \mathcal{H}^{\prime}}{\partial \vec{p}_{j}}\right] \\
=& \int \prod_{i=s+1}^{N} d V_{i}\left[\sum_{n=1}^{s} \frac{\partial \rho}{\partial \vec{p}_{n}} \cdot \sum_{j=s+1}^{N} \frac{\partial \mathcal{V}\left(\vec{q}_{n}-\vec{q}_{j}\right)}{\partial \vec{q}_{n}}+\sum_{j=s+1}^{N} \frac{\partial \rho}{\partial \vec{p}_{j}} \cdot \sum_{n=1}^{s} \frac{\partial \mathcal{V}\left(\vec{q}_{j}-\vec{q}_{n}\right)}{\partial \vec{q}_{j}}\right]
\end{aligned}
$$

where the sum over all particles has been subdivided into the two groups. (Note that $\mathcal{H}^{\prime}$ in eq.(III.22) has no dependence on the momenta.) Integration by parts shows that the second term in the above expression is zero. The first term involves the sum of $(N-s)$ expressions that are equal by symmetry and simplifies to

$$
\begin{aligned}
&(N-s) \int \prod_{i=s+1}^{N} d V_{i} \sum_{n=1}^{s} \frac{\partial \mathcal{V}\left(\vec{q}_{n}-\vec{q}_{s+1}\right)}{\partial \vec{q}_{n}} \cdot \frac{\partial \rho}{\partial \vec{p}_{n}} \\
=&(N-s) \sum_{n=1}^{s} \int d V_{s+1} \frac{\partial \mathcal{V}\left(\vec{q}_{n}-\vec{q}_{s+1}\right)}{\partial \vec{q}_{n}} \cdot \frac{\partial}{\partial \vec{p}_{n}}\left[\int \prod_{i=s+2}^{N} d V_{i} \rho\right]
\end{aligned}
$$

Note that the quantity in the above square brackets is $\rho_{s+1} .$ Thus, adding up eqs.(III.24), (III.25), and (III.26),

$$
\frac{\partial \rho_{s}}{\partial t}-\left\{\mathcal{H}_{s}, \rho_{s}\right\}=(N-s) \sum_{n=1}^{s} \int d V_{s+1} \frac{\partial \mathcal{V}\left(\vec{q}_{n}-\vec{q}_{s+1}\right)}{\partial \vec{q}_{n}} \cdot \frac{\partial \rho_{s+1}}{\partial \vec{p}_{n}}
$$

or in terms of the densities $f_{s}$

$$
\frac{\partial f_{s}}{\partial t}-\left\{\mathcal{H}_{s}, f_{s}\right\}=\sum_{n=1}^{s} \int d V_{s+1} \frac{\partial \mathcal{V}\left(\vec{q}_{n}-\vec{q}_{s+1}\right)}{\partial \vec{q}_{n}} \cdot \frac{\partial f_{s+1}}{\partial \vec{p}_{n}}
$$

In the absence of interactions with other particles, the density $\rho_{s}$ for a group of $s$ particles evolves as the density of an incompressible fluid (as required by Liouville's theorem), and is described by the streaming terms on the left hand side of eq.(III.27). However, because of interactions with the remaining $N-s$ particles, the flow is modified by the collision terms on the right hand side. The collision integral is the sum of the terms corresponding to a potential collision of any of the particles in the group of $s$, with any of the remaining $N-s$ particles. To describe the probability of finding the additional particle that collides with a member of this group, the result must depend on the joint PDF of $s+1$ particles described by $\rho_{s+1} .$ This results in a hierarchy of equations in which $\partial \rho_{1} / \partial t$ depends on $\rho_{2}, \partial \rho_{2} / \partial t$ depends on $\rho_{3}$, etc., which is at least as complicated as the original equation for the full phase space density. To proceed further, a physically motivated approximation for terminating the hierarchy is needed. 

\section{III.D The Boltzmann Equation}

To estimate the relative importance of the different terms appearing in eqs.(III.28), let us examine the first two equations in the hierarchy,

$$
\left[\frac{\partial}{\partial t}-\frac{\partial U}{\partial \vec{q}_{1}} \cdot \frac{\partial}{\partial \vec{p}_{1}}+\frac{\vec{p}_{1}}{m} \cdot \frac{\partial}{\partial \vec{q}_{1}}\right] f_{1}=\int d V_{2} \frac{\partial \mathcal{V}\left(\vec{q}_{1}-\vec{q}_{2}\right)}{\partial \vec{q}_{1}} \cdot \frac{\partial f_{2}}{\partial \vec{p}_{1}}
$$

and

$$
\begin{gathered}
{\left[\frac{\partial}{\partial t}-\frac{\partial U}{\partial \vec{q}_{1}} \cdot \frac{\partial}{\partial \vec{p}_{1}}-\frac{\partial U}{\partial \vec{q}_{2}} \cdot \frac{\partial}{\partial \vec{p}_{2}}+\frac{\vec{p}_{1}}{m} \cdot \frac{\partial}{\partial \vec{q}_{1}}+\frac{\vec{p}_{2}}{m} \cdot \frac{\partial}{\partial \vec{q}_{2}}-\frac{\partial \mathcal{V}\left(\vec{q}_{1}-\vec{q}_{2}\right)}{\partial \vec{q}_{1}} \cdot\left(\frac{\partial}{\partial \vec{p}_{1}}-\frac{\partial}{\partial \vec{p}_{2}}\right)\right] f_{2}=} \\
\int d V_{3}\left[\frac{\partial \mathcal{V}\left(\vec{q}_{1}-\vec{q}_{3}\right)}{\partial \vec{q}_{1}} \cdot \frac{\partial}{\partial \vec{p}_{1}}+\frac{\partial \mathcal{V}\left(\vec{q}_{2}-\vec{q}_{3}\right)}{\partial \vec{q}_{2}} \cdot \frac{\partial}{\partial \vec{p}_{2}}\right] f_{3}
\end{gathered}
$$

Note that two of the streaming terms in eq.(III.30) have been combined by using $\partial \mathcal{V}\left(\vec{q}_{1}-\vec{q}_{2}\right) / \partial \vec{q}_{1}=-\partial \mathcal{V}\left(\vec{q}_{2}-\vec{q}_{1}\right) / \partial \vec{q}_{2}$, which is valid for a symmetric potential such that $\mathcal{V}\left(\vec{q}_{1}-\vec{q}_{2}\right)=\mathcal{V}\left(\vec{q}_{2}-\vec{q}_{1}\right)$

- Time scales: All terms within square brackets in the above equations have dimensions of inverse time, and we estimate their relative magnitudes by dimensional analysis, using typical velocities and length scales. The typical speed of a gas particle at room temperature is $v \approx 10^{2} \mathrm{~ms}^{-1}$. For terms involving the external potential $U$, or the inter-atomic potential $\mathcal{V}$, an appropriate length scale can be extracted from the range of variations of the potential.

(a) The terms proportional to

$$
\frac{1}{\tau_{U}} \sim \frac{\partial U}{\partial \vec{q}} \cdot \frac{\partial}{\partial \vec{p}}
$$

involve spatial variations of the external potential $U(\vec{q})$, which take place over macroscopic distances $L .$ We shall refer to the associated time $\tau_{U}$, as an extrinsic time scale, as it can be made arbitrarily long by increasing system size. For a typical value of $L \approx 10^{-3} \mathrm{~m}$, we get $\tau_{U} \approx L / v \approx 10^{-5} s$

(b) From the terms involving the inter-atomic potential $\mathcal{V}$, we can extract two additional time scales, which are intrinsic to the gas under study. In particular, the collision duration

$$
\frac{1}{\tau_{c}} \sim \frac{\partial \mathcal{V}}{\partial \vec{q}} \cdot \frac{\partial}{\partial \vec{p}}
$$

is the typical time over which two particles are within the effective range $d$, of their interaction. For short range interactions (including van der Waals and Lenard-Jones, despite their power law decaying tails), $d \approx 10^{-10} m$ is of the order of a typical atomic size, resulting in $\tau_{c} \approx 10^{-12} s$. This is usually the shortest time scale in the problem. The analysis is somewhat more complicated for long range interactions, such as the Coulomb gas in a plasma. For a neutral plasma, the Debye screening length $\lambda$ replaces $d$ in the above equation, as discussed in the problems.

(c) There are also collision terms on the right hand side of eqs.(III.28), which depend on $f_{s+1}$, and lead to an inverse time scale

$$
\frac{1}{\tau_{\times}} \sim \int d V \frac{\partial \mathcal{V}}{\partial \vec{q}} \cdot \frac{\partial}{\partial \vec{p}} \frac{f_{s+1}}{f_{s}} \sim \int d V \frac{\partial \mathcal{V}}{\partial \vec{q}} \cdot \frac{\partial}{\partial \vec{p}} N \frac{\rho_{s+1}}{\rho_{s}}
$$

The integrals are only non-zero over the volume of the inter-particle potential $d^{3}$. The term $f_{s+1} / f_{s}$ is related to the probability of finding another particle per unit volume, which is roughly the particle density $n=N / V \approx 10^{26} m^{-3} .$ We thus obtain the mean free time

$$
\tau_{\times} \approx \frac{\tau_{c}}{n d^{3}} \approx \frac{1}{n v d^{2}}
$$

which is the typical distance a particle travels between collisions. For short range interactions, $\tau_{\times} \approx 10^{-8} s$ is much longer than $\tau_{c}$, and the collision terms on the right hand side of eqs.(III.28) are smaller by a factor of $n d^{3} \approx\left(10^{26} m^{-3}\right)\left(10^{-10} m\right)^{3} \approx 10^{-4}$. The Boltzmann equation is obtained for short range interactions in the dilute regime by exploiting $\tau_{c} / \tau_{\times} \approx n d^{3} \ll 1 .$ (By contrast, for long range interactions such that $n d^{3} \gg 1$, the Vlasov equation is obtained by dropping the collision terms on the left hand side, as discussed in the problems.) From the above discussion, it is apparent that eq.(III.29) is different from the rest of the hierarchy: It is the only one in which the collision terms are absent from the left hand side. For all other equations, the right hand side is smaller by a factor of $n d^{3}$, while in eq.(III.29) it may indeed dominate the left hand side. Thus a possible approximation scheme is to truncate the equations after the first two, by setting the right hand side of eq.(III.30) to zero.

Setting the right hand side of the equation for $f_{2}$ to zero implies that the two body density evolves as in an isolated two-particle system. The relatively simple mechanical processes that govern this evolution result in streaming terms for $f_{2}$ which are proportional to both $\tau_{U}^{-1}$ and $\tau_{c}^{-1} .$ The two sets of terms can be more or less treated independently: the former describe the evolution of the center of mass of the two particles, while the latter govern the dependence on relative coordinates. The density $f_{2}$ is proportional to the joint PDF $\rho_{2}$ for finding one particle at $\left(\vec{p}_{1}, \vec{q}_{1}\right)$, and another at $\left(\vec{p}_{2}, \vec{q}_{2}\right)$, at the same time $t .$ It is reasonable to expect that at distances much larger than the range of the potential $\mathcal{V}$, the particles are independent, i.e.

$$
\left\{\begin{array}{l}
\rho_{2}\left(\vec{p}_{1}, \vec{q}_{1}, \vec{p}_{2}, \vec{q}_{2}, t\right) \longrightarrow \rho_{1}\left(\vec{p}_{1}, \vec{q}_{1}, t\right) \rho_{1}\left(\vec{p}_{2}, \vec{q}_{2}, t\right), \text { or } \\
f_{2}\left(\vec{p}_{1}, \vec{q}_{1}, \vec{p}_{2}, \vec{q}_{2}, t\right) \longrightarrow f_{1}\left(\vec{p}_{1}, \vec{q}_{1}, t\right) f_{1}\left(\vec{p}_{2}, \vec{q}_{2}, t\right), \quad \text { for } \quad\left|\vec{q}_{2}-\vec{q}_{1}\right| \gg d
\end{array}\right.
$$

The above statement should be true even for situations out of equilibrium. For example, imagine that the gas particles in a chamber are suddenly allowed to invade an empty volume after the removal of a barrier. The density $f_{1}$ will undergo a complicated evolution, and its relaxation time will be at least comparable to $\tau_{U} .$ The two particle density $f_{2}$, will also reach its final value at a comparable time interval. However, it is expected to relax to a form similar to eq.(III.32) over a much shorter time of the order of $\tau_{c}$.

For the collision term on the right hand side of eq.(III.29), we actually need the precise dependence of $f_{2}$ on the relative coordinates and momenta at separations comparable to $d$. At time intervals longer than $\tau_{c}$ (but possibly shorter than $\left.\tau_{U}\right)$, the 'steady state' behavior of $f_{2}$ at small relative distances is obtained by equating the largest streaming terms in eq.(III.30), i.e.

$$
\left[\frac{\vec{p}_{1}}{m} \cdot \frac{\partial}{\partial \vec{q}_{1}}+\frac{\vec{p}_{2}}{m} \cdot \frac{\partial}{\partial \vec{q}_{2}}-\frac{\partial \mathcal{V}\left(\vec{q}_{1}-\vec{q}_{2}\right)}{\partial \vec{q}_{1}} \cdot\left(\frac{\partial}{\partial \vec{p}_{1}}-\frac{\partial}{\partial \vec{p}_{2}}\right)\right] f_{2}=0
$$

We expect $f_{2}\left(\vec{q}_{1}, \vec{q}_{2}\right)$ to have slow variations over the center of mass coordinate $\vec{Q}=\left(\vec{q}_{1}+\right.$ $\left.\vec{q}_{2}\right) / 2$, and large variations over the relative coordinate $\vec{q}=\vec{q}_{2}-\vec{q}_{1} .$ Therefore, $\partial f_{2} / \partial \vec{q} \gg$ $\partial f_{2} / \partial \vec{Q}$, and $\partial f_{2} / \vec{q}_{2} \approx-\partial f_{2} / \partial \vec{q}_{1} \approx \partial f_{2} / \partial \vec{q}$, leading to

$$
\frac{\partial \mathcal{V}\left(\vec{q}_{1}-\vec{q}_{2}\right)}{\partial \vec{q}_{1}} \cdot\left(\frac{\partial}{\partial \vec{p}_{1}}-\frac{\partial}{\partial \vec{p}_{2}}\right) f_{2}=-\left(\frac{\vec{p}_{1}-\vec{p}_{2}}{m}\right) \cdot \frac{\partial}{\partial \vec{q}} f_{2}
$$

The above equation provides a precise mathematical expression for how $f_{2}$ is constrained along the trajectories that describe the collision of the two particles.

The collision term on the right hand side of eq.(III.29) can now be written as

$$
\begin{aligned}
\left.\frac{d f_{1}}{d t}\right|_{\text {coll. }} &=\int d^{3} \vec{p}_{2} d^{3} \vec{q}_{2} \frac{\partial \mathcal{V}\left(\vec{q}_{1}-\vec{q}_{2}\right)}{\partial \vec{q}_{1}} \cdot\left(\frac{\partial}{\partial \vec{p}_{1}}-\frac{\partial}{\partial \vec{p}_{2}}\right) f_{2} \\
& \approx \int d^{3} \vec{p}_{2} d^{3} \vec{q}\left(\frac{\vec{p}_{2}-\vec{p}_{1}}{m}\right) \cdot \frac{\partial}{\partial \vec{q}} f_{2}\left(\vec{p}_{1}, \vec{q}_{1}, \vec{p}_{2}, \vec{q} ; t\right)
\end{aligned}
$$

The first identity if obtained from eq.(III.29) by noting that the added term proportional to $\partial f_{2} / \partial \vec{p}_{2}$ is a complete derivative and integrates to zero, while the second equality follows from eq.(III.34), after the change of variables to $\vec{q}=\vec{q}_{2}-\vec{q}_{1}$. (Since it relies on establishing the 'steady state' in the relative coordinates, this approximation is valid as long as we examine events in time with a resolution longer than $\tau_{c}$.)

- Kinematics of collision and scattering: The integrand in eq.(III.35) is a derivative of $f_{2}$ with respect to $\vec{q}$ along the direction of relative motion $\vec{p}=\vec{p}_{2}-\vec{p}_{1}$, of the colliding particles. To perform this integration we introduce a convenient coordinate system for $\vec{q}$, guided by the formalism used to describe the scattering of particles. Naturally, we choose one axis to be parallel to $\vec{p}_{2}-\vec{p}_{1}$, with the corresponding coordinate $a$ which is negative before a collision, and positive afterwards. The other two coordinates of $\vec{q}$ are represented by an impact vector $\vec{b}$ which is $\overrightarrow{0}$ for a head-on collision $\left(\left[\vec{p}_{1}-\vec{p}_{2}\right] \|\left[\vec{q}_{1}-\vec{q}_{2}\right]\right) .$ We can now integrate over $a$ to get

$$
\left.\frac{d f_{1}}{d t}\right|_{\text {coll. }}=\int d^{3} \vec{p}_{2} d^{2} \vec{b}\left|\vec{v}_{1}-\vec{v}_{2}\right|\left[f_{2}\left(\vec{p}_{1}, \vec{q}_{1}, \vec{p}_{2}, \vec{b},+; t\right)-f_{2}\left(\vec{p}_{1}, \vec{q}_{1}, \vec{p}_{2}, \vec{b},-; t\right)\right]
$$

where $\left|\vec{v}_{1}-\vec{v}_{2}\right|=\left|\vec{p}_{1}-\vec{p}_{2}\right| / m$ is the relative speed of the two particles, with $(\vec{b},-)$ and $(\vec{b},+)$ referring to relative coordinates before and after the collision. Note that $d^{2} \vec{b}\left|\vec{v}_{1}-\vec{v}_{2}\right|$ is just the flux of particles impinging on the element of area $d^{2} \vec{b}$

In principle, the integration over $a$ is from $-\infty$ to $+\infty$, but as the variations of $f_{2}$ are only significant over the interaction range $d$, we can evaluate the above quantities at separations of a few $d$ from the collision point. This is a good compromise, allowing us to evaluate $f_{2}$ away from the collisions, but at small enough separations so that we can ignore the difference between $\vec{q}_{1}$ and $\vec{q}_{2}$. This amounts to a coarse-graining in space which eliminates variations on scales finer than $d .$ With these provisos, it is tempting to close the equation for $f_{1}$, by using the assumption of uncorrelated particles in eq.(III.32). Clearly some care is necessary as a naive substitution gives zero! The key observation is that the densities $f_{2}$ for situations corresponding to before and after the collision have to be treated differently. For example, soon after opening of the slot separating empty and full gas containers, the momenta of the gas particles are likely to point away from the slot. Collisions will tend to randomize momenta, yielding a more isotropic distribution. However, the densities $f_{2}$ before and after the collision are related by streaming, implying that $f_{2}\left(\vec{p}_{1}, \vec{q}_{1}, \vec{p}_{2}, \vec{b},+; t\right)=f_{2}\left(\vec{p}_{1}^{\prime}, \vec{q}_{1}, \vec{p}_{2}^{\prime}, \vec{b},-; t\right)$, where $\vec{p}_{1}^{\prime}$ and $\vec{p}_{2}^{\prime}$ are momenta whose collision at an impact vector $\vec{b}$ results in production of outgoing particles with momenta $\vec{p}_{1}$ and $\vec{p}_{2}$. They can be obtained using time reversal symmetry, by integrating the equations of motion for incoming colliding particles of momenta $-\vec{p}_{1}$ and $-\vec{p}_{2} .$ In terms of these momenta, we can write

$$
\left.\frac{d f_{1}}{d t}\right|_{\text {coll. }}=\int d^{3} \vec{p}_{2} d^{2} \vec{b}\left|\vec{v}_{1}-\vec{v}_{2}\right|\left[f_{2}\left(\vec{p}_{1}^{\prime}, \vec{q}_{1}, \vec{p}_{2}^{\prime}, \vec{b},-; t\right)-f_{2}\left(\vec{p}_{1}, \vec{q}_{1}, \vec{p}_{2}, \vec{b},-; t\right)\right]
$$

It is sometimes more convenient to describe the scattering of two particles in terms of the relative momenta $\vec{p}=\vec{p}_{1}-\vec{p}_{2}$ and $\vec{p}^{\prime}=\vec{p}_{1}^{\prime}-\vec{p}_{2}^{\prime}$, before and after the collision. For a given $\vec{b}$, the initial momentum $\vec{p}$ is deterministically transformed to the final momentum $\vec{p}^{\prime} .$ To find the functional form $\vec{p}^{\prime}(|\vec{p}|, \vec{b})$, one must integrate the equations of motion. However, it is possible to make some general statements based on conservation laws: In elastic collisions, the magnitude of $\vec{p}$ is preserved, and it merely rotates to a final direction indicated by the angles $(\theta, \phi) \equiv \hat{\Omega}(\vec{b})$ (a unit vector) in spherical coordinates. Since there is a one to one correspondence between the impact vector $\vec{b}$, and the solid angle $\Omega$, we make a change of variables between the two, resulting in

$$
\left.\frac{d f_{1}}{d t}\right|_{\text {coll. }}=\int d^{3} \vec{p}_{2} d^{2} \Omega\left|\frac{d \sigma}{d \Omega}\right|\left|\vec{v}_{1}-\vec{v}_{2}\right|\left[f_{2}\left(\vec{p}_{1}^{\prime}, \vec{q}_{1}, \vec{p}_{2}^{\prime}, \vec{b},-; t\right)-f_{2}\left(\vec{p}_{1}, \vec{q}_{1}, \vec{p}_{2}, \vec{b},-; t\right)\right]
$$

The Jacobian of this transformation, $|d \sigma / d \Omega|$, has dimensions of area, and is known as the differential cross-section. It is equal to the area presented to an incoming beam which scatters into the solid angle $\Omega .$ The out-going momenta $\vec{p}_{1}^{\prime}$ and $\vec{p}_{2}^{\prime}$ in eq.(III.38) are now obtained from the two conditions $\vec{p}_{1}^{\prime}+\vec{p}_{2}^{\prime}=\vec{p}_{1}+\vec{p}_{2}$ (conservation of momentum), and $\vec{p}_{1}^{\prime}-\vec{p}_{2}^{\prime}=\left|\vec{p}_{1}-\vec{p}_{2}\right| \hat{\Omega}(\vec{b})($ conservation of energy $)$, as

$$
\left\{\begin{array}{l}
\vec{p}_{1}^{\prime}=\left(\vec{p}_{1}+\vec{p}_{2}+\left|\vec{p}_{1}-\vec{p}_{2}\right| \hat{\Omega}(\vec{b})\right) / 2 \\
\vec{p}_{2}^{\prime}=\left(\vec{p}_{1}+\vec{p}_{2}-\left|\vec{p}_{1}-\vec{p}_{2}\right| \hat{\Omega}(\vec{b})\right) / 2
\end{array}\right.
$$

For the scattering of two hard spheres of diameter $D$, it is easy to show that the scattering angle is related to the impact parameter $b$ by $\cos (\theta / 2)=b / D$ for all $\phi .$ The differential cross-section is then obtained from

$$
d^{2} \sigma=b d b d \phi=D \cos \left(\frac{\theta}{2}\right) D \sin \left(\frac{\theta}{2}\right) \frac{d \theta}{2} d \phi=\frac{D^{2}}{4} \sin \theta d \theta d \phi=\frac{D^{2}}{4} d^{2} \Omega
$$

(Note that the solid angle in three dimensions is given by $\left.d^{2} \Omega=\sin \theta d \theta d \phi .\right)$ Integrating over all angles leads to the total cross-section of $\sigma=\pi D^{2}$, which is evidently correct. The differential cross-section for hard spheres is independent of both $\theta$ and $|\vec{P}| .$ This is not the case for soft potentials. For example, the Coulomb potential $\mathcal{V}=e^{2} /|\vec{Q}|$ leads to

$$
\left|\frac{d \sigma}{d \Omega}\right|=\left(\frac{m e^{2}}{2|\vec{P}|^{2} \sin ^{2}(\theta / 2)}\right)^{2}
$$

(The dependence on $|\vec{P}|$ can be justified by obtaining a distance of closest approach from $\left.|\vec{P}|^{2} / m+e^{2} / b \approx 0 .\right)$

- The Boltzmann equation is obtained from eq.(III.38) after the substitution

$$
f_{2}\left(\vec{p}_{1}, \vec{q}_{1}, \vec{p}_{2}, \vec{b},-; t\right)=f_{1}\left(\vec{p}_{1}, \vec{q}_{1}, t\right) \cdot f_{1}\left(\vec{p}_{2}, \vec{q}_{1}, t\right)
$$

known as the assumption of molecular chaos. Note that even if one starts with an uncorrelated initial probability distribution for particles, there is no guarantee that correlations are not generated as a result of collisions. The final result is the following closed form equation for $f_{1}$

$$
\begin{aligned}
&{\left[\frac{\partial}{\partial t}-\frac{\partial U}{\partial \vec{q}_{1}} \cdot \frac{\partial}{\partial \vec{p}_{1}}+\frac{\vec{p}_{1}}{m} \cdot \frac{\partial}{\partial \vec{q}_{1}}\right] f_{1}=} \\
&-\int d^{3} \vec{p}_{2} d^{2} \Omega\left|\frac{d \sigma}{d \Omega}\right|\left|\vec{v}_{1}-\vec{v}_{2}\right|\left[f_{1}\left(\vec{p}_{1}, \vec{q}_{1}, t\right) f_{1}\left(\vec{p}_{2}, \vec{q}_{1}, t\right)-f_{1}\left(\vec{p}_{1}^{\prime}, \vec{q}_{1}, t\right) f_{1}\left(\vec{p}_{2}^{\prime}, \vec{q}_{1}, t\right)\right]
\end{aligned}
$$

Given the complexity of the above 'derivation' of the Boltzmann equation, it is appropriate to provide a heuristic explanation. The streaming terms on the left hand side of the equation describe the motion of a single particle in the external potential $U$. The collision terms on the right hand side have a simple physical interpretation: The probability of finding a particle of momentum $\vec{p}_{1}$ at $\vec{q}_{1}$ is suddenly altered if it undergoes a collision with another particle of momentum $\vec{p}_{2}$. The probability of such a collision is the product of kinematic factors described by the differential cross-section $|d \sigma / d \Omega|$, the 'flux' of incident particles proportional to $\left|\vec{v}_{2}-\vec{v}_{1}\right|$, and the joint probability of finding the two particles, approximated by $f_{1}\left(\vec{p}_{1}\right) f_{1}\left(\vec{p}_{2}\right) .$ The first term on the right hand side of eq.(III.41) subtracts this probability and integrates over all possible momenta and solid angles describing the collision. The second term represents an addition to the probability which results from the inverse process: A particle can suddenly appear with coordinates $\left(\vec{p}_{1}, \vec{q}_{1}\right)$ as a result of a collision between two particles initially with momenta $\vec{p}_{1}^{\prime}$ and $\vec{p}_{2}^{\prime} .$ The cross-section, and the momenta $\left(\vec{p}_{1}^{\prime}, \vec{p}_{2}^{\prime}\right)$ may have a complicated dependence on $\left(\vec{p}_{1}, \vec{p}_{2}\right)$ and $\Omega$, determined by the specific form of the potential $\mathcal{V}$. Remarkably, various equilibrium properties of the gas are quite independent of this potential. MIT OpenCourseWare

http://ocw.mit.edu

\subsection{Statistical Mechanics I: Statistical Mechanics of Particles \\ Fall 2013}

For information about citing these materials or our Terms of Use, visit: http://ocw.mit.edu/terms.
