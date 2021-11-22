---
id: MqYqthMjNgnNdkwI5jUDy
title: Lec15
desc: ''
updated: 1637530120228
created: 1637530120228
---
\section{Interacting Particles}

\section{V.A The Cumulant Expansion}

The examples studied in the previous section involve non-interacting particles. It is precisely the lack of interactions that renders these problems exactly solvable. Interactions, however, are responsible for the wealth of interesting materials and phases observed in nature. We would thus like to understand the role of interactions amongst particles, and learn how to treat them in statistical mechanics. For a general Hamiltonian,

$$
\mathcal{H}_{N}=\sum_{i=1}^{N} \frac{\vec{p}_{i}^{2}}{2 m}+\mathcal{U}\left(\vec{q}_{1}, \cdots, \vec{q}_{N}\right)
$$

the partition function can be written as

$$
\begin{aligned}
Z(T, V, N) &=\frac{1}{N !} \int \prod_{i=1}^{N}\left(\frac{d^{3} \vec{p}_{i} d^{3} \vec{q}_{i}}{h^{3}}\right) \exp \left[-\beta \sum_{i} \frac{\vec{p}_{i}^{2}}{2 m}\right] \exp \left[-\beta \mathcal{U}\left(\vec{q}_{1}, \cdots, \vec{q}_{N}\right)\right] \\
&=Z_{0}(T, V, N)\left\langle\exp \left[-\beta \mathcal{U}\left(\vec{q}_{1}, \cdots, \vec{q}_{N}\right)\right]\right\rangle^{0}
\end{aligned}
$$

where $Z_{0}(T, V, N)=\left(V / \lambda^{3}\right)^{N} / N !$ is the partition function of the ideal gas $($ eq. $($ IV. 73$))$ and $\langle\mathcal{O}\rangle^{0}$ denotes the expectation value of $\mathcal{O}$ computed with the probability distribution of the non-interacting system. In terms of the cumulants of the random variable $\mathcal{U}$, eq.(V.2) can be recast as

$$
\ln Z=\ln Z_{0}+\sum_{\ell=1}^{\infty} \frac{(-\beta)^{\ell}}{\ell !}\left\langle\mathcal{U}^{\ell}\right\rangle_{c}^{0}
$$

The cumulants are related to the moments by the relations in section II.B. Since $\mathcal{U}$ depends only on $\left\{\vec{q}_{i}\right\}$ which are uniformly and independently distributed within the box of volume $V$, the moments are given by

$$
\left\langle\mathcal{U}^{\ell}\right\rangle^{0}=\int\left(\prod_{i=1}^{N} \frac{d^{3} \vec{q}_{i}}{V}\right) \mathcal{U}\left(\vec{q}_{1}, \cdots, \vec{q}_{N}\right)^{\ell}
$$

Various expectation values can also be calculated perturbatively, from

$$
\begin{aligned}
\langle\mathcal{O}\rangle &=\frac{1}{Z} \frac{1}{N !} \int \prod_{i=1}^{N}\left(\frac{d^{3} \vec{p}_{i} d^{3} \vec{q}_{i}}{h^{3}}\right) \exp \left[-\beta \sum_{i} \frac{\vec{p}_{i}^{2}}{2 m}\right] \exp \left[-\beta \mathcal{U}\left(\vec{q}_{1}, \cdots, \vec{q}_{N}\right)\right] \times \mathcal{O} \\
&=\frac{\langle\mathcal{O} \exp [-\beta \mathcal{U}]\rangle^{0}}{\langle\exp [-\beta \mathcal{U}]\rangle^{0}}=\left.i \frac{\partial}{\partial k} \ln \langle\exp [-i k \mathcal{O}-\beta \mathcal{U}]\rangle^{0}\right|_{k=0}
\end{aligned}
$$

The final expectation value generates the joint cumulants of the random variables $\mathcal{O}$ and $\mathcal{U}$, as

$$
\ln \langle\exp [-i k \mathcal{O}-\beta \mathcal{U}]\rangle^{0} \equiv \sum_{\ell, \ell^{\prime}=1}^{\infty} \frac{(-i k)^{\ell^{\prime}}}{\ell^{\prime} !} \frac{(-\beta)^{\ell}}{\ell !}\left\langle\mathcal{O}^{\ell^{\prime}} \mathcal{U}^{\ell}\right\rangle_{c}^{0}
$$

resulting in

$$
\langle\mathcal{O}\rangle=\sum_{\ell=0}^{\infty} \frac{(-\beta)^{\ell}}{\ell !}\left\langle\mathcal{O} \mathcal{U}^{\ell}\right\rangle_{c}^{0}
$$

The simplest system for treating interactions is again the dilute gas. As discussed in chapter II, for a weakly interacting gas we can specialize to

