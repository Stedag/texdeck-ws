---
id: v5pPQ5obe1K4m94KJq80g
title: Lec13
desc: ''
updated: 1637530120227
created: 1637530120227
---
\section{IV.D The Ideal Gas}

As discussed in chapter II, micro-states of a gas of $N$ particles correspond to points $\mu \equiv$ $\left\{\vec{p}_{i}, \vec{q}_{i}\right\}$, in the $6 N$ -dimensional phase space. Ignoring the potential energy of interactions, the particles are subject to a Hamiltonian

$$
\mathcal{H}=\sum_{i=1}^{N}\left[\frac{\vec{p}_{i}^{2}}{2 m}+U\left(\vec{q}_{i}\right)\right]
$$

where $U(\vec{q})$ describes the potential imposed by a box of volume $V .$ A microcanonical ensemble is specified by its energy, volume, and number of particles, $M \equiv(E, V, N)$. The joint PDF for a micro-state is

$$
p(\mu)=\frac{1}{\Omega(E, V, N)} \cdot \begin{cases}1 & \text { for } \vec{q}_{i} \in \text { box, and } \sum_{i} \vec{p}_{i}^{2} / 2 m=E \quad\left(\pm \Delta_{E}\right) \\ 0 \quad \text { otherwise }\end{cases}
$$

In the allowed micro-states, coordinates of the particles must be within the box, while the momenta are constrained to the surface of the (hyper-)sphere $\sum_{i=1}^{N} \vec{p}_{i}^{2}=2 m E .$ The allowed phase space is thus the product of a contribution $V^{N}$ from the coordinates, with the surface area of a $3 N$ -dimensional sphere of radius $\sqrt{2 m E}$ from the momenta. (If the microstate energies are accepted in the energy interval $E \pm \Delta_{E}$, the corresponding volume in momentum space is that of a (hyper-)spherical shell of thickness $\left.\Delta_{R}=\sqrt{2 m / E} \Delta E .\right)$ The area of a $d$ -dimensional sphere is $\mathcal{A}_{d}=S_{d} R^{d-1}$, where $S_{d}$ is the generalized solid angle.

A simple way to calculate the $d$ -dimensional solid angle is to consider the product of $d$ Gaussian integrals,

$$
I_{d} \equiv\left(\int_{-\infty}^{\infty} d x e^{-x^{2}}\right)^{d}=\pi^{d / 2}
$$

Alternatively, we may consider $I_{d}$ as an integral over an entire $d$ -dimensional space, i.e.

$$
I_{d}=\int \prod_{i=1}^{d} d x_{i} \exp \left(-x_{i}^{2}\right)
$$

The integrand is spherically symmetric, and we can change coordinates to $R^{2}=\sum_{i} x_{i}^{2}$ Noting that the corresponding volume element in these coordinates is $d V_{d}=S_{d} R^{d-1} d R$

$$
I_{d}=\int_{0}^{\infty} d R S_{d} R^{d-1} e^{-R^{2}}=\frac{S_{d}}{2} \int_{0}^{\infty} d y y^{d / 2-1} e^{-y}=\frac{S_{d}}{2}(d / 2-1) !
$$

where we have first made a change of variables to $y=R^{2}$, and then used the integral representation of $n ! .$ Equating expressions $(\mathrm{IV} .28)$ and $(\mathrm{IV} .30)$ for $I_{d}$ gives the final result for the solid angle,

$$
S_{d}=\frac{2 \pi^{d / 2}}{(d / 2-1) !}
$$

The volume of the available phase space is thus given by

$$
\Omega(E, V, N)=V^{N} \frac{2 \pi^{3 N / 2}}{(3 N / 2-1) !}(2 m E)^{(3 N-1) / 2} \Delta_{R}
$$

The entropy is obtained from the logarithm of the above expression. Using Stirling's formula, and neglecting terms of order of 1 or $\ln E \sim \ln N$ in the large $N$ limit, results in

$$
\begin{aligned}
S(E, V, N) &=k_{B}\left[N \ln V+\frac{3 N}{2} \ln (2 \pi m E)-\frac{3 N}{2} \ln \frac{3 N}{2}+\frac{3 N}{2}\right] \\
&=N k_{B} \ln \left[V\left(\frac{4 \pi e m E}{3 N}\right)^{3 / 2}\right]
\end{aligned}
$$

