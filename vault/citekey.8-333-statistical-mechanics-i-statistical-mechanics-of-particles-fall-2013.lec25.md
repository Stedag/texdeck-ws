---
id: k54BBpSpHYhrp4kjV46EG
title: Lec25
desc: ''
updated: 1637530120233
created: 1637530120233
---
\section{VII.F The Degenerate Bose Gas}

The average boson occupation number,

$$
\left\langle n_{\vec{k}}\right\rangle_{+}=\frac{1}{\exp [\beta(\mathcal{E}(\vec{k})-\mu)]-1}
$$

must be always positive. This requires $\mathcal{E}(\vec{k})-\mu$ to be positive for all $\vec{k}$, and hence $\mu<$ $\min [\mathcal{E}(\vec{k})]_{\vec{k}}=0$ (for $\left.\mathcal{E}(\vec{k})=\hbar^{2} k^{2} / 2 m\right)$. At high temperatures (classical limit), $\mu$ is large and negative, and increases towards zero as $-k_{B} T \ln \left(n \lambda^{3} / g\right)$ as temperature is reduced. In the degenerate quantum limit, $\mu$ approaches its limiting value of zero. To see how this limit is achieved, and to find out about the behavior of the degenerate bose gas, we have to examine the limiting behavior of the functions $f_{m}^{+}(z)$ in eqs.(VII.35) as $z=\exp (\beta \mu)$ goes to unity.

The functions $f_{m}^{+}(z)$ are monotonically increasing with $z$ in the interval $0 \leq z \leq 1$ The maximum value attained at $z=1$ is

$$
\zeta_{m} \equiv f_{m}^{+}(1)=\frac{1}{(m-1) !} \int_{0}^{\infty} \frac{d x x^{m-1}}{e^{x}-1}
$$

The integrand has a pole as $x \rightarrow 0$, where it behaves as $\int d x x^{m-2} .$ Therefore, $\zeta_{m}$ is finite for $m>1$ and infinite for $m<1 .$ A useful recursive property of these functions is (for $m>1)$

$$
\begin{aligned}
\frac{d}{d z} f_{m}^{+}(z) &=\int_{0}^{\infty} d x \frac{x^{m-1}}{(m-1) !} \frac{d}{d z}\left(\frac{1}{z^{-1} e^{x}-1}\right) \\
\left(\text { use } \frac{d}{d z} f\left(z^{-1} e^{x}\right)=-\frac{e^{x}}{z^{2}} f^{\prime}=-\frac{1}{z} \frac{d}{d x} f\left(z^{-1} e^{x}\right)\right) \\
&=-\frac{1}{z} \int_{0}^{\infty} d x \frac{x^{m-1}}{(m-1) !} \frac{d}{d x}\left(\frac{1}{z^{-1} e^{x}-1}\right) \quad \text { (integrate by parts) } \\
&=\frac{1}{z} \int_{0}^{\infty} d x \frac{x^{m-2}}{(m-2) !} \frac{1}{z^{-1} e^{x}-1}=\frac{1}{z} f_{m-1}^{+}(z)
\end{aligned}
$$

Hence, a sufficiently high derivative of $f_{m}^{+}(z)$ will be divergent at $z=1$ for all $m$.

The density of excited states for the non-relativistic bose gas in three dimensions is thus bounded by

$$
n_{\times}=\frac{g}{\lambda^{3}} f_{3 / 2}^{+}(z) \leq n^{*}=\frac{g}{\lambda^{3}} \zeta_{3 / 2}
$$

At sufficiently high temperatures, such that

$$
\frac{n \lambda^{3}}{g}=\frac{n}{g}\left(\frac{h}{\sqrt{2 \pi m k_{B} T}}\right)^{3} \leq \zeta_{3 / 2} \approx 2.612 \cdots
$$

this bound is not relevant and $n_{\times}=n .$ However, on lowering temperature, the limiting density of excited states is achieved at

$$
T_{c}(n)=\frac{h^{2}}{2 \pi m k_{B}}\left(\frac{n}{g \zeta_{3 / 2}}\right)^{2 / 3}
$$

