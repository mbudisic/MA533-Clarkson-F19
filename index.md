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

Let's try it out.



We will attempt to strike a balance between computational aspects (writing computer programs) and analysis aspects (proving, analyzing, comparing). The main audience for this class are graduate students in mathematics. However, engineers and scientists may also benefit from this content.

## Basic course info

* Instructor: **Marko Budisic** <marko@clarkson.edu>
* Office: **Science Center 391**
* Meetings: **MoWeFr 2pm-2.50pm** in **SC342** (attendance is mandatory)
* Textbook: _Arieh **Iserles_**, A First Course in the Numerical Analysis of Differential Equations (Cambridge), **2nd Edition** (any format is fine)
* Homeworks will be assigned and collected on <https://cocalc.com/app> -- no exceptions. You'll have the freedom of working in Python, Julia, or Matlab/Octave. The analytical components will be typeset in either LaTeX or Markdown.
