\section{V.C The Second Virial Coefficient \& van der Waals Equation}

Let us study the second virial coefficient $B_{2}$, for a typical gas using eq.(V.33). As discussed before, the two-body potential is characterized by a hard core repulsion at short distances and a van der Waals attraction at large distances. To make the computations easier, we shall use the following approximation for the potential,

$$
\mathcal{V}(r)= \begin{cases}+\infty & \text { for } r<r_{0} \\ -u_{0}\left(r_{0} / r\right)^{6} & \text { for } r>r_{0}\end{cases}
$$

which combines both features. The contributions of the two portions can then be calculated separately as,

$$
\begin{aligned}
\delta_{2} &=\int_{0}^{\infty} d^{3} \vec{r}\left(e^{-\beta \mathcal{V}(r)}-1\right) \\
&=\int_{0}^{r_{0}} 4 \pi r^{2} d r(-1)+\int_{r_{0}}^{\infty} 4 \pi r^{2} d r\left[e^{+\beta u_{0}\left(r_{0} / r\right)^{6}}-1\right]
\end{aligned}
$$

The second integrand can be approximated by $\beta u_{0}\left(r_{0} / r\right)^{6}$ in the high temperature limit, $\beta u_{0} \gg 1$, and leads to

$$
B_{2}=-\frac{1}{2}\left[-\frac{4 \pi r_{0}^{3}}{3}+\left.4 \pi \beta u_{0} r_{0}^{6}\left(-\frac{r^{-3}}{3}\right)\right|_{r_{0}} ^{\infty}\right]=\frac{2 \pi r_{0}^{3}}{3}\left(1-\beta u_{0}\right)
$$

We can define an excluded volume of $\Omega=4 \pi r_{0}^{3} / 3$ which is 8 times the atomic volume (since the distance of minimum approach $r_{0}$, is twice an atomic radius), to get

$$
B_{2}(T)=\frac{\Omega}{2}\left(1-\frac{u_{0}}{k_{B} T}\right)
$$

- Remarks and observations:

(1) The tail of the van der Waals attractive potential $\left(\propto r^{-6}\right)$ extends to very long separations. Yet, its integral in eq.(V.39) is dominated by contributions from the short scales $r_{0} .$ In this limited context, the van der Waals potential is short-ranged, and results in corrections to the ideal gas behavior that are analytical in density $n$, leading to the virial series.

(2) By contrast, potentials that fall off with separation as $1 / r^{3}$ or slower, are long-ranged. The integral appearing in calculation of the second virial coefficient is dominated by long distances, and is divergent. As a result, corrections to the ideal gas behavior can not be written in the form of a virial series, and are in fact non-analytic. A good example is provided by the Coulomb interactions (see problems for the test), where the non-analytic corrections can be obtained by summing all the ring diagrams in the cumulant (or cluster) expansions.

(3) The second virial coefficient has dimensions of volume, and (for short-range potentials) is proportional to the atomic volume $\Omega .$ In the high temperature limit, the importance of corrections to ideal gas behavior can be estimated by comparing the first two terms of eq. $(\mathrm{V} .14)$

$$
\frac{B_{2} n^{2}}{n}=\frac{B_{2}}{n^{-1}} \sim \frac{\text { Atomic volume }}{\text { volume per particle in gas }} \sim \frac{\text { gas density }}{\text { liquid density }}
$$

This ratio is roughly $10^{-3}$ for air at room temperature and pressure. The corrections to ideal gas behavior are thus small at low densities. On dimensional grounds, a similar ratio is expected for the higher order terms, $B_{\ell} n^{\ell} / B_{\ell-1} n^{\ell-1}$, in the virial series. We may thus suspect the convergence of the series at high enough densities (when the gas liquifies).

(4) The virial expansion breaks down not only at high densities, but also at low temperatures. This is suggested by the divergences in eqs.(V.40) and (V.38) as $T \rightarrow 0$, and reflects the fact that in the presence of attractive interactions the particles can lower their energy at low temperatures by condensing into a liquid state.

(5) The truncated virial expansion,

$$
\frac{P}{k_{B} T}=n+\frac{\Omega}{2}\left(1-\frac{u_{0}}{k_{B} T}\right) n^{2}+\cdots
$$

can be rearranged as

