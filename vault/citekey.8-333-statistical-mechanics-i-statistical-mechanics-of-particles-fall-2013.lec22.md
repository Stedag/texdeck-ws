---
id: 3tUTvsVmlLyyPFHbYot4A
title: Lec22
desc: ''
updated: 1637530120232
created: 1637530120232
---
\section{Ideal Quantum Gases}

\section{VII.A Hilbert Space of Identical Particles}

In chapter IV, we discussed the Gibbs paradox for the mixing entropy of gases of identical particles. This difficulty was overcome by postulating that the phase space for $N$ identical particles must be divided by $N !$, the number of permutations. This is not quite satisfactory as the classical equations of motion implicitly treat the particles as distinct. In quantum mechanics, by contrast, the identity of particles appears at the level of allowed states in Hilbert space. For example, the probability of finding two identical particles at positions $\vec{x}_{1}$ and $\vec{x}_{2}$ is $\left|\Psi\left(\vec{x}_{1}, \vec{x}_{2}\right)\right|^{2} .$ Since the exchange of particles 1 and 2 leads to the same configurations, we must have $\left|\Psi\left(\vec{x}_{1}, \vec{x}_{2}\right)\right|^{2}=\left|\Psi\left(\vec{x}_{2}, \vec{x}_{1}\right)\right|^{2}$. For a single-valued function, this leads to two possibilities:

$$
|\psi(1,2)\rangle=+|\psi(2,1)\rangle, \quad \text { or } \quad|\psi(1,2)\rangle=-|\psi(2,1)\rangle
$$

The Hilbert space used to describe identical particles is thus restricted to obey certain symmetries.

For a system of $N$ identical particles, there are $N !$ permutations $P$, forming a group $S_{N} .$ There are several ways for representing a permutation; e.g., $P(1234)=(3241)$ for $N=4$ can alternatively be indicated by

$$
P=\left(\begin{array}{cccc}
1 & 2 & 3 & 4 \\
3 & 2 & 4 & 1
\end{array}\right)
$$

Any permutation can be obtained from a sequence of two particle exchanges. For example, the above permutation is obtained by the exchanges $(1,3)$ and $(1,4)$ performed in sequence. The parity of a permutation is defined as

$$
(-1)^{P} \equiv \begin{cases}+1 & \text { if } P \text { involves to an even number of exchanges, e.g. }(123) \rightarrow(231) \\ -1 & \text { if } P \text { involves an odd number of exchanges, e.g. }(123) \rightarrow(213)\end{cases}
$$

(Note that if lines are drawn connecting the initial an final locations of each integer in eq.(VII.2), the parity is $(-1)$ raised to the number of intersections of these lines.)

The action of permutations on an $N$ -particle quantum state leads to a representation of the permutation group in Hilbert space. Requiring the wave-function to be single valued, and to give equal probabilities under particle exchange, restricts the representation to be MIT OpenCourseWare

http://ocw.mit.edu

\subsection{Statistical Mechanics I: Statistical Mechanics of Particles \\ Fall 2013}

For information about citing these materials or our Terms of Use, visit: http://ocw.mit.edu/terms. either fully symmetric or anti-symmetric. This allows for two types of identical particles in nature:

(1) Bosons correspond to the fully symmetric representation such that

$$
P|\psi(1, \cdots, N)\rangle=+|\psi(1, \cdots, N)\rangle
$$

(2) Fermions correspond to the fully anti-symmetric representation such that

$$
P|\psi(1, \cdots, N)\rangle=(-1)^{P}|\psi(1, \cdots, N)\rangle
$$

Of course, the Hamiltonian for identical particles must itself be symmetric, i.e. $P \mathcal{H}=$ $\mathcal{H}$. However, for a given $\mathcal{H}$, there are many eigen-states with different symmetries under permutations. To select the correct set of eigen-states, in quantum mechanics the statistics of the particles (bosons or fermions) is specified independently. For example, consider $N$ non-interacting particles in a box of volume $V$, with a Hamiltonian

$$
\mathcal{H}=\sum_{\alpha=1}^{N} \mathcal{H}_{\alpha}=\sum_{\alpha=1}^{N}\left(-\frac{\hbar^{2}}{2 m} \nabla_{\alpha}^{2}\right)
$$

Each $\mathcal{H}_{\alpha}$ can be separately diagonalized, with plane wave states $\{|\vec{k}\rangle\}$ and corresponding energies $\mathcal{E}(\vec{k})=\hbar^{2} k^{2} / 2 m .$ Using sums and products of these one-particle states, we can construct the following $-N$ particle states:

(1) The product Hilbert space is obtained by simple multiplication of the one-body states, i.e.

$$
\left|\vec{k}_{1}, \cdots, \vec{k}_{N}\right\rangle_{\otimes} \equiv\left|\vec{k}_{1}\right\rangle \cdots\left|\vec{k}_{N}\right\rangle
$$

In the coordinate representation,

$$
\left\langle\vec{x}_{1}, \cdots, \vec{x}_{N} \mid \vec{k}_{1}, \cdots, \vec{k}_{N}\right\rangle_{\otimes}=\frac{1}{V^{N / 2}} \exp \left(i \sum_{\alpha=1}^{N} \vec{k}_{\alpha} \cdot \vec{x}_{\alpha}\right)
$$

and

