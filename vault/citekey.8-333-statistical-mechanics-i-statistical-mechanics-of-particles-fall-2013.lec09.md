---
id: I9AvI9DweOK4kIROxWEp2
title: Lec09
desc: ''
updated: 1637539305185
created: 1637530120235
---

\section{III.E The H-Theorem and Irreversibility}

The second question posed at the beginning of this chapter was whether a collection of particles naturally evolves towards an equilibrium state. While it is possible to obtain steady state solutions for the full phase space density $\rho_{N}$, because of time reversal symmetry these solutions are not attractors of generic non-equilibrium densities. Does the unconditional one particle PDF $\rho_{1}$, suffer the same problem? While the exact density $\rho_{1}$ must necessarily reflect this property of $\rho_{N}$, the $\mathrm{H}$ -theorem proves that an approximate $\rho_{1}$, governed by the Boltzmann equation, does in fact non-reversibly approach an equilibrium form. This theorem states that:

- If $f_{1}(\vec{p}, \vec{q}, t)$ satisfies the Boltzmann equation, then $d \mathrm{H} / d t \leq 0$, where

$$
\mathrm{H}(t)=\int d^{3} \vec{p} d^{3} \vec{q} f_{1}(\vec{p}, \vec{q}, t) \ln f_{1}(\vec{p}, \vec{q}, t)
$$

The function $\mathrm{H}(t)$ is related to the information content of the one particle PDF. Up to an overall constant, the information content of $\rho_{1}=f_{1} / N$ is given by $I\left[\rho_{1}\right]=\left\langle\ln \rho_{1}\right\rangle$, which is clearly similar to $\mathrm{H}(t)$.

Proof: The time derivative of $\mathrm{H}$ is

$$
\frac{d \mathrm{H}}{d t}=\int d^{3} \vec{p}_{1} d^{3} \vec{q}_{1} \frac{\partial f_{1}}{\partial t}\left(\ln f_{1}+1\right)=\int d^{3} \vec{p}_{1} d^{3} \vec{q}_{1} \ln f_{1} \frac{\partial f_{1}}{\partial t}
$$

since $\int d V_{1} f_{1}=N \int d \Gamma \rho=N$ is time independent. Using eq.(III.41), we obtain

$$
\begin{gathered}
\frac{d \mathrm{H}}{d t}=\int d^{3} \vec{p}_{1} d^{3} \vec{q}_{1} \ln f_{1}\left(\frac{\partial U}{\partial \vec{q}_{1}} \cdot \frac{\partial f_{1}}{\partial \vec{p}_{1}}-\frac{\vec{p}_{1}}{m} \cdot \frac{\partial f_{1}}{\partial \vec{q}_{1}}\right) \\
-\int d^{3} \vec{p}_{1} d^{3} \vec{q}_{1} d^{3} \vec{p}_{2} d^{2} \sigma\left|\vec{v}_{1}-\vec{v}_{2}\right|\left[f_{1}\left(\vec{p}_{1}, \vec{q}_{1}\right) f_{1}\left(\vec{p}_{2}, \vec{q}_{1}\right)-f_{1}\left(\vec{p}_{1}^{\prime}, \vec{q}_{1}\right) f_{1}\left(\vec{p}_{2}^{\prime}, \vec{q}_{1}\right)\right] \ln f_{1}\left(\vec{p}_{1}, \vec{q}_{1}\right)
\end{gathered}
$$

where we shall interchangeably use $d^{2} \sigma, d^{2} \vec{b}$, or $d^{2} \Omega|d \sigma / d \Omega|$ for the differential crosssection. The streaming terms in the above expression are zero, as shown through successive integrations by part,

