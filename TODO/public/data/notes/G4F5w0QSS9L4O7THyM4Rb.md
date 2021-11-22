\section{Quantum Statistical Mechanics}

There are limitations to the applicability of classical statistical mechanics. The need to include quantum mechanical effects becomes specially apparent at low temperatures. In this section we shall first demonstrate the failure of the classical results in the contexts of heat capacities of molecular gases and solids, and the ultra-violet catastrophe in black body radiation. We shall then reformulate statistical mechanics using quantum concepts.

\section{VI.A Dilute Polyatomic Gases}

Consider a dilute gas of polyatomic molecules. The Hamiltonian for each molecule of $n$ atoms is

$$
\mathcal{H}_{1}=\sum_{i=1}^{n} \frac{\vec{p}_{i}^{2}}{2 m}+\mathcal{V}\left(\vec{q}_{1}, \ldots, \vec{q}_{n}\right)
$$

where the potential energy $\mathcal{V}$, contains all the information on molecular bonds. For simplicity, we have assumed that all atoms in the molecule have the same mass. If the masses are different, the Hamiltonian can be brought into the above form by rescaling the coordinates $\vec{q}_{i}$ by $\sqrt{m_{i} / m}$ (and the momenta by $\left.\sqrt{m / m_{i}}\right)$, where $m_{i}$ is the mass of the $i^{\text {th }}$ atom. Ignoring the interactions between molecules, the partition function of a dilute gas is

$$
Z(N)=\frac{Z_{1}^{N}}{N !}=\frac{1}{N !}\left\{\int \prod_{i=1}^{n} \frac{d^{3} \vec{p}_{i} d^{3} \vec{q}_{i}}{h^{3}} \exp \left[-\beta \sum_{i=1}^{n} \frac{\vec{p}_{i}^{2}}{2 m}-\beta \mathcal{V}\left(\vec{q}_{1}, \ldots, \vec{q}_{n}\right)\right]\right\}^{N}
$$

The chemical bonds that keep the molecule together are usually quite strong (energies of the order of electron volts). At typical accessible temperatures, which are much smaller than the corresponding dissociation temperatures $\left(\approx 10^{4 \circ} \mathrm{K}\right)$, the molecule has a well defined shape and only undergoes small deformations. The contribution of these deformations to the one particle partition function $Z_{1}$, can be computed as follows:

(a) The first step is to find the equilibrium positions, $\left(\vec{q}_{1}^{*}, \ldots, \vec{q}_{n}^{*}\right)$, by minimizing the potential $\mathcal{V}$.

(b) The energy cost of small deformations about equilibrium is then obtained by setting $\vec{q}_{i}=\vec{q}_{i}^{*}+\vec{u}_{i}$, and making an expansion in powers of $\vec{u}$

$$
\mathcal{V}=\mathcal{V}^{*}+\frac{1}{2} \sum_{i, j=1}^{n} \sum_{\alpha, \beta=1}^{3} \frac{\partial^{2} \mathcal{V}}{\partial q_{i, \alpha} \partial q_{j, \beta}} u_{i, \alpha} u_{j, \beta}+\mathcal{O}\left(u^{3}\right)
$$

(Here $i, j=1, \cdots, n$, identify the atoms, and $\alpha, \beta=1,2,3$ label a particular component.) Since the expansion is around a stable equilibrium configuration, the first derivatives are absent in eq.(VI.3), and the matrix of second derivatives is positive definite, i.e. it has only non-negative eigenvalues.

(c) The normal modes of the molecule are obtained by diagonalizing the $3 n \times 3 n$ matrix $\partial^{2} \mathcal{V} / \partial q_{i, \alpha} \partial q_{j, \beta} .$ The resulting $3 n$ eigenvalues $K_{s}$, indicate the stiffness of each mode. We can change variables from the original deformations $\left\{\vec{u}_{i}\right\}$, to the amplitudes $\left\{\tilde{u}_{s}\right\}$, of the eigenmodes. The corresponding conjugate momenta are $\tilde{p}_{s}=m \dot{\tilde{u}}_{s} .$ Since the transformation from $\left\{\vec{u}_{i}\right\}$ to $\left\{\tilde{u}_{s}\right\}$ is unitary (preserving the length of a vector), $\sum_{i} \vec{p}_{i}{ }^{2}=\sum_{s} \tilde{p}_{s}^{2}$, and the quadratic part of the resulting deformation Hamiltonian is

$$
\mathcal{H}_{1}=\mathcal{V}^{*}+\sum_{s=1}^{3 n}\left[\frac{1}{2 m} \tilde{p}_{s}^{2}+\frac{K_{s}}{2} \tilde{u}_{s}^{2}\right]
$$

(Such transformations are also canonical, preserving the measure of integration in phase space, $\left.\prod_{i, \alpha} d u_{i, \alpha} d p_{i, \alpha}=\prod_{s} d \tilde{u}_{s} d \tilde{p}_{s} .\right)$

The average energy of each molecule is the expectation value of the above Hamiltonian. Since each quadratic degree of freedom classically contributes a factor of $k_{B} T / 2$ to the energy,

$$
\left\langle\mathcal{H}_{1}\right\rangle=\mathcal{V}^{*}+\frac{3 n+m}{2} k_{B} T
$$

Only modes with a finite stiffness can store potential energy, and $m$ is defined as the number such modes with non-zero $K_{s} .$ The following symmetries of the potential force some eigenvalues to zero:

