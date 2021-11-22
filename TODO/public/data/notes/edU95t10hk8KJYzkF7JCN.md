\section{VII.B Canonical Formulation}

Using the states constructed in the previous section, we can calculate the canonical density matrix for non-interacting identical particles. In the coordinate representation we have

$$
\left\langle\left\{\vec{x}^{\prime}\right\}|\rho|\{\vec{x}\}\right\rangle_{\eta}=\sum_{\{\vec{k}\}}^{\prime} \sum_{P, P^{\prime}} \eta^{P} \eta^{P^{\prime}}\left\langle\left\{\vec{x}^{\prime}\right\} \mid P^{\prime}\{\vec{k}\}\right\rangle \rho(\{\vec{k}\})\langle P\{\vec{k}\} \mid\{\vec{x}\}\rangle \frac{1}{N_{\eta}}
$$

where $\rho(\{\vec{k}\})=\exp \left[-\beta\left(\sum_{\alpha=1}^{N} \hbar^{2} k_{\alpha}^{2} / 2 m\right)\right] / Z_{N} .$ The sum, $\sum_{\left\{\vec{k}_{1}, \vec{k}_{2}, \cdots, \vec{k}_{N}\right\}}^{\prime}$, is restricted to ensure that each identical particle state appears once and only once. In both the bosonic and fermionic subspaces, the set of occupation numbers $\left\{n_{\vec{k}}\right\}$ uniquely identify a state. We can, however, remove this restriction from eq.(VII.11), if we divide by the resulting over-counting factor (for bosons) of $N ! /\left(\prod_{\vec{k}} n_{\vec{k}} !\right)$, i.e.,

$$
\sum_{\{\vec{k}\}}^{\prime}=\sum_{\{\vec{k}\}} \frac{\prod_{\vec{k}} n_{\vec{k}} !}{N !}
$$

(Note that for fermions, the $(-1)^{P}$ factors cancel out the contributions from cases where any $n_{\vec{k}}$ is larger than one.) Therefore,

$$
\begin{aligned}
\left\langle\left\{\vec{x}^{\prime}\right\}|\rho|\{\vec{x}\}\right\rangle=& \sum_{\{\vec{k}\}} \frac{\prod_{\vec{k}} n_{\vec{k}} !}{N !} \cdot \frac{1}{N ! \prod_{\vec{k}} n_{\vec{k}} !} \\
& \sum_{P, P^{\prime}} \frac{\eta^{P} \eta^{P^{\prime}}}{Z_{N}} \exp \left(-\beta \sum_{\alpha=1}^{N} \frac{\hbar^{2} k_{\alpha}^{2}}{2 m}\right)\left\langle\left\{\vec{x}^{\prime}\right\} \mid P^{\prime}\{\vec{k}\}\right\rangle\langle P\{\vec{k}\} \mid\{\vec{x}\}\rangle
\end{aligned}
$$

In the limit of large volume, the sums over $\{\vec{k}\}$ can be replaced by integrals, and using the plane wave representation of wavefunctions, we have

$$
\begin{aligned}
\left\langle\left\{\vec{x}^{\prime}\right\}|\rho|\{\vec{x}\}\right\rangle=& \frac{1}{Z_{N}(N !)^{2}} \sum_{P, P^{\prime}} \eta^{P} \eta^{P^{\prime}} \int \prod_{\alpha=1}^{N} \frac{V d^{3} \vec{k}_{\alpha}}{(2 \pi)^{3}} \exp \left(-\frac{\beta \hbar^{2} k_{\alpha}^{2}}{2 m}\right) \\
& \times\left\{\frac{\exp \left[-i \sum_{\alpha=1}^{N}\left(\vec{k}_{P \alpha} \cdot \vec{x}_{\alpha}-\vec{k}_{P^{\prime} \alpha} \cdot \vec{x}_{\alpha}^{\prime}\right)\right]}{V^{N}}\right\}
\end{aligned}
$$

We can order the sum in the exponent by focusing on a particular $\vec{k}$ -vector. Since $\sum_{\alpha} f(P \alpha) g(\alpha)=\sum_{\beta} f(\beta) g\left(P^{-1} \beta\right)$, where $\beta=P \alpha$ and $\alpha=P^{-1} \beta$, we obtain

