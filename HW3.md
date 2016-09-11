##Question 1A
\[
  \\
  \frac{dp}{dt} + \gamma p = \alpha - \alpha e^{-\mu t}
  \\
  u(t)\frac{dp}{dt} + u(t)\gamma p = u(t)(\alpha - \alpha e^{-\mu t})
\]
We then derive u(t)
\[
  u(t)\gamma = u'(t)
  \\
  \gamma = \frac{u'(t)}{u(t)}
  \\
  \gamma = (ln(u(t)))'
  \\
  ln(u(t)) = \int \gamma dt = \gamma t + C_2
  \\
  u(t) = e^{\gamma t + C_2}
\]
And substitute it in to a manipulated form:
\[
  u(t)\frac{dp}{dt}+u'(t)p = (u(t)p(t))'
  \\
  (u(t)p(t))' = u(t)(\alpha - \alpha e^{-\mu t})
  \\
  u(t)p(t) + C_1 = \int u(t)(\alpha - \alpha e^{-\mu t})dt
  \\
  p(t) = \frac
  {\int u(t)(\alpha - \alpha e^{-\mu t})dt - C_1}
  {u(t)}
  \\
  p(t) = \frac
  {\gamma^{-1} \alpha e^{\gamma t + C_2} - \int \alpha e^{-\mu t} e^{\gamma t + C_2}dt - C_1}
  {e^{\gamma t + C_2}}
  \\
  \int \alpha e^{-\mu t} e^{\gamma t + C_2}dt = \frac{\alpha e^{t(\gamma - \mu) + C_2}}
  {\gamma - \mu}
  \\
  p(t) = \frac{\alpha \gamma e^{\gamma t + C_2} - \frac{\alpha e^{t(\gamma - \mu) + C_2}}
  {\gamma - \mu}- C_1}
  {e^{\gamma t + C_2}}
  \\
  p(t) = \alpha \gamma - \frac{\alpha e^{- \mu t}}
  {\gamma - \mu} - e^{-\gamma t + C_3}
\]
When t=0 then p(t)=0:
\[
  p(0) = 0 = \alpha\gamma - \frac{\alpha}{\gamma - \mu} - e^{C_3}
  \\
  C_3 = ln(\alpha\gamma - \frac{\alpha}{\gamma - \mu})
\]
Therefore:
\[
  p(t) = \alpha \gamma - \frac{a^{-\mu t}}{\gamma - \mu} - e^{-\gamma t} (\alpha\gamma - \frac{\alpha}{\gamma - \mu})
  \\
  p(t) = \alpha \gamma (1 - e^{-\gamma t} )- \frac{a^{-\mu t}}{\gamma - \mu}  - \frac{\alpha}{\gamma - \mu}e^{-\gamma t}
\]
When \(\mu = \gamma\) then:
\[
  p(t) = \alpha \gamma - \frac{a^{-\mu t}}{\gamma - \mu ln(\alpha)}
\]
