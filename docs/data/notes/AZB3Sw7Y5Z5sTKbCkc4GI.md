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



\section{V.G Corresponding States}

We now have a good perturbative understanding of the behavior of a dilute interacting gas at high temperatures. At lower temperatures, attractive interactions lead to condensation into the liquid state. The qualitative behavior of the phase diagram is the same for most simple gases. There is a line of transitions in the coordinates $(P, T)$ (corresponding to the coexistence of liquid and gas in the $(V, T)$ plane) that terminates at a so called critical point. It is thus possible to transform a liquid to a gas without encountering any singularities. Since the ideal gas law is universal, i.e. independent of material, we may hope that there is also a generalized universal equation of state (presumably more complicated) that describes interacting gases, including liquid/gas condensation phenomena. This hope motivated the search for a law of corresponding states, obtained by appropriate rescalings of state functions. The most natural choice of scales for pressure, volume, and temperature are those of the critical point, $\left(P_{c}, V_{c}, T_{c}\right)$

The van der Waals equation is an example of a generalized equation of state. Its critical point is found by setting $\partial P /\left.\partial V\right|_{T}$ and $\partial^{2} P /\left.\partial V^{2}\right|_{T}$ to zero. The former is the limit of the flat coexistence portion of liquid/gas isotherms; the latter follows from the stability requirement $\kappa_{T}>0$ (see the discussion after eq.(I.72)). The coordinates of the critical point are thus obtained from solving the following coupled equations,

