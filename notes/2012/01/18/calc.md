#Integration by parts

[[!toc startlevel=2]]
[[!tag notes/1272]]

##General form

$$
\int\!u\ dv = uv - \int\!v\ du
$$

##Integration examples

Find $\int \! x \! \cos x \, \mathrm{d} x$ :

*Bad example:*

$$
\begin{aligned}
\boxed{u = \cos x        \qquad  dv = x \ dx \\
du = -\sin x \ dx \qquad  v = {x^2 \over 2}\\}
\\
{x^2 \over 2} \cos x + \int\! \sin x {x^2 \over 2} \ dx
\end{aligned}
$$

Worse than the initial problem, we now have a fraction and an exponent
in the integral.

- - -

*Good example:*

$$
\begin{aligned}
\boxed{u = x   \qquad v = \cos x \ dx \\
du = dx \qquad v = \sin x \\}
\\
x \sin x - \int\! \sin x \ dx\\
\boxed{x\sin x + \cos x + C}
\end{aligned}
$$

No Integral!

- - - 

Find $\int\! \ln x \ dx$:
$$
\begin{aligned}
\boxed{
u = \ln x         \qquad dv = dx\\
du = { 1 \over x} \qquad v=x\\
}\\