(a) Translation symmetry: Since $\mathcal{V}\left(\overrightarrow{q_{1}}+\vec{c}, \cdots, \vec{q}_{n}+\vec{c}\right)=\mathcal{V}\left(\vec{q}_{1}, \cdots, \vec{q}_{n}\right)$, no energy is stored the center of mass coordinate $\vec{Q}=\sum_{\alpha} \vec{q}_{\alpha} / n$, i.e. $\mathcal{V}(\vec{Q})=\mathcal{V}(\vec{Q}+\vec{c})$, and the corresponding three values of $K_{\text {trans }}$ are zero.

(b) Rotation symmetry: There is also no potential energy associated with rotations of the molecule, and $K_{\mathrm{rot}}=0$ for the corresponding stiffnesses. The number of rotational modes, $0 \leq r \leq 3$, depends on the shape of the molecule; for example, a rod shaped molecule has $r=2$, as a rotation parallel to its axis does not result in a new configuration.

The remaining $m=3 n-3-r$ eigenvectors of the matrix have non-zero stiffness, and correspond to the vibrational normal modes. The energy per molecule, from eq.(VI.5), is thus

$$
\left\langle\mathcal{H}_{1}\right\rangle=\frac{6 n-3-r}{2} k_{B} T
$$

The corresponding heat capacities,

$$
C_{V}=\frac{(6 n-3-r)}{2} k_{B}, \quad \text { and } \quad C_{P}=C_{V}+k_{B}=\frac{(6 n-1-r)}{2} k_{B}
$$

are temperature independent. The ratio $\gamma=C_{P} / C_{V}$ is easily measured in adiabatic processes. Values of $\gamma$, expected on the basis of the above argument, are listed below for a number of different molecules.

Monatomic

$\theta(n)$

Diatomic

Tetra-atomic

$0.5$

$\mathrm{NH}_{3}$

$$
n=4
$$

$$
r=3 \quad \gamma=20 / 18=10 / 9
$$

Measurements of the heat capacity of dilute gases do not agree with the above predictions. For example, the value $C_{V} / k_{B}=7 / 2$, for a diatomic gas such as oxygen, is only observed at temperatures higher than a few thousand degrees Kelvin. At room temperatures, a lower value of $5 / 2$ is observed, while at even lower temperatures of around $10^{0} K$, it is further reduced to $3 / 2 .$ The low temperature value is similar to that of a monatomic gas, and suggests that no energy is stored in the rotational and vibrational degrees of freedom. These observations can be explained if the allowed energy levels are quantized.

- Vibrational modes: A diatomic molecule has one vibrational mode with stiffness $K \equiv m \omega^{2}$, where $\omega$ is the frequency of oscillations. The classical partition function for this mode is

$$
\begin{aligned}
Z_{\mathrm{vib}}^{c} &=\int \frac{d p d q}{h} \exp \left[-\beta\left(\frac{p^{2}}{2 m}+\frac{m \omega^{2} q^{2}}{2}\right)\right] \\
&=\frac{1}{h} \sqrt{\left(\frac{2 \pi m}{\beta}\right)\left(\frac{2 \pi}{\beta m \omega^{2}}\right)}=\frac{2 \pi}{h \beta \omega}=\frac{k_{B} T}{\hbar \omega}
\end{aligned}
$$

where $\hbar=h / 2 \pi$. The corresponding energy stored in this mode,

$$
\left\langle\mathcal{H}_{\mathrm{vib}}\right\rangle^{c}=-\frac{\partial \ln Z}{\partial \beta}=\frac{\partial \ln (\beta \hbar \omega)}{\partial \beta}=\frac{1}{\beta}=k_{B} T
$$

comes from $k_{B} T / 2$ per kinetic and potential degrees of freedom. In quantum mechanics, the allowed values of energy are quantized such that

$$
\mathcal{H}_{\mathrm{vib}}^{q}=\hbar \omega\left(n+\frac{1}{2}\right)
$$

with $n=0,1,2, \cdots$. Assuming that the probability of each discrete level is proportional to its Boltzmann weight (as will be justified later on), there is a normalization factor

$$
Z_{\mathrm{vib}}^{q}=\sum_{n=0}^{\infty} e^{-\beta \hbar \omega(n+1 / 2)}=\frac{e^{-\beta \hbar \omega / 2}}{1-e^{-\beta \hbar \omega}}
$$

The high temperature limit,

$$
\lim _{\beta \rightarrow 0} Z_{\mathrm{vib}}^{q}=\frac{1}{\beta \hbar \omega}=\frac{k_{B} T}{\hbar \omega}
$$

coincides with eq.(VI.8)(due in part to the choice of $h$ as the measure of classical phase space).

The expectation value of vibrational energy is

$$
E_{\mathrm{vib}}^{q}=-\frac{\partial \ln Z}{\partial \beta}=\frac{\hbar \omega}{2}+\frac{\partial}{\partial \beta} \ln \left(1-e^{-\beta \hbar \omega}\right)=\frac{\hbar \omega}{2}+\hbar \omega \frac{e^{-\beta \hbar \omega}}{1-e^{-\beta \hbar \omega}}
$$

The first term is the energy cost of quantum fluctuations that are present even in the zero temperature ground state. The second term describes the additional energy due to thermal fluctuations. The resulting heat capacity,

$$
C_{\mathrm{vib}}^{q}=\frac{d E_{\mathrm{vib}}^{q}}{d T}=k_{B}\left(\frac{\hbar \omega}{k_{B} T}\right)^{2} \frac{e^{-\beta \hbar \omega}}{\left(1-e^{-\beta \hbar \omega}\right)^{2}}
$$