Properties of the ideal gas can now be recovered from $T d S=d E+P d V-\mu d N$,

$$
\frac{1}{T}=\left.\frac{\partial S}{\partial E}\right|_{N, V}=\frac{3}{2} \frac{N k_{B}}{E}
$$

The internal energy $E=3 N k_{B} T / 2$, is only a function of $T$, and the heat capacity $C_{V}=$ $3 N k_{B} / 2$, is a constant. The equation of state is obtained from

$$
\frac{P}{T}=\left.\frac{\partial S}{\partial V}\right|_{N, E}=\frac{N k_{B}}{V}, \quad \Longrightarrow \quad P V=N k_{B} T
$$

The unconditional probability of finding a particle of momentum $\vec{p}_{1}$ in the gas can be calculated from the joint $\mathrm{PDF}$ in eq.(IV.27), by integrating over all other variables,

$$
\begin{aligned}
p\left(\vec{p}_{1}\right) &=\int d^{3} \vec{q}_{1} \prod_{i=2}^{N} d^{3} \vec{q}_{i} d^{3} \vec{p}_{i} p\left(\left\{\vec{q}_{i}, \vec{p}_{i}\right\}\right) \\
&=\frac{V \Omega\left(E-\vec{p}_{1}^{2} / 2 m, V, N-1\right)}{\Omega(E, V, N)}
\end{aligned}
$$

The final expression indicates that once the kinetic energy of one particle is specified, the remaining energy must be shared amongst the other $N-1$. Using eq.(IV.32),

$$
\begin{aligned}
p\left(\vec{p}_{1}\right) &=\frac{V^{N} \pi^{3(N-1) / 2}\left(2 m E-\vec{p}_{1}^{2}\right)^{(3 N-4) / 2}}{(3(N-1) / 2-1) !} \cdot \frac{(3 N / 2-1) !}{V^{N} \pi^{3 N / 2}(2 m E)^{(3 N-1) / 2}} \\
&=\left(1-\frac{\vec{p}_{1}^{2}}{2 m E}\right)^{3 N / 2-2} \frac{1}{(2 \pi m E)^{3 / 2}} \frac{(3 N / 2-1) !}{(3(N-1) / 2-1) !}
\end{aligned}
$$

From Stirling's formula, the ratio of $(3 N / 2-1) !$ to $(3(N-1) / 2-1) !$ is approximately $(3 N / 2)^{3 / 2}$, and in the large $E$ limit,

$$
p\left(\vec{p}_{1}\right)=\left(\frac{3 N}{4 \pi m E}\right)^{3 / 2} \exp \left(-\frac{3 N}{2} \frac{\vec{p}_{1}^{2}}{2 m E}\right)
$$

This is a properly normalized Maxwell-Boltzmann distribution, which can be displayed in its more familiar form after the substitution $E=3 N k_{B} T / 2$,

$$
p\left(\vec{p}_{1}\right)=\frac{1}{\left(2 \pi m k_{B} T\right)^{3 / 2}} \exp \left(-\frac{\vec{p}_{1}^{2}}{2 m k_{B} T}\right)
$$

