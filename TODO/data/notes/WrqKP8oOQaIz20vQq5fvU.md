\section{VI.D Quantum microstates}

In the previous sections we indicated several failures of classical statistical mechanics, which were heuristically remedied by assuming quantized energy levels, while still calculating thermodynamic quantities from a partition sum $Z=\sum_{n} \exp \left(-\beta E_{n}\right)$. This implicitly assumes that the micro-states of a quantum system are specified by its discretized energy levels, and governed by a probability distribution similar to a Boltzmann weight. This 'analogy' to classical statistical mechanics needs to be justified. Furthermore, quantum mechanics is itself inherently probabilistic, with uncertainties unrelated to those that lead to probabilities in statistical mechanics. Here, we shall construct a quantum formulation of statistical mechanics by closely following the steps that lead to the classical formulation.

Micro-states of a classical system of particles are described by the set of coordinates and conjugate momenta $\left\{\vec{p}_{i}, \vec{q}_{i}\right\} ;$ i.e. by a point in the $6 N$ -dimensional phase space. In quantum mechanics $\left\{\vec{q}_{i}\right\}$ and $\left\{\vec{p}_{i}\right\}$ are not independent observables. Instead:

- The (micro-) state of a quantum system is completely specified by a unit vector $|\Psi\rangle$, which belongs to an infinite dimensional Hilbert space. The vector $|\Psi\rangle$ can be written in terms of its components $\langle n \mid \Psi\rangle$, which are complex numbers, along a suitable set of ortho-normal basis vectors $|n\rangle .$ In the convenient notation introduced by Dirac, this decomposition is written as

$$
|\Psi\rangle=\sum_{n}\langle n \mid \Psi\rangle|n\rangle
$$

The most familiar basis is that of coordinates $\left|\left\{\vec{q}_{i}\right\}\right\rangle$, and $\left\langle\left\{\vec{q}_{i}\right\} \mid \Psi\right\rangle \equiv \Psi\left(\vec{q}_{1}, \ldots, \vec{q}_{N}\right)$ is the wave-function. The normalization condition is

$$
\langle\Psi \mid \Psi\rangle=\sum_{n}\langle\Psi \mid n\rangle\langle n \mid \Psi\rangle=1, \quad \text { where } \quad\langle\Psi \mid n\rangle \equiv\langle n \mid \Psi\rangle^{*}
$$

For example, in the coordinate basis, we must require

$$
\langle\Psi \mid \Psi\rangle=\int \prod_{i=1}^{N} d^{d} \vec{q}_{i}\left|\Psi\left(\vec{q}_{1}, \ldots, \vec{q}_{N}\right)\right|^{2}=1
$$

- Classically, various observables are functions $\mathcal{O}\left(\left\{\vec{p}_{i}, \vec{q}_{i}\right\}\right)$, defined in phase space. In quantum mechanics, these functions are replaced by Hermitian matrices (operators) in Hilbert space, obtained by substituting operators for $\left\{\vec{q}_{i}\right\}$ and $\left\{\vec{p}_{i}\right\}$ in the classical expression (after proper symmetrization of products, e.g. $p q \rightarrow(p q+q p) / 2)$. These basic operators satisfy the commutation relations,

$$
\left[p_{j}, q_{k}\right] \equiv p_{j} q_{k}-q_{k} p_{j}=\frac{\hbar}{i} \delta_{j, k}
$$

For example, in the coordinate basis $\left|\left\{\vec{q}_{i}\right\}\right\rangle$, the momentum operators are

$$
p_{j}=\frac{\hbar}{i} \frac{\partial}{\partial q_{j}}
$$

(Note that classical Poisson brackets satisfy $\left\{p_{j}, q_{k}\right\}=-\delta_{j, k} .$ Quite generally, quantum commutation relations are obtained by multiplying the corresponding classical Poisson brackets by $i \hbar .)$

- Unlike in classical mechanics, the value of an operator $\mathcal{O}$ is not uniquely determined for a particular micro-state. It is instead a random variable, whose average in a state $|\Psi\rangle$ is given by

$$
\langle\mathcal{O}\rangle \equiv\langle\Psi|\mathcal{O}| \Psi\rangle \equiv \sum_{m, n}\langle\Psi \mid m\rangle\langle m|\mathcal{O}| n\rangle\langle n \mid \Psi\rangle
$$

For example,

