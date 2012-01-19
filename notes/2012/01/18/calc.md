#Integration by parts

[[!toc startlevel=2]]
[[!tag notes/1272]]

##Integration examples

Find $\int \! x \! \cos x \, \mathrm{d} x$ :

*Bad example:*

$\begin{aligned}
u = \cos x \qquad                           \mathrm{d}v = x \!\mathrm{d}x \\
\mathrm{d}u = -\sin x \!\mathrm{d}x \qquad  v = {x^2 \over 2}\\
\\
{x^2 \over 2} \cos x + \int\! \sin x {x^2 \over 2} \mathrm{d}x
\end{aligned}$

Worse than the initial problem, we now have a fraction and an exponent
in the integral.

*Good example:*

\[
\begin{aligned}
u \eq x \qquad \mathrm{d}v \eq \cos x \!\mathrm{d}x\\
\mathrm{d}u \eq \mathrm{d}x \qquad v \eq \sin x\\
\\
x \sin x - \int\! \sin x \mathrm{d}x
\mbox{x\sin x + \cos x + C}
\]