$$
\frac{1}{k_{B} T}\left(P+\frac{u_{0} \Omega}{2} n^{2}\right)=n\left(1+n \frac{\Omega}{2}+\cdots\right) \approx \frac{n}{1-n \Omega / 2}=\frac{N}{V-N \Omega / 2}
$$

This is precisely in the form of the van der Waals equation

$$
\left[P+\frac{u_{0} \Omega}{2}\left(\frac{N}{V}\right)^{2}\right]\left[V-\frac{N \Omega}{2}\right]=N k_{B} T
$$

and we can identify the van der Waals parameters, $a=u_{0} \Omega / 2$ and $b=\Omega / 2$.

- Physical interpretation of the van der Waals equation: Historically, van der Waals suggested eq.(V.44) on the basis of experimental results for the equation of state of various gases, towards the end of the19th century. At that time the microscopic interactions between gas particles were not known, and van der Waals postulated the necessity of an attractive interaction between gas atoms based on the observed decreases in pressure. It was only later on that such interactions were observed directly, and then attributed to the induced dipole-dipole forces by London. The physical justification of the correction terms is as follows.

(a) There is a correction to the gas volume $V$ due to the hard core exclusions. At first sight, it may appear surprising that the excluded volume $b$, in eq.(V.44) is one half of the volume that is excluded around each particle. This is because this factor measures a joint excluded volume involving all particles in phase space. In fact, the contribution of coordinates to the partition function of the hard-core gas can be estimated at low densities, from

$$
\mathcal{S}_{N}=\int^{\prime} \frac{\prod_{i} d^{3} \vec{q}_{i}}{N !}=\frac{1}{N !} V(V-\Omega)(V-2 \Omega) \cdots(V-(N-1) \Omega) \approx \frac{1}{N !}\left(V-\frac{N \Omega}{2}\right)^{N}
$$

The above result is obtained by adding particles one at a time, and noting that the available volume for the $m^{\text {th }}$ particle is $(V-m \Omega)$. At low densities, the overall effect is a reduction of the volume available to each particle by approximately $\Omega / 2 .$ Of course, the above result is only approximate, since the effects of excluded volume involving more than two particles are not correctly taken into account. The relatively simple form of eq.(V.45) is only exact at for spatial dimensions $d=1$ and infinity. As proved in problems for the test, the exact excluded volume in $d=1$ is in fact $\Omega$.

(b) The decrease in pressure $P$, due to attractive interactions, is somewhat harder to quantify. In sec.III.F, the gas pressure was related to the impacts of particles on a wall via

$$
P=\left.\overline{\left(n v_{x}\right)\left(2 m v_{x}\right)}\right|_{v_{x}<0}=n m \overline{v_{x}^{2}}
$$

where the first term is the number of collisions per unit time and area, while the second is the momentum imparted by each particle. For the ideal gas, the usual equation of state is recovered by noting that the average kinetic energy is $m \overline{v_{x}^{2}} / 2=k_{B} T / 2 . \quad$ Attractive interactions lead to a reduction in pressure given by

$$
\delta P=\delta n\left(m \overline{v_{x}^{2}}\right)+n \delta\left(m \overline{v_{x}^{2}}\right)
$$

While different statistical ensembles give the same pressure, which is a bulk state function, they may lead to different behaviors at the surface. We must thus be careful, and consistent, in evaluation of eq.(V.47), which depends of surface properties. In a canonical ensemble, the gas density is reduced at the walls. This is because the particles in the middle of the box experience an attractive potential $V$ from all sides, while at the edge only an attractive energy of $V / 2$ is available from half of the space. The resulting change in density is approximately

$$
\delta n \approx n\left(e^{-\beta V / 2}-e^{-\beta V}\right) \approx \beta n V / 2
$$

Integrating the interaction of one particle in the bulk with the rest gives

$$
V=\int d^{3} \vec{r} \mathcal{V}_{\mathrm{attr} .}(r) n=-n \Omega u_{0}
$$

The change in density thus gives the pressure correction of $\delta P=-n^{2} \Omega u_{0} / 2$ calculated in eq.(V.44). There is no correction to the kinetic energy of the particles impinging on the wall, since in the canonical formulation the probabilites for momentum and location of the particles are independent variables. The probability distribution for momentum is uniform in space, giving the average kinetic energy of $k_{B} T / 2$ for each direction of motion.