$$
\left.\left\langle\left\{\vec{x}^{\prime}\right\}|\rho|\{\vec{x}\}\right\rangle=\frac{1}{Z_{N}(N !)^{2}} \sum_{P, P^{\prime}} \eta^{P} \eta^{P^{\prime}} \prod_{\alpha=1}^{N}\left[\int \frac{d^{3} \vec{k}_{\alpha}}{(2 \pi)^{3}} e^{-i \vec{k}_{\alpha} \cdot\left(\vec{x}_{P^{-1} \alpha}-\vec{x}_{P^{\prime}-1}^{\prime}\right.}\right)-\beta \hbar^{2} k_{\alpha}^{2} / 2 m\right]
$$

The gaussian integrals in the square brackets are equal to

$$
\frac{1}{\lambda^{3}} \exp \left[-\frac{\pi}{\lambda^{2}}\left(\vec{x}_{P-1} \alpha-\vec{x}_{P^{\prime}-1}^{\prime}\right)^{2}\right]
$$

Setting $\beta=P^{-1} \alpha$ in eq.(VII.14) gives

$$
\left\langle\left\{\vec{x}^{\prime}\right\}|\rho|\{\vec{x}\}\right\rangle=\frac{1}{Z_{N} \lambda^{3 N}(N !)^{2}} \sum_{P, P^{\prime}} \eta^{P} \eta^{P^{\prime}} \exp \left[-\frac{\pi}{\lambda^{2}} \sum_{\beta=1}^{N}\left(\vec{x}_{\beta}-\vec{x}_{P^{\prime}-1}^{\prime}\right)^{2}\right]
$$

Finally, we set $Q=P^{\prime-1} P$, and use the results $\eta^{P}=\eta^{P^{-1}}$, and $\eta^{Q}=\eta^{P^{\prime-1} P}=\eta^{P^{\prime}} \eta^{P}$, to get (after performing $\left.\sum_{P}=N !\right)$

$$
\left\langle\left\{\vec{x}^{\prime}\right\}|\rho|\{\vec{x}\}\right\rangle=\frac{1}{Z_{N} \lambda^{3 N} N !} \sum_{Q} \eta^{Q} \exp \left[-\frac{\pi}{\lambda^{2}} \sum_{\beta=1}^{N}\left(\vec{x}_{\beta}-\vec{x}_{Q \beta}^{\prime}\right)^{2}\right]
$$

The canonical partition function, $Z_{N}$, is obtained from the normalization condition

$$
\operatorname{tr}(\rho)=1, \quad \Longrightarrow \quad \int \prod_{\alpha=1}^{N} d^{3} \vec{x}_{\alpha}\langle\{\vec{x}\}|\rho|\{\vec{x}\}\rangle=1
$$

as

$$
Z_{N}=\frac{1}{N ! \lambda^{3 N}} \int \prod_{\alpha=1}^{N} d^{3} \vec{x}_{\alpha} \sum_{Q} \eta^{Q} \exp \left[-\frac{\pi}{\lambda^{2}} \sum_{\beta=1}^{N}\left(\vec{x}_{\beta}-\vec{x}_{Q \beta}\right)^{2}\right]
$$

The quantum partition function thus involves a sum over $N !$ possible permutations. The classical result $Z_{N}=\left(V / \lambda^{3}\right)^{N} / N !$, is obtained from the term corresponding to no particle exchange, $Q \equiv 1 .$ The division by $N !$ finally justifies the factor that was (somewhat artificially) introduces in classical statistical mechanics to deal with the phase space of identical particles. However, this classical result is only valid at very high temperature and is modified by the quantum corrections coming from the remaining permutations. As any permutation involves a product of factors $\exp \left[-\pi\left(\vec{x}_{1}-\vec{x}_{2}\right)^{2} / \lambda^{2}\right]$, its contributions vanishes as $\lambda \rightarrow 0$ for $T \rightarrow \infty$

The lowest order correction comes from the simplest permutation which is the exchange of two particles. The exchange of particles 1 and 2 is accompanied by a factor of $\eta \exp \left[-2 \pi\left(\vec{x}_{1}-\vec{x}_{2}\right)^{2} / \lambda^{2}\right] .$ As each of the possible $N(N-1) / 2$ pairwise exchanges gives the same contribution to $Z_{N}$, we get

