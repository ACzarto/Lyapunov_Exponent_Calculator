# Lyapunov_Exponent_Calculator
This repository contains a function to compute the Lyapunov coefficient, which is used as a measure of chaotic behavior, based on the Lorenz Attractor.


The Lorenz System is a set of three coupled, non-linear ordinary differential equations (ODEs) that simplified the mathematical modeling of atmospheric convection. Developed by Edward Lorenz, this system became famous for demonstrating the butterfly effect, where minor perturbations in initial states lead to vastly different outcomes and for generating the iconic, butterfly-shaped Lorenz strange attractor.

The system of equations is

$$
\begin{align}
    \frac{dx}{dt} &= \sigma(y - x) \\
    \frac{dy}{dt} &= x(\rho - z) - y \\
    \frac{dz}{dt} &= xy - \beta z
\end{align}
$$

where $\sigma$, $\rho$, and $\beta$ are dimensionless parameters representing the Prandtl number, the Rayleigh number, and the geometric physical dimensions of the layer, respectively.

The goal of our algorithm is to compute the so-called Lyapunov Exponent, given by:

$$\lambda_{\max} = \lim_{t \to \infty} \lim_{d_0 \to 0} \frac{1}{t} \ln \left( \frac{d(t)}{d_0} \right)$$

For the function it will be used the Oseledets Method that uses the Jacobian Matrix and in the case of the Lorentz Atractor, we will have 3 Lyapunov Exponents.