achieves the classical value of $k_{B}$ only at temperatures $T \gg \theta_{\mathrm{vib}}$, where $\theta_{\mathrm{vib}}=\hbar \omega / k_{B}$ is a characteristic temperature associated with the quanta of vibrational energy. For $T \ll \theta_{\text {vib }}$, $C_{\text {vib }}^{q}$ goes to zero as $\exp \left(-\theta_{\text {vib }} / T\right)$. Typical values of $\theta_{\text {vib }}$ are in the range of $10^{3}$ to $10^{4}$ degrees Kelvin, explaining why the classical value of heat capacity is observed only at higher temperatures.

- Rotational modes: To account for the low temperature anomaly in the heat capacity of diatomic molecules, we have to study the quantization of the rotational degrees of freedom. Classically, the orientation of a diatomic molecule is specified by two angles $\theta$ and $\phi$, and its Lagrangian (equal to the kinetic energy) is

$$
\mathcal{L}=\frac{I}{2}\left(\dot{\theta}^{2}+\sin ^{2} \theta \dot{\phi}^{2}\right)
$$

where $I$ is the moment of inertia. In terms of the conjugate momenta,

$$
p_{\theta}=\frac{\partial \mathcal{L}}{d \dot{\theta}}=I \dot{\theta}, \quad p_{\phi}=\frac{\partial \mathcal{L}}{d \dot{\phi}}=I \sin ^{2} \theta \dot{\phi}
$$

the Hamiltonian for rotations is

$$
\mathcal{H}_{\mathrm{rot}}=\frac{1}{2 I}\left(p_{\theta}^{2}+\frac{p_{\phi}^{2}}{\sin ^{2} \theta}\right) \equiv \frac{\vec{L}^{2}}{2 I}
$$

where $\vec{L}$ is the angular momentum. From the classical partition function,

$$
\begin{aligned}
Z_{\text {rot }}^{c} &=\frac{1}{h^{2}} \int_{0}^{\pi} d \theta \int_{0}^{2 \pi} d \phi \int_{-\infty}^{\infty} d p_{\theta} d p_{\phi} \exp \left[-\frac{\beta}{2 I}\left(p_{\theta}^{2}+\frac{p_{\phi}^{2}}{\sin ^{2} \theta}\right)\right] \\
&=\left(\frac{2 \pi I}{\beta}\right)\left(\frac{4 \pi}{h^{2}}\right)=\frac{2 I k_{B} T}{\hbar^{2}}
\end{aligned}
$$

the stored energy is

$$
\left\langle E_{\mathrm{rot}}\right\rangle^{c}=-\frac{\partial \ln Z}{\partial \beta}=\frac{\partial}{\partial \beta} \ln \left(\frac{\beta \hbar^{2}}{2 I}\right)=k_{B} T
$$

as expected for two degrees of freedom. In quantum mechanics, the allowed values of angular momentum are quantized to $\vec{L}^{2}=\hbar^{2} \ell(\ell+1)$ with $\ell=0,1,2, \cdots$, and each state has a degeneracy of $2 \ell+1$ (along a selected direction, $\left.L_{z}=-\ell, \cdots,+\ell\right) .$ A partition function is now obtained for these levels as

$$
Z_{\text {rot }}^{q}=\sum_{\ell=0}^{\infty} \exp \left[-\frac{\beta \hbar^{2} \ell(\ell+1)}{2 I}\right](2 \ell+1)=\sum_{\ell=0}^{\infty} \exp \left[-\frac{\theta_{\text {rot }} \ell(\ell+1)}{T}\right](2 \ell+1)
$$

where $\theta_{\text {rot }}=\hbar^{2} /\left(2 I k_{B}\right)$ is a characteristic temperature associated with quanta of rotational energy. While the sum can not be analytically evaluated in general, we can study its high and low temperature limits:

(a) For $T \gg \theta_{\text {rot }}$, the terms in eq.(VI.19) vary slowly, and the sum can be replaced by the integral

$$
\begin{aligned}
\lim _{T \rightarrow \infty} Z_{\text {rot }}^{q} &=\int_{0}^{\infty} d x(2 x+1) \exp \left[-\frac{\theta_{\text {rot }} x(x+1)}{T}\right] \\
&=\int_{0}^{\infty} d y e^{-\theta_{\text {rot } y / T}}=\frac{T}{\theta_{\text {rot }}}=Z_{\text {rot }}^{c}
\end{aligned}
$$

i.e. the classical result of eq.(VI.17) is recovered.

(b) For $T \ll \theta_{\text {rot }}$, the first few terms dominate the sum, and

$$
\lim _{T \rightarrow \infty} Z_{\mathrm{rot}}^{q}=1+3 e^{-2 \theta_{\mathrm{rot}} / T}+\mathcal{O}\left(e^{-6 \theta_{\mathrm{rot}} / T}\right)
$$

leading to an energy

$$
E_{\mathrm{rot}}^{q}=-\frac{\partial \ln Z}{\partial \beta} \approx-\frac{\partial}{\partial \beta} \ln \left[1+3 e^{-2 \theta_{\mathrm{rot}} / T}\right] \approx 6 k_{B} \theta_{\mathrm{rot}} e^{-2 \theta_{\mathrm{rot}} / T}
$$

The resulting heat capacity vanishes at low temperatures as

$$
C_{\mathrm{rot}}=\frac{d E_{\mathrm{rot}}^{q}}{d T}=3 k_{B}\left(\frac{2 \theta_{\mathrm{rot}}}{T}\right)^{2} e^{-2 \theta_{\mathrm{rot}} / T}+\cdots
$$