$$
Z_{N}=\frac{1}{N ! \lambda^{3 N}} \int \prod_{\alpha=1}^{N} d^{3} \vec{x}_{\alpha}\left\{1+\frac{N(N-1)}{2} \eta \exp \left[-\frac{2 \pi}{\lambda^{2}}\left(\vec{x}_{1}-\vec{x}_{2}\right)^{2}\right]+\cdots\right\}
$$

For any $\alpha \geq 2, \int d^{3} \vec{x}_{\alpha}=V ;$ in the remaining two integrations we can use the relative, $\vec{r}_{12}=\vec{x}_{2}-\vec{x}_{1}$, and center of mass coordinates to get

$$
\begin{aligned}
Z_{N} &=\frac{1}{N ! \lambda^{3 N}} V^{N}\left[1+\frac{N(N-1)}{2 V} \eta \int d^{3} \vec{r}_{12} e^{-2 \pi \vec{r}_{12}^{2} / \lambda^{2}}+\cdots\right] \\
&=\frac{1}{N !}\left(\frac{V}{\lambda^{3}}\right)^{N}\left[1+\frac{N(N-1)}{2 V} \cdot\left(\sqrt{\frac{2 \pi \lambda^{2}}{4 \pi}}\right)^{3} \eta+\cdots\right]
\end{aligned}
$$

From the corresponding free energy,

$$
F=-k_{B} T \ln Z_{N}=-N k_{B} T \ln \left[\frac{e}{\lambda^{3}} \cdot \frac{V}{N}\right]-\frac{k_{B} T N^{2}}{2 V} \cdot \frac{\lambda^{3}}{2^{3 / 2}} \eta+\cdots
$$

the gas pressure is computed as

$$
P=-\left.\frac{\partial F}{\partial V}\right|_{T}=\frac{N k_{B} T}{V}-\frac{N^{2} k_{B} T}{V^{2}} \cdot \frac{\lambda^{3}}{2^{5 / 2}} \eta+\cdots=n k_{B} T\left[1-\frac{\eta \lambda^{3}}{2^{5 / 2}} n+\cdots\right]
$$

Note that the first quantum correction is equivalent to a second virial coefficient of

$$
B_{2}=-\frac{\eta \lambda^{3}}{2^{5 / 2}}
$$

The resulting correction to pressure is negative for bosons, and positive for fermions. In the classical formulation, a second virial coefficient was obtained from a two-body interaction. The classical potential $\mathcal{V}(\vec{r})$ that leads to the second virial coefficient in eq.(VII.22) is obtained from

$$
\begin{aligned}
&f(\vec{r})=e^{-\beta \mathcal{V}(\vec{r})}-1=\eta e^{-2 \pi \vec{r}^{2} / \lambda^{2}}, \quad \Longrightarrow \\
&\mathcal{V}(\vec{r})=-k_{B} T \ln \left[1+\eta e^{-2 \pi \vec{r}^{2} / \lambda^{2}}\right] \approx-k_{B} T \eta e^{-2 \pi \vec{r}^{2} / \lambda^{2}}
\end{aligned}
$$

(The final approximation corresponds to high temperatures, where only the first correction is important). Thus the effects of quantum statistics at high temperatures are approximately equivalent to introducing an interaction between particles. The interaction is attractive for bosons, repulsive for fermions, and operates over distances of the order of the thermal wavelength $\lambda$. 

\section{VII.C Grand Canonical Formulation}

Calculating the partition function by performing all the sums in eq.(VII.17) is a formidable task. Alternatively, we can compute $Z_{N}$ in the energy basis as

$$
Z_{N}=\operatorname{tr}\left(e^{-\beta \mathcal{H}}\right)=\sum_{\left\{\vec{k}_{\alpha}\right\}}^{\prime} \exp \left[-\beta \sum_{\alpha=1}^{N} \mathcal{E}\left(\vec{k}_{\alpha}\right)\right]=\sum_{\left\{n_{\vec{k}}\right\}}^{\prime} \exp \left[-\beta \sum_{\vec{k}} \mathcal{E}(\vec{k}) n(\vec{k})\right]
$$

These sums are still difficult to perform due to the restrictions of symmetry on the allowed values of $\vec{k}$ or $\left\{n_{\vec{k}}\right\}:$ The occupation numbers $\left\{n_{\vec{k}}\right\}$ are restricted to $\sum_{\vec{k}} n_{\vec{k}}=N$, and $n_{\vec{k}}=0,1,2, \cdots$ for bosons, while $n_{\vec{k}}=0$ or 1 for fermions. As usual, the first constraint can be removed by looking at the grand partition function,