A different explanation is presented in a kinetic formulation in which particles follow the deterministic Hamiltonian equations of motion. In this formulation, the impinging particles lose kinetic energy in approaching the wall from the surface, since they have to climb out of the potential well set up by the attractions of bulk particles. The reduction in kinetic energy is given by

$$
\delta \frac{m v_{x}^{2}}{2}=\frac{1}{2} \int d^{3} \vec{r} \mathcal{V}_{\mathrm{attr} .}(r) n=-\frac{1}{2} n \Omega u_{0}
$$

The reduced velocities lead to an increase in the surface density in this case, as the slower particles spend a longer time $\tau$ in the vicinity of the wall! The relative change in density is given by

$$
\frac{\delta n}{n}=\frac{\delta \tau}{\tau}=-\frac{\delta v_{x}}{v_{x}}=-\frac{1}{2} \frac{\delta v_{x}^{2}}{v_{x}^{2}}, \quad \Longrightarrow \quad \delta n=-\beta n V / 2
$$

The increase in density is precisely the opposite of the result of eq.(V.48) in the canonical formulation. However, with the decrease in kinetic energy calculated in eq.(V.50), it again leads to the correct reduction in pressure. 

\section{V.D Breakdown of the van der Waals equation}

As discussed in sec.I.I, mechanical stability of a gas requires the positivity of the isothermal compressibility, $\kappa_{T}=-V^{-1} \partial V /\left.\partial P\right|_{T} .$ This condition can be obtained by examining density fluctuations in a grand canonical ensemble. The probability of finding $N$ particles in a volume $V$ is given by eq.(IV.102) as

$$
p(N, V)=\frac{e^{\beta \mu N} Z(T, N, V)}{\mathcal{Q}}
$$

Since for a gas $\ln \mathcal{Q}=-\beta \mathcal{G}=P V / k_{B} T$, eqs. $(\mathrm{IV} .103)$ and (IV.104) simplify to

