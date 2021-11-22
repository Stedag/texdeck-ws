---
id: BW9ABVlrl7Iixmd2UoYz4
title: Lec18
desc: ''
updated: 1637530120229
created: 1637530120229
---
\section{V.F Variational Methods}

Perturbative methods provide a systematic way of incorporating the effect of interactions, but are impractical for the study of strongly interacting systems. While the first few terms in the virial series slightly modify the behavior of the gas, an infinite number of terms have to be summed to obtain the condensation transition. An alternative, but approximate, method for dealing with strongly interacting systems is the use of variational methods.

Suppose that in an appropriate ensemble we need to calculate $Z=\operatorname{tr}\left(e^{-\beta \mathcal{H}}\right) .$ In the canonical formulation, $Z$ is the partition function corresponding to the Hamiltonian $\mathcal{H}$ at temperature $k_{B} T=1 / \beta$, and for a classical system tr refers to the integral over the phase space of $N$ particles. However, the method is more general and can be applied to Gibbs or Grand partition functions with the appropriate modification of the exponential factor; also in the context of quantum systems where $\mathrm{tr}$ is a sum over all allowed quantum microstates. Let us assume that calculating $Z$ is very difficult for the (interacting) Hamiltonian $\mathcal{H}$, but that there is another Hamiltonian $\mathcal{H}_{0}$ acting on the same set of degrees of freedom for which the calculations are easier. We then introduce a Hamiltonian $\mathcal{H}(\lambda)=\mathcal{H}_{0}+\lambda\left(\mathcal{H}-\mathcal{H}_{0}\right)$, and a corresponding partition function

$$
Z(\lambda)=\operatorname{tr}\left\{\exp \left[-\beta \mathcal{H}_{0}-\lambda \beta\left(\mathcal{H}-\mathcal{H}_{0}\right)\right]\right\}
$$

which interpolates between the two as $\lambda$ changes from zero to one. It is then easy to prove the convexity condition

$$
\frac{d^{2} \ln Z(\lambda)}{d \lambda^{2}}=\beta^{2}\left\langle\left(\mathcal{H}-\mathcal{H}_{0}\right)^{2}\right\rangle_{c} \geq 0
$$

where \langle\rangle is an expectation value with the appropriately normalized probability.

From the convexity of the function, it immediately follows that

$$
\ln Z(\lambda) \geq \ln Z(0)+\left.\lambda \frac{d \ln Z}{d \lambda}\right|_{\lambda=0}
$$

But it is easy to see that $d \ln Z /\left.d \lambda\right|_{\lambda=0}=\beta\left\langle\mathcal{H}_{0}-\mathcal{H}\right\rangle^{0}$, where the superscript indicates expectation values with respect to $\mathcal{H}_{0} .$ Setting $\lambda=1$, we obtain

$$
\ln Z \geq \ln Z(0)+\beta\left\langle\mathcal{H}_{0}\right\rangle^{0}-\beta\langle\mathcal{H}\rangle^{0}
$$

Eq.(V.73), known as the Gibbs inequality, is the basis for most variational estimates. Typically, the 'simpler' Hamiltonian $\mathcal{H}_{0}$ (and hence the right hand side of eq.(V.73)) includes several parameters $\left\{n_{\alpha}\right\} .$ The best estimate for $\ln Z$ is obtained by finding the maximum of the right hand side with respect to these parameters. It can now be checked that the approximate evaluation of the grand partition function $\mathcal{Q}$ in the preceding section is equivalent to a variational treatment with $\mathcal{H}_{0}$ corresponding to a gas of hard-core particles of density $n$, for which (after replacing the sum by its dominant term)

$$
\ln \mathcal{Q}_{0}=\beta \mu N+\ln Z=V\left[n\left(1+\beta \mu-\ln \left(\lambda^{3}\right)\right)+n \ln \left(n^{-1}-\frac{\Omega}{2}\right)\right]
$$

The difference $\mathcal{H}-\mathcal{H}_{0}$ contains the attractive portion of the two body interactions. In the regions of phase space not excluded by the hard core interactions the gas in $\mathcal{H}_{0}$ is described by a uniform density $n .$ Hence

$$
\beta\left\langle\mathcal{H}_{0}-\mathcal{H}\right\rangle^{0}=\beta V \frac{n^{2}}{2} u
$$

and

$$
\beta P=\frac{\ln \mathcal{Q}}{V} \geq\left[n\left(1+\beta \mu-\ln \left(\lambda^{3}\right)\right)+n \ln \left(n^{-1}-\frac{\Omega}{2}\right)\right]+\frac{1}{2} \beta u n^{2}
$$

which is the same as eq.(V.66). The density $n$ is now a parameter on the right hand side of eq.(V.76). Obtaining the best variational estimate by maximizing with respect to $n$ is then equivalent to eq.(V.65).

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

Experimentally, this ratio is found to be in the range of $0.28$ to $0.33 .$ The van der Waals equation is thus not a good candidate for the putative universal equation of state. We can attempt to construct a generalized equation empirically by using three independent critical coordinates, and finding $P_{r} \equiv p_{r}\left(v_{r}, T_{r}\right)$ from the collapse of experimental data. Such an approach has some limited success in describing similar gases, e.g. the sequence of noble gases Ne, Xe, Kr, etc. However, different types of gases (e.g. diatomic, ionic, etc.) show rather different behaviors. This is not particularly surprising given the differences in the underlying Hamiltonians. We know rigorously from the virial expansion that perturbative treatment of the interacting gas does depend on the details of the microscopic potential. Thus the hope of finding a universal equation of state for all liquids and gases has no theoretical or experimental justification; each case has to be studied separately starting from its microscopic Hamiltonian. It is thus quite surprising that the collapse of experimental data does in fact work very well in the vicinity of the critical point, as described in the next section.

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