$$
\begin{aligned}
\mathcal{Q}_{\eta}(T, \mu) &=\sum_{N=0}^{\infty} e^{\beta \mu N} \sum_{\left\{n_{\vec{k}}\right\}}^{\prime} \exp \left[-\beta \sum_{\vec{k}} \mathcal{E}(\vec{k}) n_{\vec{k}}\right] \\
&=\sum_{\left\{n_{\vec{k}}\right\}} \prod_{\vec{k}} \exp \left[-\beta(\mathcal{E}(\vec{k})-\mu) n_{\vec{k}}\right]
\end{aligned}
$$

The sums over $\left\{n_{\vec{k}}\right\}$ can now be performed independently for each $\vec{k}$, subject to the restrictions on occupation numbers imposed by particle symmetry.

- For fermions, $n_{\vec{k}}=0$ or 1, and

$$
\mathcal{Q}_{-}=\prod_{\vec{k}}[1+\exp (\beta \mu-\beta \mathcal{E}(\vec{k}))]
$$

- For bosons $n_{\vec{k}}=0,1,2, \cdots$, and summing the geometric series gives

$$
\mathcal{Q}_{+}=\prod_{\vec{k}}[1-\exp (\beta \mu-\beta \mathcal{E}(\vec{k}))]^{-1}
$$

The results for both cases can be presented simultaneously as

$$
\ln \mathcal{Q}_{\eta}=-\eta \sum_{\vec{k}} \ln [1-\eta \exp (\beta \mu-\beta \mathcal{E}(\vec{k}))]
$$

with $\eta=-1$ for fermions, and $\eta=+1$ for bosons.

In the grand canonical formulation, different one-particle states are occupied independently, with a joint probability

$$
p_{\eta}(\{n(\vec{k})\})=\frac{1}{\mathcal{Q}_{\eta}} \prod_{\vec{k}} \exp \left[-\beta(\mathcal{E}(\vec{k})-\mu) n_{\vec{k}}\right]
$$

The average occupation number of a state of energy $\mathcal{E}(\vec{k})$ is given by

$$
\left\langle n_{\vec{k}}\right\rangle_{\eta}=-\frac{\partial \ln \mathcal{Q}_{\eta}}{\partial(\beta \mathcal{E}(\vec{k}))}=\frac{1}{z^{-1} e^{\beta \mathcal{E}(\vec{k})}-\eta}
$$

where $z=\exp (\beta \mu)$. The average values of the particle number and internal energy are then given by

