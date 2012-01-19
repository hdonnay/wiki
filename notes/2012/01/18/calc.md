#Integration by parts
[[!toc startlevel=2]]
[[!tag notes/1272]]

##General form

$$
\int\!u\ dv = uv - \int\!v\ du
$$

##Integration examples

- - -

Find $\int \! x \! \cos x \, \mathrm{d} x$ :

###Bad example:

$$
\begin{gather}
u = \cos x \qquad  dv = x \ dx \\
du = -\sin x \ dx \qquad  v = {x^2 \over 2}\\
\\
{x^2 \over 2} \cos x + \int\! \sin x {x^2 \over 2} \ dx
\end{gather}
$$

Worse than the initial problem, we now have a fraction and an exponent
in the integral.


###Good example:

$$
\begin{gather}
u = x   \qquad v = \cos x \ dx \\
du = dx \qquad v = \sin x \\
\\
x \sin x - \int\! \sin x \ dx\\
\boxed{x\sin x + \cos x + C}
\end{gather}
$$

No Integral!

- - -

Find $\int\! \ln x \ dx$:

$$
\begin{gather}
u = \ln x         \qquad dv = dx\\
du = { 1 \over x} \qquad v=x\\
\\
\begin{aligned}
x\ln x &- \int\! x ({1 \over x})\ dx\\
&- \int\! 1\ dx\\
\end{aligned}\\
\boxed{x\ \ln x - x + C}
\end{gather}
$$

- - -

Find $\int\!t^2e^{-t}\ dt$:

$$
\begin{gather}
u=t^2 \qquad dv=e^{-t}\ dt\\
du=2t\ dt \qquad v=-e^{-t}\\
\\
\begin{align}
-t^2e^{-t} + &2\int\! te^{-t}\ dt\\
&\begin{gather}
u=t \qquad dv=e^{-t}\\
du=dt \qquad v=e^{-t}\\
\end{gather}
\\
&-te^{-t}+\int\!e^{-t}\\
&\boxed{-te^{-t}-e^{-t}}\\
\\
-t^2e^{-t} + &2(-te^{-t}-e^{-t})\\
-t^2e^{-t} + &-2te^{-t}-2e^{-t}\\
\end{align}
\\ \\
\boxed{e^{-t}(-t^2-2t-2)+C}
\end{gather}
$$

- - -

Find $\int_1^3 r^3 \ln r\ dr$:

$$
\begin{gather}
u=\ln r \qquad dv=r^3 \ dr\\
du={1 \over r}\ dr \qquad v={r^4 \over 4}\\
\\
{r^4 \over 4} (\ln r) - \int_1^3 {r^3 \over 4}\ dr\\
{r^4 \ln r \over 4} - {r^4 \over 16}\vert_1^3\\
\end{gather}
$$