$$
\int d^{3} \vec{p}_{1} d^{3} \vec{q}_{1} \ln f_{1} \frac{\partial U}{\partial \vec{q}_{1}} \cdot \frac{\partial f_{1}}{\partial \vec{p}_{1}}=-\int d^{3} \vec{p}_{1} d^{3} \vec{q}_{1} f_{1} \frac{\partial U}{\partial \vec{q}_{1}} \cdot \frac{1}{f_{1}} \frac{\partial f_{1}}{\partial \vec{p}_{1}}=\int d^{3} \vec{p}_{1} d^{3} \vec{q}_{1} f_{1} \frac{\partial}{\partial \vec{p}_{1}} \cdot \frac{\partial U}{\partial \vec{q}_{1}}=0
$$

and

$$
\int d^{3} \vec{p}_{1} d^{3} \vec{q}_{1} \ln f_{1} \frac{\vec{p}_{1}}{m} \cdot \frac{\partial f_{1}}{\partial \vec{q}_{1}}=-\int d^{3} \vec{p}_{1} d^{3} \vec{q}_{1} f_{1} \frac{\vec{p}_{1}}{m} \cdot \frac{1}{f_{1}} \frac{\partial f_{1}}{\partial \vec{q}_{1}}=\int d^{3} \vec{p}_{1} d^{3} \vec{q}_{1} f_{1} \frac{\partial}{\partial \vec{q}_{1}} \cdot \frac{\vec{p}_{1}}{m}=0
$$

The collision term in eq.(III.44) involves integrations over dummy variables $\vec{p}_{1}$ and $\vec{p}_{2}$. The labels (1) and (2) can thus be exchanged without any change in the value of the integral. Averaging the resulting two expressions gives

$$
\frac{d \mathrm{H}}{d t}=-\frac{1}{2} \int d^{3} \vec{q} d^{3} \vec{p}_{1} d^{3} \vec{p}_{2} d^{2} \vec{b}\left|\vec{v}_{1}-\vec{v}_{2}\right|\left[f_{1}\left(\vec{p}_{1}\right) f_{1}\left(\vec{p}_{2}\right)-f_{1}\left(\vec{p}_{1}^{\prime}\right) f_{1}\left(\vec{p}_{2}^{\prime}\right)\right] \ln \left(f_{1}\left(\vec{p}_{1}\right) f_{1}\left(\vec{p}_{2}\right)\right)
$$

(The arguments, $\vec{q}$ and $t$, of $f_{1}$ are suppressed for ease of notation.) We would now like to change the variables of integrations from the coordinates describing the initiators of the collision, $\left(\vec{p}_{1}, \vec{p}_{2}, \vec{b}\right)$, to those of their products, $\left(\vec{p}_{1}^{\prime}, \vec{p}_{2}^{\prime}, \vec{b}^{\prime}\right) .$ The explicit functional forms describing this transformation are complicated because of the dependence of the solid angle $\hat{\Omega}$ in eq.(III.39) on $\vec{b}$ and $\left|\vec{p}_{2}-\vec{p}_{1}\right| .$ However, we are assured that the Jacobian of the transformation is unity because of time reversal symmetry; since for every collision there is an inverse one obtained by reversing the momenta of the products. In terms of the new coordinates

$$
\frac{d \mathrm{H}}{d t}=-\frac{1}{2} \int d^{3} \vec{q} d^{3} \vec{p}_{1}^{\prime} d^{3} \vec{p}_{2}^{\prime} d^{2} \vec{b}^{\prime}\left|\vec{v}_{1}-\vec{v}_{2}\right|\left[f_{1}\left(\vec{p}_{1}\right) f_{1}\left(\vec{p}_{2}\right)-f_{1}\left(\vec{p}_{1}^{\prime}\right) f_{1}\left(\vec{p}_{2}^{\prime}\right)\right] \ln \left(f_{1}\left(\vec{p}_{1}\right) f_{1}\left(\vec{p}_{2}\right)\right)
$$