$$
\mathcal{U}\left(\vec{q}_{1}, \cdots, \vec{q}_{N}\right)=\sum_{i<j} \mathcal{V}\left(\vec{q}_{i}-\vec{q}_{j}\right)
$$

where $\mathcal{V}\left(\vec{q}_{i}-\vec{q}_{j}\right)$ is a pair-wise interaction between particles. The first correction in eq.(V.3) is

$$
\begin{aligned}
\langle\mathcal{U}\rangle_{c}^{0} &=\sum_{i<j} \int \frac{d^{3} \vec{q}_{i}}{V} \frac{d^{3} \vec{q}_{j}}{V} \mathcal{V}\left(\vec{q}_{i}-\vec{q}_{j}\right) \\
&=\frac{N(N-1)}{2 V} \int d^{3} \vec{q} \mathcal{V}(\vec{q})
\end{aligned}
$$

The final result is obtained by performing the integrals over the relative and center of mass coordinates of $\vec{q}_{i}$ and $\vec{q}_{j}$ separately. (Each of the $N(N-1) / 2$ pairs makes an identical contribution.)

The second order correction,

$$
\left\langle\mathcal{U}^{2}\right\rangle_{c}^{0}=\sum_{i<j, k<l}\left[\left\langle\mathcal{V}\left(\vec{q}_{i}-\vec{q}_{j}\right) \mathcal{V}\left(\vec{q}_{k}-\vec{q}_{l}\right)\right\rangle^{0}-\left\langle\mathcal{V}\left(\vec{q}_{i}-\vec{q}_{j}\right)\right\rangle^{0}\left\langle\mathcal{V}\left(\vec{q}_{k}-\vec{q}_{l}\right)\right\rangle^{0}\right]
$$

is the sum of $[N(N-1) / 2]^{2}$ terms that can be grouped as follows:

(i) There is no contribution from terms in which the four indices $\{i, j, k, l\}$ are different. This is because the different $\left\{\vec{q}_{i}\right\}$ are independently distributed and $\left\langle\mathcal{V}\left(\vec{q}_{i}-\vec{q}_{j}\right) \mathcal{V}\left(\vec{q}_{k}-\vec{q}_{l}\right)\right\rangle^{0}$ equals $\left\langle\mathcal{V}\left(\vec{q}_{i}-\vec{q}_{j}\right)\right\rangle^{0}\left\langle\mathcal{V}\left(\vec{q}_{k}-\vec{q}_{l}\right)\right\rangle^{0}$

(ii) There is one common index between the two pairs, e.g. $\{(i, j),(i, l)\} .$ By changing coordinates to $\vec{q}_{i j}=\vec{q}_{i}-\vec{q}_{j}$ and $\vec{q}_{i l}=\vec{q}_{i}-\vec{q}_{l}$, it again follows that $\left\langle\mathcal{V}\left(\vec{q}_{i}-\vec{q}_{j}\right) \mathcal{V}\left(\vec{q}_{i}-\vec{q}_{l}\right)\right\rangle^{0}$ equals $\left\langle\mathcal{V}\left(\vec{q}_{i}-\vec{q}_{j}\right)\right\rangle^{0}\left\langle\mathcal{V}\left(\vec{q}_{i}-\vec{q}_{l}\right)\right\rangle^{0} .$ The vanishing of these terms is a consequence of the translational symmetry of the problem in the absence of an external potential. (iii) In the remaining $N(N-1) / 2$ terms the pairs are identical, resulting in

$$
\left\langle\mathcal{U}^{2}\right\rangle_{c}^{0}=\frac{N(N-1)}{2}\left[\int \frac{d^{3} \vec{q}}{V} \mathcal{V}(\vec{q})^{2}-\left(\int \frac{d^{3} \vec{q}}{V} \mathcal{V}(\vec{q})\right)^{2}\right]
$$

The second term in the above equation is smaller by a factor of $d^{3} / V$, where $d$ is a characteristic range for the potential $\mathcal{V} .$ For any reasonable potential that decays with distance, this term vanishes in the thermodynamic limit.

Similar groupings occur for higher order terms in this cumulant expansion. It is helpful to visualize the terms in the expansion diagrammatically as follows:

(a) For a term of order $\ell$, draw $\ell$ pairs of points (representing $\vec{q}_{i}$ and $\left.\vec{q}_{j}\right)$ connected by bonds, representing the interaction $\mathcal{V}_{i j} \equiv \mathcal{V}\left(\vec{q}_{i}-\vec{q}_{j}\right) .$ An overall factor of $1 / \ell !$ accompanies such graphs.