$$
\left\{\begin{array}{l}
N_{\eta}=\sum_{\vec{k}}\left\langle n_{\vec{k}}\right\rangle_{\eta}=\sum_{\vec{k}} \frac{1}{z^{-1} e^{\beta \mathcal{E}(\vec{k})}-\eta} \\
E_{\eta}=\sum_{\vec{k}} \mathcal{E}(\vec{k})\left\langle n_{\vec{k}}\right\rangle_{\eta}=\sum_{\vec{k}} \frac{\mathcal{E}(\vec{k})}{z^{-1} e^{\beta \mathcal{E}(\vec{k})}-\eta}
\end{array}\right.
$$

\section{VII.D Non-relativistic Gas}

Quantum particles are further characterized by a spin s. In the absence of a magnetic field different spin states have the same energy, and a spin degeneracy factor, $g=2 s+1$, multiplies eqs.(VII.28)-(VII.31). In particular, for a non-relativistic gas in three dimensions $\left(\mathcal{E}(\vec{k})=\hbar^{2} k^{2} / 2 m\right.$, and $\left.\sum_{\vec{k}} \rightarrow V \int d^{3} \vec{k} /(2 \pi)^{3}\right)$ these equations reduce to

$$
\left\{\begin{array}{l}
\beta P_{\eta}=\frac{\ln \mathcal{Q}_{\eta}}{V}=\eta g \int \frac{d^{3} \vec{k}}{(2 \pi)^{3}} \ln \left[1-\eta z \exp \left(-\frac{\beta \hbar^{2} k^{2}}{2 m}\right)\right] \\
n_{\eta} \equiv \frac{N_{\eta}}{V}=g \int \frac{d^{3} \vec{k}}{(2 \pi)^{3}} \frac{1}{z^{-1} \exp \left(\frac{\beta \hbar^{2} k^{2}}{2 m}\right)-\eta} \\
\varepsilon_{\eta} \equiv \frac{E_{\eta}}{V}=g \int \frac{d^{3} \vec{k}}{(2 \pi)^{3}} \frac{\hbar^{2} k^{2}}{2 m} \frac{1}{z^{-1} \exp \left(\frac{\beta \hbar^{2} k^{2}}{2 m}\right)-\eta}
\end{array}\right.
$$

To simplify these equations, we change variables to $x=\beta \hbar^{2} k^{2} /(2 m)$, so that

$$
k=\frac{\sqrt{2 m k_{B} T}}{\hbar} x^{1 / 2}=\frac{2 \pi^{1 / 2}}{\lambda} x^{1 / 2}, \quad \Longrightarrow \quad d k=\frac{\pi^{1 / 2}}{\lambda} x^{-1 / 2} d x
$$

Substituting into eqs.(VII.32) gives

$$
\left\{\begin{aligned}
\beta P_{\eta}=&-\eta \frac{g}{2 \pi^{2}} \frac{4 \pi^{3 / 2}}{\lambda^{3}} \int_{0}^{\infty} d x x^{1 / 2} \ln \left(1-\eta z e^{-x}\right) \\
&=\frac{g}{\lambda^{3}} \frac{4}{3 \sqrt{\pi}} \int_{0}^{\infty} \frac{d x x^{3 / 2}}{z^{-1} e^{x}-\eta}, \quad \text { (integration by parts) } \\
n_{\eta}=& \frac{g}{\lambda^{3}} \frac{2}{\sqrt{\pi}} \int_{0}^{\infty} \frac{d x x^{1 / 2}}{z^{-1} e^{x}-\eta} \\
\beta \varepsilon_{\eta}=& \frac{g}{\lambda^{3}} \frac{2}{\sqrt{\pi}} \int_{0}^{\infty} \frac{d x x^{3 / 2}}{z^{-1} e^{x}-\eta}
\end{aligned}\right.
$$

We now define two sets of functions by

$$
f_{m}^{\eta}(z)=\frac{1}{(m-1) !} \int_{0}^{\infty} \frac{d x x^{m-1}}{z^{-1} e^{x}-\eta}
$$

For non-integer arguments, the function $m ! \equiv \Gamma(m+1)$ is defined by the integral $\int_{0}^{\infty} d x x^{m} e^{-x} . \quad$ In particular, from this definition it follows that $(1 / 2) !=\sqrt{\pi} / 2$, and $(3 / 2) !=(3 / 2) \sqrt{\pi} / 2 .$ Eqs.(VII.33) now take the simple form

$$
\left\{\begin{aligned}
\beta P_{\eta} &=\frac{g}{\lambda^{3}} f_{5 / 2}^{\eta}(z) \\
n_{\eta} &=\frac{g}{\lambda^{3}} f_{3 / 2}^{\eta}(z) \\
\varepsilon_{\eta} &=\frac{3}{2} P_{\eta}
\end{aligned}\right.
$$

These results completely describe the thermodynamics of ideal quantum gases as a function of $z$. To find the equation of state $P_{\eta}\left(n_{\eta}, T\right)$, we need to solve for $z$ in terms of density. This requires knowledge of the behavior of the functions $f_{m}^{\eta}(z)$.

The high temperature, low density (non-degenerate) limit will be examined first. In this limit, $z$ is small, and

$$
\begin{aligned}
f_{m}^{\eta}(z) &=\frac{1}{(m-1) !} \int_{0}^{\infty} \frac{d x x^{m-1}}{z^{-1} e^{x}-\eta}=\frac{1}{(m-1) !} \int_{0}^{\infty} d x x^{m-1}\left(z e^{-x}\right)\left(1-\eta z e^{-x}\right)^{-1} \\
&=\frac{1}{(m-1) !} \int_{0}^{\infty} d x x^{m-1} \sum_{\alpha=1}^{\infty}\left(z e^{-x}\right)^{\alpha} \eta^{\alpha+1} \\
&=\sum_{\alpha=1}^{\infty} \eta^{\alpha+1} z^{\alpha} \frac{1}{(m-1) !} \int_{0}^{\infty} d x x^{m-1} e^{-\alpha x} \\
&=\sum_{\alpha=1}^{\infty} \eta^{\alpha+1} \frac{z^{\alpha}}{\alpha^{m}}=z+\eta \frac{z^{2}}{2^{m}}+\frac{z^{3}}{3^{m}}+\eta \frac{z^{4}}{4^{m}}+\cdots
\end{aligned}
$$

We thus find (self-consistently) that $f_{m}^{\eta}(z)$, and hence $n_{\eta}(z)$ and $P_{\eta}(z)$, are indeed small as $z \rightarrow 0$. Eqs.(VII.35) in this limit give,

$$
\left\{\begin{array}{c}
\frac{n_{\eta} \lambda^{3}}{g}=f_{3 / 2}^{\eta}(z)=z+\eta \frac{z^{2}}{2^{3 / 2}}+\frac{z^{3}}{3^{3 / 2}}+\eta \frac{z^{4}}{4^{3 / 2}}+\cdots \\
\frac{\beta P_{\eta} \lambda^{3}}{g}=f_{5 / 2}^{\eta}(z)=z+\eta \frac{z^{2}}{2^{5 / 2}}+\frac{z^{3}}{3^{5 / 2}}+\eta \frac{z^{4}}{4^{5 / 2}}+\cdots
\end{array}\right.
$$

The first of the above equations can be solved perturbatively, by the recursive procedure of substituting the solution up to a lower order, as

$$
\begin{aligned}
z &=\frac{n_{\eta} \lambda^{3}}{g}-\eta \frac{z^{2}}{2^{3 / 2}}-\frac{z^{3}}{3^{3 / 2}}-\cdots \\
&=\left(\frac{n_{\eta} \lambda^{3}}{g}\right)-\frac{\eta}{2^{3 / 2}}\left(\frac{n_{\eta} \lambda^{3}}{g}\right)^{2}-\cdots \\
&=\left(\frac{n_{\eta} \lambda^{3}}{g}\right)-\frac{\eta}{2^{3 / 2}}\left(\frac{n_{\eta} \lambda^{3}}{g}\right)^{2}+\left(\frac{1}{4}-\frac{1}{3^{3 / 2}}\right)\left(\frac{n_{\eta} \lambda^{3}}{g}\right)^{3}-\cdots
\end{aligned}
$$

Substituting this solution into the second leads to

$$
\begin{aligned}
\frac{\beta P_{\eta} \lambda^{3}}{g} &=\left(\frac{n_{\eta} \lambda^{3}}{g}\right)-\frac{\eta}{2^{3 / 2}}\left(\frac{n_{\eta} \lambda^{3}}{g}\right)^{2}+\left(\frac{1}{4}-\frac{1}{3^{3 / 2}}\right)\left(\frac{n_{\eta} \lambda^{3}}{g}\right)^{3} \\
&+\frac{\eta}{2^{5 / 2}}\left(\frac{n_{\eta} \lambda^{3}}{g}\right)^{2}-\frac{1}{8}\left(\frac{n_{\eta} \lambda^{3}}{g}\right)^{3}+\frac{1}{3^{5 / 2}}\left(\frac{n_{\eta} \lambda^{3}}{g}\right)^{3}+\cdots
\end{aligned}
$$

The pressure of the quantum gas can thus be obtained from the virial expansion,

$$
P_{\eta}=n_{\eta} k_{B} T\left[1-\frac{\eta}{2^{5 / 2}}\left(\frac{n_{\eta} \lambda^{3}}{g}\right)+\left(\frac{1}{8}-\frac{2}{3^{5 / 2}}\right)\left(\frac{n_{\eta} \lambda^{3}}{g}\right)^{2}+\cdots\right]
$$

The second virial coefficient $B_{2}=-\eta \lambda^{3} /\left(2^{5 / 2} g\right)$, agrees with eq.(VII.22) computed in the canonical ensemble for $g=1 .$ The natural (dimensionless) expansion parameter is $n_{\eta} \lambda^{3} / g$, and quantum mechanical effects become important when $n_{\eta} \lambda^{3} \geq g ;$ the quantum degenerate limit. The behavior of fermi and bose gases is very different in this degenerate limit of low temperatures and high densities, and the two cases will be discussed separately in the following sections. MIT OpenCourseWare

http://ocw.mit.edu

\subsection{Statistical Mechanics I: Statistical Mechanics of Particles \\ Fall 2013}

For information about citing these materials or our Terms of Use, visit: http://ocw.mit.edu/terms.