where we should now regard $\left(\vec{p}_{1}, \vec{p}_{2}\right)$ in the above equation, as functions of the integration variables $\left(\vec{p}_{1}^{\prime}, \vec{p}_{2}^{\prime}, \vec{b}^{\prime}\right)$ as in eq.(III.39). As noted earlier, $\left|\vec{v}_{1}-\vec{v}_{2}\right|=\left|\vec{v}_{1}^{\prime}-\vec{v}_{2}^{\prime}\right|$ for any elastic collision, and we can use these quantities interchangeably. Finally, we relabel the dummy integration variables such that the primes are removed. Noting that the functional dependence of $\left(\vec{p}_{1}, \vec{p}_{2}, \vec{b}\right)$ on $\left(\vec{p}_{1}^{\prime}, \vec{p}_{2}^{\prime}, \vec{b}^{\prime}\right)$ is exactly the same as its inverse, we obtain

$$
\frac{d \mathrm{H}}{d t}=-\frac{1}{2} \int d^{3} \vec{q} d^{3} \vec{p}_{1} d^{3} \vec{p}_{2} d^{2} \vec{b}\left|\vec{v}_{1}-\vec{v}_{2}\right|\left[f_{1}\left(\vec{p}_{1}^{\prime}\right) f_{1}\left(\vec{p}_{2}^{\prime}\right)-f_{1}\left(\vec{p}_{1}\right) f_{1}\left(\vec{p}_{2}\right)\right] \ln \left(f_{1}\left(\vec{p}_{1}^{\prime}\right) f_{1}\left(\vec{p}_{2}^{\prime}\right)\right)
$$

Averaging eqs.(III.45) and (III.47) results in

$$
\begin{aligned}
\frac{d \mathrm{H}}{d t}=-\frac{1}{4} \int d^{3} \vec{q} d^{3} \vec{p}_{1} d^{3} \vec{p}_{2} d^{2} \vec{b}\left|\vec{v}_{1}-\vec{v}_{2}\right|\left[f_{1}\left(\vec{p}_{1}\right) f_{1}\left(\vec{p}_{2}\right)-f_{1}\left(\vec{p}_{1}^{\prime}\right) f_{1}\left(\vec{p}_{2}^{\prime}\right)\right] \\
\left[\ln \left(f_{1}\left(\vec{p}_{1}\right) f_{1}\left(\vec{p}_{2}\right)\right)-\ln \left(f_{1}\left(\vec{p}_{1}^{\prime}\right) f_{1}\left(\vec{p}_{2}^{\prime}\right)\right)\right]
\end{aligned}
$$

The integrand of the above expression is always positive. If $f_{1}\left(\vec{p}_{1}\right) f_{1}\left(\vec{p}_{2}\right)>f_{1}\left(\vec{p}_{1}^{\prime}\right) f_{1}\left(\vec{p}_{2}^{\prime}\right)$ both terms in square brackets are positive, while both are negative if $f_{1}\left(\vec{p}_{1}\right) f_{1}\left(\vec{p}_{2}\right)<$ $f_{1}\left(\vec{p}_{1}^{\prime}\right) f_{1}\left(\vec{p}_{2}^{\prime}\right) .$ In either case, their product is positive. The positivity of the integrand establishes the validity of the H-theorem,

$$
\frac{d \mathrm{H}}{d t} \leq 0
$$

- Irreversibility: The second law is an empirical formulation of the vast number of everyday observations which support the existence of an arrow of time. Reconciling the reversibility of laws of physics governing the microscopic domain with the observed irreversibility of macroscopic phenomena is a fundamental problem. Of course, not all microscopic laws of physics are reversible: weak nuclear interactions violate time reversal symmetry, and the collapse of the quantum wave-function in the act of observation is irreversible. The former interactions in fact do not play any significant role in everyday observations that lead to the second law. The irreversible collapse of the wave-function may itself be an artifact of treating macroscopic observers and microscopic observables distinctly. $^{\dagger}$ There are proponents of the view that the reversibility of the currently accepted microscopic equations of motion (classical or quantum) is indicative of their inadequacy. However, the advent of powerful computers has made it possible to simulate the evolution of collections of large numbers of particles, governed by classical, reversible equations of motion. Although simulations are currently limited to relatively small numbers of particles $\left(10^{6}\right)$, they do exhibit the irreversible macroscopic behaviors similar to those observed in nature (typically involving $10^{23}$ particles). For example, particles initially occupying one half of a box proceed to irreversibly, and uniformly, occupy the whole box. (This has nothing to do with limitations of computational accuracy; the same macroscopic irreversibility is observed in exactly reversible integer based simulations, such as with cellular automata.) Thus the origin of the observed irreversibilities should be sought in the classical evolution of large collections of particles.