(b) By multiple selections of the same index $i$, two or more bonds can be joined together forming a diagram of interconnected points. There is a factor $S_{\ell}$ associated with the number of ways of assigning labels 1 through $N$ to the different points of the graph. Ignoring the differences between $N, N-1$, etc., a diagram with $n_{s}$ points makes a contribution proportional to $N^{n_{s}}$. There is typically also division by a symmetry factor which takes into account the number of equivalent assignments. For example, the diagrams involving a pair of points, calculated in eqs.(V.9) and (V.11), have a symmetry factor of $1 / 2$.

(c) Apart from these numerical prefactors, the contribution of a diagram is an integral $R_{\ell}$ over all the $n_{s}$ coordinates $\vec{q}_{i}$, of products of corresponding $\mathcal{V}_{i j} .$ If the graphs has $n_{c}$ disconnected clusters, integration over the center of mass coordinates of the clusters gives a factor of $V^{n_{c}}$

Fortunately, many cancellations occur in calculating cumulants. In particular:

- When calculating the moment $\left\langle U^{\ell}\right\rangle^{0}$, the contribution of a disconnected diagram is simply the product of its disjoint clusters. The coordinates of these clusters are independent random variables, and make no contribution to the joint cumulant $\left\langle U^{\ell}\right\rangle_{c}^{0}$. This result also ensures the extensivity of $\ln Z$, as the surviving connected diagrams give a factor of $V$ from their center of mass integration. (Disconnected clusters have more factors of $V$, and are non-extensive.)

- There are also one particle reducible clusters which are fully connected, yet fall to disjoint fragments if a single coordinate point is removed. By measuring all other coordinates relative to this special point, it can be seen that (in a translationally invariant system) the value of such a diagram is the product of its disjoint fragments. It can be shown that such diagrams are also cancelled out in calculating the cumulant. Thus only one particle irreducible clusters survive in this cumulant expansion. A cluster with $n_{s}$ sites and $\ell$ bonds makes a contribution of order of $N(N / V)^{n_{s}-1}(\beta \mathcal{V})^{\ell}$ to $\ln Z$

Ignoring terms of order of $1 / N$, the cumulant expansion leads to a corrected free energy,

$$
\begin{aligned}
F(T, V, N)=F_{0}(T, V, N)+& \frac{N^{2}}{2 V}\left(\int d^{3} \vec{q} \mathcal{V}(\vec{q})-\frac{\beta}{2} \int d^{3} \vec{q} \mathcal{V}(\vec{q})^{2}+\mathcal{O}\left(\beta^{2} \mathcal{V}^{3}\right)\right) \\
&+\mathcal{O}\left(\frac{N^{3} \beta^{2} \mathcal{V}^{3}}{V^{2}}\right)
\end{aligned}
$$

From this expression we can proceed to calculate other modified state functions, e.g. $P=$ $-\partial F /\left.\partial V\right|_{T, N} .$ Unfortunately, the expansion in powers of $\beta \mathcal{V}$ is not particularly useful. The inter-atomic potential $\mathcal{V}(\vec{r})$ for most particles has an attractive tail due to van der Waals interactions that decays as $-1 / r^{6}$ at large separations $r=|\vec{r}| .$ At short distances the overlap of the electron clouds makes the potential strongly repulsive. Typically there is a minimum of depth a few hundred degrees Kelvin, at a distance of a few angstroms. The infinity in $\mathcal{V}(\vec{r})$ at short distances makes it an unsuitable expansion parameter. This problem can be alleviated by a partial resummation of diagrams. For example, to get the correction at order of $N^{2} / V$, we need to sum over all two point clusters, independent of the number of bonds. The resulting sum is actually quite trivial, and leads to

$$
\begin{aligned}
\ln Z &=\ln Z_{0}+\sum_{n=1}^{\infty} \frac{(-\beta)^{n}}{n !} \frac{N(N-1)}{2} \int \frac{d^{3} \vec{q}}{V} \mathcal{V}(\vec{q})^{n}+\mathcal{O}\left(\frac{N^{3}}{V^{2}}\right) \\
&=\ln Z_{0}+\frac{N(N-1)}{2 V} \int d^{3} \vec{q}[\exp (-\beta \mathcal{V}(\vec{q}))-1]+\mathcal{O}\left(\frac{N^{3}}{V^{2}}\right)
\end{aligned}
$$

The quantity $f(\vec{q})=\exp (-\beta \mathcal{V}(\vec{q}))-1$ is a much more convenient expansion parameter which goes to $-1$ at short distances and rapidly vanishes for large separations. In the next section we shall recast the perturbative expansion in terms of this quantity. MIT OpenCourseWare

http://ocw.mit.edu

\subsection{Statistical Mechanics I: Statistical Mechanics of Particles \\ Fall 2013}

For information about citing these materials or our Terms of Use, visit: http://ocw.mit.edu/terms.