$$
\left\{\begin{array}{c}
\langle N\rangle_{c}=N=\frac{\partial(\ln \mathcal{Q})}{\partial(\beta \mu)}=\left.V \frac{\partial P}{\partial \mu}\right|_{T, V} \\
\left\langle N^{2}\right\rangle_{c}=\frac{\partial^{2}(\ln \mathcal{Q})}{\partial(\beta \mu)^{2}}=\frac{\partial\langle N\rangle_{c}}{\partial(\beta \mu)}=\left.k_{B} T \frac{\partial N}{\partial \mu}\right|_{T, V}
\end{array}\right.
$$

Dividing the two equations, and using the chain rule, results in

$$
\frac{\left\langle N^{2}\right\rangle_{c}}{N}=\left.\frac{k_{B} T}{V} \frac{\partial N}{\partial P}\right|_{T, V}=-\left.\left.\frac{k_{B} T}{V} \frac{\partial N}{\partial V}\right|_{P, T} \frac{\partial V}{\partial P}\right|_{N, T}=n k_{B} T \kappa_{T}
$$

The positivity of $\kappa_{T}$ is thus tied to that of the variance of $N$. A stable value of $N$ corresponds to a maximum of the probability $p(N, V)$, i.e. a positive compressibility. A negative $\kappa_{T}$ actually corresponds to a minimum in $p(N, V)$ implying that the system is least likely to be found at such densities. Fluctuations in density will then occur spontaneously and change the density to a stable value.

Any approximate equation of state, such as the van der Waals equation, must at least satisfy the stability requirements. However, the van der Waals isotherms contain a portion with $-\partial P /\left.\partial V\right|_{T}<0$, for temperatures less than a critical value $T_{c} .$ The negative compressibility implies an instability towards forming domains of lower and higher density, i.e. phase separation. The attractive interactions in real gases do indeed result in a liquidgas phase separation at low temperatures. The isotherms then include a flat portion, $\partial P /\left.\partial V\right|_{T}=0$, at the coexistence of the two phases. Can the (unstable) van der Waals isotherms be used to construct the phase diagram of a real gas?

One way of doing so is by the following Maxwell construction: The variations of the chemical potential $\mu(T, P)$, along an isotherm are obtained by integrating eq.(V.53), as

$$
d \mu=\frac{V}{N} d P, \quad \Longrightarrow \quad \mu(T, P)=\mu\left(T, P_{A}\right)+\int_{P_{A}}^{P} d P^{\prime} \frac{V\left(T, P^{\prime}\right)}{N}
$$

Since the van der Waals isotherms for $T<T_{c}$ are non-monotonic, there is a range of pressures that correspond to three different values, $\left\{\mu_{\alpha}\right\}$, of the chemical potential. The possibility of several values of $\mu$ at a given temperature and pressure indicates phase coexistence. In equilibrium, the number of particles in each phase $N_{\alpha}$, adjusts so as to minimize the Gibbs free energy $G=\sum_{\alpha} \mu_{\alpha} N_{\alpha} .$ Clearly, the phase with lowest $\mu_{\alpha}$ will acquire all the particles. A phase transition occurs when two branches of allowed chemical potentials intersect. From eq.(V.55), the critical pressure $P_{c}$, for this intersection is obtained from the condition

$$
\oint_{P_{c}}^{P_{c}} d P^{\prime} V\left(T, P^{\prime}\right)=0
$$

A geometrical interpretation of the above result is that $P_{c}$ corresponds to a pressure that encloses equal areas of the non-monotonic isotherm on each side. The Maxwell construction approach to phase condensation is somewhat unsatisfactory, as it relies on integrating a clearly unphysical portion the van der Waals isotherm. A better approach that makes the approximations involved more apparent is presented in the next section.

\section{V.E Mean Field Theory of Condensation}

In principle, all properties of the interacting system, including phase separation, are contained within the thermodynamic potentials that can be obtained by evaluating $Z(T, N)$ or $\mathcal{Q}(T, \mu) .$ Phase transitions, however, are characterized by discontinuities in various state functions and must correspond to the appearance of singularities in the partition functions. At first glance, it is somewhat surprising that any singular behavior should emerge from computing such well behaved integrals (for short-ranged interactions) as

$$
Z(T, N, V)=\int \frac{\prod_{i=1}^{N} d^{3} \vec{p}_{i} d^{3} \vec{q}_{i}}{N ! h^{3 N}} \exp \left[-\beta \sum_{i=1}^{N} \frac{p_{i}^{2}}{2 m}-\beta \sum_{i<j} \mathcal{V}\left(\vec{q}_{i}-\vec{q}_{j}\right)\right]
$$

Instead of evaluating the integrals perturbatively, we shall now set up a reasonable approximation scheme. The contributions of the hard core and attractive portions of the potential are again treated separately, and the partition function approximated by

$$
Z(T, N, V) \approx \frac{1}{N !} \frac{1}{\lambda^{3 N}} \underbrace{V(V-\Omega) \cdots(V-(N-1) \Omega)}_{\text {Excluded volume effects }} \exp (-\beta \bar{U})
$$

Here $\bar{U}$ represents an average attraction energy, obtained by assuming a uniform density $n=N / V$, as

$$
\begin{aligned}
\bar{U} &=\frac{1}{2} \sum_{i, j} \mathcal{V}_{\text {attr. }}\left(\vec{q}_{i}-\vec{q}_{j}\right)=\frac{1}{2} \int d^{3} \vec{r}_{1} d^{3} \vec{r}_{2} n\left(\vec{r}_{1}\right) n\left(\vec{r}_{2}\right) \mathcal{V}_{\text {attr. }}\left(\vec{r}_{1}-\vec{r}_{2}\right) \\
& \approx \frac{n^{2}}{2} V \int d^{3} \vec{r} \mathcal{V}_{\text {attr. }}(\vec{r}) \equiv-\frac{N^{2}}{2 V} u
\end{aligned}
$$

The parameter $u$ describes the net effect of the attractive interactions. Substituting into eq.(V.58) leads to the following approximation for the partition function

$$
Z(T, N, V) \approx \frac{(V-N \Omega / 2)^{N}}{N ! \lambda^{3 N}} \exp \left[\frac{\beta u N^{2}}{2 V}\right]
$$

From the resulting free energy,

$$
F=-k_{B} T \ln Z=-N k_{B} T \ln (V-N \Omega / 2)+N k_{B} T \ln (N / e)+3 N k_{B} T \ln \lambda-\frac{u N^{2}}{2 V}
$$

we obtain the expression for the pressure in the canonical ensemble as

$$
P_{\text {can }}=-\left.\frac{\partial F}{\partial V}\right|_{T, N}=\frac{N k_{B} T}{V-N \Omega / 2}-\frac{u N^{2}}{2 V^{2}}
$$

Remarkably, the uniform density approximation reproduces the van der Waals equation of state. However, the self-consistency of this approximation can now be checked. As long as $\kappa_{T}$ is positive, eq.(V.54) implies that the variance of density vanishes for large volumes as $\left\langle n^{2}\right\rangle_{c}=k_{B} T n^{2} \kappa_{T} / V .$ But $\kappa_{T}$ diverges at $T_{c}$, and at lower temperatures its negativity implies an instability towards density fluctuations as discussed in the previous section. When condensation occurs, there is phase separation into high (liquid) and low (gas) density states, and the uniform density assumption becomes manifestly incorrect. This difficulty is circumvented in the grand canonical ensemble. Once the chemical potential is fixed, the number of particles (and hence density) in this ensemble is automatically adjusted to that of the appropriate phase.

As the assumption of a uniform density is correct for both the liquid and gas phases, we can use the approximations of eqs.(V.59) and (V.60) to estimate the grand partition function

$$
\mathcal{Q}(T, \mu, V)=\sum_{N=0}^{\infty} e^{\beta \mu N} Z(T, N, V) \approx \sum_{N=0}^{\infty} \exp \left[N \ln \left(\frac{V}{N}-\frac{\Omega}{2}\right)+\frac{\beta u N^{2}}{2 V}+\Delta N\right]
$$

where $\Delta=1+\beta \mu-\ln \left(\lambda^{3}\right) .$ As in any sum over exponentials in $N$, the above expression is dominated by a particular value of particle number (hence density), and given by

$$
\mathcal{Q}(T, \mu, V) \approx \exp \left\{\max \left[N \Delta+N \ln \left(\frac{V}{N}-\frac{\Omega}{2}\right)+\frac{\beta u N^{2}}{2 V}\right]_{N}\right\}
$$

Hence, the grand canonical expression for the gas pressure is obtained from

$$
\beta P_{\mathrm{g} \cdot \mathrm{c}}=\frac{\ln \mathcal{Q}}{V}=\max [\Psi(n)]_{n}
$$

where

$$
\Psi(n)=n \Delta+n \ln \left(n^{-1}-\frac{\Omega}{2}\right)+\frac{\beta u}{2} n^{2}
$$

The possible values of density are obtained from $d \Psi /\left.d n\right|_{n_{\alpha}}=0$, and satisfy

$$
\Delta=-\ln \left(n_{\alpha}^{-1}-\frac{\Omega}{2}\right)+\frac{1}{1-n_{\alpha} \Omega / 2}-\beta u n_{\alpha}
$$

The above equation in fact admits multiple solutions $n_{\alpha}$ for the density. Substituting the resulting $\Delta$ into eq.(V.65) leads after some manipulation to

$$
P_{\text {g.c. }}=\max \left[\frac{n_{\alpha} k_{B} T}{1-n_{\alpha} \Omega / 2}-\frac{u}{2} n_{\alpha}^{2}\right]_{\alpha}=\max \left[P_{\text {can }}\left(n_{\alpha}\right)\right]_{\alpha}
$$

i.e. the grand canonical and canonical values of pressure are identical at a particular density. However, if eq.(V.67) admits multiple solutions for the density at a particular chemical potential, the correct density is uniquely determined as the one that maximizes the canonical expression for pressure (or for $\psi(n)$ ).

The mechanism for the liquid-gas phase transition is therefore the following. The sum in eq.(V.63) is dominated by two large terms at the liquid and gas densities. At a particular chemical potential, the stable phase is determined by the larger of the two terms. The phase transition occurs when the dominant term changes upon varying the temperature. In mathematical form

$$
\ln \mathcal{Q}=\lim _{V \rightarrow \infty} \ln \left[e^{\beta V P_{\text {liquid }}}+e^{\beta V P_{\mathrm{gas}}}\right]= \begin{cases}\beta V P_{\text {gas }} & \text { for } T>T^{*} \\ \beta V P_{\text {liquid }} & \text { for } T<T^{*}\end{cases}
$$

The origin of the singularity in density can thus be traced to the thermodynamic limit of $V \rightarrow \infty .$ There are no phase transitions in finite systems! MIT OpenCourseWare

http://ocw.mit.edu

\subsection{Statistical Mechanics I: Statistical Mechanics of Particles \\ Fall 2013}

For information about citing these materials or our Terms of Use, visit: http://ocw.mit.edu/terms.