For $T \leq T_{c}, z$ gets stuck to unity $(\mu=0)$. The limiting density of excited states, $n^{*}=g \zeta_{3 / 2} / \lambda^{3} \propto T^{3 / 2}$, is then less than the total particle density. The remaining gas particles, with density $n_{0}=n-n^{*}$, occupy the lowest energy state with $\vec{k}=0 .$ The phenomenon of a macroscopic occupation of a single one- particle state is known as BoseEinstein condensation.

The bose condensate has some unusual properties. The gas pressure for $T<T_{c}$,

$$
\beta P=\frac{g}{\lambda^{3}} f_{5 / 2}^{+}(1)=\frac{g}{\lambda^{3}} \zeta_{5 / 2} \approx 1.341 \frac{g}{\lambda^{3}}
$$

vanishes as $T^{5 / 2}$ and is independent of density. This is because only the excited fraction $n^{*}$ has finite momentum and contributes to the pressure. Alternatively, bose condensation can be achieved at a fixed temperature by increasing density (reducing volume). From eq.(VII.54), the transition occurs at a specific volume

$$
v^{*}=\frac{1}{n^{*}}=\frac{\lambda^{3}}{g \zeta_{3 / 2}}
$$

For $v<v^{*}$, the pressure-volume isotherm is flat, since $\partial P / \partial v \propto \partial P / \partial n=0$ from eq.(VII.56). The flat portion of isotherms is reminiscent of coexisting liquid and gas phases. We can similarly regard bose condensation as the coexistence of a "normal gas" of specific volume $v^{*}$, and a "liquid" of volume $0 .$ The vanishing of the "liquid" volume is an unrealistic feature due to the absence of any interaction potential between the particles.

Bose condensation combines features of discontinuous (first order), and continuous (second order) transitions; there is a finite latent heat while the compressibility diverges. The latent heat of the transition can be obtained from the Clausius-Clapeyron equation which gives the change of the transition temperature with pressure as

$$
\left.\frac{d T}{d P}\right|_{\text {Coexistence }}=\frac{\Delta V}{\Delta S}=\frac{T_{c}\left(v^{*}-v_{0}\right)}{L}
$$

Since eq.(VII.56) gives the gas pressure right up to the transition point,

$$
\left.\frac{d P}{d T}\right|_{\text {Coexistence }}=\frac{5}{2} \frac{P}{T}
$$

Using the above equations we find a latent heat,

$$
\begin{aligned}
L=T_{c} v^{*} \frac{d P}{d T} &\left.\right|_{\text {Coexistence }} &=\frac{5}{2} P v^{*}=\frac{5}{2} \frac{g}{\lambda^{3}} \zeta_{5 / 2} k_{B} T_{c}\left(\frac{g}{\lambda^{3}} \zeta_{3 / 2}\right)^{-1} \\
& \Longrightarrow \quad L=\frac{5}{2} \frac{\zeta_{5 / 2}}{\zeta_{3 / 2}} k_{B} T_{c} \approx 1.28 k_{B} T_{c}
\end{aligned}
$$

To find the compressibility $\kappa_{T}=\partial n /\left.\partial P\right|_{T} / n$, take derivatives of eqs.(VII.35), and take advantage of the identity in eq.(VII.52) to get