\section{IV.E Mixing Entropy and Gibbs' Paradox}

The expression in eq.(IV.33) for the entropy of the ideal gas has a major shortcoming in that it is not extensive. Under the transformation $(E, V, N) \rightarrow(\lambda E, \lambda V, \lambda N)$, the entropy changes to $\lambda\left(S+N k_{B} \ln \lambda\right)$. The additional term comes from the contribution $V^{N}$, of the coordinates to the available phase space. This difficulty is intimately related to the mixing entropy of two gases. Consider two distinct gases, initially occupying volumes $V_{1}$ and $V_{2}$ at the same temperature $T$. The partition between them is removed, and they are allowed to expand and occupy the combined volume $V=V_{1}+V_{2} .$ The mixing process is clearly irreversible, and must be accompanied by an increase in entropy, calculated as follows. According to eq.(IV.33), the initial entropy is

$$
S_{i}=S_{1}+S_{2}=N_{1} k_{B}\left(\ln V_{1}+\sigma_{1}\right)+N_{2} k_{B}\left(\ln V_{2}+\sigma_{2}\right)
$$

where,

$$
\sigma_{\alpha}=\ln \left(\frac{4 \pi e m_{\alpha}}{3} \cdot \frac{E_{\alpha}}{N_{\alpha}}\right)^{3 / 2}
$$

is the momentum contribution to the entropy of the $\alpha^{\mathrm{th}}$ gas. Since $E_{\alpha} / N_{\alpha}=3 k_{B} T / 2$ for a monotonic gas,

$$
\sigma_{\alpha}(T)=\frac{3}{2} \ln \left(2 \pi e m_{\alpha} k_{B} T\right)
$$

The temperature of the gas is unchanged by mixing, since

$$
\frac{3}{2} k_{B} T_{f}=\frac{E_{1}+E_{2}}{N_{1}+N_{2}}=\frac{E_{1}}{N_{1}}=\frac{E_{2}}{N_{2}}=\frac{3}{2} k_{B} T
$$

The final entropy of the mixed gas is

$$
S_{f}=N_{1} k_{B} \ln \left(V_{1}+V_{2}\right)+N_{2} k_{B} \ln \left(V_{1}+V_{2}\right)+k_{B}\left(N_{1} \sigma_{1}+N_{2} \sigma_{2}\right)
$$

There is no change in the contribution from the momenta which depends only on temperature. The mixing entropy,

$$
\Delta S_{\mathrm{Mix}}=S_{f}-S_{i}=N_{1} k_{B} \ln \frac{V}{V_{1}}+N_{2} k_{B} \ln \frac{V}{V_{2}}=-N k_{B}\left[\frac{N_{1}}{N} \ln \frac{V_{1}}{V}+\frac{N_{2}}{N} \ln \frac{V_{2}}{V}\right]
$$

is solely from the contribution of the coordinates. The above expression is easily generalized to the mixing of many components, with $\Delta S_{\mathrm{Mix}}=-N k_{B} \sum_{\alpha}\left(N_{\alpha} / N\right) \ln \left(V_{\alpha} / V\right)$.

Gibbs' Paradox is related to what happens when the two gases, initially on the two sides of the partition, are identical with the same density, $n=N_{1} / V_{1}=N_{2} / V_{2} .$ Since removing or inserting the partition does not change the state of the system, there should be no entropy of mixing, while eq.(IV.45) does predict such a change. For the resolution of this paradox, note that while after removing and reinserting the partition, the system does return to its initial configuration, the actual particles that occupy the two components are not the same. But as the particles are by assumption identical, these configurations cannot be distinguished. In other words, while the exchange of distinct particles leads to two configurations

![](https://cdn.mathpix.com/cropped/4076ae3326a79790e1b6e6a3d54bd8d5-04.jpg?height=74&width=311&top_left_y=941&top_left_x=482)

a similar exchange has no effect on identical particles, as in

$$
\frac{\bullet \mid}{A \mid B} \text { and } \frac{\bullet \mid \bullet}{A} \mid \frac{\bullet}{B}
$$

Therefore, we have over-counted the phase space associated with $N$ identical particles by the number of possible permutations. As there are $N !$ permutations leading to indistinguishable micro-states, eq.(IV.32) should be corrected to

$$
\Omega(N, E, V)=\frac{V^{N}}{N !} \frac{2 \pi^{3 N / 2}}{(3 N / 2-1) !}(2 m E)^{(3 N-1) / 2} \Delta_{R}
$$

resulting in a modified entropy,

$$
S=k_{B} \ln \Omega=k_{B}[N \ln V-N \ln N+N \ln e]+N k_{B} \sigma=N k_{B}\left[\ln \frac{e V}{N}+\sigma\right]
$$

As the argument of the logarithm has changed from $V$ to $V / N$, the final expression is now properly extensive. The mixing entropies can be recalculated using eq.(IV.47). For the mixing of distinct gases,

$$
\begin{aligned}
\Delta S_{\mathrm{Mix}}=S_{f}-S_{i} &=N_{1} k_{B} \ln \frac{V}{N_{1}}+N_{2} k_{B} \ln \frac{V}{N_{2}}-N_{1} k_{B} \ln \frac{V_{1}}{N_{1}}-N_{2} k_{B} \ln \frac{V_{2}}{N_{2}} \\
&=N_{1} k_{B} \ln \left(\frac{V}{N_{1}} \cdot \frac{N_{1}}{V_{1}}\right)+N_{2} k_{B} \ln \left(\frac{V}{N_{2}} \cdot \frac{N_{2}}{V_{2}}\right) \\
&=-N k_{B}\left[\frac{N_{1}}{N} \ln \frac{V_{1}}{V}+\frac{N_{2}}{N} \ln \frac{V_{2}}{V}\right]
\end{aligned}
$$

exactly as obtained before in eq.(IV.45). For the 'mixing' of two identical gases, with $N_{1} / V_{1}=N_{2} / V_{2}=\left(N_{1}+N_{2}\right) /\left(V_{1}+V_{2}\right)$

$$
\Delta S_{\mathrm{Mix}}=S_{f}-S_{i}=\left(N_{1}+N_{2}\right) k_{B} \ln \frac{V_{1}+V_{2}}{N_{1}+N_{2}}-N_{1} k_{B} \ln \frac{V_{1}}{N_{1}}-N_{2} k_{B} \ln \frac{V_{2}}{N_{2}}=0
$$

Note that after taking the permutations of identical particles into account, the available volume in the final state is $V^{N_{1}+N_{2}} / N_{1} ! N_{2} !$ for distinct particles, and $V^{N_{1}+N_{2}} /\left(N_{1}+N_{2}\right) !$ for identical particles.

- Additional comments on the microcanonical entropy:

1. In the example of two-level impurities in a solid matrix (sec.IV.C), there is no need for the additional factor of $N !$, as the defects can be distinguished by their locations.

2. The corrected formula for the ideal gas entropy in eq.(IV.47) does not affect the computations of energy and pressure in eqs.(IV.34) and (IV.35). It is essential to obtaining an intensive chemical potential,

$$
\frac{\mu}{T}=-\left.\frac{\partial S}{\partial N}\right|_{E, V}=-\frac{S}{N}+\frac{5}{2} k_{B}=k_{B} \ln \left[\frac{V}{N}\left(\frac{4 \pi m E}{3 N}\right)^{3 / 2}\right]
$$

3. The above treatment of identical particles is somewhat artificial. This is because the concept of identical particles does not easily fit within the framework of classical mechanics. To implement the Hamiltonian equations of motion on a computer, one has to keep track of the coordinates of the $N$ particles. The computer will have no difficulty in distinguishing exchanged particles. The indistinguishability of their phase spaces is in a sense an additional postulate of classical statistical mechanics. This problem is elegantly resolved within the framework of quantum statistical mechanics. Description of identical particles in quantum mechanics requires proper symmetrization of the wave function. The corresponding quantum microstates naturally yield the $N !$ factor, as will be shown later on.

4. Yet another difficulty with the expression (IV.47), resolved in quantum statistical mechanics, is the arbitrary constant that appears in changing the units of measurement for $q$ and $p$. The volume of phase space involves products $p q$, of coordinates and conjugate momenta, and hence has dimensions of (action) $^{N}$. Quantum mechanics provides the appropriate measure of action in Planck's constant $h .$ Anticipating these quantum results, we shall henceforth set the measure of phase space for identical particles to

$$
d \Gamma_{N}=\frac{1}{h^{3 N} N !} \prod_{i=1}^{N} d^{3} \vec{q}_{i} d^{3} \vec{p}_{i}
$$

\section{IV.F The Canonical Ensemble}

In the microcanonical ensemble, the energy $E$, of a large macroscopic system is precisely specified, and its equilibrium temperature $T$, emerges as a consequence (eq.(IV.7)). However, from a thermodynamic perspective, $E$ and $T$ are both functions of state and on the same footing. It is possible to construct a statistical mechanical formulation in which the temperature of the system is specified and its internal energy is then deduced. This is achieved in the canonical ensemble where the macro-states, specified by $M \equiv(T, \mathbf{x})$, allow the input of heat into the system, but no external work. The system $S$, is maintained at a constant temperature through contact with a reservoir $\mathrm{R}$. The reservoir is another macroscopic system that is sufficiently large so that its temperature is not changed due to interactions with S. To find the probabilities $p_{(T, \mathbf{x})}(\mu)$, of the various micro-states of S, note that the combined system $R \oplus S$, belongs to a microcanonical ensemble of energy $E_{\mathrm{Tot}} \gg E_{S} .$ As in eq.(IV.3), the joint probability of micro-states $\left(\mu_{S} \otimes \mu_{R}\right)$ is

$$
p\left(\mu_{\mathrm{S}} \otimes \mu_{\mathrm{R}}\right)=\frac{1}{\Omega_{\mathrm{S} \oplus \mathrm{R}}\left(E_{\mathrm{Tot}}\right)} \cdot\left\{\begin{array}{l}
1 \quad \text { for } \mathcal{H}_{\mathrm{S}}\left(\mu_{\mathrm{S}}\right)+\mathcal{H}_{\mathrm{R}}\left(\mu_{\mathrm{R}}\right)=E_{\mathrm{Tot}} \\
0 \quad \text { otherwise }
\end{array}\right.
$$

The unconditional probability for micro-states of $\mathrm{S}$ is now obtained from

$$
p\left(\mu_{\mathrm{S}}\right)=\sum_{\left\{\mu_{\mathrm{R}}\right\}} p\left(\mu_{\mathrm{S}} \otimes \mu_{\mathrm{R}}\right)
$$

Once $\mu_{\mathrm{S}}$ is specified, the above sum is restricted to micro-states of the reservoir with energy $E_{\text {Tot }}-\mathcal{H}_{\mathrm{S}}\left(\mu_{\mathrm{S}}\right) .$ The number of the such states is related to the entropy of the reservoir, and leads to

$$
p\left(\mu_{\mathrm{S}}\right)=\frac{\Omega_{\mathrm{R}}\left(E_{\mathrm{Tot}}-\mathcal{H}_{\mathrm{S}}\left(\mu_{\mathrm{S}}\right)\right)}{\Omega_{\mathrm{S} \oplus \mathrm{R}}\left(E_{\mathrm{Tot}}\right)} \propto \exp \left[\frac{1}{k_{B}} S_{\mathrm{R}}\left(E_{\mathrm{Tot}}-\mathcal{H}_{\mathrm{S}}\left(\mu_{\mathrm{S}}\right)\right)\right]
$$

Since by assumption the energy of the system is insignificant compared to that of the reservoir,

$$
S_{\mathrm{R}}\left(E_{\mathrm{Tot}}-\mathcal{H}_{\mathrm{S}}\left(\mu_{\mathrm{S}}\right)\right) \approx S_{\mathrm{R}}\left(E_{\mathrm{Tot}}\right)-\mathcal{H}_{\mathrm{S}}\left(\mu_{\mathrm{S}}\right) \frac{\partial S_{\mathrm{R}}}{\partial E_{\mathrm{R}}}=S_{\mathrm{R}}\left(E_{\mathrm{Tot}}\right)-\frac{\mathcal{H}_{\mathrm{S}}\left(\mu_{\mathrm{S}}\right)}{T}
$$

Dropping the subscript $\mathrm{S}$, the normalized probabilities are given by

$$
p_{(T, \mathbf{x})}(\mu)=\frac{e^{-\beta \mathcal{H}(\mu)}}{Z(T, \mathbf{x})}
$$

The normalization,

$$
Z(T, \mathbf{x})=\sum_{\{\mu\}} e^{-\beta \mathcal{H}(\mu)}
$$

is known as the partition function, and $\beta \equiv 1 / k_{B} T$. (Note that probabilities similar to eq.(IV.56) were already obtained in eqs.(IV.25), and (IV.39), when considering a portion of the system in equilibrium with the rest of it.)

Is the internal energy $E$, of the system $\mathrm{S}$ well defined? Unlike in a microcanonical ensemble, the energy of a system exchanging heat with a reservoir is a random variable. Its probability distribution $p(\mathcal{E})$, is obtained by changing variables from $\mu$ to $\mathcal{H}(\mu)$ in $p(\mu)$, resulting in

$$
p(\mathcal{E})=\sum_{\{\mu\}} p(\mu) \delta(\mathcal{H}(\mu)-\mathcal{E})=\frac{e^{-\beta \mathcal{E}}}{Z} \sum_{\{\mu\}} \delta(\mathcal{H}(\mu)-\mathcal{E})
$$

Since the restricted sum is just the number $\Omega(\mathcal{E})$, of micro-states of appropriate energy,

$$
p(\mathcal{E})=\frac{\Omega(\mathcal{E}) e^{-\beta \mathcal{E}}}{Z}=\frac{1}{Z} \exp \left[\frac{S(\mathcal{E})}{k_{B}}-\frac{\mathcal{E}}{k_{B} T}\right]=\frac{1}{Z} \exp \left[-\frac{F(\mathcal{E})}{k_{B} T}\right]
$$

where we have set $F=\mathcal{E}-T S(\mathcal{E})$, in anticipation of its relation to the Helmholtz free energy. The probability $p(\mathcal{E})$, is sharply peaked at a most probable energy $E^{*}$, which minimizes $F(\mathcal{E})$. Using the result in sec.(II.F) for sums over exponentials,

$$
Z=\sum_{\{\mu\}} e^{-\beta \mathcal{H}(\mu)}=\sum_{\mathcal{E}} e^{-\beta F(\mathcal{E})} \approx e^{-\beta F\left(E^{*}\right)}
$$

The average energy computed from the distribution in eq.(IV.59) is

$$
\langle\mathcal{H}\rangle=\sum_{\mu} \mathcal{H}(\mu) \frac{e^{-\beta \mathcal{H}(\mu)}}{Z}=-\frac{1}{Z} \frac{\partial}{\partial \beta} \sum_{\mu} e^{-\beta \mathcal{H}}=-\frac{\partial \ln Z}{\partial \beta}
$$

In thermodynamics, a similar expression was encountered for the energy (eq.(I.37)),

$$
E=F+T S=F-\left.T \frac{\partial F}{\partial T}\right|_{\mathbf{x}}=-T^{2} \frac{\partial}{\partial T}\left(\frac{F}{T}\right)=\frac{\partial(\beta F)}{\partial \beta}
$$

Eqs.(IV.60) and (IV.61), both suggest identifying

$$
F(T, \mathbf{x})=-k_{B} T \ln Z(T, \mathbf{x})
$$

However, note that eq.(IV.60) refers to the most likely energy, while the average energy appears in eq.(IV.61). How close are these two values of the energy? We can get an idea of the width of the probability distribution $p(\mathcal{E})$, by computing the variance $\left\langle\mathcal{H}^{2}\right\rangle_{c} .$ This is most easily accomplished by noting that $Z(\beta)$ is proportional to the characteristic function for $\mathcal{H}$ (with $\beta$ replacing $i k$ ) and,

$$
-\frac{\partial Z}{\partial \beta}=\sum_{\mu} \mathcal{H} e^{-\beta \mathcal{H}}, \quad \text { and } \quad \frac{\partial^{2} Z}{\partial \beta^{2}}=\sum_{\mu} \mathcal{H}^{2} e^{-\beta \mathcal{H}}
$$

Cumulants of $\mathcal{H}$ are generated by $\ln Z(\beta)$,

$$
\langle\mathcal{H}\rangle_{c}=\frac{1}{Z} \sum_{\mu} \mathcal{H} e^{-\beta \mathcal{H}}=-\frac{1}{Z} \frac{\partial Z}{\partial \beta}=-\frac{\partial \ln Z}{\partial \beta}
$$

and

$$
\left\langle\mathcal{H}^{2}\right\rangle_{c}=\left\langle\mathcal{H}^{2}\right\rangle-\langle\mathcal{H}\rangle^{2}=\frac{1}{Z} \sum_{\mu} \mathcal{H}^{2} e^{-\beta \mathcal{H}}-\frac{1}{Z^{2}}\left(\sum_{\mu} \mathcal{H} e^{-\beta \mathcal{H}}\right)^{2}=\frac{\partial^{2} \ln Z}{\partial \beta^{2}}=-\frac{\partial\langle\mathcal{H}\rangle}{\partial \beta}
$$

More generally, the $n^{\text {th }}$ cumulant of $\mathcal{H}$ is given by

$$
\left\langle\mathcal{H}^{n}\right\rangle_{c}=(-1)^{n} \frac{\partial^{n} \ln Z}{\partial \beta^{n}}
$$

From eq.(IV.66),

$$
\left\langle\mathcal{H}^{2}\right\rangle_{c}=-\frac{\partial\langle\mathcal{H}\rangle}{\partial\left(1 / k_{B} T\right)}=\left.k_{B} T^{2} \frac{\partial\langle\mathcal{H}\rangle}{\partial T}\right|_{\mathbf{x}}, \quad \Rightarrow \quad\left\langle\mathcal{H}^{2}\right\rangle_{c}=k_{B} T^{2} C_{\mathbf{x}}
$$

where we have identified the heat capacity with the thermal derivative of the average energy $\langle\mathcal{H}\rangle$. Eq.(IV.68) shows that it is justified to treat the mean and most likely energies interchangeably, since the width of the distribution $p(\mathcal{E})$, only grows as $\sqrt{\left\langle\mathcal{H}^{2}\right\rangle_{c}} \propto N^{1 / 2}$ The relative error, $\sqrt{\left\langle\mathcal{H}^{2}\right\rangle_{c}} /\langle\mathcal{H}\rangle_{c}$ vanishes in the thermodynamic limit as $1 / \sqrt{N}$. (In fact eq.(IV.67) shows that all cumulants of $\mathcal{H}$ are proportional to $N .)$ The PDF for energy in a canonical ensemble can thus be approximated by

$$
p(\mathcal{E})=\frac{1}{Z} e^{-\beta F(\mathcal{E})} \approx \exp \left(-\frac{(\mathcal{E}-\langle\mathcal{H}\rangle)^{2}}{2 k_{B} T^{2} C_{\mathbf{x}}}\right) \frac{1}{\sqrt{2 \pi k_{B} T^{2} C_{\mathbf{x}}}}
$$

The above distribution is sufficiently sharp to make the internal energy in a canonical ensemble unambiguous in the $N \rightarrow \infty$ limit. Some care is necessary if the heat capacity $C_{\mathbf{x}}$ is divergent, as is the case in some continuous phase transitions.

The canonical probabilities in eq.(IV.56) are unbiased estimates obtained (as in sec.(II.G)) by constraining the average energy. The entropy of the canonical ensemble can also be calculated directly from eq.(IV.56) (using eq.(III.68)) as

$$
S=-k_{B}\langle\ln p(\mu)\rangle=-k_{B}\langle(-\beta \mathcal{H}-\ln Z)\rangle=\frac{E-F}{T}
$$

again using the identification of $\ln Z$ with the free energy from eq.(IV.63). For any finite system, the canonical and microcanonical probabilities are distinct. However, in the so called thermodynamic limit of $N \rightarrow \infty$ limit, the canonical probabilities are so sharply peaked around the average energy that they are essentially indistinct from microcanonical probabilities at that energy. The following table compares the prescriptions used in the two ensembles.

\begin{tabular}{|c|c|c|c|}
\hline Ensemble & Macro-state & $p(\mu)$ & Normalization \\
\hline \hline Microcanonical & $(E, \mathbf{x})$ & $\delta_{\Delta}(\mathcal{H}(\mu)-E) / \Omega$ & $S(E, \mathbf{x})=k_{B} \ln \Omega$ \\
\hline Canonical & $(T, \mathbf{x})$ & $\exp (-\beta \mathcal{H}(\mu)) / Z$ & $F(T, \mathbf{x})=-k_{B} T \ln Z$ \\
\hline
\end{tabular}

Table 3: Comparison of canonical and microcanonical ensembles. MIT OpenCourseWare

http://ocw.mit.edu

\subsection{Statistical Mechanics I: Statistical Mechanics of Particles \\ Fall 2013}

For information about citing these materials or our Terms of Use, visit: http://ocw.mit.edu/terms.
