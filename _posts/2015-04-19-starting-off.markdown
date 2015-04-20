---
layout: post
title:  "Cracking it open: Chapter 0"
date:   2015-04-19 21:28:17
categories: [intro, motivation] 
---
The following covers pages 1 - 6
##0: Overture

#0.1: What is quantum field theory

We start off the text with the simple but profound idea:

>Every particle and every wave in the Universe is simply an excitation of a quantum field that is defined over all space and time.

The initial motivation for doing QFT points out a lot of the successes of QED (a kind of QFT) and other related theories.

>Interactions in QFT involve products of operators which are found to create and annihilate particles and so interactions correspond to processes in which particles are created or annihilated; hence there is also the possibility of creating and destroying virtual particles which medite forces.

This statement seems like an excellent summary of the general philosophy of QFT.



#0.2 What is a field?
A field is a machine that takes as an input a spacetime position, and outputs a scalar, vector or higher order amplitude of some kind related to that position. The field can vary as spacetime varies also.

There is an awkward run-on sentence here about Kepler and Newton, but the main idea isn't lost.

Gravity and electromagnetism are fields, and each has a set of equations to show how they behave. In the case of E&M, the field oscillates in space and time, so we find wave-like excitations of the field. [LIGO](http://www.ligo.caltech.edu/) is still keeping it's eyes open for gravity waves. 


#0.3 Who is this book for?
Well hopefully this book is for me, since I already have it... I don't plan to do much QFT, but I do want to be able to understand it.


#0.4 Special Relativity
Special relativity states that *c* is the same in all inertial frames. It implies that the (spacetime) coordinates of an event $$S$$ should be related to $$\overline{S}$$ by a [Lorentz Transformation](http://en.wikipedia.org/wiki/Lorentz_transformation#Boost_in_the_x-direction). They list the bost along the x-axis in the book, but of course we would expect it to be true more generally.

A theory is *covariant* when it transforms sensibly under coordinate transformations. A quantity is *Lorentz covariant* if it transforms according to the [Lorentz group](http://en.wikipedia.org/wiki/Lorentz_group). This statement doesn't feel all that meaningful to me. I remember from group theory that the Lorentz group is SO(1,3) which is something like SO(4). So presumably, if a theory can be a representation of SO(1,3), it satisfies the Lorentz group, and is Lorentz covariant.

From here the authors discuss the transformation of scalars, vectors, etc. These are the things that a field can consist of, so it is reasonable to think that we might look at them here.

* *Scalars* - scalars look the same from every intertial reference frame. Everyone agrees that they get the same measurement of a scalar from their own Frame of Reference.
* *Vectors* - A vector has a scalar length, so the magnitude of a vector is invariant. The direction it appears to point will vary by observer.


A generic way of talking about a coordinate transformation between two inertial reference frames is to think of it as a map $$ \{x^{\mu}\} \rightarrow \{\overline{x}^{\mu}\}$$. This map would transform a vector $$a^{\mu}$$ as


$$
\begin{equation}
\overline{a}^{\mu} = \left( \frac{\partial \overline{x}^{\mu}}{\partial x^{\nu}} \right) a^{\nu}  = \sum_{\nu=0}^{3}\left( \frac{\partial \overline{x}^{\mu}}{\partial x^{\nu}} \right) a^{\nu}
\end{equation}
$$

This should be pretty straight forward to understand. Note in particular that the indices change, and that we're using [Einstein Summation notation](http://en.wikipedia.org/wiki/Einstein_notation#Introduction), which implies the summation over all the repeated indices (only $$\nu$$ is a repeated index on the RHS). I've indicated this in the second (R)RHS

This general map is general. Other vectors are different. They mention the gradient vector $$\partial_{\mu}\phi \equiv \partial\phi/\partial x^{\mu}$$, which transforms a bit differently.

$$
\begin{equation}
\left( \frac{ \partial x^{\nu} }{\partial \overline{x}^{\mu} }\right) \frac{\partial \phi}{\partial x^{\nu} }
= \frac{ \partial \phi}{\partial \overline{x}^{\mu}}
\end{equation}
$$

So in this case, the index we're left with ends up on the bottom of a fraction (derivative). This is referred to as a covariant vector, and $$a^{\mu}$$ is called a contravariant vector. 