$$
\left\{\begin{aligned}
P &=\frac{k_{B} T}{v-b}-\frac{a}{v^{2}} \\
\left.\frac{\partial P}{\partial v}\right|_{T} &=-\frac{k_{B} T}{(v-b)^{2}}+\frac{2 a}{v^{3}}=0 \\
\left.\frac{\partial^{2} P}{\partial v^{2}}\right|_{T} &=\frac{2 k_{B} T}{(v-b)^{3}}-\frac{6 a}{v^{4}}=0
\end{aligned}\right.
$$

where $v=V / N$ is the volume per particle. The solution to these equations is 

$$
\left\{\begin{aligned}
P_{c} &=\frac{a}{27 b^{2}} \\
v_{c} &=3 b \\
k_{B} T_{c} &=\frac{8 a}{27 b}
\end{aligned}\right.
$$

Naturally, the critical point depends on the microscopic Hamiltonian (e.g. on the 2body interaction) via the parameters $a$ and $b$. However, we can scale out such dependencies by measuring $P, T$, and $v$ in units of $P_{c}, T_{c}$ and $v_{c} .$ Setting $P_{r}=P / P_{c}, v_{r}=v / v_{c}$, and $T_{r}=T / T_{c}$, a reduced version of the van der Waals equation is obtained as

$$
P_{r}=\frac{8}{3} \frac{T_{r}}{v_{r}-1 / 3}-\frac{3}{v_{r}^{2}}
$$

We have thus constructed a universal (material independent) equation of state. Since the original van der Waals equation depends only on two two parameters, eqs.(V.78) predict a universal dimensionless ratio,

$$
\frac{P_{c} v_{c}}{k_{B} T_{c}}=\frac{3}{8}=0.375
$$

Experimentally, this ratio is found to be in the range of $0.28$ to $0.33 .$ The van der Waals equation is thus not a good candidate for the putative universal equation of state.

We can attempt to construct a generalized equation empirically by using three inde pendent critical coordinates, and finding $P_{r} \equiv p_{r}\left(v_{r}, T_{r}\right)$ from the collapse of experimental data. Such an approach has some limited success in describing similar gases, e.g. the sequence of noble gases Ne, Xe, Kr, etc. However, different types of gases (e.g. diatomic, ionic, etc.) show rather different behaviors. This is not particularly surprising given the differences in the underlying Hamiltonians. We know rigorously from the virial expansion that perturbative treatment of the interacting gas does depend on the details of the mi croscopic potential. Thus the hope of finding a universal equation of state for all liquids and gases has no theoretical or experimental justification; each case has to be studied separately starting from its microscopic Hamiltonian. It is thus quite surprising that the collapse of experimental data does in fact work very well in the vicinity of the critical point, as described in the next section. 

\section{V.H Critical Point Behavior}

To account for the universal behavior of gases close to their critical point, let us examine the isotherms in the vicinity of $\left(P_{c}, v_{c}, T_{c}\right) .$ For $T \geq T_{c}$, a Taylor expansion of $P(T, v)$ in the vicinity of $v_{c}$, for any $T$ gives,

$$
P(T, v)=P\left(T, v_{c}\right)+\left.\frac{\partial P}{\partial v}\right|_{T}\left(v-v_{c}\right)+\left.\frac{1}{2} \frac{\partial^{2} P}{\partial v^{2}}\right|_{T}\left(v-v_{c}\right)^{2}+\left.\frac{1}{6} \frac{\partial^{3} P}{\partial v^{3}}\right|_{T}\left(v-v_{c}\right)^{3}+\cdots
$$

Since $\partial P /\left.\partial v\right|_{T}$ and $\partial^{2} P /\left.\partial v^{2}\right|_{T}$ are both zero at $T_{c}$, the expansion of the derivatives around the critical point gives

$$
\begin{aligned}
P\left(T, v_{c}\right) &=P_{c}+\alpha\left(T-T_{c}\right)+\mathcal{O}\left[(T-T)^{2}\right] \\
\left.\frac{\partial P}{\partial v}\right|_{T, v_{c}} &=-a\left(T-T_{c}\right)+\mathcal{O}\left[\left(T-T_{c}\right)^{2}\right] \\
\left.\frac{\partial^{2} P}{\partial v^{2}}\right|_{T, v_{c}} &=b\left(T-T_{c}\right)+\mathcal{O}\left[(T-T)^{2}\right] \\
\left.\frac{\partial^{3} P}{\partial v^{3}}\right|_{T_{c}, v_{c}} &=-c+\mathcal{O}\left[\left(T-T_{c}\right)\right]
\end{aligned}
$$

where $a, b$, and $c$ are material dependent constants. The stability condition, $\delta P \delta v \leq 0$, requires $a>0\left(\right.$ for $\left.T>T_{c}\right)$ and $c>0\left(\right.$ for $\left.T=T_{c}\right)$, but provides no information on the sign of $b$. If an analytical expansion is possible, the isotherms of any gas in the vicinity of its critical point must have the general form,

$$
P(T, v)=P_{c}+\alpha\left(T-T_{c}\right)-a\left(T-T_{c}\right)\left(v-v_{C}\right)+\frac{b}{2}\left(T-T_{c}\right)\left(v-v_{c}\right)^{2}-\frac{c}{6}\left(v-v_{c}\right)^{3}+\cdots
$$

Note that the third and fifth terms are of comparable magnitude for $\left(T-T_{c}\right) \sim\left(v-v_{c}\right)^{2}$ The fourth (and higher order terms) can then be neglected when this condition is satisfied. - The analytic expansion of eq.(V.83) results in the following predictions for behavior close to the critical point:

(a) The gas compressibility diverges on approaching the critical point from the high temperature side, along the critical isochore $\left(v=v_{c}\right)$ as,

$$
\lim _{T \rightarrow T_{c}^{+}} \kappa\left(T, v_{c}\right)=-\left.\frac{1}{v_{c}} \frac{\partial P}{\partial v}\right|_{T} ^{-1}=\frac{1}{v_{c} a\left(T-T_{c}\right)}
$$

(b) The critical isotherm $\left(T=T_{c}\right)$ behaves as

$$
P=P_{c}-\frac{c}{6}\left(v-v_{c}\right)^{3}+\cdots
$$

(c) Eq.(V.83) is manifestly inapplicable to $T<T_{c} .$ However, we can try to extract information for the low temperature side by applying the Maxwell construction to the unstable isotherms. Actually, dimensional considerations are sufficient to show that on approaching $T_{c}$ from the low temperature side, the specific volumes of the coexisting liquid and gas phases approach each other as

$$
\lim _{T \rightarrow T_{c}^{-}}\left(v_{\text {gas }}-v_{\text {liquid }}\right) \propto\left(T_{c}-T\right)^{1 / 2}
$$

The liquid-gas transition for $T<T_{c}$ is accompanied by a discontinuity in density, and the release of latent heat $L .$ This kind of transition is usually referred to as first order or discontinuous. The difference between the two phases disappears as the line of first order transitions terminates at the critical point. The singular behavior at this point is attributed to a second order or continuous transition. Eq.(V.83) follows from no more than the constraints of mechanical stability, and the assumption of analytical isotherms. Although there are some unknown coefficients, eqs.(V.85)-(V.86) predict universal forms for the singularities close to the critical point and can be compared to experimental data. The experimental results do indeed confirm the general expectations of singular behavior, and there is universality in the results for different gases which can be summarized as

(a) The compressibility diverges on approaching the critical point as

$$
\lim _{T \rightarrow T_{c}^{+}} \kappa\left(T, v_{c}\right) \propto\left(T-T_{c}\right)^{-\gamma}, \quad \text { with } \quad \gamma \approx 1.3
$$

(b) The critical isotherm behaves as

$$
\left(P-P_{c}\right) \propto\left(v-v_{c}\right)^{\delta}, \quad \text { with } \quad \delta \approx 5.0
$$

(c) The difference between liquid and gas densities vanishes close to the critical point as

$$
\lim _{T \rightarrow T_{c}^{-}}\left(\rho_{\text {liquid }}-\rho_{\text {gas }}\right) \propto \lim _{T \rightarrow T_{c}^{-}}\left(v_{\text {gas }}-v_{\text {liquid }}\right) \propto\left(T_{c}-T\right)^{\beta}, \quad \text { with } \quad \beta \approx 0.3
$$

These results clearly indicate that the assumption of analyticity of the isotherms, leading to eq.(V.83), is not correct. The exponents $\delta, \gamma$, and $\beta$ appearing in eqs.(V.88)(V.89) are known as critical indices. Understanding the origin, universality, and numerical values of these exponents is the a fascinating subject explored in the modern theory of critical phenomena. MIT OpenCourseWare

http://ocw.mit.edu

\subsection{Statistical Mechanics I: Statistical Mechanics of Particles \\ Fall 2013}

For information about citing these materials or our Terms of Use, visit: http://ocw.mit.edu/terms.