$$
\begin{aligned}
&\langle U(\{\vec{q}\})\rangle=\int \prod_{i=1}^{N} d^{3} \vec{q}_{i} \Psi^{*} U(\{\vec{q}\}) \Psi, \quad \text { and } \\
&\langle K(\{\vec{p}\})\rangle=\int \prod_{i=1}^{N} d^{3} \vec{q}_{i} \Psi^{*} K\left(\left\{\frac{\hbar}{i} \frac{d}{d \vec{q}}\right\}\right) \Psi
\end{aligned}
$$

To ensure that the expectation value $\langle\mathcal{O}\rangle$ is real, the operators $\mathcal{O}$ must be Hermitian, i.e. satisfy

$$
\mathcal{O}^{\dagger}=\mathcal{O}, \quad \text { where } \quad\left\langle m\left|\mathcal{O}^{\dagger}\right| n\right\rangle \equiv\langle n|\mathcal{O}| m\rangle^{*}
$$

When replacing $\vec{p}$ and $\vec{q}$ in a classical operator $\mathcal{O}\left(\left\{\vec{p}_{i}, \vec{q}_{i}\right\}\right)$ by corresponding matrices, proper symmetrization of various products is necessary to ensure the above Hermiticity.

Time evolution of micro-states is governed by the Hamiltonian $\mathcal{H}\left(\left\{\vec{p}_{i}, \vec{q}_{i}\right\}\right) .$ A classical microstate evolves according to Hamilton's equations of motion, while in quantum mechanics the state vector changes in time according to

$$
i \hbar \frac{\partial}{\partial t}|\Psi(t)\rangle=\mathcal{H}|\Psi(t)\rangle
$$

A convenient basis is one that diagonalizes the matrix $\mathcal{H}$. The energy eigen-states satisfy $\mathcal{H}|n\rangle=\mathcal{E}_{n}|n\rangle$, where $\mathcal{E}_{n}$ are the eigen-energies. Substituting $|\Psi(t)\rangle=\sum_{n}\langle n \mid \Psi(t)\rangle|n\rangle$ in eq.(VI.69), and taking advantage of the ortho-normality condition $\langle m \mid n\rangle=\delta_{m, n}$, yields

$$
i \hbar \frac{d}{d t}\langle n \mid \Psi(t)\rangle=\mathcal{E}_{n}\langle n \mid \Psi(t)\rangle, \quad \Longrightarrow \quad\langle n \mid \Psi(t)\rangle=\exp \left(-\frac{i \mathcal{E}_{n} t}{\hbar}\right)\langle n \mid \Psi(0)\rangle
$$

The quantum states at two different times can be related by a time evolution operator, as

$$
|\Psi(t)\rangle=U\left(t, t_{0}\right)\left|\Psi\left(t_{0}\right)\right\rangle
$$

which satisfies $i \hbar \partial_{t} U\left(t, t_{0}\right)=\mathcal{H} U\left(t, t_{0}\right)$, with the boundary condition $U\left(t_{0}, t_{0}\right)=1 .$ If $\mathcal{H}$ is independent of $t$, we can solve these equations to yield

$$
U\left(t, t_{0}\right)=\exp \left[-\frac{i}{\hbar} \mathcal{H}\left(t-t_{0}\right)\right]
$$

\section{VI.E Quantum macrostates}

Macro-states of the system depend on only a few thermodynamic functions. We can form an ensemble of a large number $\mathcal{N}$, of micro-states $\mu_{\alpha}$, corresponding to a given macrostate. The different micro-states occur with probabilities $p_{\alpha} .$ (For example $p_{\alpha}=1 / \mathcal{N}$ in the absence of any other information.) When we no longer have exact knowledge of the microstate, it is said to be in a mixed state.

Classically, ensemble averages are calculated from

$$
\overline{\mathcal{O}\left(\left\{\vec{p}_{i}, \vec{q}_{i}\right\}\right)_{t}}=\sum_{\alpha} p_{\alpha} \mathcal{O}\left(\mu_{\alpha}(t)\right)=\int \prod_{i=1}^{N} d^{3} \vec{p}_{i} d^{3} \overrightarrow{q_{i}} \mathcal{O}\left(\left\{\vec{p}_{i}, \vec{q}_{i}\right\}\right) \rho\left(\left\{\vec{p}_{i}, \vec{q}_{i}\right\}, t\right)
$$

