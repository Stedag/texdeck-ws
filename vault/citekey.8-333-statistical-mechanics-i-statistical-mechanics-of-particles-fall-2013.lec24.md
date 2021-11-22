---
id: M9YaRIvbIssCHfNR2znAZ
title: Lec24
desc: ''
updated: 1637530120232
created: 1637530120232
---
\section{VII.E The Degenerate Fermi Gas}

At zero temperature, the fermi occupation number,

$$
\left\langle n_{\vec{k}}\right\rangle_{-}=\frac{1}{e^{\beta(\mathcal{E}(k)-\mu)}+1}
$$

is one for $\mathcal{E}(\vec{k})<\mu$, and zero otherwise. The limiting value of $\mu$ at zero temperature is called the fermi energy, $\mathcal{E}_{F}$, and all one-particle states of energy less than $\mathcal{E}_{F}$ are occupied, forming a fermi sea. For the ideal gas with $\mathcal{E}(\vec{k})=\hbar^{2} k^{2} /(2 m)$, there is a corresponding fermi wavenumber $k_{F}$, calculated from

$$
N=\sum_{|\vec{k}| \leq k_{F}}(2 s+1)=g V \int^{k<k_{F}} \frac{d^{3} \vec{k}}{(2 \pi)^{3}}=g \frac{V}{6 \pi^{2}} k_{F}^{3}
$$

In terms of the density $n=N / V$,

$$
k_{F}=\left(\frac{6 \pi^{2} n}{g}\right)^{1 / 3}, \quad \Longrightarrow \quad \mathcal{E}_{F}(n)=\frac{\hbar^{2} k_{F}^{2}}{2 m}=\frac{\hbar^{2}}{2 m}\left(\frac{6 \pi^{2} n}{g}\right)^{2 / 3}
$$

Note that while in a classical treatment the ideal gas has a large density of states at $T=0$ (from $\left.\Omega_{\text {Classical }}=V^{N} / N !\right)$, the quantum fermi gas has a unique ground state with $\Omega=1 .$ Once the one-particle momenta are specified (all $\vec{k}$ for $\left.|\vec{k}|<k_{F}\right)$, there is only one anti-symmetrized state, as constructed in eq.(VII.7).

To see how the fermi sea is modified at small temperatures, we need the behavior of $f_{m}^{-}(z)$ for large $z$ which, after integration by parts, is

$$
f_{m}^{-}(z)=\frac{1}{m !} \int_{0}^{\infty} d x x^{m} \frac{d}{d x}\left(\frac{-1}{z^{-1} e^{x}+1}\right)
$$

Since the fermi occupation number changes abruptly from one to zero, its derivative in the above equation is sharply peaked. We can expand around this peak by setting $x=\ln z+t$, and extending the range of integration to $-\infty<t<+\infty$, as

$$
\begin{aligned}
f_{m}^{-}(z) & \approx \frac{1}{m !} \int_{-\infty}^{\infty} d t(\ln z+t)^{m} \frac{d}{d t}\left(\frac{-1}{e^{t}+1}\right) \\
&=\frac{1}{m !} \int_{-\infty}^{\infty} d t \sum_{\alpha=0}^{\infty}\left(\begin{array}{c}
m \\
\alpha
\end{array}\right) t^{\alpha}(\ln z)^{m-\alpha} \frac{d}{d t}\left(\frac{-1}{e^{t}+1}\right) \\
&=\frac{(\ln z)^{m}}{m !} \sum_{\alpha=0}^{\infty} \frac{m !}{\alpha !(m-\alpha) !}(\ln z)^{-\alpha} \int_{-\infty}^{\infty} d t t^{\alpha} \frac{d}{d t}\left(\frac{-1}{e^{t}+1}\right)
\end{aligned}
$$

Using the (anti-) symmetry of the integrand under $t \rightarrow-t$, and un-doing the integration by parts yields,

