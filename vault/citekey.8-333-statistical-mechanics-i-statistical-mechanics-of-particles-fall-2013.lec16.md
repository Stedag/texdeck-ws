---
id: 5whO10xoMZLnaxb7DvbwL
title: Lec16
desc: ''
updated: 1637530120228
created: 1637530120228
---
\section{V.B The Cluster Expansion}

For short range interactions, specially with a hard core, it is much better to replace the expansion parameter $\mathcal{V}(\vec{q})$ by $f(\vec{q})=\exp (-\beta \mathcal{V}(\vec{q}))-1$, which is obtained by summing over all possible number of bonds between two points on a cumulant graph. The resulting series is organized in powers of the density $N / V$, and is most suitable for obtaining a virial expansion, which expresses the deviations from the ideal gas equation of state in a power series

$$
\frac{P}{k_{B} T}=\frac{N}{V}\left[1+B_{2}(T) \frac{N}{V}+B_{3}(T)\left(\frac{N}{V}\right)^{2}+\cdots\right]
$$

The temperature dependent parameters, $B_{i}(T)$, are known as the virial coefficients and originate from the inter-particle interactions. Our initial goal is to compute these coefficients from first principles.

To illustrate a different method of expansion, we shall perform computations in the grand canonical ensemble. With a macro-state $M \equiv(T, \mu, V)$, the grand partition function is given by

$$
\mathcal{Q}(\mu, T, V)=\sum_{N=0}^{\infty} e^{\beta \mu N} Z(N, T, V)=\sum_{N=0}^{\infty} \frac{1}{N !}\left(\frac{e^{\beta \mu}}{\lambda^{3}}\right)^{N} \mathcal{S}_{N}
$$

where

$$
\mathcal{S}_{N}=\int \prod_{i=1}^{N} d^{3} \vec{q}_{i} \prod_{i<j}\left(1+f_{i j}\right)
$$

and $f_{i j}=f\left(\vec{q}_{i}-\vec{q}_{j}\right)$.

The $2^{N(N-1) / 2}$ terms in $\mathcal{S}_{N}$ can now be ordered in powers of $f_{i j}$ as

$$
\mathcal{S}_{N}=\int \prod_{i=1}^{N} d^{3} \vec{q}_{i}\left(1+\sum_{i<j} f_{i j}+\sum_{i<j, k<l} f_{i j} f_{k l}+\cdots\right)
$$

An efficient method for organizing the perturbation series is to represent the various contributions diagrammatically. In particular we shall apply the following conventions:

(a) Draw $N$ dots labelled by $i=1, \cdots, N$ to represent the coordinates $\vec{q}_{1}$ through $\vec{q}_{N}$

(b) Each term in eq.(V.17) corresponds to a product of $f_{i j}$, represented by drawing lines connecting $i$ and $j$ for each $f_{i j} .$ For example, the graph,

$$
\begin{array}{lllllll}
\bullet & \bullet-\bullet & \bullet-\bullet-\bullet & \multirow{2}{*} {6} & \bullet \\
1 & 2 & 3 & 4 & 5 & 6 & & N
\end{array},
$$

represents the integral

$$
\left(\int d^{3} \vec{q}_{1}\right)\left(\int d^{3} \overrightarrow{q_{2}} d^{3} \vec{q}_{3} f_{23}\right)\left(\int d^{3} \overrightarrow{q_{4}} d^{3} \overrightarrow{q_{5}} d^{3} \vec{q}_{6} f_{45} f_{56}\right) \cdots\left(\int d^{3} \vec{q}_{N}\right)
$$

As the above example indicates, the value of each graph is the product of the contributions from its linked clusters. Since these clusters are more fundamental, we reformulate the sum in terms of them by defining a quantity $b_{\ell}$, equal to the sum over all $\ell$ -particle linked clusters (one-particle irreducible or not). For example

$$
b_{1}=\bullet \quad=\int d^{3} \vec{q}=V
$$

and

$$
b_{2}=\bullet-\bullet=\int d^{3} \vec{q}_{1} d^{3} \vec{q}_{2} f\left(\vec{q}_{1}-\vec{q}_{2}\right)
$$