where

$$
\rho\left(\left\{\vec{p}_{i}, \vec{q}_{i}\right\}, t\right)=\sum_{\alpha} p_{\alpha} \prod_{i=1}^{N} \delta^{3}\left(\vec{q}_{i}-\vec{q}_{i}(t)_{\alpha}\right) \delta^{3}\left(\vec{p}_{i}-\vec{p}_{i}(t)_{\alpha}\right)
$$

is the ensemble density.

Similarly, a mixed quantum state is obtained from a set of possible states $\left\{\left|\psi_{\alpha}\right\rangle\right\}$, with probabilities $\left\{p_{\alpha}\right\}$. The ensemble average of the quantum mechanical expectation value in eq.(VI.67) is then given by

$$
\begin{aligned}
\overline{\langle\mathcal{O}\rangle} &=\sum_{\alpha} p_{\alpha}\left\langle\Psi_{\alpha}|\mathcal{O}| \Psi_{\alpha}\right\rangle=\sum_{\alpha, m, n} p_{\alpha}\left\langle\Psi_{\alpha} \mid m\right\rangle\left\langle n \mid \Psi_{\alpha}\right\rangle\langle m|\mathcal{O}| n\rangle \\
&=\sum_{m, n}\langle n|\rho| m\rangle\langle m|\mathcal{O}| n\rangle=\operatorname{tr}(\rho \mathcal{O})
\end{aligned}
$$

where we have introduced a basis $\{|n\rangle\}$, and defined the density matrix

$$
\langle n|\rho(t)| m\rangle \equiv \sum_{\alpha} p_{\alpha}\left\langle n \mid \Psi_{\alpha}(t)\right\rangle\left\langle\Psi_{\alpha}(t) \mid m\right\rangle
$$

Classically, the probability (density) $\rho(t)$ is a function defined on phase space. As all operators in phase space, it is replaced by a matrix in quantum mechanics. Stripped of the choice of basis, the density matrix is

$$
\rho(t)=\sum_{\alpha} p_{\alpha}\left|\Psi_{\alpha}(t)\right\rangle\left\langle\Psi_{\alpha}(t)\right|
$$

Clearly, $\rho$ corresponds to a pure state if and only if $\rho^{2}=\rho$

The density matrix satisfies the following properties:

(i) Normalization: Since each $\left|\Psi_{\alpha}\right\rangle$ is normalized to unity,

$$
\langle 1\rangle=\operatorname{tr}(\rho)=\sum_{n}\langle n|\rho| n\rangle=\sum_{\alpha, n} p_{\alpha}\left|\left\langle n \mid \Psi_{\alpha}\right\rangle\right|^{2}=\sum_{\alpha} p_{\alpha}=1
$$

(ii) Hermiticity: The density matrix is Hermitian, i.e. $\rho^{\dagger}=\rho$, since

$$
\left\langle m\left|\rho^{\dagger}\right| n\right\rangle=\langle n|\rho| m\rangle^{*}=\sum_{\alpha} p_{\alpha}\left\langle\Psi_{\alpha} \mid m\right\rangle\left\langle n \mid \Psi_{\alpha}\right\rangle=\langle n|\rho| m\rangle
$$

ensuring that the averages in eq.(VI.76) are real numbers.

(iii) Positivity: For any $|\Phi\rangle$,

$$
\langle\Phi|\rho| \Phi\rangle=\sum_{\alpha} p_{\alpha}\left\langle\Phi \mid \Psi_{\alpha}\right\rangle\left\langle\Psi_{\alpha} \mid \Phi\right\rangle=\sum_{\alpha} p_{\alpha}\left|\left\langle\Phi \mid \Psi_{\alpha}\right\rangle\right|^{2} \geq 0
$$

Thus $\rho$ is positive definite, implying that all its eigenvalues must be positive.

- Liouville's theorem governs the time evolution of the classical density as

$$
\frac{d \rho}{d t}=\frac{\partial \rho}{\partial t}-\{\mathcal{H}, \rho\}=0
$$

It is most convenient to examine the evolution of the quantum density matrix in the basis of energy eigen-states, where according to eq.(VI.70)

