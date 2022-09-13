---
layout: post
title:  "Chainmail math 2: primary decomposition for the set of weaves"
date:   2022-09-12
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

\newcommand{\Fr}{\operatorname{Fr}}

\newcommand{\cbr}[1]{\left\{ #1 \right\}}
\newcommand{\brk}[1]{\left\[ #1 \right\]}
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


$$


**This post is under construction.**
See <a href="https://nataliesstewart.github.io/blog/chainmail-math/2022/09/09/the-moduli-space-of-weaves.html"> the previous post</a> in this series for context.

As a convention, whenever $$\cO$$ is an operad in $$\cC$$, we write $$\Fr_\cO:\cC \rightarrow \cO(\cC)$$ for the <a href="https://ncatlab.org/nlab/show/operad#the_monad_attached_to_an_operad"</a>free functor</a> to $$\cO$$-algebras..

### What is primary decomposition?

In elementary algebra, we note that a positive integer is written as a product of prime factors, unique up to permutation of the factors.
In knot theory, the same is true for knots and prime knots under connect sum.
Secretly, these facts are reflective of the fact that these commutative monoids are *freely generated* by the prime elements:
  <p align="center">
    $$\ZZ_{>0}^{\times} \simeq \Fr_{\Comm}\prn{\cbr{\text{primes}}}$$
  </p>
  <p align="center">
    $$\operatorname{Knots}^{\#} \simeq \Fr_{\Comm}\prn{\cbr{\text{prime knots}}}$$
  </p>

### The additive structure on the space of weaves
For primary decomposition to be well defined on the level of spaces, we have to work on the level of $$\EE_3$$ algebras:
this is the fancy way of essentially adding weaves by placing them disjointly adjacent to each other.

Note that one presentation of the $$\EE_3$$ operad, as the little 3-disks operad, asserts that each little 3-disk has the same fixed radius $$1 + \varepsilon$$, and the large 3-disk has some fixed radius of at least $$1 + \varepsilon$$.
We implicitly refer to this presentation, embedded into graded spaces concentrated in degree 0, as $$\EE_3(j)$$.
Note that, by translation after a choice of designated components, $\cW$ deformation retracts onto the graded subspace where a weave of $$n$$ components lives within the open ball of radius $$n + \varepsilon$$ about the origin.

> **Definition 1**.
> The *obvious $$\EE_3$$ structure on $$\cW$$* is made up of maps $$\EE_3 (j) \otimes \prn{\bigotimes_{i \in [j]} \cW_{n_i}} \rightarrow \cW_{\Sigma_i n_i}$$ wherein, given a point $$(d,w_1,\dots,w_j)$$, a new weave is made by dilating $$d$$ to consist of balls of radius $$n + \varepsilon$$, then canonically embedding the weaves $$w_i$$ into the balls in $$d$$.
> The pushforward graded commutative monoid structure on $$\pi_0 \cW = W$$ is called the *obvious additive structure on $$W$$.*

### Primary decomposition on the set of weaves

Let $$\widetilde \cW_*$$ be the graded summand consisting of weaves who do not have realizations whose complement has an isometrically embedded $$S^2$$ which is nontrivial after passing to the complement in $$S^3$$;
these are "prime weaves," who cannot be realized by placing nonempty weaves in disjoint balls.

We perform primary decomposition using the map $$f:\Fr_3\prn{\widetilde{\cW_*}} \rightarrow \cW_*$$ induced by the inclusion of graded spaces $$\widetilde{\cW_*} \hookrightarrow \cW_*$$ under the free-forgetful adjunction.

> **Claim**.
> The map $$f$$ is a $$\pi_0$$-equivalence; hence $$W_* \simeq \Fr_{\operatorname{Comm}}\prn{\widetilde{W}_*}$$.

We refer to a partition of the set $$\abs{w}$$ of components as a *decomposition* if there exists a realization of $$w$$ such that each part occupies a ball in $$\RR^3$$ such that the collection of such balls is disjoint.
We refer to such a partition as being *primary* if it doesn't have any proper refinements;
equivalently, a partition is primary if the weaves corresponding to the parts are each prime.

Given two decompositions $$d,d'$$ of $$w$$, let $$d \cap d'$$ be the coarsest common refinement of $$d$$ and $$d'$$.
Note that $$d \cap d'$$ is a decomposition;
hence the decompositions of $$w$$ form a finite upper-semilattice, implying they have a unique upper bound;
this is a unique primary decomposition $$d^{w}$$ for $$w$$.

In order to prove that $$f$$ is $$\pi_0$$-surjective, note that the sum of primary parts $$\sum_i d^w_i$$ yields a representative for $$\brk{w} \in \pi_0 \cW_*$$ in the image of $$f$$.

In order to prove that it's $\pi_0$-injective, suppose we have a path $$h:w \sim w'$$ for $$w,w'$ \in \operatorname{im}(f)$$;
note that the boundary of the ball around a prime subweave of size $$\varepsilon$$ of $$w$$ is equivalent to $$S^2$$, and hence is connected.
We may partition $$h$$ into intervals of time where these $$S^2$$ are disjoint and where they are not, noting that the parts containing $$t=0$$ and $$t=1$$ have disjoint spheres, and in fact it is enough to rectify $$h$$ to a homotopy during which these spheres remain disjoint.
This rectification can be done by modifying times with nondisjoint spheres to travel along a distinguished path from the starting intersection to the ending intersection, using connectedness of $$S^1$$.
This implies that $$\pi_0 f_*$$ is injective, so we are done.

**NOTE: this proof is horrible.**

The upshot is that the graded commutative monoid freely generated by a graded set is well understood:
it's explicitly the tensor algebra
  <p align="center">
    $$W \simeq T(\widetilde W) \simeq \frac{\oplus_k W^{\times k}}{\prn{w \otimes v - v \otimes w}}.$$
  </p>
in particular, we have
  <p align="center">
    $$W_n = \coprod_{n_1 + \cdots + n_k = n} \prod_i \widetilde W_{n_i}.$$
  </p>

One can prove that $$f$$ is not an equivalence of $$\EE_3$$-algebras, or even a $$1$$-equivalence;
essentially, there are elements of $$\pi_1 \cW_*$$ which always force a component in one ball to travel through the ball bounding another one.
If $$L_n$$ is a loop of $$n$$ components for $$n \gg 0$$, and $$O$$ is a weave with one component, then we can explicitly produce an element $$\pi_1(\cW_*; L_n + O)$$ which is not in the image of $$\pi_1 f$$ where $$O$$ travels around a "meridian" of $$L_n$$.
However, one can ask whether we just haven't found the correct generated graded space:

> **Question 3.** is $$\cW_*$$ equivalent to a free $$\EE_3$$-algebra? 
> More generally, is there a free $$\EE_n$$-algenra whose underlying $$\EE_3$$-algebra is the obvious $$\EE_3$$-structure on $$\cW_*$$?

This is essentially asking whether there's a topological primary decomposition for the space of weaves.