There are four diagrams contributing to $b_{3}$, leading to

$$
\begin{gathered}
b_{3}=\int d^{3} \vec{q}_{1} d^{3} \vec{q}_{2} d^{3} \vec{q}_{3}\left[f\left(\vec{q}_{1}-\vec{q}_{2}\right) f\left(\vec{q}_{2}-\vec{q}_{3}\right)+f\left(\vec{q}_{2}-\vec{q}_{3}\right) f\left(\vec{q}_{3}-\vec{q}_{1}\right)+f\left(\vec{q}_{3}-\vec{q}_{1}\right) f\left(\vec{q}_{1}-\right.\right. \\
\left.+f\left(\vec{q}_{1}-\vec{q}_{2}\right) f\left(\vec{q}_{2}-\vec{q}_{3}\right) f\left(\vec{q}_{3}-\vec{q}_{1}\right)\right]
\end{gathered}
$$

A given $N$ -particle graph can be decomposed to $n_{1}$ 1-clusters, $n_{2}$ 2-clusters, $\cdots, n_{\ell} \ell$ clusters, etc. Hence,

$$
\mathcal{S}_{N}=\sum_{\left\{n_{\ell}\right\}^{\prime}} \prod_{\ell} b_{\ell}^{n_{\ell}} W\left(\left\{n_{\ell}\right\}\right)
$$

where the restricted sum is over all distinct divisions of $N$ points into a set of clusters $\left\{n_{\ell}\right\}$, such that $\sum_{\ell} \ln _{\ell}=N .$ The coefficients $W\left(\left\{n_{\ell}\right\}\right)$ are the number of ways of assigning $N$ particle labels to groups of $n_{\ell} \ell$ -clusters. For example, the divisions of 3 particles into a 1-cluster and a 2-cluster are

![](https://cdn.mathpix.com/cropped/c952bf7240094200e653c03bc840021d-2.jpg?height=86&width=620&top_left_y=1196&top_left_x=326)

All above graphs have $n_{1}=1$ and $n_{2}=1$, and contribute a factor of $b_{1} b_{2}$ to $S_{3} ;$ thus $W(1,1)=3$

In general, $W\left(\left\{n_{\ell}\right\}\right)$ is the number of distinct ways of grouping the labels $1, \ldots, N$ into bins of $n_{\ell} \ell$ -clusters. It can be obtained from the total number of permutations, $N !$, after dividing by the number of equivalent assignments. Within each bin of $\ell n_{\ell}$ particles, equivalent assignments are obtained by: (i) permuting the $\ell$ labels in each subgroup in $\ell !$ ways, for a total of $(\ell !)^{n_{\ell}}$ permutations; and (ii) the $n_{\ell} !$ rearrangements of the $n_{\ell}$ subgroups. Hence,

$$
W\left(\left\{n_{\ell}\right\}\right)=\frac{N !}{\prod_{\ell} n_{\ell} !(\ell !)^{n_{\ell}}}
$$

(We can indeed check that $W(1,1)=3 ! /(1 !)(2 !)=3$ as obtained above.)

Using the above value of $W$, the expression for $\mathcal{S}_{N}$ in eq.(V.21) can be evaluated. However, the restriction of the sum to configurations such that $\sum_{\ell} \ell n_{\ell}=N$ complicates the evaluation. Fortunately, this restriction disappears in the expression for the grand partition function in eq.(V.16),

$$
\mathcal{Q}=\sum_{N=0}^{\infty} \frac{1}{N !}\left(\frac{e^{\beta \mu}}{\lambda^{3}}\right)^{N} \sum_{\left\{n_{\ell}\right\}^{\prime}} \frac{N !}{\prod_{\ell} n_{\ell} !(\ell !)^{n_{\ell}}} \prod_{\ell} b_{\ell}^{n_{\ell}}
$$

The restriction in the second sum is now removed by noting that $\sum_{N=0}^{\infty} \sum_{\left\{n_{\ell}\right\}} \delta \sum_{\ell} \ell_{n_{\ell}, N}=$ $\sum_{\left\{n_{\ell}\right\}} .$ Therefore,

$$
\begin{aligned}
\mathcal{Q} &=\sum_{\left\{n_{\ell}\right\}}\left(\frac{e^{\beta \mu}}{\lambda^{3}}\right)^{\sum_{\ell} \ell n_{\ell}} \prod_{\ell} \frac{b_{\ell}^{n_{\ell}}}{n_{\ell} !(\ell !)^{n_{\ell}}}=\sum_{\left\{n_{\ell}\right\}} \prod_{\ell} \frac{1}{n_{\ell} !}\left(\frac{e^{\beta \mu \ell} b_{\ell}}{\lambda^{3 \ell} \ell !}\right)^{n_{\ell}} \\
&=\prod_{\ell} \sum_{\left\{n_{\ell}\right\}} \frac{1}{n_{\ell} !}\left[\left(\frac{e^{\beta \mu}}{\lambda^{3}}\right)^{\ell} \frac{b_{\ell}}{\ell !}\right]^{n_{\ell}}=\prod_{\ell} \exp \left[\left(\frac{e^{\beta \mu}}{\lambda^{3}}\right)^{\ell} \frac{b_{\ell}}{\ell !}\right] \\
&=\exp \left[\sum_{\ell=1}^{\infty}\left(\frac{e^{\beta \mu}}{\lambda^{3}}\right)^{\ell} \frac{b_{\ell}}{\ell !}\right]
\end{aligned}
$$

The above result has the simple geometrical interpretation that the sum over all graphs, connected or not, equals the exponential of the sum over connected graphs. This is a quite general result that is also related to the graphical connection between moments and cumulants discussed in sec.II.B.

The grand potential is now obtained from

$$
\ln \mathcal{Q}=-\beta \mathcal{G}=\frac{P V}{k T}=\sum_{\ell=1}^{\infty}\left(\frac{e^{\beta \mu}}{\lambda^{3}}\right)^{\ell} \frac{b_{\ell}}{l !}
$$

In eq.(V.25), the extensivity condition is used to get $\mathcal{G}=E-T S-\mu N=-P V$. Thus the terms on the right hand side of the above equation must also be proportional to the volume $V$. This can be explicitly verified by noting that in evaluating each $b_{\ell}$ there is an integral over the center of mass coordinate that explores the whole volume. For example, $b_{2}=\int d^{3} \vec{q}_{1} d^{3} \vec{q}_{2} f\left(\vec{q}_{1}-\vec{q}_{2}\right)=V \int d^{3} \vec{q}_{12} f\left(\vec{q}_{12}\right) .$ Quite generally, we can set

$$
\lim _{V \rightarrow \infty} b_{\ell}=V b_{\ell}
$$

and the pressure is now obtained from

$$
\frac{P}{k T}=\sum_{\ell=1}^{\infty}\left(\frac{e^{\beta \mu}}{\lambda^{3}}\right)^{\ell} \frac{b_{\ell}}{\ell !}
$$

The linked cluster theorem ensures $\mathcal{G} \propto V$, since if any non-linked cluster had appeared in $\ln \mathcal{Q}$, it would have contributed a higher power of $V$.

Although an expansion for the gas pressure, eq.(V.27) is quite different from eq.(V.14) in that it involves powers of $e^{\beta \mu}$ rather than the density $n=N / V .$ This difference can be removed by solving for the density in terms of the chemical potential, using

$$
N=\frac{\partial \ln \mathcal{Q}}{\partial(\beta \mu)}=\sum_{\ell=1}^{\infty} \ell\left(\frac{e^{\beta \mu}}{\lambda^{3}}\right)^{\ell} \frac{V b_{\ell}}{\ell !}
$$

The equation of state can be obtained by eliminating the fugacity $x=e^{\beta \mu} / \lambda^{3}$, between the equations

$$
n=\sum_{\ell=1}^{\infty} \frac{x^{\ell}}{(\ell-1) !} \bar{\ell}_{\ell}, \quad \text { and } \quad \frac{P}{k T}=\sum_{\ell=1}^{\infty} \frac{x^{\ell}}{\ell !} b_{\ell}
$$

using the following steps:

(a) Solve for $x(n)$ from $\left(\bar{b}_{1}=\int d^{3} \vec{q} / V=1\right)$

$$
x=n-b_{2} x^{2}-\frac{b_{3}}{2} x^{3}-\cdots
$$

The perturbative solution at each order is obtained by substituting the solution at the previous order in eq.(V.30),

$$
\begin{aligned}
&x_{1}=n+\mathcal{O}\left(n^{2}\right) \\
&x_{2}=n-b_{2} n^{2}+\mathcal{O}\left(n^{3}\right) \\
&x_{3}=n-b_{2}\left(n-b_{2} n\right)^{2}-\frac{b_{3}}{2} n^{3}+\mathcal{O}\left(n^{4}\right)=n-b_{2} n^{2}+\left(2 b_{2}^{2}-\frac{b_{3}}{2}\right) n^{3}+\mathcal{O}\left(n^{4}\right)
\end{aligned}
$$

(b) Substitute the perturbative result for $x(n)$ into eq.(V.29), yielding

$$
\begin{aligned}
\beta P &=x+\frac{b_{2}}{2} x^{2}+\frac{b_{3}}{6} x^{3}+\cdots \\
&=n-b_{2} n^{2}+\left(2 b_{2}^{2}-\frac{5_{3}}{2}\right) n^{3}+\frac{b_{2}}{2} n^{2}-b_{2}^{2} n^{3}+\frac{b_{3}}{6} n^{3}+\cdots \\
&=n-\frac{b_{2}}{2} n^{2}+\left(b_{2}^{2}-\frac{b_{3}}{3}\right) n^{3}+\mathcal{O}\left(n^{4}\right)
\end{aligned}
$$

The final result is in the form of the virial expansion of eq.(V.14),

$$
\beta P=n+\sum_{\ell=2}^{\infty} B_{\ell}(T) n^{\ell}
$$

The first term in the series reproduces the ideal gas result. The next two corrections are

$$
B_{2}=-\frac{b_{2}}{2}=-\frac{1}{2} \int d^{3} \vec{q}\left(e^{-\beta \mathcal{V}(\vec{q})}-1\right)
$$

and

$$
\begin{aligned}
B_{3} &=b_{2}^{2}-\frac{b_{3}}{3} \\
&=\left(\int d^{3} \vec{q}\left(e^{-\beta \mathcal{V}(\vec{q})}-1\right)\right)^{2} \\
&-\frac{1}{3}\left[3 \int d^{3} \vec{q}_{12} d^{3} \vec{q}_{13} f\left(\vec{q}_{12}\right) f\left(\vec{q}_{13}\right)+\int d^{3} \vec{q}_{12} d^{3} \vec{q}_{13} f\left(\vec{q}_{12}\right) f\left(\vec{q}_{13}\right) f\left(\vec{q}_{12}-\vec{q}_{13}\right)\right] \\
&=-\frac{1}{3} \int d^{3} \vec{q}_{12} d^{3} \vec{q}_{13} f\left(\vec{q}_{12}\right) f\left(\vec{q}_{13}\right) f\left(\vec{q}_{12}-\vec{q}_{13}\right)
\end{aligned}
$$

The above example demonstrates the cancellation of the one particle reducible cluster that appears in $b_{3} .$ While all clusters (reducible or not) appear in the sum for $b_{\ell}$, as demonstrated in the previous section, only the one particle irreducible ones can appear in an expansion in powers of density. The final expression for the $\ell^{\text {th }}$ virial coefficient is

$$
B_{\ell}(T)=-\frac{(\ell-1)}{\ell !} d_{\ell}
$$

where $d_{\ell}$ is defined as the sum over all one-particle-irreducible clusters of $\ell$ points. Note that in terms of $d_{\ell}$, the partition function can be organized as

$$
\ln Z=\ln Z_{0}+V \sum_{\ell=2}^{\infty} \frac{n^{\ell}}{\ell !} d_{\ell}
$$

reproducing the above virial expansion from $\beta P=\partial \ln Z / \partial V$. MIT OpenCourseWare

http://ocw.mit.edu

\subsection{Statistical Mechanics I: Statistical Mechanics of Particles \\ Fall 2013}

For information about citing these materials or our Terms of Use, visit: http://ocw.mit.edu/terms.