Typical values of $\theta_{\text {rot }}$ are between 1 and $10^{\circ} K$, explaining the lower temperature shoulder in the heat capacity measurements. At very low temperatures, the only contributions come from the kinetic energy of the center of mass, and the molecule behaves as a monatomic particle. (The heat capacity vanishes at even lower temperatures due to quantum statistics, as will be discussed in the context of identical particles.)

\section{VI.B Vibrations of a Solid}

Attractive interactions between particles first lead to condensation from a gas to liquid at low temperatures, and finally cause freezing into a solid state at even lower temperatures. For the purpose of discussing its thermodynamics, the solid can be regarded as a very large molecule subject to a Hamiltonian similar to eq.(VI.1), with $n=N \gg 1$ atoms. We can then proceed with the steps outlined in the previous section.

(a) The classical ground state configuration of the solid is obtained by minimizing the potential $\mathcal{V}$. In almost all cases, the minimum energy corresponds to a periodic arrangement of atoms forming a lattice. In terms of the three basis vectors, $\hat{a}, \hat{b}$, and $\hat{c}$, the locations of atoms in a simple crystal are given by

$$
\vec{q}^{*}(\ell, m, n)=[\ell \hat{a}+m \hat{b}+n \hat{c}] \equiv \vec{r}
$$

where $\{\ell, m, n\}$ is a triplet of integers.

(b) At finite temperatures, the atoms may undergo small deformations

$$
\vec{q}_{\vec{r}}=\vec{r}+\vec{u}(\vec{r})
$$

with a cost in potential energy of

$$
\mathcal{V}=\mathcal{V}^{*}+\frac{1}{2} \sum_{\vec{r}, \vec{r}^{\prime} \atop \alpha, \beta} \frac{\partial^{2} \mathcal{V}}{\partial q_{\vec{r}, \alpha} \partial q_{\vec{r}^{\prime}, \beta}} u_{\alpha}(\vec{r}) u_{\beta}\left(\vec{r}^{\prime}\right)+O\left(u^{3}\right)
$$

(c) Finding the normal modes of a crystal is considerably simplified by its translational symmetry. In particular, the matrix of second derivatives only depends on the relative separation of two points,

$$
\frac{\partial^{2} \mathcal{V}}{\partial q_{\vec{r}, \alpha} \partial q_{\vec{r}^{\prime}, \beta}}=K_{\alpha \beta}\left(\vec{r}-\vec{r}^{\prime}\right)
$$

It is always possible to take advantage of such a symmetry to at least partially diagonalize the matrix by using a Fourier basis,

$$
u_{\alpha}(\vec{r})=\sum_{\vec{k}}^{\prime} \frac{e^{i \vec{k} \cdot \vec{r}}}{\sqrt{N}} \tilde{u}_{\alpha}(\vec{k})
$$

The sum is restricted to wavevectors $\vec{k}$ inside a Brillouin zone. For example, in a cubic lattice of spacing $a$, each component of $\vec{k}$ is restricted to the interval $[-\pi / a, \pi / a]$ This is because wavevectors outside this interval carry no additional information as $\left(k_{x}+2 \pi m / a\right)(n a)=k_{x}(n a)+2 m n \pi$, and any phase that is a multiple of $2 \pi$ does not effect the sum in eq.(VI.28). In terms of the Fourier modes, the potential energy of deformations is

$$
\mathcal{V}=\mathcal{V}^{*}+\frac{1}{2 N} \sum_{\left(\vec{r}, \vec{r}^{\prime}\right),\left(\vec{k}, \vec{k}^{\prime}\right)}_{\alpha, \beta} K_{\alpha \beta}\left(\vec{r}-\vec{r}^{\prime}\right) e^{i \vec{k} \cdot \vec{r}} \tilde{u}_{\alpha}(\vec{k}) e^{i \vec{k}^{\prime} \cdot \vec{r}^{\prime}} \tilde{u}_{\beta}\left(\vec{k}^{\prime}\right)
$$

We can change variables to relative and center of mass coordinates,

$$
\vec{\rho}=\vec{r}-\vec{r}^{\prime}, \quad \text { and } \quad \vec{R}=\frac{\vec{r}+\vec{r}^{\prime}}{2}
$$

by setting

$$
\vec{r}=\vec{R}+\frac{\vec{\rho}}{2}, \quad \text { and } \quad \vec{r}^{\prime}=\vec{R}-\frac{\vec{\rho}}{2}
$$

Eq.(VI.29) now simplifies to

$$
\mathcal{V}=\mathcal{V}^{*}+\frac{1}{2 N} \sum_{\vec{k}, \vec{k}^{\prime} \atop \alpha, \beta}\left(\sum_{\vec{R}} e^{i\left(\vec{k}+\vec{k}^{\prime}\right) \cdot \vec{R}}\right)\left(\sum_{\vec{\rho}} K_{\alpha \beta}(\vec{\rho}) e^{i\left(\vec{k}-\vec{k}^{\prime}\right) \cdot \vec{\rho} / 2} \tilde{u}_{\alpha}(\vec{k}) \tilde{u}_{\beta}\left(\vec{k}^{\prime}\right)\right)
$$

As the sum in the first brackets is $N \delta_{\vec{k}+\vec{k}^{\prime}, 0}$,