The Boltzmann equation is the first formula we have encountered that is clearly not time reversible, as indicated by eq.(III.49). We can thus ask the question of how we obtained this result from the Hamiltonian equations of motion. The key to this, of course, resides in the physically motivated approximations used to obtain eq.(III.41). The first steps of the approximation were dropping the three body collision term on the right hand side of eq.(III.30), and the implicit coarse-graining of the resolution in the spatial and temporal scales. Neither of these steps explicitly violates time reversal symmetry, and the collision term in eq.(III.37) retains this property. The next step in getting to eq.(III.41) is to replace the two-body density $f_{2}(-)$, evaluated before the collision, with the product of two one body densities according to eq.(III.32). This treats the two body densities before

$\dagger$ The time dependent Schrödinger equation is fully time reversible. If it is possible to write a complicated wave-function that includes the observing apparatus (possibly the whole universe), it is hard to see how any irreversibility may occur. and after the collision differently. We could have alternatively expressed eq.(III.37) in terms of the two body densities $f_{2}(+)$ evaluated after the collision. Replacing $f_{2}(+)$ with the product of two one particle densities would then lead to the opposite conclusion, with $d \mathrm{H} / d t \geq 0 !$ For a system in equilibrium, it is hard to justify one choice over the other. However, once the system is out of equilibrium, the coordinates after the collision are more quite likely to be correlated, and hence the substitution of eq.(III.32) for $f_{2}(+)$ does not make sense. Time reversal symmetry implies that there should also be subtle correlations in $f_{2}(-)$ which are ignored in the so-called assumption of molecular chaos.

While the assumption of molecular chaos before (but not after) collisions is the key to the irreversibility of the Boltzmann equation, the resulting loss of information is best justified in terms of the coarse graining of space and time: The Liouville equation and its descendants contain precise information about the evolution of a pure state. This information, however, is inevitably transported to shorter scales. A useful image is that of mixing two immiscible fluids. While the two fluids remain distinct at each point, the transitions in space from one to the next occur at finer resolution on subsequent mixing. At some point, a finite resolution in any measuring apparatus will prevent keeping track of the two components. In the Boltzmann equation the precise information of the pure state is lost at the scale of collisions. The resulting one body density only describes space and time resolutions longer than those of a two-body collision, becoming more and more probabilistic as further information is lost.

\section{III.F Equilibrium Properties}

What is the nature of the equilibrium state described by $f_{1}$, for a homogeneous gas? (1) The equilibrium distribution: After the gas has reached equilibrium, the function $\mathrm{H}$ should no longer decrease with time. Since the integrand in eq.(III.48) is always positive, a necessary condition for $d \mathrm{H} / d t=0$ is that

$$
f_{1}\left(\vec{p}_{1}, \vec{q}_{1}\right) f_{1}\left(\vec{p}_{2}, \vec{q}_{1}\right)-f_{1}\left(\vec{p}_{1}^{\prime}, \vec{q}_{1}\right) f_{1}\left(\vec{p}_{2}^{\prime}, \vec{q}_{1}\right)=0
$$

i.e. at each point $\vec{q}$, we must have

$$
\ln f_{1}\left(\vec{p}_{1}, \vec{q}\right)+\ln f_{1}\left(\vec{p}_{2}, \vec{q}\right)=\ln f_{1}\left(\vec{p}_{1}^{\prime}, \vec{q}\right)+\ln f_{1}\left(\vec{p}_{2}^{\prime}, \vec{q}\right)
$$

