\section{III.H Zeroth Order Hydrodynamics}

As a first approximation, we shall assume that in local equilibrium, the density $f_{1}$ at each point in space can be represented as in eq.(III.56), i.e.

$$
f_{1}^{0}(\vec{p}, \vec{q}, t)=\frac{n(\vec{q}, t)}{\left(2 \pi m k_{B} T(\vec{q}, t)\right)^{3 / 2}} \exp \left[-\frac{(\vec{p}-m \vec{u}(\vec{q}, t))^{2}}{2 m k_{B} T(\vec{q}, t)}\right]
$$

The choice of parameters clearly enforces $\int d^{3} \vec{p} f_{1}^{0}=n$, and $\langle\vec{p} / m\rangle^{0}=\vec{u}$, as required. Average values are easily calculated from this Gaussian weight; in particular

$$
\left\langle c_{\alpha} c_{\beta}\right\rangle^{0}=\frac{k_{B} T}{m} \delta_{\alpha \beta}
$$

leading to

$$
P_{\alpha \beta}^{0}=n k_{B} T \delta_{\alpha \beta}, \quad \text { and } \quad \varepsilon=\frac{3}{2} k_{B} T
$$

Since the density $f_{1}^{0}$ is even in $\vec{c}$, all odd expectation values vanish, and in particular

$$
\vec{h}^{0}=0
$$

The conservation laws in this approximation take the simple forms

