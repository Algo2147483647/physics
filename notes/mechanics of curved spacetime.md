# Mechanics of curved spacetime

[TOC]

## Curved spacetime: differential geometry

### Metric & Metric tensor

A **metric** is a function that defines the distance between two points in a given space.

A **metric tensor** is a mathematical object that encodes the information about the metric of a space. It is a type of tensor that describes how distances are measured, taking into account both the curvature of space and the coordinate system in use. For a space with coordinates $x^1, x^2, \dots, x^n$, the metric tensor $g_{\mu \nu}$ is a symmetric matrix whose components define the inner product of the differential position vectors in the space. In local coordinates, the differential of distance squared (the square of the infinitesimal length) is written as:
$$
ds^2 = g_{\mu \nu} dx^\mu dx^\nu
$$


### Christoffel symbol
$$
\Gamma^{\lambda}_{\mu\nu} = \frac{1}{2} g^{\lambda\sigma} (\partial_{\mu}g_{\nu\sigma} + \partial_{\nu}g_{\mu\sigma} - \partial_{\sigma}g_{\mu\nu})
$$

The Christoffel symbols represent the connection coefficients that describe how the coordinate basis vectors change from point to point in a curved space or spacetime. The Christoffel symbols provide a way to compute how vectors change when they are parallel transported along a curve in a curved space or spacetime. They are not tensors themselves but are used to construct tensors.


### Geodesic & Geodesic equation
$$
\frac{d^2 x^\mu}{d\lambda^2} + \Gamma^{\mu}_{\alpha\beta} \frac{dx^\alpha}{d\lambda} \frac{dx^\beta}{d\lambda} = 0
$$

Geodesic equation describes free-falling objects follow the straightest possible paths (geodesics) in curved spacetime.

## Action

### Action of Gravitational field

$$
S=-\frac{1}{c}\int L_m \sqrt{-g} d^4x + \frac{c^3}{16\pi G}\int R\sqrt{-g} d^4x
$$


$$
\begin{align*}
S &= S_m + S_g  \\
S_m &= -\frac{1}{c}\int L_m \sqrt{-g} d^4x \tag{matter action}\\
S_g &= \frac{c^3}{16\pi G}\int R\sqrt{-g} d^4x \tag{gravitational action}
\end{align*}
$$



$$
\frac{\delta S}{\delta g_{\mu\nu}} = 0
$$



### Einstein gravitational field equation

$$
G_{\mu\nu} = \frac{8\pi G}{c^4} T_{\mu\nu}
$$

爱因斯坦-希尔伯特动作：
$$
S = \int d^4x \sqrt{-g} \left( \frac{R}{16\pi G} + \mathcal{L}_M \right)
$$