$$
\mathcal{H}\left|\vec{k}_{1}, \cdots, \vec{k}_{N}\right\rangle_{\otimes}=\left(\sum_{\alpha=1}^{N} \frac{\hbar^{2}}{2 m} k_{\alpha}^{2}\right)\left|\vec{k}_{1}, \cdots, \vec{k}_{N}\right\rangle_{\otimes}
$$

But the product states do not satisfy the symmetry requirements for identical particles, and we must find the appropriate subspaces of correct symmetry. (2) The fermionic subspace is constructed as

$$
\left|\vec{k}_{1}, \cdots, \vec{k}_{N}\right\rangle_{-}=\frac{1}{\sqrt{N_{-}}} \sum_{P}(-1)^{P} P\left|\vec{k}_{1}, \cdots, \vec{k}_{N}\right\rangle_{\otimes}
$$

where the sum is over all $N !$ permutations. Clearly, if any one-particle label $\vec{k}$, appears more than once in the above list, the result is zero and there is no anti-symmetrized state. Anti-symmetrization is possible only when all the $N$ values of $\vec{k}_{\alpha}$ are different. In this case, there are $N !$ terms in the above sum, and $N_{-}=N !$ is necessary to ensure normalization. For example, a two-particle anti-symmetrized state is

$$
\left|\vec{k}_{1}, \vec{k}_{2}\right\rangle_{-}=\frac{\left(\left|\vec{k}_{1}, \vec{k}_{2}\right\rangle-\left|\vec{k}_{2}, \vec{k}_{1}\right\rangle\right)}{\sqrt{2}}
$$

(If not otherwise indicated, $\left|\vec{k}_{1}, \cdots, \vec{k}_{N}\right\rangle$ refers to the product state.)

(3) Similarly, the bosonic subspace is constructed as

$$
\left|\vec{k}_{1}, \cdots, \vec{k}_{N}\right\rangle_{+}=\frac{1}{\sqrt{N_{+}}} \sum_{P} P\left|\vec{k}_{1}, \cdots, \vec{k}_{N}\right\rangle_{\otimes}
$$

In this case, there are no restrictions on the allowed values of $\vec{k}$. A particular oneparticle state may be repeated $n_{\vec{k}}$ times in the list, with $\sum_{\vec{k}} n_{\vec{k}}=N .$ As we shall prove shortly, proper normalization requires $N_{+}=N ! \prod_{\vec{k}} n_{\vec{k}} ! . \quad$ For example, a correctly normalized 3-particle bosonic state is constructed from two one-particle states $|\alpha\rangle$, and one one- particle state $|\beta\rangle$ as $\left(n_{\alpha}=2, n_{\beta}=1\right.$, and $\left.N_{+}=3 ! 2 ! 1 !=12\right)$

$$
\begin{aligned}
|\alpha \alpha \beta\rangle_{+} &=\frac{1}{\sqrt{12}}(|\alpha\rangle|\alpha\rangle|\beta\rangle+|\alpha\rangle|\beta\rangle|\alpha\rangle+|\beta\rangle|\alpha\rangle|\alpha\rangle+|\alpha\rangle|\alpha\rangle|\beta\rangle+|\beta\rangle|\alpha\rangle|\alpha\rangle+|\alpha\rangle|\beta\rangle|\alpha\rangle) \\
&=\frac{1}{\sqrt{3}}(|\alpha\rangle|\alpha\rangle|\beta\rangle+|\alpha\rangle|\beta\rangle|\alpha\rangle+|\beta\rangle|\alpha\rangle|\alpha\rangle)
\end{aligned}
$$

- It is convenient to discuss bosons and fermions simultaneously by defining

$$
|\{\vec{k}\}\rangle_{\eta}=\frac{1}{\sqrt{N_{\eta}}} \sum_{P} \eta^{P} P|\{\vec{k}\}\rangle, \text { with } \eta= \begin{cases}+1 & \text { for bosons } \\ -1 & \text { for fermions }\end{cases}
$$

Each state is uniquely specified by a set of occupation numbers $\left\{n_{\vec{k}}\right\}$, such that $\sum_{\vec{k}} n_{\vec{k}}=N$, and

(1) For fermions, $|\{\vec{k}\}\rangle_{-}=0$, unless $n_{\vec{k}}=0$ or 1, and $N_{-}=N ! \prod_{k} n_{\vec{k}} !=N !$

(2) For bosons, any $\vec{k}$ may be repeated $n_{\vec{k}}$ times, and the normalization is calculated from

$$
\begin{aligned}
+\langle\{\vec{k}\} \mid\{\vec{k}\}\rangle_{+} &=\frac{1}{N_{+}} \sum_{P, P^{\prime}}\left\langle P\{\vec{k}\} \mid P^{\prime}\{\vec{k}\}\right\rangle=\frac{N !}{N_{+}} \sum_{P}\langle\{\vec{k}\} \mid P\{\vec{k}\}\rangle \\
&=\frac{N ! \prod_{\vec{k}} n_{\vec{k}} !}{N_{+}}=1, \quad \Rightarrow \quad N_{+}=N ! \prod_{k} n_{\vec{k}} !
\end{aligned}
$$

(The $\operatorname{term}\langle\{\vec{k}\} \mid P\{\vec{k}\}\rangle$ is zero unless the permuted $\vec{k}$ 's are identical to the original set, which happens $\prod_{\vec{k}} n_{\vec{k}} !$ times. $)$
