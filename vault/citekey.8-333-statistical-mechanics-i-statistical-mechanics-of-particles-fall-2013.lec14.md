---
id: 2vOCfmU15keVaREWoIBYv
title: Lec14
desc: ''
updated: 1637530120228
created: 1637530120228
---
\section{IV.G Examples}

The two examples of sections (IV.C) and (IV.D) are now reexamined in the canonical ensemble.

1. Two level systems: The $N$ impurities are described by a macro-state $M \equiv(T, N)$. Subject to the Hamiltonian $\mathcal{H}=\epsilon \sum_{i=1}^{N} n_{i}$, the canonical probabilities of the micro-states $\mu \equiv\left\{n_{i}\right\}$, are given by

$$
p\left(\left\{n_{i}\right\}\right)=\frac{1}{Z} \exp \left[-\beta \epsilon \sum_{i=1}^{N} n_{i}\right]
$$

From the partition function,

$$
\begin{aligned}
Z(T, N) &=\sum_{\left\{n_{i}\right\}} \exp \left[-\beta \epsilon \sum_{i=1}^{N} n_{i}\right]=\left(\sum_{n_{1}=0}^{1} e^{-\beta \epsilon n_{1}}\right) \cdots\left(\sum_{n_{N}=0}^{1} e^{-\beta \epsilon n_{N}}\right) \\
&=\left(1+e^{-\beta \epsilon}\right)^{N}
\end{aligned}
$$

we obtain the free energy

$$
F(T, N)=-k_{B} T \ln Z=-N k_{B} T \ln \left[1+e^{-\epsilon /\left(k_{B} T\right)}\right]
$$

The entropy is now given by

$$
S=-\left.\frac{\partial F}{\partial T}\right|_{N}=\underbrace{N k_{B} \ln \left[1+e^{-\epsilon /\left(k_{B} T\right)}\right]}_{-F / T}+N k_{B} T\left(\frac{\epsilon}{k_{B} T^{2}}\right) \frac{e^{-\epsilon /\left(k_{B} T\right)}}{1+e^{-\epsilon /\left(k_{B} T\right)}}
$$

The internal energy,

$$
E=F+T S=\frac{N \epsilon}{1+e^{\epsilon /\left(k_{B} T\right)}}
$$

can also be obtained from

$$
E=-\frac{\partial \ln Z}{\partial \beta}=\frac{N \epsilon e^{-\beta \epsilon}}{1+e^{-\beta \epsilon}}
$$

Since the joint probability in eq.(IV.71) is in the form of a product, the excitations of different impurities are independent of each other, with the unconditional distribution

$$
p(n)=\frac{e^{-\beta \epsilon n}}{1+e^{-\beta \epsilon}}
$$

This result coincides with eqs.(IV.25), obtained through a more elaborate analysis in the microcanonical ensemble. As expected, in the large $N$ limit, the canonical and microcanonical ensembles describe exactly the same physics, both at the macroscopic and microscopic levels. 2. The Ideal Gas: For the canonical macro-state $M \equiv(T, V, N)$, the joint PDF for the micro-states $\mu \equiv\left\{\vec{p}_{i}, \vec{q}_{i}\right\}$, is

