---
layout: post
title:  "Hello world // categorical structures on the l-pieces part 1"
date:   2020-08-20
categories: geometric-topology
---
<script type="text/javascript" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"> </script> 
$$\newcommand{\KO}{\mathrm{KO}} \newcommand{\TMF}{\mathrm{TMF}}
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

\newcommand{\bm}{\mathbf{m}}
\newcommand{\bS}{\mathbf{S}}
$$

Hello world.

I'm going to start sparsely writing down my thoughts which I think are interesting, but which are not quite put together enough to stick in a paper.
I'll start now with some abstract nonsense conceived during my time at the SMALL reu this summer.

See <a href="https://nataliesstewart.github.io/blog/geometric-topology/2020/08/21/the-l-pieces-2.html">part 2 here.</a>

# Basics of $$\ell$$-pieces 
I'm going to briefly introduce and motivate a geometric topology construct, called an $$\ell$$<i>-piece</i>, to appear in an upcoming paper from my group in the SMALL reu.
I'll endow these with a notion of hyperbolicity and hyperbolic volume, which also appears in this paper.

In a future post, I'll briefly introduce the concept of an $$n$$-fold category, guided by the $$n=2$$ case of a <i>double category</i>, and show how the collection of $$\ell$$-pieces can be made into the $$\ell$$-cells of an $$\ell$$-fold category.
I'll attempt to describe a convenient $$\ell$$-fold subcategory of such hyperbolic pieces.

Keep in mind that a few of the results are not completely worked out yet.
I'll try to weaken such results accordingly.

### What $$\ell$$-pieces are 
I'm going to talk intuitively about 3-manifolds;
for the purpose of this blog, we may assume that these are either smooth or piecewise-linear, however we will talk purely in the smooth category.
All manifolds have boundary.
Not all surfaces in a manifold are properly embedded, and they are usually not connected.

**Definition.** We say the data $$(M,\cbr{V_1,V_2})$$ are a _piece_ if $$M$$ is a 3-manifold and $$V_1,V_2 \subset \partial M$$ are spaces satisfying one of the two following conditions:
* $$V_1$$ and $$V_2$$ are surfaces and $$V_1 \cap V_2$$ is a properly embedded 1-submanifold of $$\partial M$$. 

* $$V_1 = V_2 = \varnothing$$.
  
We further say that the data $$\prn{M,\prn{\cbr{V_{2i},V_{2i + 1}} \mid 1 \leq i \leq \ell}}$$ are an _$$\ell$$-piece_ if each tuple $$(M,\cbr{V_{2i},V_{2i + 1}})$$ is a piece and the intersections $$V_i \cap V_j$$ are each contained in a 1-manifold.

_Remark_: this definition actually differs somewhat from the analogous definition in the paper;
this definition is a tiny bit more complicated, in a way which does not help with hyperbolic geometry but does help with abstract nonsense.

The intersection condition is necessary for the following construction:

**Definition.** Suppose $$(M,\prn{\cbr{V_i}})$$ and $$(M',\prn{\cbr{V'_i}})$$ are two $$\ell$$-pieces and suppose $$\psi:V_2 \rightarrow V'_1$$ is a diffeomorphism.
The _composition_ $$(M,\prn{\cbr{V_i}}) \circ_\psi (M',\prn{\cbr{V'_i}})$$ is an $$\ell$$-piece defined as follows:

<p align="center">
$$
  \prn{M \cup_\psi M', \left(\cbr{V_1,V'_2},\cbr{V_3 \cup V'_3,V_4 \cup V'_4},\cbr{V_5 \cup V'_5,V_6 \cup V'_6},\dots\right)}.   
$$
</p>

This feels painfully topological, but it gets a little bit easier with some examples.
We'll use examples from knot theory, which require a bit more definitions.

**Definition.** Suppose $$M$$ is a 3-manifold and $$\Sigma \subset \partial M$$ is a surface in the boundary of $$M$$.
Then, We say that a _tangle in $$(M,\Sigma)$$_ is a compact smooth properly embedded 1-submanifold $$(\mathcal{T},\partial \mathcal{T}) \subset (M,\Sigma)$$.
If $$(M,\prn{\cbr{V_i}})$$ is an $$\ell$$-piece, we may define a tangle in $$(M,\prn{\cbr{V_i}})$$ to be a tanle in $$(M,\bigcup_i V_i - \bigcup_{ij} V_i \cap V_j)$$.
The complement of such a tangle determines a piece.
There is an evident notion of composition of tangles, and composition commutes with taking complements.