$$
\begin{aligned}
i \hbar \frac{\partial}{\partial t}\langle n|\rho(t)| m\rangle &=i \hbar \frac{\partial}{\partial t} \sum_{\alpha} p_{\alpha}\left\langle n \mid \Psi_{\alpha}(t)\right\rangle\left\langle\Psi_{\alpha}(t) \mid m\right\rangle \\
&=\sum_{\alpha} p_{\alpha}\left[\left(\mathcal{E}_{n}-\mathcal{E}_{m}\right)\left\langle n \mid \Psi_{\alpha}\right\rangle\left\langle\Psi_{\alpha} \mid m\right\rangle\right] \\
&=\langle n|(\mathcal{H} \rho-\rho \mathcal{H})| m\rangle
\end{aligned}
$$

The final result is a tensorial identity, and hence, independent of the choice of basis

$$
i \hbar \frac{\partial}{\partial t} \rho=[\mathcal{H}, \rho]
$$

Equilibrium requires time independent averages, and suggests $\partial \rho / \partial t=0 .$ This condition is satisfied in both eqs.(VI.81) and (VI.83) by choosing $\rho=\rho(\mathcal{H}) .$ (As discussed in chapter III, $\rho$ may also depend on conserved quantities such that $[\mathcal{H}, L]=0 .)$ Various equilibrium quantum density matrices can now be constructed in analogy to classical statistical mechanics.

- Microcanonical ensemble: As the internal energy has a fixed value $E$, a density matrix that includes this constraint is

$$
\rho(E)=\frac{\delta(\mathcal{H}-E)}{\Omega(E)}
$$

In particular, in the basis of energy eigen-states,

$$
\langle n|\rho| m\rangle=\sum_{\alpha} p_{\alpha}\left\langle n \mid \Psi_{\alpha}\right\rangle\left\langle\Psi_{\alpha} \mid m\right\rangle= \begin{cases}\frac{1}{\Omega} & \text { if } \mathcal{E}_{n}=E, \text { and } m=n \\ 0 & \text { if } \mathcal{E}_{n} \neq E, \text { or } m \neq n\end{cases}
$$

The first condition states that only eigen-states of the correct energy can appear in the quantum wave-function, and that (for $\left.p_{\alpha}=1 / \mathcal{N}\right)$ such states on average have the same amplitude, $\overline{\left.\langle n \mid \Psi\rangle\right|^{2}}=1 / \Omega .$ This is equivalent to the classical postulate of equal a priori equilibrium probabilities. The second (additional) condition states that the $\Omega$ eigen-states of energy $E$ are combined in a typical micro-state with independent random phases. (Note that the normalization condition $\operatorname{tr} \rho=1$, implies that $\Omega(E)=\sum_{n} \delta\left(E-E_{n}\right)$ is the number of eigen-states of $\mathcal{H}$ with energy $E .)$

- Canonical ensemble: A fixed temperature $T=1 / k_{B} \beta$, can be achieved by putting the system in contact with a reservoir. By considering the combined system, the canonical density matrix is obtained as

$$
\rho(\beta)=\frac{\exp (-\beta \mathcal{H})}{Z(\beta)}
$$

The normalization condition $\operatorname{tr}(\rho)=1$, leads to the quantum partition function

$$
Z=\operatorname{tr}\left(e^{-\beta \mathcal{H}}\right)=\sum_{n} e^{-\beta \mathcal{E}_{n}}
$$

The final sum is over the (discrete) energy levels of $\mathcal{H}$, and justifies the calculations performed in the previous sections.

- Grand Canonical Ensemble: The number of particles $N$, is no longer fixed. Quantum micro-states with indefinite particle number span a so called Fock space. The density matrix is

$$
\rho(\beta, \mu)=\frac{e^{-\beta \mathcal{H}+\beta \mu N}}{\mathcal{Q}}, \quad \text { where } \quad \mathcal{Q}(\beta, \mu)=\operatorname{tr}\left(e^{-\beta \mathcal{H}+\beta \mu N}\right)=\sum_{N=0}^{\infty} e^{\beta \mu N} Z_{N}(\beta)
$$

Example: Consider a single particle in a quantum canonical ensemble in a box of volume $V$. The energy eigen-states of the Hamiltonian

$$
\mathcal{H}_{1}=\frac{\vec{p}^{2}}{2 m}=-\frac{\hbar^{2}}{2 m} \nabla^{2}, \quad \text { (in coordinate basis) }
$$

obtained from $\mathcal{H}_{1}|\vec{k}\rangle=\mathcal{E}(\vec{k})|\vec{k}\rangle$, are

