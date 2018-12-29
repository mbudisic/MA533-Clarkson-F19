---
title: 'MA571: Numerical Solutions of Differential Equations'
description: 'Instructor: Dr. Marko Budišić (SC391) &mdash; <a href="mailto:marko@clarkson.edu">marko@clarkson.edu</a> &mdash; MoWeFr 2-2.50p  (SC342) &mdash; Text: Iserles, 2nd ed.'
layout: default
published: true
---

**Welcome to MA571!** So what's this class about?

Say that you have an ODE system to solve in order to generate a cool video of the [Lorenz system](https://en.wikipedia.org/wiki/Lorenz_system) as on Wikipedia's website.
![](https://upload.wikimedia.org/wikipedia/commons/1/13/A_Trajectory_Through_Phase_Space_in_a_Lorenz_Attractor.gif){: style="float: right;margin-right: 7px;margin-top: 7px;" width="20%"}

OK, so you learn that this is an ODE system whose equations are

$$\begin{aligned}
\dot x &= \sigma(y-x)\\
\dot y &= x(\rho - z) - y \\
\dot z &= xy - \beta z \\
\end{aligned}$$

where $$\rho = 28,\ \sigma = 10, \beta = 8/3$$.


Hm, solving those was not covered in your ODE class, but look at that, Wikipedia even has code available. [Let's try it out.](https://nbviewer.jupyter.org/github/mbudisic/MA571-Clarkson-S19/blob/gh-pages/materials/wikipedia-lorenz.ipynb)

![./img/wikipedia-lorenz.png]({{site.baseurl}}/img/wikipedia-lorenz.png){:width="50%" style="float: right;margin-right: 7px;margin-top: 7px;"}
```matlab
sigma = 10;
beta = 8/3;
rho = 28;
f = @(t,a) [...
    -sigma*a(1) + sigma*a(2); ...
    rho*a(1) - a(2) - a(1)*a(3); ...
    -beta*a(3) + a(1)*a(2)];
[t,a] = ode45(f,[0 100],[1 1 1]); % Runge-Kutta 4th/5th order ODE solver
plot3(a(:,1),a(:,2),a(:,3))
```

 Close enough, but what's up with that jagged edge! Ah, that's right, this is a _numerical approximation_, so perhaps if we reduce the stepsize, we'd get a better result. How do I do that?  [Let's check help for ode45.](https://octave.sourceforge.io/octave/function/ode45.html)

![./img/ode45-help.png]({{site.baseurl}}/img/ode45-help.png){:style="border:1px solid" width="75%"}

**What's all of this???? What's Dormand-Prince, what's Runge-Kutta, wait, there's something called adaptive timestep, and I set it using "relative and absolute tolerance"! Tolerance to WHAT.**

_You decide that it must be Matlab's implementation of this technique that is arcane. Let's check other techniques/languages: [Matlab](https://www.mathworks.com/help/matlab/math/choose-an-ode-solver.html), Python [scipy.integrate.ode](https://docs.scipy.org/doc/scipy-0.14.0/reference/generated/scipy.integrate.ode.html), and Julia [DifferentialEquations.jl](http://docs.juliadiffeq.org/latest/solvers/ode_solve.html#Recommended-Methods-1). No help. You feel the walls closing in._

**Breathe.** After taking MA571 you'll be able to work through all these things. And more. You'll have a sense of how to integrate Partial Differential Equations, perhaps learn something about Stochastic Differential Equations. Sort out why there are so many options to choose from if you decide to use something instead of `ode45`.

---

Our goal will be to get enough knowledge to make the best choice when solving a specific differential equation, and provide foundation for further study. Sometimes, we'll code things up, just to get our hands dirty, and sometimes we'll do proofs. We'll also read journal articles and present on them, to see how these topics behave in research context.

---
