---
title: MA571 Syllabus
description: 'Numerical Solutions to Differential Equations in Spring 2019 as taught by Marko Budišić'
---
{::options toc_levels="1..2" /}

1. TOC
{: toc style="font-size:10pt; column-count:3; column-width: 20px; column-gap: 20px;" }

## Learning Objectives

* gain experience in analyzing numerical algorithms according to order, stability, and convergence (including proving that algorithms do/don't satisfy a criterion)
* assessing which algorithm is a good fit for a problem at hand
* ability to interpret and decypher descriptions of numerical algorithms for DEs in one of the three programming languages PyJuMa
* ability to implement (code) basic numerical algorithms for a variety of DEs, and grapple with complexities/difficulties of implementation
* ability to read and interpret research articles in numerical algorithms for DEs

## Topics and textbook

The course will be split between topics in numerical solutions of ODEs and PDEs:

* 1st order ODE schemes with overview of main desirable properties of numerical schemes
* multistep ODE methods
* Runge-Kutta ODE methods
* stiffness and adaptive timestepping
* canonical PDE BVP: Poisson Equation $$\Delta u = f$$.
  * finite difference schemes
  * finite element schemes
  * spectral methods
* canonical PDE Initial Value Problems
  * parabolic case (heat and diffusion) $$\partial_t u = \Delta u$$
  * hyperbolic case (advection, wave, nonlinear) $$\partial_t u = \partial_x u $$, $$\partial_{tt} u = \Delta u$$

These topics roughly correspond to chapters 1-4, 6, 8-10, 16-17 in the textbook by **Arieh Iserles, _A First Course in the Numerical Analysis of Differential Equations_ (Cambridge), 2nd Ed.**

**Regular and frequent access to textbook is mandatory.** Any format of the textbook is fine (ebook, hardcopy, borrowed, owned), but don't count that "sharing a textbook" and occassionally looking at it will be enough. First edition of the textbook is missing the chapter on spectral methods, and it may have different exercises. If you choose to use the first edition, you have to make sure to check with a colleague that your assigments are current.

## Prerequisites

Undergraduate level multivariate calculus, differential equations (ODEs and PDEs), ability to code in either PyJuMa. An excellent catch-all reference book is [Kreyszig's Advanced Engineering Mathematics](https://www.goodreads.com/book/show/1426461.Advanced_Engineering_Mathematics) (any fairly-recent edition).

You will not do well in this class if you've never used a programming language independently. If you think you need to brush up on your programming skills, take the time ahead of the class to practice.

## Course work

##### Participation

##### Homeworks

Homework will be collected roughly bi-weekly. Before I (Marko) grade your homework, you'll also be required to grade a homework for a randomly-assigned classmate.


##### Projects

##### Exams



## Assessment

TBA

## Accommodations

## Ethical Behavior

## Additional Resources

##### Online programming resources

* Julia: <https://youtu.be/4igzy3bGVkQ>
* Python3: <https://www.datacamp.com/courses/intro-to-python-for-data-science>
* Matlab: <https://matlabacademy.mathworks.com/>
* General skills: <https://software-carpentry.org/lessons/>
* Jupyter/IPython notebooks: <https://www.dataquest.io/blog/jupyter-notebook-tutorial/>

##### Reference books

Students nowadays try to find help on programming by furiously googling for clues. This can take you some distance, but having a good (printed) reference book is invaluable.

H.P.Langtangen is a master, anything he wrote is good, but I especially recommend:
  * [his general scientific computing book](https://hplgit.github.io/prog4comp/index.html)
  * [his numerical DEs book, focusing more on implementation than theory](http://hplgit.github.io/decay-book/doc/pub/book/html/decay-book.html)

##### Journal articles

* Lamport, L. [_How to Write a 21st Century Proof_](./pdfs/lamport2012.pdf) Journal of Fixed Point Theory and Applications 11, no. 1 (2012): 43–63. doi:10.1007/s11784-012-0071-6
*  Wilson, G., et al. [_Best Practices for Scientific Computing_](./pdfs/wilson2014.pdf) PLoS Biol 12, no. 1 (2014): e1001745. doi:10.1371/journal.pbio.1001745

{% include_relative abbrevs.md %}