$$
\frac{1}{\alpha !} \int_{-\infty}^{\infty} d t t^{\alpha} \frac{d}{d t}\left(\frac{-1}{e^{t}+1}\right)=\left\{\begin{array}{c}
0 \\
\frac{2}{(\alpha-1) !} \int_{0}^{\infty} d t \frac{t^{\alpha-1}}{e^{t}+1}=2 f_{\alpha}^{-}(1)
\end{array} \quad \text { for } \alpha\right. \text { odd }
$$

Inserting the above into eq.(VII.43), and using tabulated values for the integrals $f_{\alpha}^{-}(1)$, leads to the Sommerfeld expansion,

$$
\begin{aligned}
\lim _{z \rightarrow \infty} f_{m}^{-}(z) &=\frac{(\ln z)^{m}}{m !} \sum_{\alpha=0}^{\text {even }} 2 f_{\alpha}^{-}(1) \frac{m !}{(m-\alpha) !}(\ln z)^{-\alpha} \\
&=\frac{(\ln z)^{m}}{m !}\left[1+\frac{\pi^{2}}{6} \frac{m(m-1)}{(\ln z)^{2}}+\frac{7 \pi^{4}}{360} \frac{m(m-1)(m-2)(m-3)}{(\ln z)^{4}}+\cdots\right]
\end{aligned}
$$

In the degenerate limit, the density and chemical potential are related by

$$
\frac{n \lambda^{3}}{g}=f_{3 / 2}^{-}(z)=\frac{(\ln z)^{3 / 2}}{(3 / 2) !}\left[1+\frac{\pi^{2}}{6} \frac{3}{2} \frac{1}{2}(\ln z)^{-2}+\cdots\right] \gg 1
$$

The lowest order result reproduces the expression in eq.(VII.41) for the fermi energy,

$$
\lim _{T \rightarrow 0} \ln z=\left[\frac{3}{4 \sqrt{\pi}} \frac{n \lambda^{3}}{g}\right]^{2 / 3}=\frac{\beta \hbar^{2}}{2 m}\left(\frac{6 \pi^{2} n}{g}\right)^{2 / 3}=\beta \mathcal{E}_{F}
$$

Inserting the zero temperature limit into eq.(VII.45) gives the first order correction,

$$
\ln z=\beta \mathcal{E}_{F}\left[1+\frac{\pi^{2}}{8}\left(\frac{k_{B} T}{\mathcal{E}_{F}}\right)^{2}+\cdots\right]^{-2 / 3}=\beta \mathcal{E}_{F}\left[1-\frac{\pi^{2}}{12}\left(\frac{k_{B} T}{\mathcal{E}_{F}}\right)^{2}+\cdots\right]
$$

The appropriate dimensionless expansion parameter is $\left(k_{B} T / \mathcal{E}_{F}\right) .$ Note that the fermion chemical potential $\mu=k_{B} T \ln z$, is positive at low temperatures, and negative at high temperatures (from eq.(VII.38)). It changes sign at a temperature proportional to $\mathcal{E}_{F} / k_{B}$.

The low temperature expansion for the pressure is

$$
\begin{aligned}
\beta P &=\frac{g}{\lambda^{3}} f_{5 / 2}^{-}(z)=\frac{g}{\lambda^{3}} \frac{(\ln z)^{5 / 2}}{(5 / 2) !}\left[1+\frac{\pi^{2}}{6} \frac{5}{2} \frac{3}{2}(\ln z)^{-2}+\cdots\right] \\
&=\frac{g}{\lambda^{3}} \frac{8\left(\beta \mathcal{E}_{F}\right)^{5 / 2}}{15 \sqrt{\pi}}\left[1-\frac{5}{2} \frac{\pi^{2}}{12}\left(\frac{k_{B} T}{\mathcal{E}_{F}}\right)^{2}+\cdots\right]\left[1+\frac{5 \pi^{2}}{8}\left(\frac{k_{B} T}{\mathcal{E}_{F}}\right)^{2}+\cdots\right] \\
&=P_{F}\left[1+\frac{5}{12} \pi^{2}\left(\frac{k_{B} T}{\mathcal{E}_{F}}\right)^{2}+\cdots\right]
\end{aligned}
$$

where $P_{F}=(2 / 5) n \mathcal{E}_{F}$ if the fermi pressure. Unlike its classical counterpart, the fermi gas at zero temperature has finite pressure and internal energy.

The low temperature expansion for the internal energy is obtained easily from eq.(VII.47) using

$$
\frac{E}{V}=\frac{3}{2} P=\frac{3}{5} n k_{B} T_{F}\left[1+\frac{5}{12} \pi^{2}\left(\frac{T}{T_{F}}\right)^{2}+\cdots\right]
$$

where we have introduced the fermi temperature $T_{F}=\mathcal{E}_{F} / k_{B} .$ Eq.(VII.48) leads to a low temperature heat capacity,

$$
C_{V}=\frac{d E}{d T}=\frac{\pi^{2}}{2} N k_{B}\left(\frac{T}{T_{F}}\right)+\mathcal{O}\left(\frac{T}{T_{F}}\right)^{2}
$$

The linear vanishing of the heat capacity as $T \rightarrow 0$ is a general feature of a fermi gas, valid in all dimensions. It has the following simple physical interpretation: The probability of occupying single-particle states, eq.(VII.40), is very close to a step function at small temperatures. Only particles within a distance of approximately $k_{B} T$ of the fermi energy can be thermally excited. This represents only a small fraction $T / T_{F}$, of the total number of electrons. Each excited particle gains an energy of the order of $k_{B} T$, leading to a change in the internal energy of approximately $k_{B} T N\left(T / T_{F}\right) .$ Hence the heat capacity is given by $C_{V}=d E / d T \sim N k_{B} T / T_{F}$. This conclusion is also valid for an interacting fermi gas. The fact that only a small number, $N\left(T / T_{F}\right)$, of fermions are excited at small temperatures accounts for many interesting properties of fermi gases. For example, the magnetic susceptibility of a classical gas of $N$ non-interacting particles of magnetic moment $\mu_{B}$ follows the Curie law, $\chi \propto N \mu_{B}^{2} /\left(k_{B} T\right)$. Since quantum mechanically, only a fraction of spins contributes at low temperatures, the low temperature susceptibility saturates to a (Pauli) value of $\chi \propto N \mu_{B}^{2} /\left(k_{B} T_{F}\right)$. (See review problems for the details of this calculation.) MIT OpenCourseWare

http://ocw.mit.edu

\subsection{Statistical Mechanics I: Statistical Mechanics of Particles \\ Fall 2013}

For information about citing these materials or our Terms of Use, visit: http://ocw.mit.edu/terms.