$$
\left\{\begin{array}{l}
\frac{d P}{d z}=\frac{g k_{B} T}{\lambda^{3}} \frac{1}{z} f_{3 / 2}^{+}(z) \\
\frac{d n}{d z}=\frac{g}{\lambda^{3}} \frac{1}{z} f_{1 / 2}^{+}(z)
\end{array}\right.
$$

The ratio of these equations leads to

$$
\kappa_{T}=\frac{f_{1 / 2}^{+}(z)}{n k_{B} T f_{3 / 2}^{+}(z)}
$$

which diverges at the transition since $\lim _{z \rightarrow 1} f_{1 / 2}^{+}(z) \rightarrow \infty$, i.e. the isotherms approach the flat coexistence portion tangentially.

From the expression for energy in the grand canonical ensemble,

$$
E=\frac{3}{2} P V=\frac{3}{2} V \frac{g}{\lambda^{3}} k_{B} T f_{5 / 2}^{+}(z) \propto T^{5 / 2} f_{5 / 2}^{+}(z)
$$

and using eq.(VII.52), the heat capacity is obtained as

$$
C_{V, N}=\left.\frac{d E}{d T}\right|_{V, N}=\frac{3}{2} V \frac{g}{\lambda^{3}} k_{B} T\left[\frac{5}{2 T} f_{5 / 2}^{+}(z)+\left.\frac{1}{z} f_{3 / 2}^{+}(z) \frac{d z}{d T}\right|_{V, N}\right]
$$

The derivative $d z /\left.d T\right|_{V, N}$ is found from the condition of fixed particle number, using

$$
\left.\frac{d N}{d T}\right|_{V}=0=\frac{g}{\lambda^{3}} V\left[\frac{3}{2 T} f_{3 / 2}^{+}(z)+\left.\frac{1}{z} f_{1 / 2}^{+}(z) \frac{d z}{d T}\right|_{V, N}\right]
$$

Substituting the solution

$$
\left.\frac{T}{z} \frac{d z}{d T}\right|_{V, N}=-\frac{3}{2} \frac{f_{3 / 2}^{+}(z)}{f_{1 / 2}^{+}(z)}
$$

into eq.(VII.64) yields

$$
\frac{C_{V}}{V k_{B}}=\frac{3}{2} \frac{g}{\lambda^{3}}\left[\frac{5}{2} f_{5 / 2}^{+}(z)-\frac{3}{2} \frac{f_{3 / 2}^{+}(z)^{2}}{f_{1 / 2}^{+}(z)}\right]
$$

Expanding the result in powers of $z$ indicates that at high temperatures the heat capacity is larger than the classical value; $C_{V} / N k_{B}=3 / 2\left[1+n \lambda^{3} / 2^{7 / 2}+\cdots\right] .$ At low temperatures, $z=1$ and

$$
\frac{C_{V}}{N k_{B}}=\frac{15}{4} \frac{g}{n \lambda^{3}} \zeta_{5 / 2}=\frac{15}{4} \frac{\zeta_{5 / 2}}{\zeta_{3 / 2}}\left(\frac{T}{T_{c}}\right)^{3 / 2}
$$

The origin of the $T^{3 / 2}$ behavior at low temperatures is easily understood. At $T=0$ all particles occupy the $\vec{k}=0$ state. At small but finite temperatures there is occupation of states of finite momentum, up to a value of approximately $k_{m}$ such that $\hbar^{2} k_{m}^{2} / 2 m=k_{B} T$. Each of these states has an energy proportional to $k_{B} T .$ The excitation energy in $d$ dimensions is thus given by $E_{\times} \propto V k_{m}^{d} k_{B} T .$ The resulting heat capacity is $C_{V} \propto V k_{B} T^{d / 2}$. The reasoning is similar to that used to calculate the heat capacities of a phonon (or photon) gas. The difference in the power laws simply originates from the difference in the energy spectrum of low energy excitations $\left(\mathcal{E}(k) \propto k^{2}\right.$ in the former and $\mathcal{E}(k) \propto k$ for the latter). In both cases the total number of excitations is not conserved, corresponding to $\mu=0 .$ For the bose gas, this lack of conservation only persists up to the transition temperature, at which point all particles are excited out of the reservoir with $\mu=0$ at $\vec{k}=0 . \quad C_{V}$ is continuous at $T_{c}$, reaching a maximum value of approximately $1.92 k_{B}$ per particle, but has a discontinuous derivative at this point. MIT OpenCourseWare

http://ocw.mit.edu

\subsection{Statistical Mechanics I: Statistical Mechanics of Particles \\ Fall 2013}

For information about citing these materials or our Terms of Use, visit: http://ocw.mit.edu/terms.
