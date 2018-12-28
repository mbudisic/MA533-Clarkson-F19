---
title: 'MA571: Numerical Solutions of Differential Equations'
layout: default
published: true
---

**Welcome to MA571!**

Say that you have an ODE system to solve in order to generate a cool video as on Wikipedia's website:
![](https://upload.wikimedia.org/wikipedia/commons/1/13/A_Trajectory_Through_Phase_Space_in_a_Lorenz_Attractor.gif)

OK, so you learn that this is a [Lorenz system](https://en.wikipedia.org/wiki/Lorenz_system) whose equations are

$$\dot x = \sigma(y-x)\,\ \dot y = x(\rho - z) - y,\ \dot z = xy - \beta z$$

where $$\rho = 28,\ \sigma = 10, \beta = 8/3$$. 

Hm, solving those was not covered in your ODE class, but look at that, Wikipedia even has code available.

```
sigma = 10;
beta = 8/3;
rho = 28;
f = @(t,a) [-sigma*a(1) + sigma*a(2); rho*a(1) - a(2) - a(1)*a(3); -beta*a(3) + a(1)*a(2)];
[t,a] = ode45(f,[0 100],[1 1 1]);     % Runge-Kutta 4th/5th order ODE solver
plot3(a(:,1),a(:,2),a(:,3))

```

[Let's try it out](https://nbviewer.jupyter.org/github/mbudisic/MA571-Clarkson-S19/blob/gh-pages/materials/wikipedia-lorenz.ipynb)
![wikipedia-lorenz.png]({{site.baseurl}}/wikipedia-lorenz.png)

Close enough, but what's up with that jagged edge! Ah, that's right, this is a _numerical approximation_, so perhaps if we reduce the stepsize, we'd get a better result. Let's check the help:

[help for ode45](https://octave.sourceforge.io/octave/function/ode45.html)

What's all of this???? What's Dormand-Prince, what's Runge-Kutta, wait, there's something called adaptive timestep, and I set it using "relative and absolute tolerance"! Tolerance to WHAT. 

**Breathe.** After taking MA571 you'll be able to work through all these things. And more. You'll have a sense of how to integrate Partial Differential Equations, perhaps learn something about Stochastic Differential Equations. Sort out why there are so many options to choose from if you decide to use something instead of `ode45`.

**Our goal** will be to get enough knowledge to make the best choice when solving a specific differential equation, and provide foundation for further study. Sometimes, we'll code things up, just to get our hands dirty, and sometimes we'll do proofs. We'll also read journal articles and present on them, to see how these topics behave in research context.

## Basic course info

* Instructor: **Marko Budisic** <marko@clarkson.edu>
* Office: **Science Center 391**
* Meetings: **MoWeFr 2pm-2.50pm** in **SC342** (attendance is mandatory)
* Textbook: _Arieh **Iserles_**, A First Course in the Numerical Analysis of Differential Equations (Cambridge), **2nd Edition** (any format is fine)
* Homeworks will be assigned and collected on <https://cocalc.com/app> -- no exceptions. You'll have the freedom of working in Python, Julia, or Matlab/Octave. The analytical components will be typeset in either LaTeX or Markdown.