$$
\left\{\begin{array}{l}
D_{t} n=-n \partial_{\alpha} u_{\alpha} \\
m D_{t} u_{\alpha}=F_{\alpha}-\frac{1}{n} \partial_{\alpha}\left(n k_{B} T\right) \\
D_{t} T=-\frac{2}{3} T \partial_{\alpha} u_{\alpha}
\end{array}\right.
$$

In the above expression, we have introduced the material derivative

$$
D_{t} \equiv\left[\partial_{t}+u_{\beta} \partial_{\beta}\right]
$$

which measures the time variations of any quantity as it moves along the stream-lines set up by the average velocity field $\vec{u} .$ By combining the first and third equations, it is easy to get

$$
D_{t} \ln \left(n T^{-3 / 2}\right)=0
$$

The quantity $\ln \left(n T^{-3 / 2}\right)$ is like a local entropy for the gas (see eq.(III.67)), which according to the above equation is not changed along stream-lines. The zeroth order hydrodynamics thus predicts that the gas flow is adiabatic. This prevents the local equilibrium solution of eq.(III.93) from reaching a true global equilibrium form which necessitates an increase in entropy.

To demonstrate that eqs.(III.97) do not describe a satisfactory approach to equilibrium, examine the evolution of small deformations about a stationary $\left(\vec{u}_{0}=0\right)$ state, in a uniform box $(\vec{F}=0)$, by setting

$$
\left\{\begin{array}{l}
n(\vec{q}, t)=\bar{n}+\nu(\vec{q}, t) \\
T(\vec{q}, t)=\bar{T}+\theta(\vec{q}, t)
\end{array}\right.
$$

We shall next expand eqs.(III.97) to first order in the deviations $(\nu, \theta, \vec{u}) .$ Note that to lowest order, $D_{t}=\partial_{t}+O(u)$, leading to the linearized zeroth order hydrodynamic equations

$$
\left\{\begin{array}{l}
\partial_{t} \nu=-\bar{n} \partial_{\alpha} u_{\alpha} \\
m \partial_{t} u_{\alpha}=-\frac{k_{B} \bar{T}}{\bar{n}} \partial_{\alpha} \nu-k_{B} \partial_{\alpha} \theta \\
\partial_{t} \theta=-\frac{2}{3} \bar{T} \partial_{\alpha} u_{\alpha}
\end{array}\right.
$$

- Normal modes of the system are obtained by Fourier transformations,

$$
A(\vec{k}, \omega)=\int d^{3} \vec{q} d t \exp [i(\vec{k} \cdot \vec{q}-\omega t)] A(\vec{q}, t)
$$

where $A$ stands for any of the three fields $(\nu, \theta, \vec{u}) .$ The natural vibration frequencies are solutions to the matrix equation

$$
\omega\left(\begin{array}{c}
\nu \\
u_{\alpha} \\
\theta
\end{array}\right)=\left(\begin{array}{ccc}
0 & \bar{n} k_{\beta} & 0 \\
\frac{k_{B} \bar{T}}{m \bar{n}} \delta_{\alpha \beta} k_{\beta} & 0 & \frac{k_{B}}{m} \delta_{\alpha \beta} k_{\beta} \\
0 & \frac{2}{3} \bar{T} k_{\beta} & 0
\end{array}\right)\left(\begin{array}{c}
\nu \\
u_{\beta} \\
\theta
\end{array}\right)
$$

It is easy to check that this equation has the following modes, the first three with zero frequency:

(a) Two modes describe shear flows in a uniform $(n=\bar{n})$ and isothermal $(T=\bar{T})$ fluid, in which the velocity varies along a direction normal to its orientation (e.g. $\vec{u}=f(x, t) \hat{y})$. In terms of Fourier modes $\vec{k} \cdot \vec{u}_{T}(\vec{k})=0$, indicating transverse flows that are not relaxed in this zeroth order approximation.

(b) A third zero frequency mode describes a stationary fluid with uniform pressure $P=$ $n k_{B} T .$ While $n$ and $T$ may vary across space, their product is constant, insuring that the fluid will not start moving due to pressure variations. The corresponding eigenvector of eq.(III.103) is

$$
\mathbf{v}_{\mathbf{e}}=\left(\begin{array}{c}
\bar{n} \\
0 \\
-\bar{T}
\end{array}\right)
$$

(c) Finally, the longitudinal velocity $\left(\vec{u}_{\ell} \| \vec{k}\right)$ combines with density and temperature variations in eigenmodes of the form

$$
\mathbf{v}_{\mathbf{l}}=\left(\begin{array}{c}
\bar{n}|\vec{k}| \\
\omega(\vec{k}) \\
\frac{2}{3} \bar{T}|\vec{k}|
\end{array}\right), \quad \text { with } \quad \omega(\vec{k})=\pm v_{\ell}|\vec{k}|
$$

where

$$
v_{\ell}=\sqrt{\frac{5 k_{B} \bar{T}}{3}}
$$

is the longitudinal sound velocity. Note that the density and temperature variations in this mode are adiabatic, i.e. the local entropy (proportional to $\left.\ln \left(n T^{-3 / 2}\right)\right)$ is left unchanged.

We thus find that none of the conserved quantities relaxes to equilibrium in the zeroth order approximation. Shear flow and entropy modes persist forever, while the two sound modes have undamped oscillations. This is a deficiency of the zeroth order approximation which is removed by finding a better solution to the Boltzmann equation.

\section{III.I First Order Hydrodynamics}

While $f_{1}^{0}(\vec{p}, \vec{q}, t)$ of eq.(III.93) does set the right hand side of the Boltzmann equation to zero, it is not a full solution, as the left hand side causes its form to vary. The left hand side is a linear differential operator, which using the various notations introduced in the previous sections, can be written as

$$
\mathcal{L}[f] \equiv\left[\partial_{t}+\frac{p_{\alpha}}{m} \partial_{\alpha}+F_{\alpha} \frac{\partial}{\partial p_{\alpha}}\right] f=\left[D_{t}+c_{\alpha} \partial_{\alpha}+\frac{F_{\alpha}}{m} \frac{\partial}{\partial c_{\alpha}}\right] f
$$

It is simpler to examine the effect of $\mathcal{L}$ on $\ln f_{1}^{0}$. which can be written as

$$
\ln f_{1}^{0}=\ln \left(n T^{-3 / 2}\right)-\frac{m c^{2}}{2 k_{B} T}-\frac{3}{2} \ln \left(2 \pi m k_{B}\right)
$$

Using the relation $\partial\left(c^{2} / 2\right)=c_{\beta} \partial c_{\beta}=-c_{\beta} \partial u_{\beta}$, we get

$$
\begin{aligned}
\mathcal{L}\left[\ln f_{1}^{0}\right] &=D_{t} \ln \left(n T^{-3 / 2}\right)+\frac{m c^{2}}{2 k_{B} T^{2}} D_{t} T+\frac{m}{k_{B} T} c_{\alpha} D_{t} u_{\alpha} \\
&+c_{\alpha}\left(\frac{\partial_{\alpha} n}{n}-\frac{3}{2} \frac{\partial_{\alpha} T}{T}\right)+\frac{m c^{2}}{2 k_{B} T^{2}} c_{\alpha} \partial_{\alpha} T+\frac{m}{k_{B} T} c_{\alpha} c_{\beta} \partial_{\alpha} u_{\beta}-\frac{F_{\alpha} c_{\alpha}}{k_{B} T}
\end{aligned}
$$

If the fields $n, T$, and $u_{\alpha}$, satisfy the zeroth order hydrodynamic eqs.(III.97), we can simplify the above equation to

$$
\begin{aligned}
\mathcal{L}\left[\ln f_{1}^{0}\right] &=0-\frac{m c^{2}}{3 k_{B} T} \partial_{\alpha} u_{\alpha}+c_{\alpha}\left[\left(\frac{F_{\alpha}}{k_{B} T}-\frac{\partial_{\alpha} n}{n}-\frac{\partial_{\alpha} T}{T}\right)+\left(\frac{\partial_{\alpha} n}{n}-\frac{3}{2} \frac{\partial_{\alpha} T}{T}\right)-\frac{F_{\alpha}}{k_{B} T}\right] \\
&+\frac{m c^{2}}{2 k_{B} T^{2}} c_{\alpha} \partial_{\alpha} T+\frac{m}{k_{B} T} c_{\alpha} c_{\beta} u_{\alpha \beta} \\
&=\frac{m}{k_{B} T}\left(c_{\alpha} c_{\beta}-\frac{\delta_{\alpha \beta}}{3} c^{2}\right) u_{\alpha \beta}+\left(\frac{m c^{2}}{2 k_{B} T}-\frac{5}{2}\right) \frac{c_{\alpha}}{T} \partial_{\alpha} T
\end{aligned}
$$

The characteristic time scale $\tau_{U}$ for $\mathcal{L}$ is extrinsic, and can be made much larger than $\tau_{\times} .$ The zeroth order result is thus exact in the limit $\left(\tau_{\times} / \tau_{U}\right) \rightarrow 0 ;$ and corrections can be constructed in a perturbation series in $\left(\tau_{\times} / \tau_{U}\right)$. To this purpose, we set $f_{1}=f_{1}^{0}(1+g)$ and linearize the collision operator as

$$
\begin{aligned}
C\left[f_{1}, f_{1}\right] &=-\int d^{3} \vec{p}_{2} d^{2} \vec{b}\left|\vec{v}_{1}-\vec{v}_{2}\right| f_{1}^{0}\left(\vec{p}_{1}\right) f_{1}^{0}\left(\vec{p}_{2}\right)\left[g\left(\vec{p}_{1}\right)+g\left(\vec{p}_{2}\right)-g\left(\vec{p}_{1}^{\prime}\right)-g\left(\vec{p}_{2}^{\prime}\right)\right] \\
& \equiv-f_{1}^{0}\left(\vec{p}_{1}\right) C_{L}[g]
\end{aligned}
$$

While linear, the above integral operator is still difficult to manipulate in general. As a first approximation, and noting its characteristic magnitude, we set

$$
C_{L}[g] \approx \frac{g}{\tau_{\times}}
$$

This is known as the single collision time approximation, and from the linearized Boltzmann equation $\mathcal{L}\left[f_{1}\right]=-f_{1}^{0} C_{L}[g]$, we obtain

$$
g=-\tau_{\times} \frac{1}{f_{1}^{0}} \mathcal{L}\left[f_{1}\right] \approx-\tau_{\times} \mathcal{L}\left[\ln f_{1}^{0}\right]
$$

where we have kept only the leading term. Thus the first order solution is given by (using eq. $($ III. 110$)$ )

$$
f_{1}^{1}(\vec{p}, \vec{q}, t)=f_{1}^{0}(\vec{p}, \vec{q}, t)\left[1-\frac{\tau_{\mu} m}{k_{B} T}\left(c_{\alpha} c_{\beta}-\frac{\delta_{\alpha \beta}}{3} c^{2}\right) u_{\alpha \beta}-\tau_{K}\left(\frac{m c^{2}}{2 k_{B} T}-\frac{5}{2}\right) \frac{c_{\alpha}}{T} \partial_{\alpha} T\right]
$$

where $\tau_{\mu}=\tau_{K}=\tau_{\times}$ in the single collision time approximation. However, in writing the above equation, we have anticipated the possibility of $\tau_{\mu} \neq \tau_{K}$ which arises in more sophisticated treatments (although both times are still of order of $\left.\tau_{\times}\right)$

It is easy to check that $\int d^{3} \vec{p} f_{1}^{1}=\int d^{3} \vec{p} f_{1}^{0}=n$, and thus various local expectation values are calculated to first order as

$$
\langle\mathcal{O}\rangle^{1}=\frac{1}{n} \int d^{3} \vec{p} \mathcal{O} f_{1}^{0}(1+g)=\langle\mathcal{O}\rangle^{0}+\langle g \mathcal{O}\rangle^{0}
$$

The calculation of averages over products of $c_{\alpha}$ 's, distributed according to the Gaussian weight of $f_{1}^{0}$, is greatly simplified by the use of Wick's theorem, which states that expectation value of the product is the sum over all possible products of paired expectation values, for example

$$
\left\langle c_{\alpha} c_{\beta} c_{\gamma} c_{\delta}\right\rangle_{0}=\left(\frac{k_{B} T}{m}\right)^{2}\left(\delta_{\alpha \beta} \delta_{\gamma \delta}+\delta_{\alpha \gamma} \delta_{\beta \delta}+\delta_{\alpha \delta} \delta_{\beta \gamma}\right)
$$

(Expectation values involving a product of an odd number of $c_{\alpha}$ 's are zero by symmetry.) Using this result, it is easy to verify that

$$
\left\langle\frac{p_{\alpha}}{m}\right\rangle^{1}=u_{\alpha}-\tau_{K} \frac{\partial_{\beta} T}{T}\left\langle\left(\frac{m c^{2}}{2 k_{B} T}-\frac{5}{2}\right) c_{\alpha} c_{\beta}\right\rangle^{0}=u_{\alpha}
$$

The pressure tensor at first order is given by

$$
\begin{aligned}
P_{\alpha \beta}^{1} &=n m\left\langle c_{\alpha} c_{\beta}\right\rangle^{1}=n m\left[\left\langle c_{\alpha} c_{\beta}\right\rangle^{0}-\frac{\tau_{\mu} m}{k_{B} T}\left\langle c_{\alpha} c_{\beta}\left(c_{\mu} c_{\nu}-\frac{\delta_{\mu \nu}}{3} c^{2}\right)\right\rangle^{0} u_{\mu \nu}\right] \\
&=n k_{B} T \delta_{\alpha \beta}-2 n k_{B} T \tau_{\mu}\left(u_{\alpha \beta}-\frac{\delta_{\alpha \beta}}{3} u_{\gamma \gamma}\right)
\end{aligned}
$$

(Using the above result, we can further verify that $\varepsilon^{1}=\left\langle m c^{2} / 2\right\rangle^{1}=3 k_{B} T / 2$, as before. $)$ Finally, the heat flux is given by

$$
\begin{aligned}
h_{\alpha}^{1} &=n\left\langle c_{\alpha} \frac{m c^{2}}{2}\right\rangle^{1}=-\frac{n m \tau_{K}}{2} \frac{\partial_{\beta} T}{T}\left\langle\left(\frac{m c^{2}}{2 k_{B} T}-\frac{5}{2}\right) c_{\alpha} c_{\beta} c^{2}\right\rangle^{0} \\
&=-\frac{5}{2} \frac{n k_{B}^{2} T \tau_{K}}{m} \partial_{\alpha} T
\end{aligned}
$$

At this order, we find that spatial variations in temperature generate a heat flow that tends to smooth them out, while shear flows are opposed by the off-diagonal terms in the pressure tensor. These effects are sufficient to cause relaxation to equilibrium, as can be seen by examining the modified behavior of the modes discussed previously. (a) The pressure tensor now has an off-diagonal term

$$
P_{\alpha \neq \beta}^{1}=-2 n k_{B} T \tau_{\mu} u_{\alpha \beta} \equiv-\mu\left(\partial_{\alpha} u_{\beta}+\partial_{\beta} u_{\alpha}\right)
$$

where $\mu \equiv n k_{B} T \tau_{\mu}$ is the viscosity coefficient. A shearing of the fluid (e.g. described by a velocity $\left.u_{y}(x, t)\right)$ now leads to a a viscous force that opposes it (proportional to $\left.\mu \partial_{x}^{2} u_{y}\right)$, causing its diffusive relaxation as discussed below.

(b) Similarly, a temperature gradient leads to a heat flux

$$
\vec{h}=-K \nabla T
$$

where $K=\left(5 n k_{B}^{2} T \tau_{K}\right) /(2 m)$ is the coefficient of thermal conductivity of the gas. If the gas is at rest $\left(\vec{u}=0\right.$, and uniform $\left.P=n k_{B} T\right)$, variations in temperature now satisfy

$$
n \partial_{t} \varepsilon=\frac{3}{2} n k_{B} \partial_{t} T=-\partial_{\alpha}\left(-K \partial_{\alpha} T\right), \quad \Rightarrow \quad \partial_{t} T=\frac{2 K}{3 n k_{B}} \nabla^{2} T
$$

This is the Fourier equation and shows that temperature variations relax by diffusion. We can discuss the behavior of all the modes by linearizing the equations of motion. The first order contribution to $D_{t} u_{\alpha} \approx \partial_{t} u_{\alpha}$ is

$$
\delta^{1}\left(\partial_{t} u_{\alpha}\right) \equiv \frac{1}{m n} \partial_{\beta} \delta^{1} P_{\alpha \beta} \approx-\frac{\mu}{m \bar{n}}\left(\frac{1}{3} \partial_{\alpha} \partial_{\beta}+\delta_{\alpha \beta} \partial_{\gamma} \partial_{\gamma}\right) u_{\beta}
$$

where $\mu \equiv \bar{n} k_{B} \bar{T} \tau_{\mu} .$ Similarly, the correction for $D_{t} T \approx \partial_{t} \theta$, is given by

$$
\delta^{1}\left(\partial_{t} \theta\right) \equiv-\frac{2}{3 k_{B} n} \partial_{\alpha} h_{\alpha} \approx-\frac{2 K}{3 k_{B} \bar{n}} \partial_{\alpha} \partial_{\alpha} \theta
$$

with $K=\left(5 \bar{n} k_{B}^{2} \bar{T} \tau_{K}\right) /(2 m)$. After Fourier transformation, the matrix equation (III.103) is modified to

$$
\omega\left(\begin{array}{c}
\nu \\
u_{\alpha} \\
\theta
\end{array}\right)=\left(\begin{array}{ccc}
0 & \bar{n} \delta_{\alpha \beta} k_{\beta} & 0 \\
\frac{k_{B} \bar{T}}{m \bar{n}} \delta_{\alpha \beta} k_{\beta} & -i \frac{\mu}{m \bar{n}}\left(k^{2} \delta_{\alpha \beta}+\frac{k_{\alpha} k_{\beta}}{3}\right) & \frac{k_{B}}{m} \delta_{\alpha \beta} k_{\beta} \\
0 & \frac{2}{3} \bar{T} \delta_{\alpha \beta} k_{\beta} & -i \frac{2 K k^{2}}{3 k_{B} \bar{n}}
\end{array}\right)\left(\begin{array}{c}
\nu \\
u_{\beta} \\
\theta
\end{array}\right)
$$

We can ask how the normal mode frequencies calculated in the zeroth order approximation are modified at this order. It is simple to verify that the transverse (shear) normal models $\left(\vec{k} \cdot \vec{u}_{T}=0\right)$ now have a frequency

$$
\omega_{T}=-i \frac{\mu}{m \bar{n}} k^{2}
$$

The imaginary frequency implies that these modes are damped over a characteristic time $\tau_{T}(k) \sim 1 /\left|\omega_{T}\right| \sim(\lambda)^{2} /\left(\tau_{\mu} \bar{v}^{2}\right)$, where $\lambda$ is the corresponding wavelength, and $\bar{v} \sim \sqrt{k_{B} T / m}$ is a typical gas particle velocity. We see that the characteristic time scales grow as the square of the wavelength, which is characteristic of diffusive processes.

In the remaining normal modes the velocity is parallel to $\vec{k}$, and eq.(III.125) reduces

to

$$
\omega\left(\begin{array}{c}
\nu \\
u_{\ell} \\
\theta
\end{array}\right)=\left(\begin{array}{ccc}
0 & \bar{n} k & 0 \\
\frac{k_{B} \bar{T}}{m \bar{n}} k & -i \frac{4 \mu k^{2}}{3 m \bar{n}} & \frac{k_{B}}{m} k \\
0 & \frac{2}{3} \bar{T} k & -i \frac{2 K k^{2}}{3 k_{B} \bar{n}}
\end{array}\right)\left(\begin{array}{c}
\nu \\
u_{\beta} \\
\theta
\end{array}\right)
$$

The determinant of the dynamical matrix is the product of the three eigen-frequencies, and to lowest order is given by

$$
\operatorname{det}(M)=i \frac{2 K k^{2}}{3 k_{B} \bar{n}} \cdot \bar{n} k \cdot \frac{k_{B} \bar{T} k}{m \bar{n}}+\mathcal{O}\left(\tau_{\times}^{2}\right)
$$

At zeroth order the two sound modes have $\omega_{\pm}^{0}(k)=\pm v_{\ell} k$, and hence the frequency of the isobaric mode is

$$
\omega_{e}^{1}(k) \approx \frac{\operatorname{det}(M)}{-v_{\ell}^{2} k^{2}}=-i \frac{2 K k^{2}}{5 k_{B} \bar{n}}+\mathcal{O}\left(\tau_{\times}^{2}\right)
$$

At first order, the longitudinal sound modes also turn into damped oscillations with frequencies $\omega_{\pm}^{1}(k)=\pm v_{\ell} k-i \gamma .$ The simplest way to obtain the decay rates is to note that the trace of the dynamical matrix is equal to the sum of the eigenvalues, and hence

$$
\omega_{\pm}^{1}(k)=\pm v_{\ell} k-i k^{2}\left(\frac{2 \mu}{3 m \bar{n}}+\frac{2 K}{15 k_{B} \bar{n}}\right)+\mathcal{O}\left(\tau_{\times}^{2}\right)
$$

The damping of all normal modes guarantees the, albeit slow, approach of the gas to its final uniform and stationary equilibrium state. MIT OpenCourseWare

http://ocw.mit.edu

\subsection{Statistical Mechanics I: Statistical Mechanics of Particles \\ Fall 2013}

For information about citing these materials or our Terms of Use, visit: http://ocw.mit.edu/terms.