The left hand side of the above equation refers to the momenta before a two-body collision, and the right hand side to the those after the collision. The equality is thus satisfied by any additive quantity that is conserved during the collision. There are 5 such conserved quantities for an elastic collision: the particle number, the three components of the net momentum, and the kinetic energy. Hence, a general solution for $f_{1}$ is

$$
\ln f_{1}=a(\vec{q})-\vec{\alpha}(\vec{q}) \cdot \vec{p}-\beta(\vec{q})\left(\frac{\vec{p}^{2}}{2 m}\right)
$$

We can easily accomodate the potential energy $U(\vec{q})$ in the above form, and set

$$
f_{1}(\vec{p}, \vec{q})=\mathcal{N}(\vec{q}) \exp \left[-\vec{\alpha}(\vec{q}) \cdot \vec{p}-\beta(\vec{q})\left(\frac{p^{2}}{2 m}+U(\vec{q})\right)\right]
$$

We shall refer to the above distribution as describing local equilibrium. While this form is preserved during collisions, it will evolve in time away from collisions, due to the streaming terms, unless $\left\{\mathcal{H}_{1}, f_{1}\right\}=0 .$ The latter condition is satisfied for any function $f_{1}$ that depends only on $\mathcal{H}_{1}$, or any other quantity that is conserved by it. Clearly, the above density satisfies this requirement as long as $\mathcal{N}$, and $\beta$ are independent of $\vec{q}$, and $\vec{\alpha}=0$.

According to eq.(III.16), the appropriate normalization for $f_{1}$ is

$$
\int d^{3} \vec{p} d^{3} \vec{q} f_{1}(\vec{p}, \vec{q})=N
$$

For particles in a box of volume $V$, the potential $U(\vec{q})$ is zero inside the box, and infinite on the outside. The normalization factor in eq.(III.53) can be obtained from eq.(III.54) as

$$
N=\mathcal{N} V\left[\int_{-\infty}^{\infty} d p_{i} \exp \left(-\alpha_{i} p_{i}-\frac{\beta p_{i}^{2}}{2 m}\right)\right]^{3}=\mathcal{N} V\left(\frac{2 \pi m}{\beta}\right)^{3 / 2} \exp \left(\frac{m \alpha^{2}}{2 \beta}\right)
$$

Hence, the properly normalized Gaussian distribution for momenta is

$$
f_{1}(\vec{p}, \vec{q})=n\left(\frac{\beta}{2 \pi m}\right)^{3 / 2} \exp \left[-\frac{\beta\left(\vec{p}-\vec{p}_{0}\right)^{2}}{2 m}\right]
$$

where $\vec{p}_{0}=\langle\vec{p}\rangle=m \vec{\alpha} / \beta$ is the mean value for the momentum of the gas, which is zero for a stationary box, and $n=N / V$ is the particle density. From the Gaussian form of the distribution it can be easily concluded that the variance of each component of the momentum is $\left\langle p_{i}^{2}\right\rangle=m / \beta$, and

$$
\left\langle p^{2}\right\rangle=\left\langle p_{x}^{2}+p_{y}^{2}+p_{z}^{2}\right\rangle=\frac{3 m}{\beta}
$$

(2) Equilibrium between two gases: Consider two different gases (a) and (b), moving in the same potential $U$, and subject to a two-body interaction $\mathcal{V}_{a b}\left(\vec{q}^{(a)}-\vec{q}^{(b)}\right) .$ We can define one-particle densities, $f_{1}^{(a)}$, and, $f_{1}^{(b)}$, for the two gases respectively. In terms of a generalized collision integral