The following section is not strictly necessary for understanding the $$\ell$$-fold category structure, but it will be nice for motivating this from the geometric topology angle.

### Hyperbolic $$\ell$$-pieces.
Note that a 0-piece is simply a 3-manifold.
We give a notion of hyperbolicity of $$\ell$$-pieces which bootstraps from the relevant notion for 3-manifolds;
we say that a 3-manifold is _hyperbolic_ if it possesses a complete hyperbolic metric of finite volume.
In this case, Mostow-Prasad rigidity asserts that this metric is uniquely determined by the homotopy type of the manifold, and in particular the volume of the manifold is a homotopy invariant.

**Definition.** Suppose $$(M,\cbr{V_1,V_2})$$ is a piece.
Then, we define the _$$2m$$-replica_ to be the 3-manifold
<p align="center">
$$
D^{2m}(M,\cbr{V_1,V_2}) := \frac{2n \cdot M}{(V_1,2i) \sim (V_1,2i+1) \hspace{10pt} \text{ and } \hspace{10pt} (V_2,2i-1) \sim (V_2,2i)} 
$$
</p>
where $$2n \cdot M$$ is the $$2n$$th copower $$M \coprod M \coprod \cdots \coprod M$$.
If $$(M,\prn{\cbr{V_i}})$$ is an $$\ell$$-piece, we define the $$\bm = (2m_1,\dots,2m_\ell)$$-replica to be the 3-manifold
<p align="center">
$$
D^{(2m_1,\dots,2m_\ell)}(P,\prn{\cbr{V_i}}) := D^{(2m_1,\dots,2m_{\ell-1})}\prn{D^{2m_\ell}(P,\prn{V_{2\ell - 1},V_{2\ell}}),\prn{D^{m_\ell}(V_1),\dots,D^{m_\ell}(V_{2(\ell - 1)})}}
$$
</p>
We say that $$(M,\prn{\cbr{V_i}})$$ is _$$\bm$$-hyperbolic_ if $$D^{\bm}(M,\prn{\cbr{V_i}})$$ is hyperbolic, in which case we define the volume
<p align="center">
$$
  \vol^{\bm}\prn{m,\prn{cbr{v_i}}} := \frac{\vol\prn{D^{\bm}\prn{m,\prn{\cbr{v_i}}}}}{\prod_i 2m_i}.
$$
</p>
Much of the forthcoming paper is dedicated to a precise form of the following theorem, and a special case of the following conjecture.

**Pseudo-theorem.** Suppose there exists a suitable collection of $$m$$ surfaces decomposing an $$\ell$$-piece into a collection of $$(m_1,\dots,m_\ell,m)$$-hyperbolic $$(\ell+1)$$-pieces.
Then, the $$\ell$$-piece is $$(m_1,\dots,m_\ell)$$-hyperbolic, and it's $$(m_1,\dots,m_\ell)$$-hyperbolic volume is lower bounded by the sum of the $$(m_1,\dots,m_\ell,m)$$-hyperbolic volumes of the associated $$(\ell+1)$$-pieces.
In particular, one may find a lower bound on the volume of a 3-manifold by separating it into pieces.

**Conjecture.** Suppose an $$\ell$$-piece is $$(2m_1,\dots,2m_\ell)$$-hyperbolic.
Then, it is $$(2(m_1 + 1),2m_2,\dots,2m_\ell)$$-hyperbolic.

The conjecture is known for a more specific class, given by the tangles gotten by decomposing links residing in a cycle in $$S^3$$.
I won't go into depth here, but we're looking to prove it in some greater generality.
These yield the following corollary:

**Corollary.** The composition of $$n$$-many $$(2m_1n,2m_2,\dots,2m_\ell)$$-hyperbolic $\ell$-pieces is $$(2m_1,\dots,2m_\ell)$$-hyprbolic. 
If the conjecture is true, then the composition of an arbitrary number of $$\bm$$-hyperbolic $$\ell$$-pieces is $$\bm$$-hyprbolic.

This is nice:
it appears to tell us we can construct a nice sub-categorical object corresponding with the $$\bm$$-hyperbolic $$\ell$$-pieces.

We'll work with this in a future blog post;
next time, I'll define $$\ell$$-fold categories and attempt to describe their compositionality with more abstract nonsensical language.
