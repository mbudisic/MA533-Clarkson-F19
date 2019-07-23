---
title: 'MA533: Ordinary Differential Equations'
description: 'Instructor: Dr. Marko Budišić (SC391) &mdash; <a href="mailto:marko@clarkson.edu">marko@clarkson.edu</a> &mdash; MoWeFr 3-3.50p  (SC340) &mdash; Text: Meiss, Revised ed.'
layout: default
published: true
---

**Welcome to MA533!** So what's this class about?


Differential equations are the most common mathematical framework for modeling time-changing phenomena arising in various physical sciences. Differential equations couple variables with their derivatives. _Ordinary_ differential equations are those in which only one independent variable (e.g., time, one spatial direction) is used to take the derivative of (one or more) dependent variables. 

There are other classes of differential equations: PDEs, SDEs, DAEs, etc. Does this mean ODEs are somehow boring? Not at all! If many variables (quantities of interest) are coupled, or if those couplings are nonlinear, the resulting behavior can be very rich, indeed, it can appear to be noise-like ("chaotic") even though no randomness is involved.

![](https://rogueplanet.tv/wp-content/uploads/2014/09/jurassic-park-jeff-goldblum-tyrannosaur.jpg){: style="float: left;margin-left: 7px;margin-top: 7px;" width="20%"}

<iframe width="20%" src="https://www.youtube.com/embed/n-mpifTiPV4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Those of you who have seen the original Jurassic Park movie may remember the edgy character of Ian Malcolm (played by Jeff Goldblum) who [describes the "chaos theory" to his paleobotanist colleague](https://youtu.be/n-mpifTiPV4). Well, the name "chaos theory" is really a popular-writing name for the theory of nonlinear dynamics, out of which nonlinear ODEs are typically the primary topic to be encountered by students. In this class, we will encounter such things as the "butterfly effect", the "[Lorenz system](https://en.wikipedia.org/wiki/Lorenz_system)":
![](https://upload.wikimedia.org/wikipedia/commons/1/13/A_Trajectory_Through_Phase_Space_in_a_Lorenz_Attractor.gif){: style="float: right;margin-right: 7px;margin-top: 7px;" width="20%"}

The main topic of this class are low-dimensional, nonlinear ODEs, such as equations for the system above:

$$\begin{aligned}
\dot x &= \sigma(y-x)\\
\dot y &= x(\rho - z) - y \\
\dot z &= xy - \beta z \\
\end{aligned}$$
where $$\rho = 28,\ \sigma = 10, \beta = 8/3$$.

In this  setting, we will formulate the theory that specifies when the equations give plausible models for nature ("existence and uniqueness of solutions"). In contrast with undergraduate ODE classes, which mostly focus on different techniques for _solving_ ODEs, we will deal with equations that typically cannot be solved by analytic techniques. Instead, we will learn about tools that allow us to characterize what resulting solutions ("trajectories") look like without finding formulas for them (so-called _qualitative analysis_). The crucial property we will analyze, after assuring that solutions exist, will be stability -- notion that some solutions may attract or repell nearby solutions, and so organize the overall behavior of all solutions.

If you just cannot wait for the class to start reading about this exciting area of math, I suggest you [pick up the book by James Gleick](https://www.goodreads.com/book/show/64582.Chaos) that initially got me interested in this field (when I was a 1st year undergraduate).

---

{% include_relative abbrevs.md %}