$$
\begin{aligned}
\mathcal{V} &=\mathcal{V}^{*}+\frac{1}{2} \sum_{\vec{k}, \alpha, \beta}\left[\sum_{\vec{\rho}} K_{\alpha \beta}(\vec{\rho}) e^{i \vec{k} \cdot \vec{\rho}}\right] \tilde{u}_{\alpha}(\vec{k}) \tilde{u}_{\beta}(-\vec{k}) \\
&=\mathcal{V}^{*}+\frac{1}{2} \sum_{\vec{k}, \alpha, \beta} \tilde{K}_{\alpha \beta}(\vec{k}) \tilde{u}_{\alpha}(\vec{k}) \tilde{u}_{\beta}(\vec{k})^{*}
\end{aligned}
$$

where $\tilde{K}_{\alpha \beta}(\vec{k})=\sum_{\vec{\rho}} K_{\alpha \beta}(\vec{\rho}) \exp (i \vec{k} \cdot \vec{\rho})$, and $\tilde{u}_{\beta}(\vec{k})^{*}=\tilde{u}_{\beta}(-\vec{k})$ is the complex conjugate of $\tilde{u}_{\beta}(\vec{k})$

The different Fourier modes are thus decoupled at the quadratic order, and the task of diagonalizing the $3 N \times 3 N$ matrix of second derivatives is reduced to diagonalizing the $3 \times 3$ matrix $\tilde{K}_{\alpha \beta}(\vec{k})$ separately for each $\vec{k} .$ The from of $\tilde{K}_{\alpha \beta}$ is further restricted by the point group symmetries of the crystal. The discussion of such constraints is beyond the intent of this section and for simplicity we shall assume that $\tilde{K}_{\alpha \beta}(\vec{k})=\delta_{\alpha, \beta} \tilde{K}(\vec{k})$, is already diagonal. (For an isotropic material, this implies a specific relation between bulk and shear moduli.)

The kinetic energy of deformations is

$$
\sum_{i=1}^{N} \frac{m}{2} \dot{\vec{q}}_{i}^{2}=\sum_{\vec{k}, \alpha} \frac{m}{2} \dot{\tilde{u}}_{\alpha}(\vec{k}) \dot{\tilde{u}}_{\alpha}(\vec{k})^{*}=\sum_{\vec{k}, \alpha} \frac{1}{2 m} \tilde{p}_{\alpha}(\vec{k}) \tilde{p}_{\alpha}(\vec{k})^{*}
$$

where

$$
\tilde{p}_{\alpha}(\vec{k})=\frac{\partial \mathcal{L}}{\partial \dot{\tilde{u}}_{\alpha}(\vec{k})}=m \dot{\tilde{u}}_{\alpha}(\vec{k})
$$

is the momentum conjugate to $\tilde{u}_{\alpha}(\vec{k}) .$ The resulting deformation Hamiltonian,

$$
\mathcal{H}=\mathcal{V}^{*}+\sum_{\vec{k}, \alpha}\left[\frac{1}{2 m}\left|\tilde{p}_{\alpha}(\vec{k})\right|^{2}+\frac{\tilde{K}(\vec{k})}{2}\left|\tilde{u}_{\alpha}(\vec{k})\right|^{2}\right]
$$

describes $3 N$ independent harmonic oscillators of frequencies $\omega_{\alpha}(\vec{k})=\sqrt{\tilde{K}(\vec{k}) / m}$

In a classical treatment, each harmonic oscillator of non-zero stiffness contributes $k_{B} T$ to the internal energy of the solid. At most, 6 of the $3 N$ oscillators are expected to have zero stiffness (corresponding to uniform translations and rotations of the crystal). Thus, up to non-extensive corrections of order $1 / N$, the classical internal energy associated with Hamiltonian (VI.33) is $3 N k_{B} T$, leading to a temperature independent heat capacity of $3 k_{B}$ per atom. In fact, the measured heat capacity vanishes at low temperatures. We can again relate this observation to the quantization of the energy levels of each oscillator, as discussed in the previous section. Quantizing each harmonic mode separately, gives the allowed values of the Hamiltonian as

$$
\mathcal{H}^{q}=\mathcal{V}^{*}+\sum_{\vec{k}, \alpha} \hbar \omega_{\alpha}(\vec{k})\left(n_{\vec{k}, \alpha}+\frac{1}{2}\right)
$$

where the set of integers $\left\{n_{\vec{k}, \alpha}\right\}$ describes the quantum micro-state of the oscillators. Since the oscillators are independent, their partition function,

$$
Z^{q}=\sum_{\left\{n_{\vec{k}, \alpha}\right\}} e^{-\beta \mathcal{H}^{q}}=e^{-\beta E_{0}} \prod_{\vec{k}, \alpha} \sum_{n_{\vec{k}, \alpha}} e^{-\beta \hbar \omega_{\alpha}(\vec{k}) n_{\vec{k}, \alpha}}=e^{-\beta E_{0}} \prod_{\vec{k}, \alpha}\left[\frac{1}{1-e^{-\beta \hbar \omega_{\alpha}(\vec{k})}}\right]
$$