$C_{\alpha, \beta}=-\int d^{3} \vec{p}_{2} d^{2} \Omega\left|\frac{d \sigma_{\alpha, \beta}}{d \Omega}\right|\left|\vec{v}_{1}-\vec{v}_{2}\right|\left[f_{1}^{(\alpha)}\left(\vec{p}_{1}, \vec{q}_{1}\right) f_{1}^{(\beta)}\left(\vec{p}_{2}, \vec{q}_{1}\right)-f_{1}^{(\alpha)}\left(\vec{p}_{1}^{\prime}, \vec{q}_{1}\right) f_{1}^{(\beta)}\left(\vec{p}_{2}^{\prime}, \vec{q}_{1}\right)\right]$

the evolution of these densities is governed by a simple generalization of the Boltzmann equation to

$$
\left\{\begin{array}{l}
\frac{\partial f_{1}^{(a)}}{\partial t}=-\left\{f_{1}^{(a)}, \mathcal{H}_{1}^{(a)}\right\}+C_{a, a}+C_{a, b} \\
\frac{\partial f_{1}^{(b)}}{\partial t}=-\left\{f_{1}^{(b)}, \mathcal{H}_{1}^{(b)}\right\}+C_{b, a}+C_{b, b}
\end{array}\right.
$$

Stationary distributions can be obtained if all six terms on the right hand side of eqs.(III.59) are zero. In the absence of inter-species collisions, i.e. for $C_{a, b}=C_{b, a}$, we can obtain independent stationary distributions $f_{1}^{(a)} \propto \exp \left(-\beta_{a} \mathcal{H}_{1}^{(a)}\right)$ and $f_{1}^{(b)} \propto \exp \left(-\beta_{b} \mathcal{H}_{1}^{(b)}\right)$ Requiring the vanishing of $C_{a, b}$ leads to the additional constraint,

$$
\begin{gathered}
f_{1}^{(a)}\left(\vec{p}_{1}\right) f_{1}^{(b)}\left(\vec{p}_{2}\right)-f_{1}^{(a)}\left(\vec{p}_{1}^{\prime}\right) f_{1}^{(b)}\left(\vec{p}_{2}^{\prime}\right)=0, \quad \Longrightarrow \\
\beta_{a} \mathcal{H}_{1}^{(a)}\left(\vec{p}_{1}\right)+\beta_{b} \mathcal{H}_{1}^{(b)}\left(\vec{p}_{2}\right)=\beta_{a} \mathcal{H}_{1}^{(a)}\left(\vec{p}_{1}^{\prime}\right)+\beta_{b} \mathcal{H}_{1}^{(b)}\left(\vec{p}_{2}^{\prime}\right)
\end{gathered}
$$

Since the total energy $\mathcal{H}_{1}^{(a)}+\mathcal{H}_{1}^{(b)}$ is conserved in a collision, the above equation can be satisfied for $\beta_{a}=\beta_{b}=\beta .$ From eq.(III.57) this condition implies the equality of the kinetic energies of the two species,

$$
\left\langle\frac{p_{a}^{2}}{2 m_{a}}\right\rangle=\left\langle\frac{p_{b}^{2}}{2 m_{b}}\right\rangle=\frac{3}{2 \beta}
$$

The parameter $\beta$ thus plays the role of an empirical temperature describing the equilibrium of gases.

(3) The equation of state: To complete the identification of $\beta$ with temperature $T$, consider a gas of $N$ particles confined to a box of volume $V$. The gas pressure results from the force exerted by the particles colliding with the walls of the container. Consider a wall element of area $A$ perpendicular to the $x$ direction. The number of particles impacting this area, with momenta in the interval $[\vec{p}, \vec{p}+d \vec{p}]$, over a time period $\delta t$, is

$$
d \mathcal{N}(\vec{p})=\left(f_{1}(\vec{p}) d^{3} \vec{p}\right)\left(A v_{x} \delta t\right)
$$

The final factor in the above expression is the volume of a cylinder of height $v_{x} \delta t$ perpendicular to the area element $A$. Only particles within this cylinder are close enough to impact the wall during $\delta t$. As each collision imparts a momentum $2 p_{x}$ to the wall, the net force exerted is

$$
F=\frac{1}{\delta t} \int_{-\infty}^{0} d p_{x} \int_{-\infty}^{\infty} d p_{y} \int_{-\infty}^{\infty} d p_{z} f_{1}(\vec{p})\left(A \frac{p_{x}}{m} \delta t\right)\left(2 p_{x}\right)
$$

As only particles with velocities directed towards the wall will hit it, the first integral is over half of the range of $p_{x} .$ Since the integrand is even in $p_{x}$, this restriction can be removed by dividing the full integral by $2 .$ The pressure $P$ is then obtained from the force per unit area as

$$
P=\frac{F}{A}=\int d^{3} \vec{p} f_{1}(\vec{p}) \frac{p_{x}^{2}}{m}=\frac{1}{m} \int d^{3} \vec{p} p_{x}^{2} n\left(\frac{\beta}{2 \pi m}\right)^{3 / 2} \exp \left(-\frac{\beta p^{2}}{2 m}\right)=\frac{n}{\beta}
$$

where eq.(III.56) is used for the equilibrium form of $f_{1}$. Comparing with the standard equation of state, $P V=N k_{B} T$, for an ideal gas, leads to the identification, $\beta=1 / k_{B} T$

(4) Entropy: As discussed earlier, the Boltzmann H-function is closely related to the information content of the one-particle PDF $\rho_{1} .$ We can also define a corresponding Boltzmann entropy,

$$
S_{B}(t)=-k_{B} \mathrm{H}(t)
$$

where the constant $k_{B}$ reflects the historical origins of entropy. The H-theorem implies that $S_{B}$ can only increase with time in approaching equilibrium. It has the further advantage of being defined through eq.(III.42) for situations that are clearly out of equilibrium. For a gas in equilibrium in a box of volume $V$, from eq.(III.56), we compute

$$
\begin{aligned}
\mathrm{H} &=V \int d^{3} \vec{p} f_{1}(\vec{p}) \ln f_{1}(\vec{p}) \\
&=V \int d^{3} \vec{p} \frac{N}{V}\left(2 \pi m k_{B} T\right)^{-3 / 2} \exp \left(-\frac{p^{2}}{2 m k_{B} T}\right)\left[\ln \left(\frac{n}{\left(2 \pi m k_{B} T\right)^{3 / 2}}\right)-\frac{p^{2}}{2 m k_{B} T}\right] \\
&=N\left[\ln \left(\frac{n}{\left(2 \pi m k_{B} T\right)^{3 / 2}}\right)-\frac{3}{2}\right]
\end{aligned}
$$

The entropy is now identified as

$$
S_{B}=-k_{B} \mathrm{H}=N k_{B}\left[\frac{3}{2}+\frac{3}{2} \ln \left(2 \pi m k_{B} T\right)-\ln \left(\frac{N}{V}\right)\right]
$$

The thermodynamic relation, $T d S_{B}=d E+P d V$, implies

$$
\begin{aligned}
\left.\frac{\partial E}{\partial T}\right|_{V} &=\left.T \frac{\partial S_{B}}{\partial T}\right|_{V}=\frac{3}{2} N k_{B} \\
P+\left.\frac{\partial E}{\partial V}\right|_{T} &=\left.T \frac{\partial S_{B}}{\partial V}\right|_{T}=\frac{N k_{B} T}{V}
\end{aligned}
$$

The usual properties of a monatomic ideal gas, $P V=N k_{B} T$, and $E=3 N k_{B} T / 2$, can now be obtained from the above equations. Also note that for this classical gas, the zero temperature limit of the entropy in eq.(III.67) is not independent of the density $n$, in violation of the third law of thermodynamics. MIT OpenCourseWare

http://ocw.mit.edu

\subsection{Statistical Mechanics I: Statistical Mechanics of Particles \\ Fall 2013}

For information about citing these materials or our Terms of Use, visit: http://ocw.mit.edu/terms.
