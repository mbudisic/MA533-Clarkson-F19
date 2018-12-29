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

#### Participation

Participation and attendance will be an integral and important part of the grade. I will assign structured readings _ahead_ of each block of material and I will expect you to complete it _before_ we discuss the topic in class.

During class, I will minimize lecturing, and instead I will ask students/pairs of students to work through/discuss/practice problems on the board.

I will make sure that everyone has a chance to work on the board, and also keep track of your participation.

#### Homeworks

Homework will be completed using the CoCalc system. While the basic use of CoCalc is free, for a one-time fee of \$14, you will get priority access to resources provided by CoCalc. This is roughly equivalent to buying a cup of coffee per homework.**I strongly encourage you to purchase this access for the course.** If you would like to purchase the course access, but absolutely cannot afford it, please come see me and we'll come up with the money.

For homeworks, you'll have a freedom to work in any of the three PyJuMa languages. If you are skilled in either of them, I encourage you to try to branch out, and attempt to use one of the other two languages during the course.

Homeworks will be collected roughly bi-weekly. Before I grade your work, you will also be required to grade the homework of one of your peers, so everyone can get some experience in reading code, and get feedback before the work is graded.

#### Projects

There will be two projects during the course.

The first project will consist in reading an article on numerical methods for DEs and presenting to class on it.

The second project will likewise be associated with reading an article, but you will need to provide an implementation of the technique in addition to just discussing the result.

In both cases, I will give some suggestions for papers to read, but you'll be welcome to choose your own article. In either situation, you'll first discuss the "project proposal" with me, discussing why and how you'd approach the topic of your choice, before working on the article.

#### Exams

There will be two exams and a final. I still haven't  decided if they will be take-home (24hr window) or in-class exams. They will primarily focus on definitions, and proof-writing.

## Assessment

I will discuss how grade will be assigned in the first week of class.

## Accommodations

I will do my best to arrange for any necessary accommodations that would enable you to fully participate in this class. If you require assistance during the lectures or during exams, please register with the [AccessABILITY Services](https://www.clarkson.edu/accessability-services).

**Parents:** I know that many of our graduate students juggle their graduate school with being a good and present parent for their children. If you need to bring your child to work with you during a snow day, they're welcome to sit in class and play while we work (providing they're not too loud). If you need any other arrangements made, please consult me - I am open to suggestions and will honor them, as long as they don't derail objectives (and objectivity) of the class.

## Ethical Behavior

From the Student Manual: _The Clarkson student will
not present, as his or her own, the work of another,
or any work that has not been honestly performed,
will not take any examination by improper means,
and will not aid and abet another in any dishonesty.
Failure to adhere to this code will mean a failing
grade and a report to the Dean of Students._

**Since this is a graduate class, I will be exceptionally strict regarding (un)ethical behavior.** I understand that different universities, professions, countries have different standard for ethical behavior. If you are not sure how to collaborate with your classmates in an ethical fashion, or how to use online resources, please consult me - there is no shame in asking.

In particular, your homeworks, midterms, or finals may be unsupervised, or take-home exams. During those exams, it will be incumbent upon your honor to use only allowed tools/notes, and not discuss the material with anyone else until you (and they) turn the work in.

## Additional Resources

#### Online programming resources

* Julia: <https://youtu.be/4igzy3bGVkQ>
* Python3: <https://www.datacamp.com/courses/intro-to-python-for-data-science>
* Matlab: <https://matlabacademy.mathworks.com/>
* General skills: <https://software-carpentry.org/lessons/>
* Jupyter/IPython notebooks: <https://www.dataquest.io/blog/jupyter-notebook-tutorial/>

#### Reference books

Students nowadays try to find help on programming by furiously googling for clues. This can take you some distance, but having a good (printed) reference book is invaluable.

H.P.Langtangen is a master, anything he wrote is good, but I especially recommend:
  * [his general scientific computing book](https://hplgit.github.io/prog4comp/index.html)
  * [his numerical DEs book, focusing more on implementation than theory](http://hplgit.github.io/decay-book/doc/pub/book/html/decay-book.html)

#### Journal articles

* Lamport, L. [_How to Write a 21st Century Proof_](./pdfs/lamport2012.pdf) Journal of Fixed Point Theory and Applications 11, no. 1 (2012): 43–63. doi:10.1007/s11784-012-0071-6
*  Wilson, G., et al. [_Best Practices for Scientific Computing_](./pdfs/wilson2014.pdf) PLoS Biol 12, no. 1 (2014): e1001745. doi:10.1371/journal.pbio.1001745

{% include_relative abbrevs.md %}
