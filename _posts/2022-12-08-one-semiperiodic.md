---
layout: post
title:  "Chainmail math 7: a linear weave manifesto in topological language"
date:   2022-12-08
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
\newcommand{\RR}{\mathbb{R}} \renewcommand{\S}{\mathbb{S}}
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
\newcommand{\sym}{\mathrm{Sym}} \newcommand{\per}{\operatorname{per}} 
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

\newcommand{\Fr}{\operatorname{Fr}}

\newcommand{\Op}{\operatorname{Op}}

\newcommand{\cbr}[1]{\left\{ #1 \right\}}
\newcommand{\brk}[1]{\left\[ #1 \right\]}
\newcommand{\abs}[1]{\left| #1 \right|}
\newcommand{\prn}[1]{\left( #1 \right)}
\newcommand{\vol}{\operatorname{vol}}

\newcommand{\id}{\operatorname{id}}
\newcommand{\STan}{\mathbf{sTAN}}

\newcommand{\bm}{\mathbf{m}}
\newcommand{\by}{\mathbf{y}}
\newcommand{\bC}{\mathbf{C}}
\newcommand{\bE}{\mathbf{E}}
\newcommand{\bS}{\mathbf{S}}

\newcommand{\cA}{\mathcal{A}}
\newcommand{\cO}{\mathcal{O}}
\newcommand{\cT}{\mathcal{T}}
\newcommand{\cW}{\mathcal{W}}
\newcommand{\RRP}{\mathbb{RP}}

\newcommand{\EE}{\mathbb{E}}
\renewcommand{\ZZ}{\mathbb{Z}}

\newcommand{\NN}{\mathbb{N}}

\newcommand{\Poly}{\mathbf{Poly}}

\newcommand{\Sub}{\operatorname{Sub}}

\newcommand{\Set}{\mathbf{Set}}

\newcommand{\op}{\text{op}}

\newcommand{\Comm}{\operatorname{Comm}}

\def\Nat{\operatorname{Nat}}
\def\Free{\operatorname{Free}}

\newcommand{\lin}{\mathrm{lin}}

\newcommand{\bL}{\mathbf{L}}
\newcommand{\bP}{\mathbf{P}}
$$


**This post is under construction.**
See <a href="https://nataliesstewart.github.io/blog/chainmail-math/2022/10/21/orbits.html"> the previous post</a> in this series for context, or the bottom of the <a href="https://nataliesstewart.github.io/blog/chainmail-math/2022/09/09/the-moduli-space-of-weaves.html">first in the series</a> for a table of contents.

Progress has stalled on the unit classification problem, because the hard step seems, indeed, hard; I believe the "trick" to do finitary classification will be a reduction from weave realizations to a subspace of link diagrams whose components are geometric circles.
This reduction doesn't seem to be as easy as I had hoped.

In true mathematical fashion, I will simply ask more difficult questions instead of progressing on mine.

### Linear weaves, a definition
We previously defined a (graded) space of unit weaves, and defined a unit weave to be a path component in the aformentioned space.
This time, we will define a filtered diagram of spaces, and the space of linear weaves will be realized as the (filtered) colimit of this diagram.
All of these spaces will consist of infinitely many rings, so we first need to define the space of (countably) infinite weaves.

> **Definition 1.** *The space of infinite ordered weaves is defined by*
>  <p align="center">
>    $$\cW_\omega^\sym := \cbr{\cbr{x_i,P_i}_{i \in \omega} \mid \not \exists i\neq j \text{ with } y \in P_i \cap P_j \text{     s.t. } d(x_i,y) = d(x_j,y) = 1)} \subset \prn{\RR^3 \times \RRP^2}^\omega;$$
>  </p>

This is not very useful, but allows for easy definition of linear weaves:

> **Definition 2.** * The space of *ordered n-periodic linear weaves* is be the subspace $$\cW^\sym_{\operatorname{per},n} \subset \cW^\sym_\omega$$ possessing a translational symmetry whose action on the set of embedded circles has quotient of size $$n$$.* 

There is an obvious question:
why not record the translational symmetry itself?
This turns out to not be very useful, by the following proposition:

> **Proposition 1.** Let $$w \in \cW^\sym_\omega$$ be an ordered infinite weave. Then, there is at most one translation symmetry realizing $$w$$ as an $$n$$-periodic weave.

To prove this is not too hard;
first suppose that there are translational symmetries $$\tau_1,\tau_2$$ of an infinite weave $$w$$ which are not parallel.
Then, the images of a component of $$w$$ under $$\tau_1^n$$ and $$\tau_2^n$$, exhibit an infinite sequence of pairs of components in a $$\tau_1$$-unit, with the elements of the sequence having pairwise distinct distances between their centers;
this implies that $$w$$ has infinite units with respect to $$\tau_1$$, so $$\tau_1$$ does not realize $$w$$ as linear periodic.

Next, suppose that $$\tau_1$$ and $$\tau_2$$ are parallel translational symmetries of $$w$$ different distance;
it is easy to see that units of $$\tau_1$$ and $$\tau_2$$ have different numbers of units, so at most one can be an $$n$$-periodic symmetry.

This allows us to make a global definition:
> **Definition 3.** *The space of ordered linear weaves is the union*
>  <p align="center">
>    $$\cW^{\sym}_{\lin} := \colim_n \cW_{\per,n}^{\sym} \subset \cW_{\omega}^{\sym}.$$ 
>  </p>

We can also remove the order:
> **Definition 4.** *Let $$B\Sigma := \bigoplus B\Sigma_n$$ be the groupoid corresponding with the disjoint union of deloopings of the symmetric groups $$\Sigma_n$$.*
> *Then, the space of * n-periodic linear weaves * is the orbit space
>  <p align="center">
>    $$\cW_{\per,n} := \prn{\cW_{\per,n}^\sym}_{\Sigma_n}.$$ 
>  </p>
> *The space of *linear weaves* is the colimit
>  <p align="center">
>    $$\cW_{\lin} := \colim_n \cW_{\per,n},$$ 
>  </p>
> *or equivalently, the orbit space*
>  <p align="center">
>    $$\cW_{\lin} := \prn{\cW^\sym}_\Sigma.$$ 
>  </p>

As before, we denote by $$W_\lin$$ the set $$W_\lin := \pi_0 \cW_\lin$$, and similarly for other spaces.

### Periodicity, simple periodicity, semiperiodicity
Let $$\bL$$ denote the poset of integers such that $$k \leq n$$ whenever $$k | n$$.
We say that a $$\bL$$-filtered set is of *finite type* if the associated graded $$\gr_n X_\bullet = X_n / \cup_{k | n} X_k$$ is finite for each $$n$$.

The set $$W_{\lin}$$ has an evident $$\bL$$-filtration corresponding with the *n-periodic linear weaves*.
Unfortunately, the following easy proposition establishes that the periodicity filtration is *not* of finite type:

> **Proposition 2.** The weave $$H_n$$, called *half persian n in 1*, is $$2$$-periodic with linking graph of degree $$n$$;
> in particular, $$H_n$$ is an infinite family of distinct 2-periodic linear weaves.

We may be able to rectify this!
The family $$\cbr{H_n}$$ has _unbounded interconnectedness_, in the sense that the linking graph has unbounded degree.
One way to bound interconnectedness is to restrict our periodicity symmetries to those that only interconnect adjacent units, as follows: 

> **Definition 6.** *A linear weave is * simply n-periodic * if it possesses an $$n$$-periodicity such that no two non-adjacent units have linked components;
> we write $$\cW_{s\per,n}$$ for the space of such weaves.

Let $$L(w)$$ denote the *linking graph of $$w$$*;
the following proposition is clear, and establishes that simple periodicity yields a $$\bL$$-filtration of $$\cW_{\lin}$$. 
> **Proposition 3.** Suppose $$w$$ is $$n$$-periodic;
> then, $$w$$ is simply $$(2\operatorname{deg}(L(w)) + 1)n$$-periodic.

Further, the information of *minimal length simple periodicity* is visible from a combination of the same information for periodicity and the linking graph.

Now let $$\bP$$ denote the poset of pairs of integers generated by the relations that $$(r,n) \leq (ar,n)$$ and $$(ar,n) \leq (r,an)$$.

> **Definition 7.** A linear weave is * $$(r,n)$$-semiperiodic * if it posesses a symmetry composed of a translation and an order $$r$$ isometry of the plane perpendicular to the translation, such that the quotient of the associated action on the set of components has $$n$$ components.
> A linear weave is * simply $$(r,n)$$-semiperiodic * if in addition, no non-adjacents units for this symmetry are related by nontrivial linking.

The following lemma is easy after you unwind the definition:
> **Lemma 4.** A linear $$(r,n)$$-semiperiodic weave is also $$nr$$-periodic; a simply $$(r,n)$$-semiperiodic weave is simply $$nr$$-periodic.

We can now engage in some conjectures!
> **Conjecture A**. The *size filtration* on the set of unit weaves is of finite type.

This is easier than the linear case:
> **Conjecture B.** The *simply periodic* and *simply semiperiodic* filtrations on the set of linear weaves are of finite type.