$$
p\left(\left\{\vec{p}_{i}, \vec{q}_{i}\right\}\right)=\frac{1}{Z} \exp \left[-\beta \sum_{i=1}^{N} \frac{p_{i}^{2}}{2 m}\right] \cdot\left\{\begin{array}{cc}
1 & \text { for }\left\{\vec{q}_{i}\right\} \in \text { box } \\
0 & \text { otherwise }
\end{array}\right.
$$

Including the modifications to the phase space of identical particles in eq.(IV.51), the dimensionless partition function is computed as

$$
\begin{aligned}
Z(T, V, N) &=\int \frac{1}{N !} \prod_{i=1}^{N} \frac{d^{3} \vec{q}_{i} d^{3} \vec{p}_{i}}{h^{3}} \exp \left[-\beta \sum_{i=1}^{N} \frac{p_{i}^{2}}{2 m}\right] \\
&=\frac{V^{N}}{N !}\left(\frac{2 \pi m k_{B} T}{h^{2}}\right)^{3 N / 2}=\frac{1}{N !}\left(\frac{V}{\lambda(T)^{3}}\right)^{N}
\end{aligned}
$$

where

$$
\lambda(T)=\frac{h}{\sqrt{2 \pi m k_{B} T}}
$$

is a characteristic length associated with the action $h .$ It shall be demonstrated later on that this length scale controls the onset of quantum mechanical effects in an ideal gas.

The free energy is given by

$$
\begin{aligned}
F &=-k_{B} T \ln Z=-N k_{B} T \ln V+N k_{B} T \ln N-N k_{B} T-\frac{3 N}{2} k_{B} T \ln \left(\frac{2 \pi m k_{B} T}{h^{2}}\right) \\
&=-N k_{B} T\left[\ln \left(\frac{V e}{N}\right)+\frac{3}{2} \ln \left(\frac{2 \pi m k_{B} T}{h^{2}}\right)\right]
\end{aligned}
$$

Various thermodynamic properties of the ideal gas can now be obtained from $d F=-S d T-$ $P d V+\mu d N .$ For example, from the entropy

$$
-S=\left.\frac{\partial F}{\partial T}\right|_{V, N}=-N k_{B}\left[\ln \frac{V e}{N}+\frac{3}{2} \ln \left(\frac{2 \pi m k_{B} T}{h^{2}}\right)\right]-N k_{B} T \frac{3}{2 T}=\frac{F-E}{T}
$$

we obtain the internal energy $E=3 N k_{B} T / 2 .$ The equation of state is obtained from

$$
P=-\left.\frac{\partial F}{\partial V}\right|_{T, N}=\frac{N k_{B} T}{V}, \quad \Longrightarrow \quad P V=N k_{B} T
$$

and the chemical potential is given by

$$
\mu=\left.\frac{\partial F}{\partial N}\right|_{T, V}=\frac{F}{N}+k_{B} T=\frac{E-T S+P V}{N}=k_{B} T \ln \left(n \lambda^{3}\right)
$$

Also, according to eq.(IV.78), the momenta of the $N$ particles are taken from independent Maxwell-Boltzmann distributions, consistent with eq.(IV.39). 

\section{IV.H The Gibbs Canonical Ensemble}

We can also define a generalized canonical ensemble in which the internal energy changes by the addition of both heat and work. The macrostates $M \equiv(T, \mathbf{J})$, are specified in terms of the external temperature and forces acting on the system; the thermodynamic coordinates $\mathbf{x}$ appear as additional random variables. The system is maintained at constant force through external elements (e.g. pistons or magnets). Including the work done against the forces, the energy of the combined system that includes these elements is $\mathcal{H}-\mathbf{J} \cdot \mathbf{x}$. Note that while the work done on the system is $+\mathbf{J} \cdot \mathbf{x}$, the energy change associated with the external elements with coordinates $\mathbf{x}$ has the opposite sign. The microstates of this combined system occur with the (canonical) probabilities

$$
p\left(\mu_{\mathrm{S}}, \mathbf{x}\right)=\exp \left[-\beta \mathcal{H}\left(\mu_{\mathrm{S}}\right)+\beta \mathbf{J} \cdot \mathbf{x}\right] / \mathcal{Z}(T, N, \mathbf{J})
$$

with the Gibbs partition function,

$$
\mathcal{Z}(N, T, \mathbf{J})=\sum_{\mu_{\mathrm{S}}, \mathbf{x}} e^{\beta \mathbf{J} \cdot \mathbf{x}-\beta \mathcal{H}\left(\mu_{\mathrm{S}}\right)}
$$

(Note that we have explicitly included the particle number $N$ to indicate that there is no chemical work. Chemical work is considered in the Grand Canonical Ensemble, which is discussed next.)

In this ensemble, the expectation value of the coordinates is obtained from

$$
\langle\mathbf{x}\rangle=k_{B} T \frac{\partial \ln \mathcal{Z}}{\partial \mathbf{J}}
$$

which together with the thermodynamic identity $\mathbf{x}=-\partial G / \partial \mathbf{J}$, suggests the identification

$$
G(N, T, \mathbf{J})=-k_{B} T \ln \mathcal{Z}
$$

where $G=E-T S-\mathbf{x} \cdot \mathbf{J}$ is the Gibbs free energy. (The same conclusion can be reached by equating $\mathcal{Z}$ in eq.(IV.86) to the term that maximizes the probability with respect to x.) The enthalpy $H \equiv E-\mathbf{x} \cdot \mathbf{J}$ is easily obtained in this ensemble from

$$
-\frac{\partial \ln \mathcal{Z}}{\partial \beta}=\langle\mathcal{H}-\mathbf{x} \cdot \mathbf{J}\rangle=H
$$

Note that heat capacities at constant force (which include work done against the external forces), are obtained from the enthalpy as $C_{\mathbf{J}}=\partial H / \partial T$. The following examples illustrate the use of the Gibbs canonical ensemble:

1. The Ideal Gas in the isobaric ensemble is described by the macrostate $M \equiv(N, T, P)$. A micro-state $\mu \equiv\left\{\vec{p}_{i}, \vec{q}_{i}\right\}$, with a volume $V$ occurs with the probability

$$
p\left(\left\{\vec{p}_{i}, \vec{q}_{i}\right\}, V\right)=\frac{1}{\mathcal{Z}} \exp \left[-\beta \sum_{i=1}^{N} \frac{p_{i}^{2}}{2 m}-\beta P V\right] \cdot\left\{\begin{array}{cc}
1 & \text { for }\left\{\vec{q}_{i}\right\} \in \text { box of volume } V \\
0 \quad \text { otherwise }
\end{array}\right.
$$

The normalization factor is now

$$
\begin{aligned}
\mathcal{Z}(N, T, P) &=\int_{0}^{\infty} d V e^{-\beta P V} \int \frac{1}{N !} \prod_{i=1}^{N} \frac{d^{3} \vec{q}_{i} d^{3} \vec{p}_{i}}{h^{3}} \exp \left[-\beta \sum_{i=1}^{N} \frac{p_{i}^{2}}{2 m}\right] \\
&=\int_{0}^{\infty} d V V^{N} e^{-\beta P V} \frac{1}{N ! \lambda(T)^{3 N}}=\frac{1}{\left(\beta P \lambda(T)^{3}\right)^{N}}
\end{aligned}
$$

The Gibbs free energy is given by

$$
G=-k_{B} T \ln \mathcal{Z}=N k_{B} T\left[\ln P-\frac{5}{2} \ln \left(k_{B} T\right)+\frac{3}{2} \ln \left(\frac{h^{2}}{2 \pi m}\right)\right]
$$

Starting from $d G=-S d T+V d P+\mu d N$, the volume of the gas is obtained as

$$
V=\left.\frac{\partial G}{\partial P}\right|_{T, N}=\frac{N k_{B} T}{P}, \quad \Longrightarrow \quad P V=N k_{B} T
$$

The enthalpy $H=\langle E+P V\rangle$ is easily calculated from

$$
H=-\frac{\partial \ln \mathcal{Z}}{\partial \beta}=\frac{5}{2} N k_{B} T
$$

from which we get $C_{P}=d H / d T=5 / 2 N k_{B}$

2. Spins in an external magnetic field $\vec{B}$, provide a common example for usage of the Gibbs canonical ensemble. Adding the work done against the magnetic field to the internal Hamiltonian $\mathcal{H}$, results in the Gibbs partition function

$$
\mathcal{Z}(N, T, B)=\operatorname{tr}[\exp (-\beta \mathcal{H}+\beta \vec{B} \cdot \vec{M})]
$$

where $\vec{M}$ is the net magnetization. The symbol $\mathrm{tr}$ is used to indicate the sum over all spin degrees of freedom, which in a quantum mechanical formulation are restricted to discrete values. The simplest case is spin of $1 / 2$, with two possible projections of the spin along the magnetic field. A microstate of $N$ spins is now described by the set of Ising variables $\left\{\sigma_{i}=\pm 1\right\} .$ The corresponding magnetization along the field direction is given by $M=\mu_{0} \sum_{i=1}^{N} \sigma_{i}$, where $\mu_{0}$ is a microscopic magnetic moment. Assuming that there are no interactions between spins $(\mathcal{H}=0)$, the probability of a microstate is

$$
p\left(\left\{\sigma_{i}\right\}\right)=\frac{1}{\mathcal{Z}} \exp \left[\beta B \mu_{0} \sum_{i=1}^{N} \sigma_{i}\right]
$$

Clearly, this is closely related to the example of two level systems discussed in the canonical ensemble, and we can easily obtain the Gibbs partition function

$$
\mathcal{Z}(N, T, B)=\left[2 \cosh \left(\beta \mu_{0} B\right)\right]^{N}
$$

and the Gibbs free energy

$$
G=-k_{B} T \ln \mathcal{Z}=-N k_{B} T \ln \left[2 \cosh \left(\beta \mu_{0} B\right)\right]
$$

The average magnetization is given by

$$
M=-\frac{\partial G}{\partial B}=N \mu_{0} \tanh \left(\beta \mu_{0} B\right)
$$

Expanding eq.(IV.97) for small $B$ results in the well-known Curie law for magnetic susceptibility of non-interacting spins,

$$
\chi(T)=\left.\frac{\partial M}{\partial B}\right|_{B=0}=\frac{N \mu_{0}^{2}}{k_{B} T}
$$

The enthalpy is simply $H=\langle\mathcal{H}-B M\rangle=-B M$, and $C_{B}=-B \partial M / \partial T$.

\section{IV.I The Grand Canonical Ensemble}

The previous sections demonstrate that while the canonical and microcanonical ensembles are completely equivalent in the thermodynamic limit, it is frequently much easier to perform statistical mechanical computations in the canonical framework. Sometimes it is more convenient to allow chemical work (by fixing the chemical potential $\mu$, rather than at a fixed number of particles), but no mechanical work. The resulting macro-states $M \equiv(T, \mu, \mathbf{x})$, are governed by the grand canonical ensemble. The corresponding microstates $\mu_{\mathrm{S}}$, contain an indefinite number of particles $N\left(\mu_{\mathrm{S}}\right) .$ As in the case of the canonical ensemble, the system $\mathrm{S}$, can be maintained at a constant chemical potential through contact with a reservoir $\mathrm{R}$, at temperature $T$ and chemical potential $\mu .$ The probability distribution for the micro-states of $\mathrm{S}$ is obtained by summing over all states of the reservoir, as in eq.(IV. 53$)$, and is given by

$$
p\left(\mu_{\mathrm{S}}\right)=\exp \left[\beta \mu N\left(\mu_{\mathrm{S}}\right)-\beta \mathcal{H}\left(\mu_{\mathrm{S}}\right)\right] / \mathcal{Q}
$$

The normalization factor is the grand partition function,

$$
\mathcal{Q}(T, \mu, \mathbf{x})=\sum_{\mu_{\mathrm{S}}} e^{\beta \mu N\left(\mu_{\mathrm{S}}\right)-\beta \mathcal{H}\left(\mu_{\mathrm{S}}\right)}
$$

We can reorganize the above summation by grouping together all micro-states with a given number of particles, i.e.

$$
\mathcal{Q}(T, \mu, \mathbf{x})=\sum_{N=0}^{\infty} e^{\beta \mu N} \sum_{\left(\mu_{\mathrm{S}} \mid N\right)} e^{-\beta \mathcal{H}_{N}\left(\mu_{\mathrm{S}}\right)}
$$

The restricted sums in eq.(IV.101) are just the $N$ -particle partition functions. As each term in $\mathcal{Q}$ is the total weight of all micro-states of $N$ particles, the unconditional probability of finding $N$ particles in the system is

$$
p(N)=\frac{e^{\beta \mu N} Z(T, N, \mathbf{x})}{\mathcal{Q}(T, \mu, \mathbf{x})}
$$

The average number of particles in the system is

$$
\langle N\rangle=\frac{1}{\mathcal{Q}} \frac{\partial}{\partial(\beta \mu)} \mathcal{Q}=\frac{\partial}{\partial(\beta \mu)} \ln \mathcal{Q}
$$

while the number fluctuations are related to the variance

$$
\left\langle N^{2}\right\rangle_{C}=\left\langle N^{2}\right\rangle-\langle N\rangle^{2}=\frac{1}{\mathcal{Q}} \frac{\partial^{2}}{\partial(\beta \mu)^{2}} \ln \mathcal{Q}-\left(\frac{\partial}{\partial(\beta \mu)} \ln \mathcal{Q}\right)^{2}=\frac{\partial^{2}}{\partial(\beta \mu)^{2}} \ln \mathcal{Q}=\frac{\partial\langle N\rangle}{\partial(\beta \mu)}
$$

The variance is thus proportional to $N$, and the relative number fluctuations vanish in the thermodynamic limit, establishing the equivalence of this ensemble to the previous ones.

Because of the sharpness of the distribution for $N$, the sum in eq.(IV.101) can be approximated by its largest term at $N=N^{*} \approx<N>$, i.e.

$$
\begin{aligned}
\mathcal{Q}(T, \mu, \mathbf{x})=& \lim _{N \rightarrow \infty} \sum_{N=0}^{\infty} e^{\beta \mu N} Z(T, N, \mathbf{x})=e^{\beta \mu N^{*}} Z\left(T, N^{*}, \mathbf{x}\right)=e^{\beta \mu N^{*}-\beta F} \\
&=e^{-\beta\left(-\mu N^{*}+E-T S\right)}=e^{-\beta \mathcal{G}}
\end{aligned}
$$

where

$$
\mathcal{G}(T, \mu, \mathbf{x})=E-T S-\mu N=-k_{B} T \ln \mathcal{Q}
$$

is the grand potential. Thermodynamic information is obtained by using $d \mathcal{G}=-S d T-$ $N d \mu+\mathbf{J} \cdot d \mathbf{x}$, as

$$
-S=\left.\frac{\partial \mathcal{G}}{\partial T}\right|_{\mu, \mathbf{x}}, \quad N=-\left.\frac{\partial \mathcal{G}}{\partial \mu}\right|_{T, \mathbf{x}}, \quad \quad J_{i}=\left.\frac{\partial \mathcal{G}}{\partial x_{i}}\right|_{T, \mu}
$$

As a final example, we compute the properties of the ideal gas of non-interacting particles in the grand canonical ensemble. The macro-state is $M \equiv(T, \mu, V)$, and the corresponding micro-states $\left\{\vec{p}_{1}, \vec{q}_{1}, \vec{p}_{2}, \vec{q}_{2}, \cdots\right\}$ have indefinite particle number. The grand partition function is given by

$$
\begin{aligned}
\mathcal{Q}(T, \mu, V) &=\sum_{N=0}^{\infty} e^{\beta \mu N} \frac{1}{N !} \int\left(\prod_{i=1}^{N} \frac{d^{3} \vec{q}_{i} d^{3} \vec{p}_{i}}{h^{3}}\right) \exp \left[-\beta \sum_{i} \frac{p_{i}^{2}}{2 m}\right] \\
&=\sum_{N=0}^{\infty} \frac{e^{\beta \mu N}}{N !}\left(\frac{V}{\lambda^{3}}\right)^{N} \quad\left(\text { with } \lambda=\frac{h}{\sqrt{2 \pi m k_{B} T}}\right) \\
&=\exp \left[e^{\beta \mu} \frac{V}{\lambda^{3}}\right]
\end{aligned}
$$

and the grand potential is

$$
\mathcal{G}(T, \mu, V)=-k_{B} T \ln \mathcal{Q}=-k_{B} T e^{\beta \mu} \frac{V}{\lambda^{3}}
$$

But, since $\mathcal{G}=E-T S-\mu N=-P V$, the gas pressure can be obtained directly as

$$
P=-\frac{\mathcal{G}}{V}=-\left.\frac{\partial \mathcal{G}}{\partial V}\right|_{\mu, T}=k_{B} T \frac{e^{\beta \mu}}{\lambda^{3}}
$$

The particle number and the chemical potential are related by

$$
N=-\left.\frac{\partial \mathcal{G}}{\partial \mu}\right|_{T, V}=\frac{e^{\beta \mu} V}{\lambda^{3}}
$$

The equation of state is obtained by comparing eqs.(IV.110) and (IV.111), as $P=$ $k_{B} T N / V .$ Finally, the chemical potential is given by

$$
\mu=k_{B} T \ln \left(\lambda^{3} \frac{N}{V}\right)=k_{B} T \ln \left(\frac{P \lambda^{3}}{k_{B} T}\right)
$$

MIT OpenCourseWare

http://ocw.mit.edu

\subsection{Statistical Mechanics I: Statistical Mechanics of Particles \\ Fall 2013}

For information about citing these materials or our Terms of Use, visit: http://ocw.mit.edu/terms.
