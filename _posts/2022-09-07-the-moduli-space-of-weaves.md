---
layout: post
title:  "Chainmail math 1: a weave is a path component of the (coarse) moduli space of weaves"
date:   2022-09-09
categories: chainmail-math
---
<script type="text/javascript" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"> </script> 
<link rel="stylesheet" type="text/css" href="https://tikzjax.com/v1/fonts.css">
<script src="https://tikzjax.com/v1/tikzjax.js"></script>

$$
\newcommand{\KO}{\mathrm{KO}} \newcommand{\TMF}{\mathrm{TMF}}
\newcommand{\KU}{\mathrm{KU}} \newcommand{\Mfg}{M_\mathrm{fg}}
\newcommand{\spec}{\mathrm{Spec}} \newcommand{\dX}{\mathcal{X}}
\newcommand{\co}{\mathcal{O}} \newcommand{\Z}{\mathbf{Z}}
\newcommand{\top}{\mathrm{top}} \newcommand{\E}{\mathbf{E}}
\newcommand{\GG}{\mathbf{G}} \newcommand{\DD}{\mathbf{D}}
\newcommand{\Mell}{M_\mathrm{ell}} \newcommand{\ce}{\mathcal{E}}
\newcommand{\H}{\mathrm{H}} \newcommand{\dR}{\mathrm{dR}}
\newcommand{\cf}{\mathcal{F}} \newcommand{\FF}{\mathbf{F}}
\newcommand{\spf}{\mathrm{Spf}\ } \newcommand{\cA}{\mathcal{A}}
\newcommand{\Mcub}{M_\mathrm{cub}} \newcommand{\Mqd}{M_\mathrm{qd}}
\newcommand{\Aut}{\mathrm{Aut}} \newcommand{\tmf}{\mathrm{tmf}}
\newcommand{\Tmf}{\mathrm{Tmf}} \newcommand{\Map}{\mathrm{Map}}
\newcommand{\Ext}{\mathrm{Ext}} \newcommand{\End}{\mathrm{End}}
\newcommand{\cg}{\mathcal{G}} \newcommand{\Hom}{\mathrm{Hom}}
\newcommand{BP}[1]{\mathrm{BP}\langle #1\rangle} \newcommand{\QQ}{\mathbf{Q}}
\newcommand{\PP}{\mathbf{P}} \newcommand{\Gal}{\mathrm{Gal}}
\newcommand{\proj}{\mathrm{Proj}\ } \newcommand{\Ltwo}{L_{K(2)}}
\newcommand{\Eoo}{\mathbf{E}_\infty} \newcommand{\ol}[1]{\overline #1}
\newcommand{\pic}{\mathrm{Pic}} \newcommand{\RP}{\mathbf{R}P}
\newcommand{\BO}{\mathrm{BO}} \newcommand{\cc}{\mathbf{C}}
\newcommand{\CP}{\mathbf{CP}} \newcommand{\wt}[1]{\widetilde #1}
\newcommand{\RR}{\mathbf{R}} \renewcommand{\S}{\mathbb{S}}
\newcommand{\Lone}{L_{K(1)}} \newcommand{\Ltwo}{L_{K(2)}}
\newcommand{\gl}{\mathrm{gl}} \newcommand{\Lk}{L_{K(n)}}
\newcommand{\ku}{\mathrm{ku}} \newcommand{\ko}{\mathrm{ko}}
\newcommand{\GL}{\mathrm{GL}} \newcommand{\Ln}{L_n} \newcommand{\Lt}{L_{K(t)}}
\newcommand{\W}{\mathrm{W}} \newcommand{\BU}{\mathrm{BU}}
\newcommand{\SU}{\mathrm{SU}} \newcommand{\MU}{\mathrm{MU}}
\newcommand{\ul}[1]{\underline #1} \newcommand{\Sq}{\mathrm{Sq}}
\newcommand{\Tr}{\mathrm{Tr}} \newcommand{\d}{\mathrm{d}}
\newcommand{\HP}{\mathrm{HP}} \newcommand{\cL}{\mathcal{L}}
\newcommand{\cs}{\mathrm{cs}} \newcommand{\cd}{\mathcal{D}}
\newcommand{\Bord}{\mathrm{Bord}} \newcommand{\SO}{\mathrm{SO}}
\newcommand{\cC}{\mathcal{C}} \newcommand{\Sp}{\mathrm{Sp}}
\newcommand{\Lkd}{L_{K(d)}} \newcommand{\Mod}{\mathrm{Mod}}
\newcommand{\cH}{\mathcal{H}} \newcommand{\ket}[1]{|#1 \rangle}
\newcommand{\Bun}{\mathrm{Bun}} \newcommand{\cM}{\mathcal{M}}
\newcommand{\MTH}{\mathrm{MT}H} \newcommand{\MSO}{\mathrm{MSO}}
\newcommand{\twsm}{\ \widetilde{\wedge} \ } \newcommand{\BSpin}{\mathrm{BSpin}}
\newcommand{\MSpin}{\mathrm{MSpin}} \newcommand{\BString}{\mathrm{BString}}
\newcommand{\MString}{\mathrm{MString}} \newcommand{\B}{\mathrm{B}}
\newcommand{\der}{\mathrm{der}} \newcommand{\Cat}{\mathrm{Cat}}
\newcommand{\QCoh}{\mathrm{QCoh}} \newcommand{\LMod}{\mathrm{LMod}}
\newcommand{\Rep}{\mathrm{Rep}} \newcommand{\HH}{\mathrm{HH}}
\newcommand{\ZZ}{\mathfrak{Z}} \newcommand{\fr}{\mathrm{fr}}
\newcommand{\BSO}{\mathrm{BSO}} \newcommand{\BSU}{\mathrm{BSU}}
\newcommand{\id}{\mathrm{id}} \newcommand{\Top}{\mathrm{Top}}
\newcommand{\cP}{\mathcal{P}} \newcommand{\U}{\mathrm{U}}
\newcommand{\Sym}{\mathrm{Sym}} \newcommand{\coker}{\mathrm{coker}}
\newcommand{\Vect}{\mathrm{Vect}} \newcommand{\Fun}{\mathrm{Fun}}
\newcommand{\cT}{\mathcal{T}} \newcommand{\cJ}{\mathcal{J}}
\newcommand{\Res}{\mathrm{Res}} \newcommand{\Ind}{\mathrm{Ind}}
\newcommand{\MO}{\mathrm{MO}} \newcommand{\MSO}{\mathrm{MSO}}
\newcommand{\colim}{\mathrm{colim}} \newcommand{\hocolim}{\mathrm{hocolim}}
\newcommand{\fin}{\mathrm{fin}} \newcommand{\Tot}{\mathrm{Tot}}
\newcommand{\im}{\mathrm{im}} \newcommand{\FT}{\mathrm{FT}}
\newcommand{\AA}{\mathbf{A}} \newcommand{\Frob}{\mathrm{Frob}}
\newcommand{\ex}{\mathrm{ex,pr}} \newcommand{\fil}{\mathrm{fil}}
\newcommand{\gr}{\mathrm{gr}} \newcommand{\un}{\mathrm{un}}
\newcommand{\Syn}{\mathrm{Syn}} \newcommand{\Cart}{\mathrm{Cart}}
\newcommand{\bo}{\mathrm{bo}} \newcommand{\mmod}{/\!\!/}
\newcommand{\bsp}{\mathrm{bsp}} \newcommand{\BPP}{\mathrm{BP}}
\newcommand{\CAlg}{\mathrm{CAlg}} \newcommand{\TCart}{\mathrm{TCart}}
\newcommand{\BW}{\mathrm{BW}} \newcommand{\Br}{\mathrm{Br}}
\newcommand{\Pic}{\mathrm{Pic}} \newcommand{\ext}{\mathrm{ext}}
\newcommand{\Cl}{\mathrm{Cl}} \newcommand{\disc}{\mathrm{disc}}
\newcommand{\dir}{D\!\!\!\!/} \newcommand{\bb}{\mathrm{bb}}
\newcommand{\Ran}{\mathrm{Ran}} \newcommand{\cu}{\mathcal{U}}
\newcommand{\Gr}{\mathrm{Gr}} \newcommand{\Alg}{\mathrm{Alg}}
\newcommand{\G}{\Gamma} \newcommand{\dY}{\mathcal{Y}}
\newcommand{\Line}{\mathrm{Line}} \newcommand{\MUP}{\mathrm{MUP}}
\newcommand{\Bl}{\mathrm{Bl}} \newcommand{\St}{\mathrm{St}}
\newcommand{\cB}{\mathcal{B}} \newcommand{\SL}{\mathrm{SL}}
\newcommand{\XX}{\mathrm{X}} \newcommand{\gp}{\mathrm{gp}}
\newcommand{\Q}{\mathrm{Q}} \newcommand{\cI}{\mathcal{I}}
\newcommand{\T}{\mathrm{T}} \newcommand{\D}{\mathrm{D}}
\newcommand{\Aff}{\mathrm{Aff}} \newcommand{\BGL}{\mathrm{BGL}}
\newcommand{\an}{\mathrm{an}} \newcommand{\Tel}{\mathrm{Tel}}
\renewcommand{\|}{|} \newcommand{\MGL}{\mathrm{MGL}}
\newcommand{\CH}{\mathrm{CH}} \newcommand{\fr}[1]{\mathfrak #1}
\newcommand{\ch}{\mathrm{ch}} \newcommand{\Td}{\mathrm{Td}}
\newcommand{\Spin}{\mathrm{Spin}} \newcommand{\G}{\mathrm{G}}
\newcommand{\cHH}{\mathcal{H}} \newcommand{\F}{\mathrm{F}}
\newcommand{\B}{\mathrm{B}} \newcommand{\HC}{\mathrm{HC}}
\newcommand{\fib}{\mathrm{fib}} \newcommand{\tr}{\mathrm{tr}}
\newcommand{\TR}{\mathrm{TR}} \newcommand{\THH}{\mathrm{THH}}
\newcommand{\TP}{\mathrm{TP}} \newcommand{\crys}{\mathrm{crys}}
\newcommand{\even}{\mathrm{even}} \newcommand{\odd}{\mathrm{odd}}
\newcommand{\hodge}{\mathrm{Hodge}} \newcommand{\V}{\mathrm{V}}
\newcommand{\C}{C} \newcommand{\K}{K} \newcommand{\M}{M} \newcommand{\X}{X}
\newcommand{\h}{h} \newcommand{\TC}{\mathrm{TC}} \newcommand{\t}{t}
\newcommand{\DC}{\mathrm{DC}} \newcommand{\str}{\mathrm{str}}
\newcommand{\gen}{\mathrm{gen}} \newcommand{\Cyc}{\mathrm{CycSp}}
\newcommand{\DA}{\mathrm{DA}} \newcommand{\AG}{\mathbf{A}^1/\mathbf{G}_m}
\newcommand{\Crys}{\mathrm{Crys}} \newcommand{\cV}{\mathcal{V}}
\newcommand{\can}{\mathrm{can}} \newcommand{\Coh}{\mathrm{Coh}}
\newcommand{\SH}{\mathrm{SH}}

\newcommand{\cbr}[1]{\left\{ #1 \right\}}
\newcommand{\prn}[1]{\left( #1 \right)}
\newcommand{\vol}{\operatorname{vol}}

\newcommand{\id}{\operatorname{id}}
\newcommand{\STan}{\mathbf{sTAN}}

\newcommand{\bm}{\mathbf{m}}
\newcommand{\by}{\mathbf{y}}
\newcommand{\bC}{\mathbf{C}}
\newcommand{\bE}{\mathbf{E}}
\newcommand{\bS}{\mathbf{S}}

\newcommand{\cW}{\mathcal{W}}
\newcommand{\cT}{\mathcal{T}}
\newcommand{\RRP}{\mathbb{RP}}

\newcommand{\EE}{\mathbb{E}}

\newcommand{\NN}{\mathbb{N}}

\newcommand{\Poly}{\mathbf{Poly}}

\newcommand{\Sub}{\operatorname{Sub}}

\newcommand{\Set}{\mathbf{Set}}

\newcommand{\op}{\text{op}}

\def\Nat{\operatorname{Nat}}
\def\Free{\operatorname{Free}}


$$


**This post is under construction.**

This post is the first of a stream-of-conciousness series on *chain mail math*, and in particular, on classification problems for weaves of chainmail.
There is no intended audience, but if all is right in the world, it will be accessible to individuals possessing a working knowledge of basic topology (as this project does not currently involve ideas sophisticated to leave that realm), and occasionally of algebra and category theory;
if you do not know what the homotopy groups of a topological space are, consider that to be the main prerequisite at this time.

At some point in time, after significant results are said and done, I plan on making a document summarizing the work which is accessible to the topology-curious chainmailler.

### What chainmail really is, and what a (unit) weave ought be

Throughout many regions of the world and many times in history, people have been inspired to make protective garments (armor, butcher gloves, etc.) out of an interlinked collection of small metal pieces, each in the shape of a solid torus.
Such garments are examples of *chainmail*;
roughly, we may consider chainmail to be the craft wherein one interlinks metal solid tori.

Through this definition, we see that fabricating traditional chains with circle components can be considered chainmail;
in fact, using the traditional armor weave of *European 4 in 1*, one may see that a plane of European armor is crafted placing a solid torus at each point in a lattice, and if we restrict this construction to two adjacent rows, we recover a traditional 2-in-1 chain, up to physical manipulation.
We may view European 4-in-1 armor as a line's worth of interlocking chains.

Advancing to the past few decades, perhaps growing out of *ren fairs,* another craft has emerged under the name "chainmail:"
nowadays people craft jewelry out of more complicated and varied patterns of interlocking metal solid tori.
These often take the form of *units,* which are attached to a necklace chain as a pendant or to an earwire as an earring.

It is these units, initially, that we're interested in classifying.
So we may begin by asking an incorrect question:

> **Incorrect question 1**. *What are the ways of isometrically embedding finitely many solid tori into $$\RR^3$$?

One reason this is incorrect is that it has a tautological answer which is uncountably infinite:
there is one for every isometric embedding \(\coprod_n T_i \rightarrow \RR^3\), where \(T_i\) is a standard solid torus of a given inner radius and "wire" radius!
This is not of interest, and it doesn't help us work with chainmail in practice.

Another reason this is incorrect is that it appears to distinguish between weaves which are secretly the same;
if I have a generic piece of chainmail, then I can easily deform it to represent an uncountable collection of distinct weaves.
This is a bit encouraging:
we have uncountably many weaves with uncountable overcounting.
We can attempt to rectify this:

> **Incorrect question 2**. What are the ways of isometrically embedding finitely many solid tori into $$\RR^3$$ up to "physical deformation?"

I've called this incorrect for a reason:
this still uncountably overcounts!
To explain why, I'll introduce a bit of specific terminology.

In chainmail, there is a (redundant) list of three measurements which specify the geometry of a jump ring:
the *inner diameter* (diameter of the smallest longitudinal circle), the *wire diameter* (diameter of the largest meridian), and the *aspect ratio* (inner diameter divided by wire diameter).
My preferred way of referring to rings is by wire diameter and AR, so that for single-AR designs, I can dialate my specification of the design with a single datum.

However, we often use mixed-AR designs:
for instance, given a weave made of rings of core diameter $1$ (i.e. inner diameter $+$ half wire diameter) and a fixed AR $A$, I can form another "weave" of rings of core diameter $1$ and AR $$A + \varepsilon$$ by "shrinking" each ring.

Our classification should identify rings which are related by this procedure;
we might as well shrink rings to infinitesimally small, and note that as $A \gg 0$, weaves become idenfied with AR $A$ iff they're identified with AR $A + \varepsilon$.
I'll skip the ponderance of the (co)limit of the procedure, and say what we get:

> **Correct question 1**. What are the ways of "rigidly" embedding finitely many circles into $$\RR^3$$ up to deformations of rigidly embedded circles?

However, in chainmail, there are sometimes phenomena that we care about which are specific towards ID relationships, called *captivation* and *orbiting*;
a circle is *captivated* if it spans a plane not intersecting any other circles, yet it is not able to be "separated" from the rest of the weave to occupy disjoint isometrically embedded standard balls.
Similarly, a circle *orbits* another part of the weave if it is unlinked to the part, yet it is not able to be freed from that part intersecting its disk.

A simple example of an orbit follows, (credit: Joshua Dilberto, orbital, via RIM) **TODO: embed**

The unlinked torus can't escape so long as it's ID is at most the ID of the rings in the linking which it orbits.
however, if it's ID is any amount larger than that of the surrounding ones, it is free.

We can manage some ID specific interactions in a finitary classification if we fix ratios;
the simplest example is weaves of rings which all have the same ID:

> **Correct question 2**. What are the ways of "rigidly" embedding finitely many circles of the same radius into $$\RR^3$$ up to deformations of rigidly embedded circles?

It is this question that we endeavor to answer.
We now define "weave" in a precise way, to capture the answer to this question.
However, first, we need a bit of technology.

### Graded spaces

### The (graded) space of chain mail weaves
We hope to define a graded space $$\cW_n$$, such that $$W_n := \pi_0 \cW_n$$ is the correct notion of a *weave with $$n$$ components*.
Formally, let's write $$\cW_0 = \cbr{*}$$, i.e. it's the space consisting of a point.
We may first endeavor to define $$\cW_1$$ correctly.

These are meant to be *rigidly embedded circles of radius 1 in $$\RR^3$$*.
Every such circle is a uniquely a unit circle in an embedded (pointed) plane, which is linearly embedded in $$\RR^$3$.
We may use this as a definition:

> **Definition 1**. $$\cW_1 := \RR^3 \times \RRP^2$$.

This is scary if not unpacked:
already we're working with a non-orientable 5-manifold!
However, as we currently only care about $$\pi_0 \cW_n$$, we should only really care about $$\cW_1$$ up to homotopy equivalence;
up to equivalence, we have $$\cW_1 \simeq \RRP^2$$ (we can pull rings to the center up to contractible ambiguity), which ought be one of the least scary non-orientable surfaces.

Let's go one level up:
what ought the space of two-component weaves be?
One good answer for this is the space of pairs of circles which are nonintersecting.

Let's flesh this all the way out:

> **Definition 2.** *The $$n$$th part of the space of chainmail weaves is defined by*
  <p align="center">
    $$\cW_n := \cbr{(x_i,\ell_i)_{i \in [n]} \mid \not \exists y \in P_{\ell_i} \cap P_{\ell_j} \text{ s.t. } d(x_i,y) = d(x_j,y) = 1)} \subset \left\(\RR^3 \times \RRP^2\right\)^n;$$
  </p>
> *explicitly, this is the space of $$n$$ intersecting circles in $$\RR^3$$.*

As said before, we define $$W_n := \pi_0 \cW_n$$.
We also write $$\cW := \coprod_{n \in \NN} \cW_n$$ and $W := \pi_0 \cW = \coprod_{n \in \NN} W_n$$;
by abuse of notation, we will sometimes refer to $$\cW$$ as the graded space $$(\cW_n)$$, noting that this has underlying space $$\cW$$.


We can finally make a definition:

> **Definition 3**. *A chainmail weave is an element of $$W$$. A weave has $$n$$ components if it's an element of $$W_n$$.

### Prime weaves and primary decomposition
In elementary algebra, we note that a natural number is written as a product of prime factors, unique up to permutation of the factors.
In knot theory, the same is true for knots and prime knots under connect sum.
We can also do this in chain mail math, but for it to be well defined on the level of spaces, we have to work on the level of $$\EE_3$$ algebras.

Note that one presentation of the $$\EE_3$$ operad, as the little 3-disks operad, asserts that each little 3-disk has the same fixed radius $$1 + \varepsilon$$, and the large 3-disk has some fixed radius of at least $$1 + \varepsilon$$.
We implicitly refer to this presentation, embedded into graded spaces concentrated in degree 0, as $$\EE_3(j)$$.
Note that, by translation after a choice of designated components, $\cW$ deformation retracts onto the graded subspace where a weave of $$n$$ components lives within the open ball of radius $$n + \varepsilon$$ about the origin.

> **Definition 3**.
The *obvious $$\EE_3$$ structure on $$\cW$$* is made up of maps $$\EE_3(j) \otimes \bigotimes_{i \in \brk{j}} \cW_{n_i} \rightarrow \cW_{\sum_i n_i}$$ taking wherein, given a point $(d,w_1,\dots,w_j)$, a new weave is made by dilating $$d$$ to consist of balls of radius $$n + \varepsilon$$, then canonically embedding the weaves $$w_i$$ into the balls in $$d$$.
The pushforward graded commutative monoid structure on $$\pi_0 \cW = W$$ is called the *obvious additive structure on $$W$$.*

> **Claim 4**.
The obvious $$\EE_3$$ structure on $$\cW$$ is freely generated by a graded space $$\widetilde{\cW}$$, and the pushforward graded commutative monoid $$W$$ is freely generated by $$\widetilde W := \pi_0 \widetilde{\cW}$$.