$$
\langle\vec{x} \mid \vec{k}\rangle=\frac{e^{i \vec{k} \cdot \vec{x}}}{\sqrt{V}}, \quad \text { with } \quad \mathcal{E}(\vec{k})=\frac{\hbar^{2} k^{2}}{2 m}
$$

With periodic boundary conditions in a box of size $L$, the allowed values of $\vec{k}$ are $(2 \pi / L)\left(\ell_{x}, \ell_{y}, \ell_{z}\right)$, where $\left(\ell_{x}, \ell_{y}, \ell_{z}\right)$ are integers. A particular vector in this one-particle Hilbert space is specified by its components along each of these basis states (infinite in number). The space of quantum micro-states is thus much larger than the corresponding 6-dimensional classical phase space. The partition function for $L \rightarrow \infty$,

$$
\begin{aligned}
Z_{1} &=\operatorname{tr}(\rho)=\sum_{\vec{k}} \exp \left(-\frac{\beta \hbar^{2} k^{2}}{2 m}\right)=V \int \frac{d^{3} \vec{k}}{(2 \pi)^{3}} \exp \left(-\frac{\beta \hbar^{2} k^{2}}{2 m}\right) \\
&=\frac{V}{(2 \pi)^{3}}\left(\sqrt{\frac{2 \pi m k_{B} T}{\hbar^{2}}}\right)^{3}=\frac{V}{\lambda^{3}}
\end{aligned}
$$

coincides with the classical result, with $\lambda=h / \sqrt{2 \pi m k T}$ (justifying the use of $d^{3} \vec{p} d^{3} \vec{q} / h^{3}$ as the correct dimensionless measure of phase space). Elements of the density matrix in a coordinate representation are

$$
\begin{aligned}
\left\langle\vec{x}^{\prime}|\rho| \vec{x}\right\rangle &=\sum_{\vec{k}}\left\langle\vec{x}^{\prime} \mid \vec{k}\right\rangle \frac{e^{-\beta \mathcal{E}(\vec{k})}}{Z_{1}}\langle\vec{k} \mid \vec{x}\rangle=\frac{\lambda^{3}}{V} \int \frac{V d^{3} \vec{k}}{(2 \pi)^{3}} \frac{e^{-i \vec{k} \cdot\left(\vec{x}-\vec{x}^{\prime}\right)}}{V} \exp \left(-\frac{\beta \hbar^{2} k^{2}}{2 m}\right) \\
&=\frac{1}{V} \exp \left[-\frac{m\left(\vec{x}-\vec{x}^{\prime}\right)^{2}}{2 \beta \hbar^{2}}\right]=\frac{1}{V} \exp \left[-\frac{\pi\left(\vec{x}-\vec{x}^{\prime}\right)^{2}}{\lambda^{2}}\right]
\end{aligned}
$$

The diagonal elements, $\langle\vec{x}|\rho| \vec{x}\rangle=1 / V$, are just the probabilities for finding a particle at $\vec{x}$. The off-diagonal elements have no classical analog. They suggest that the appropriate way to think of the particle is as a wave-packet of size $\lambda=h / \sqrt{2 \pi m k_{B} T}$, the thermal wavelength. As $T \rightarrow \infty, \lambda$ goes to zero, and the classical analysis is valid. As $T \rightarrow 0$, $\lambda$ diverges and quantum mechanical effects take over when $\lambda$ becomes comparable to the size of the box.

Alternatively, we could have obtained eq.(VI.92), by noting that eq.(VI.86) implies

$$
\frac{\partial}{\partial \beta} Z \rho=-\mathcal{H} Z \rho=\frac{\hbar^{2}}{2 m} \nabla^{2} Z \rho
$$

This is just the diffusion equation (for the free particle), which can be solved subject to the initial condition $\rho(\beta=0)=1$ (i.e. $\left.\left\langle\vec{x}^{\prime}|\rho(\beta=0)| \vec{x}\right\rangle=\delta^{3}\left(\vec{x}-\vec{x}^{\prime}\right) / V\right)$ to yield the result of eq.(VI.92). MIT OpenCourseWare

http://ocw.mit.edu

\subsection{Statistical Mechanics I: Statistical Mechanics of Particles \\ Fall 2013}

For information about citing these materials or our Terms of Use, visit: http://ocw.mit.edu/terms.
