---
title: Project
layout: default
---

## Due Date ##

The due date is Monday, December 11th 2017 at 9:00 AM.  We will have group 
presentations on that day.

## Course Project:  Overview

**The Goal**

You will develop a software library for a client (the teaching staff).  
The development of this library will leverage modern software development 
practices covered in the course.  Ultimately, at the end of the semester, 
the client should be able to easily install and run your package with 
little to no difficulty.

**The Topic**

You are asked to write a chemical kinetics library.  The ultimate goal is 
to return the right-hand-side of an ODE.  You do not need to solve the ODE! 
The idea is that the client will just call your package to provide the 
right-hand-side and use that right-hand-side in any way they wish.  They might 
want to use it as the righ-hand-side of the ODE, or they might want to use it 
in a neural net code to learn new reaction pathways.  Those details don't 
matter to you at the moment.

Of course, there are details in the right-hand-side function and we will 
cover these as needed.  **Note:  You are not expected to become and expert 
in chemical kinetics!  You will not be assessed on your chemical kinetics 
knowledge.**  I will teach you the basics of chemical kinetics so that you 
can implement the details into your library.

## Expectations 

The client should be able to easily install the library, run the tests, 
access the documentation, and use the library for their application.

You are required to add a non-trivial feature to your library of your choosing.  
If you are having difficulty coming up with a compelling new feature, please 
set up an appointment with me to discuss possible ideas.  The teaching staff 
will be able to give you a few suggestions if need be.  Since the in-class 
midterm demos will take place on October 18th, you should have an idea for your 
feature by October 11th.  You do not need to have your feature implemented, but 
you should have a high-level plan on how you will go about the implementation.

Documentation for every subsystem in the project should be provided. Link to the 
docs from the ``README.md`` in each folder. The top level ``README.md`` should 
contain an overview, links to other docs, and an installation guide which will help 
us install and test your system.

For those parts of the project which are modules, ``python setup.py test`` should 
suffice. For all other parts, include instructions on how to test your code. Where 
possible, provide links to Travis-CI test runs and Coveralls coverage.

## Deliverables

**Milestones**

There will be two project milestones.  The first will take place on 10/18 and the 
second on 11/20.  Each milestone will be in the form of a code review session 
during class.  Each group will sit down with members of the teaching staff and 
have their code and documentation reviewed.  The teaching staff will provide 
feedback on the code and make sure that each group is on track.  The code review 
session for each group will take roughly 10 minutes.

You should also turn in a document which describes the code, how to install it, how 
to run the tests, and how a user can run it.  The end of the document should include 
your proposed feature for the final project.  The document should be under version 
control.  This means that you should not write it in Microsoft word!  Markdown is a 
 nice way to document your code.

Finally, your library should be up to date with where we are in class.  We will be 
adding features to the library weekly, so as long as you are attending class and 
doing the assignments you should have no problem having the latest features in 
your library.  I will describe the exact details of what we expect to see in your 
library one week before the code review sessions.  This will give you a way to benchmark 
your progress and make sure you're progressing satisfactorily before the code review 
session.

### Milestone 1

The first project milestone will take place in class on October 18th.  You should 
provide a tour through your code base and show a few examples.  The teaching staff 
will try an example of their own.  The rubric for the first milestone is on the 
course webpage under the `project` directory.

### Milestone 2

The second project milestone will take place in class on November 20th.  The main 
difference between the first and second milestone is that the second milestone 
will contain additional code features and that each group must propose a nontrivial 
feature to add to their code.  The teaching staff will assess the feasibility of 
the code feature and may offer suggestions on how to proceed.  Once again, a 
rubric for the second milestone will be made available on the course webpage 
under the `project` directory.

**Final**

The deliverables for the final are essentially the same as those for the milestones.  
Of course, the main difference is that the final will include the final version 
of your product inclusive of your proposed feature.  You will have to 
demo your library to the class and provide documentation.  The teach staff will 
attempt to install your library and use it for our own purposes.

The final presentation will occur on Monday, December 11th.  This presentation will 
be a demo of your entire library.  The final deliverable will be in the form of 
documentation of your library including instructions on how to install, run the tests, 
and examples for new users.

## Assessment

The final project is worth 50% of your course grade.  Here is a breakdown of the 
components of the project:

* Milestone 1 (10/18):  10%
  * Model Document:  12.5%
  * Code Documentation:  12.5%
  * Input Parsing:  12.5%
  * Code Base:  50%
  * Test Suite:  12.5%
* Milestone 2 (11/20):  10%
  * Packaging and Installation: 30% 
  * Reversible Reactions:  40%
  * Proposed Feature:  30%
* Final deliverables:  30%
  * Presentation:  10%
  * Document:  40%
  * Library:  50%