![](https://cdn.mathpix.com/cropped/ea7abc83a73d8bc32aefd1b25740bde8-09.jpg?height=35&width=985&top_left_y=379&top_left_x=145) ground state energies of all oscillators in addition to $\left.\mathcal{V}^{*} .\right)$

The internal energy is

$$
E(T)=\left\langle\mathcal{H}^{q}\right\rangle=E_{0}+\sum_{\vec{k}, \alpha} \hbar \omega_{\alpha}(\vec{k})\left\langle n_{\alpha}(\vec{k})\right\rangle
$$

where the average occupation numbers are given by

$$
\begin{aligned}
\left\langle n_{\alpha}(\vec{k})\right\rangle &=\frac{\sum_{n=0}^{\infty} n e^{-\beta \hbar \omega_{\alpha}(\vec{k}) n}}{\sum_{n=0}^{\infty} e^{-\beta \hbar \omega_{\alpha}(\vec{k}) n}}=-\frac{\partial}{\partial\left(\beta \hbar \omega_{\alpha}(\vec{k})\right)} \ln \left(\frac{1}{1-e^{-\beta \hbar \omega_{\alpha}(\vec{k})}}\right) \\
&=\frac{e^{-\beta \hbar \omega_{\alpha}(\vec{k})}}{1-e^{-\beta \hbar \omega_{\alpha}(\vec{k})}}=\frac{1}{e^{\beta \hbar \omega_{\alpha}(\vec{k})}-1}
\end{aligned}
$$

As a first attempt at including quantum mechanical effects, we may adopt the Einstein model in which all the oscillators are assumed to have the same frequency $\omega_{E} .$ This model corresponds to atoms that are pinned to their ideal location by springs of stiffness $\bar{K}=\partial^{2} \mathcal{V} / \partial q^{2}=m \omega_{E}^{2} .$ The resulting internal energy,

$$
E=E_{0}+3 N \frac{\hbar \omega_{E} e^{-\beta \hbar \omega_{E}}}{1-e^{-\beta \hbar \omega_{E}}}
$$

and heat capacity,

$$
C=\frac{d E}{d T}=3 N k_{B}\left(\frac{T_{E}}{T}\right)^{2} \frac{e^{-T_{E} / T}}{\left(1-e^{-T_{E} / T}\right)^{2}}
$$

is simply proportional to that of a single oscillator (eqs.(VI.12) and (VI.13)). In particular, there is an exponential decay of the heat capacity to zero with a characteristic temperature $T_{E}=\hbar \omega_{E} / k_{B} .$ However, the experimentally measured heat capacity decays to zero much more slowly, as $T^{3}$

The discrepancy is resolved through the Debye model, which emphasizes that at low temperatures the main contribution to heat capacity is from the oscillators of lowest frequency that are the most easily excited. The lowest energy modes in turn correspond to smallest wavevectors $k=|\vec{k}|$, or longest wavelengths $\lambda=2 \pi / k .$ Indeed, the modes with $\vec{k}=0$ simply describe pure translations of the lattice and have zero stiffness. By continuity we expect, $\lim _{\vec{k} \rightarrow 0} \tilde{K}(\vec{k})=0$, and ignoring considerations of crystal symmetry, the expansion of $\tilde{K}(\vec{k})$ at small wavevectors takes the form

$$
\tilde{K}(\vec{k})=B k^{2}+\mathcal{O}\left(k^{4}\right)
$$

The odd terms are absent in the expansion, since $\tilde{K}(\vec{k})=\tilde{K}(-\vec{k})$ follows from $K\left(\vec{r}-\vec{r}^{\prime}\right)=$ $K\left(\vec{r}^{\prime}-\vec{r}\right)$ in real space. The corresponding frequencies at long wavelengths are

$$
\omega(\vec{k})=\sqrt{\frac{B k^{2}}{m}}=v k
$$

where $v=\sqrt{B / m}$ is the speed of sound in the crystal. (In a real material, $\tilde{K}_{\alpha \beta}$ is not proportional to $\delta_{\alpha \beta}$, and different polarizations of sound have different velocities.)

The quanta of vibrational modes are usually referred to as phonons. Using the dispersion relation in eq.(VI.40), the contribution of phonons to the internal energy is

$$
\left\langle\mathcal{H}^{q}\right\rangle=E_{0}+\sum_{\vec{k}, \alpha} \frac{\hbar v k}{e^{\beta \hbar v k}-1}
$$

With periodic boundary conditions in a box of dimensions $L_{x} \times L_{y} \times L_{z}$, the allowed wavevectors are

$$
\vec{k}=\left(\frac{2 \pi n_{x}}{L_{x}}, \frac{2 \pi n_{y}}{L_{y}}, \frac{2 \pi n_{z}}{L_{z}}\right)
$$

where $n_{x}, n_{y}$, and $n_{z}$ are integers. In the large size limit, these modes are very densely packed, and the number of modes in a volume element $d^{3} \vec{k}$ is

$$
d \mathcal{N}=\frac{d k_{x}}{2 \pi / L_{x}} \frac{d k_{y}}{2 \pi / L_{y}} \frac{d k_{x}}{2 \pi / L_{z}}=\frac{V}{(2 \pi)^{3}} d^{3} \vec{k} \equiv \rho d^{3} \vec{k}
$$

Using the phase space density $\rho$, any sum over allowed wavevectors can be replaced by an integral as

$$
\lim _{V \rightarrow \infty} \sum_{\vec{k}} f(\vec{k})=\int d^{3} \vec{k} \rho f(\vec{k})
$$

Hence, eq.(VI.41) can be re-written as

$$
E=E_{0}+3 V \int^{B . Z} \quad \frac{d^{3} \vec{k}}{(2 \pi)^{3}} \frac{\hbar v k}{e^{\beta \hbar v k}-1}
$$

where the integral is performed over the volume of the Brillouin zone, and the factor of 3 comes from assuming the same sound velocity for the three polarizations.

Due to its dependence on the shape of the Brillouin zone, it is not possible to give a simple closed form expression for the energy in eq.(VI.45). However, we can examine its high and low temperature limits. The characteristic temperature separating the two limits,

$$
T_{D}=\frac{\hbar v k_{\max }}{k_{B}} \approx \frac{\hbar v}{k_{B}} \cdot \frac{\pi}{a}
$$

corresponds to the high frequency modes at the edge of the zone. For $T \gg T_{D}$, all modes behave classically. The integrand of eq.(VI.45) is just $k_{B} T$, and since the total number of modes is $3 N=3 V \int^{\text {B.Z. }} d^{3} \vec{k} /(2 \pi)^{3}$, the classical results of $E(T)=E_{0}+3 N k_{B} T$, and $C=3 N k_{B}$ are recovered. For $T \ll T_{D}$, the factor $\exp (\beta \hbar v k)$ in the denominator of eq.(VI.45) is very large at the Brillouin zone edge. The most important contribution to the integral comes from small $k$, and the error in extending the integration range to infinity is small. After changing variables to $x=\beta \hbar v|\vec{k}|$, and using $d^{3} \vec{k}=4 \pi x^{2} d x /(\beta \hbar v)^{3}$ due to spherical symmetry, eq.(VI.45) gives

$$
\begin{aligned}
\lim _{T \ll T_{D}} E(T) & \approx E_{0}+\frac{3 V}{8 \pi^{3}}\left(\frac{k_{B} T}{\hbar v}\right)^{3} 4 \pi k_{B} T \int_{0}^{\infty} d x \frac{x^{3}}{e^{x}-1} \\
&=E_{0}+\frac{\pi^{2}}{10} V\left(\frac{k T}{\hbar v}\right)^{3} k_{B} T
\end{aligned}
$$

(The value of the definite integral, $\pi^{4} / 15 \approx 6.5$, can be found in standard tables.) The resulting heat capacity,

$$
C=\frac{d E}{d T}=k_{B} V \frac{2 \pi^{2}}{5}\left(\frac{k_{B} T}{\hbar v}\right)^{3}
$$

has the form $C \propto N k_{B}\left(T / T_{D}\right)^{3}$ in agreement with observations. The physical interpretation of this result is the following: At temperatures $T \ll T_{D}$, only a fraction of the phonon modes can be thermally excited. These are the low frequency phonons with energy quanta $\hbar \omega(\vec{k}) \ll k_{B} T .$ The excited phonons have wavevectors $|\vec{k}|<k^{*}(T) \approx\left(k_{B} T / \hbar v\right)$ Quite generally, in $d$ space dimensions, the number of these modes is approximately $V k^{*}(T)^{d} \sim V\left(k_{B} T / \hbar v\right)^{d} .$ Each excited mode can be treated classically, and contributes roughly $k_{B} T$ to the internal energy which thus scales as $E \sim V\left(k_{B} T / \hbar v\right)^{d} k_{B} T .$ The corresponding heat capacity, $C \sim V k_{B}\left(k_{B} T / \hbar v\right)^{d}$, vanishes as $T^{d}$. 

\section{VI.C Black-body Radiation}

Phonons correspond to vibrations of a solid medium. There are also (longitudinal) sound modes in liquid and gas states. However, even "empty" vacuum, can support fluctuations of the electromagnetic (EM) field, photons, which can be thermally excited at finite temperatures. The normal modes of this field are EM waves, characterized by a wave-number $\vec{k}$, and two possible polarizations $\alpha .$ (Since $\nabla \cdot \vec{E}=0$ in free space, the electric field must be normal to $\vec{k}$, and only transverse modes exist.) With appropriate choice of coordinates, the Hamiltonian for the EM field can be written as a sum of harmonic oscillators,

$$
\mathcal{H}=\frac{1}{2} \sum_{\vec{k}, \alpha}\left[\left|\tilde{p}_{\vec{k}, \alpha}\right|^{2}+\omega_{\alpha}(\vec{k})^{2}\left|\tilde{u}_{\alpha}(\vec{k})\right|^{2}\right]
$$

with $\omega_{\alpha}(\vec{k})=c k$, where $c$ is the speed of light.

With periodic boundary conditions, the allowed wavevectors in a box of size $L$ are $\vec{k}=2 \pi\left(n_{x}, n_{y}, n_{z}\right) / L$ where $\left\{n_{x}, n_{y}, n_{z}\right\}$ are integers. However, unlike phonons, there is no Brillouin zone limiting the size of $\vec{k}$, and these integers can be arbitrarily large. The lack of such a restriction leads to the ultraviolet catastrophe in a classical treatment: As there is no limit to the wavevector, assigning $k_{B} T$ per mode leads to an infinite energy stored in the high frequency modes. (The low frequencies are cut off by the finite size of the box.) It was indeed to resolve this difficulty that Planck suggested that the allowed values of EM energy must be quantized according to the Hamiltonian

$$
\mathcal{H}^{q}=\sum_{\vec{k}, \alpha} \hbar c k\left(n_{\alpha}(\vec{k})+\frac{1}{2}\right), \quad \text { with } \quad n_{\alpha}(\vec{k})=0,1,2, \cdots
$$

As for phonons, the internal energy is calculated from

$$
E=\left\langle\mathcal{H}^{q}\right\rangle=\sum_{\vec{k}, \alpha} \hbar c k\left(\frac{1}{2}+\frac{e^{-\beta \hbar c k}}{1-e^{-\beta \hbar c k}}\right)=V E_{0}+\frac{2 V}{(2 \pi)^{3}} \int d^{3} \vec{k} \frac{\hbar c k}{e^{\beta \hbar c k}-1}
$$

The zero-point energy is actually infinite, but as only energy differences are measured, it is usually ignored. The change of variables to $x=\beta \hbar c k$ allows us to calculate the excitation energy,

$$
\begin{aligned}
\frac{E^{*}}{V} &=\frac{\hbar c}{\pi^{2}}\left(\frac{k_{B} T}{\hbar c}\right)^{4} \int_{0}^{\infty} \frac{d x x}{e^{x}-1} \\
&=\frac{\pi^{2}}{15}\left(\frac{k_{B} T}{\hbar c}\right)^{3} k_{B} T
\end{aligned}
$$

The EM radiation also exerts a pressure on the walls of the container. From the partition function of the Hamiltonian (VI.50),

$$
Z=\sum_{\left\{n_{\alpha}(\vec{k})\right\}} \exp \left[-\beta \hbar \omega(\vec{k})\left(n_{\alpha}(\vec{k})+\frac{1}{2}\right)\right]=\prod_{\vec{k}, \alpha} \frac{e^{-\beta \hbar c k / 2}}{1-e^{-\beta \hbar c k}}
$$

the free energy is

$$
\begin{aligned}
F &=-k_{B} T \ln Z=k_{B} T \sum_{\vec{k}, \alpha}\left[\frac{\beta \hbar c k}{2}+\ln \left(1-e^{-\beta \hbar c k}\right)\right] \\
&=2 V \int \frac{d^{3} \vec{k}}{(2 \pi)^{3}}\left[\frac{\hbar c k}{2}+k_{B} T \ln \left(1-e^{-\beta \hbar c k}\right)\right]
\end{aligned}
$$

The pressure due to the photon gas is

$$
\begin{aligned}
P &=-\left.\frac{\partial F}{\partial V}\right|_{T}=-\int \frac{d^{3} \vec{k}}{(2 \pi)^{3}}\left[\hbar c k+2 k_{B} T \ln \left(1-e^{-\beta \hbar c k}\right)\right] \\
&=P_{0}-\frac{k_{B} T}{\pi^{2}} \int_{0}^{\infty} d k k^{2} \ln \left(1-e^{-\beta \hbar c k}\right) \quad \text { (integrate by parts) } \\
&=P_{0}+\frac{k_{B} T}{\pi^{2}} \int_{0}^{\infty} d k \frac{k^{3}}{3} \frac{\beta \hbar c e^{-\beta \hbar c k}}{1-e^{-\beta \hbar c k}} \quad(\text { compare with eq.(VI.51)) }\\
&=P_{0}+\frac{1}{3} \frac{E}{V}
\end{aligned}
$$

Note that there is also an infinite zero-point pressure $P_{0} .$ Differences in this pressure lead to the Casimir force between conducting plates, which is measurable.

The extra pressure of $1 / 3$ times the energy density can be compared to that of a gas of relativistic particles. (As shown in the test problems, a dispersion relation, $\mathcal{E} \propto|\vec{p}|^{s}$, leads to a pressure, $P=(s / d)(E / V)$ in $d$ dimensions.) Continuing with the analogy to a gas of particles, if a hole is opened in the container wall, the escaping energy flux per unit area and per unit time is

$$
\phi=\left\langle c_{\perp}\right\rangle \frac{E}{V}
$$

All photons have speed $c$, and the average of the component of the velocity perpendicular to the hole can be calculated as

$$
\left\langle c_{\perp}\right\rangle=c \times \frac{1}{4 \pi} \int_{0}^{\pi / 2} 2 \pi \sin \theta d \theta \cos \theta=\frac{c}{4}
$$

resulting in

$$
\phi=\frac{1}{4} c \frac{E}{V}=\frac{\pi^{2}}{60} \frac{k_{B}^{4} T^{4}}{\hbar^{3} c^{2}}
$$

The result, $\phi=\sigma T^{4}$, is the Stephan-Boltzmann law for blackbody radiation, and

$$
\sigma=\frac{\pi^{2}}{60} \frac{k_{B}^{4}}{\hbar^{3} c^{2}} \approx 5.67 \times 10^{-8} \mathrm{Wm}^{-2 \circ} \mathrm{K}^{-4}
$$

is Stephan's constant. Blackbody radiation has a characteristic frequency dependence: Let $E(T) / V=\int d k \mathcal{E}(k, t)$, where

$$
\mathcal{E}(k, T)=\frac{\hbar c}{\pi^{2}} \frac{k^{3}}{e^{\beta \hbar c k}-1}
$$

is the energy density in wavevector $k$. The flux of emitted radiation in the interval $[k, k+d k]$ is $I(k, T) d k$, where

$$
I(k, T)=\frac{c}{4} \mathcal{E}(k, T)=\frac{\hbar c^{2}}{4 \pi^{2}} \frac{k^{3}}{e^{\beta \hbar c k}-1} \rightarrow \begin{cases}c k_{B} T k^{2} / 4 \pi & \text { for } k \ll k^{*}(T) \\ \hbar c^{2} k^{3} e^{-\beta \hbar c k} / 4 \pi^{2} & \text { for } k \gg k^{*}(T)\end{cases}
$$

The characteristic wavevector $k^{*}(T) \approx k_{B} T / \hbar c$ separates quantum and classical regimes. It provides the upper cutoff that eliminates the ultraviolet catastrophe. MIT OpenCourseWare

http://ocw.mit.edu

\subsection{Statistical Mechanics I: Statistical Mechanics of Particles \\ Fall 2013}

For information about citing these materials or our Terms of Use, visit: http://ocw.mit.edu/terms.
