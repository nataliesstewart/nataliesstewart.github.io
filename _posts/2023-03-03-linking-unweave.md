---
layout: post
title:  "Chainmail math 8: linking detects the unit unweave"
date:   2023-3-17
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

See <a href="https://nataliesstewart.github.io/blog/chainmail-math/2023/02/22/one-semiperiodic.html"> the previous post </a> in this series for context.
See the bottom of the <a href="https://nataliesstewart.github.io/blog/chainmail-math/2022/09/09/the-moduli-space-of-weaves.html">first post in the series</a> for a table of contents.

In this post, we construct a combinatorial invariant of unit weaves and prove that it detects the unweave.
The major mathematical content of this post is a citation to the paper <a href="https://projecteuclid.org/journalArticle/Download?urlId=10.4310%2Fjdg%2F1214440725&referringURL=https%3A%2F%2Fduckduckgo.com%2F&isResultClick=False">Strange Actions of Groups on Spheres</a> by Freedman & Skora;
in particular, they claim the essence of the main proposition of this post *by synthetic geometry* in Lemma 3.2.

This note concenrs both the finite and infinite case;
for the rest of the post, $$1 \leq n \leq \infty$$.

### The linking graph
We first warm up with some unit weave constructions;
recall that weaves have underlying links, and pairs of components in links have <a href="https://en.wikipedia.org/wiki/Linking_number">linking numbers</a>.
> **Construction.**  Let $$\tilde w \in \cW_n$$ be a unit weave realization, and let $$\pi:\cW_n \rightarrow \RR^{3n} = \operatorname{Map}(n,\RR^3)$$ be projection to the centers of circles.
> The *linking grpah* of $$\tilde w$$ is the embedded graph $$L(\tilde w) \subset \RR^3$$ whose vertices embed as $$\pi(\tilde w)$$, with edges drawn linearly between vertices if the corresponding circles have nonzero linking number.

The fact that this is invariant is obvious:
> **Proposition 1.** Let $$\tilde w, \tilde u$$ be unit weave realizations;
> there is a continuous map from equivalences $$\tilde w \sim \tilde u$$ to ambient isotopies $$L(\tilde w) \sim L(\tilde u)$$;
> in particular, the underlying graph is a weave invariant.
Hence, for $$w \in W_n$$, we define $$L(w)$$ to be the underlying graph of $$L(\tilde w)$$ for any realization $$\tilde w$$ of $$w$$. 

Note that $$L$$ is naturally functorial under isometries;
that is, $$O(3)$$ acts on $$\cW_n$$, and this is naturally mapped to an action of the stabilizer $$G$$ of $$\tilde w$$ on $$L(\tilde w)$$ as an embedded graph.
This further maps to an action of $$G$$ on $$L(w)$$ as a graph.
In particular, when $$w$$ is linear, $$L(w)$$ has a natural $$\ZZ$$ action.

We will explore this in the next post.

### The ring dilation trick for units
> **Construction.** *The* $$n$$th part of the space of scaled chainmail weaves* is defined by*
>  <p align="center">
>    $$\begin{align*}
>      \cW'_n 
>        :&= \cbr{\prn{(r,\cbr{x_i,P_i}_{i \in [n]}} \mid \not \exists i\neq j \text{ with } y \in P_i \cap P_j \text{ s.t. } d(x_i,y) = d(x_j,y) = r)}\\
>        & \subset \RR \times \prn{\RR^3 \times \RRP^2}^n_{\Sigma_n};
>       \end{align*}$$
>  </p>
> *explicitly, this is the space of $$n$$ nonintersecting circles of radius $$r$$ in $$\RR^3$$.*


The following proposition is obvious.
> **Proposition 2.** The "divide by $$r$$" map $$\cW'_n \rightarrow \cW_n$$ is a trivial $$\RR$$-fiber bundle;
> in particular, it is a homotopy equivalence, so it induces a bijection on $$\pi_0$$.

We'll freely use $$\cW'_n$$ when useful from now on, which will allow us to avoid the hassle of explicit "ring resizing" tricks.

For the following argument, let $$\rho:\cW'_n \rightarrow \RR$$ be the projection to the $$\RR$$ coordinate, i.e. the radius, and for $$c,c' \in \abs{w}$$, let $$d(c,c')$$ denote the distance between their centers.
The following lemma is clear, but useful.
> **Lemma 3.** Let $$w \in \cW'_n$$ be a unit weave such that for all pairs $$c,c' \in \abs{w}$$, we have $$d(c,c') > \rho(w)/2$$.
> Then, $$w$$ is the unweave.

### Linking detects the unit unweave
> **Proposition 4.** Suppose $$w$$ is a unit weave of (possibly infinite) size $$n$$ such that $$L(w)$$ is trivial, i.e. no pairs of components are linked.
> Then, $$w$$ is the unweave.

To prove this, we use Freedman & Skora Lemma 3.2;
under the embedding $$\RR^3 \subset S^3 \subset \delta B^4$$, there exist unique hemispheres bounded by each component of $$\tilde w$$ intersecting $$S^3$$ perpendicularly.
Doubling about $$S^3$$, these turn into standard metric 2-spheres;
by an explicit euclidean geometry argument, any pair of such spheres must have intersection either empty, a circle which intersects $$S^3$$, or a single point contained in $$S^3$$.
In particular, since the intersection of such circles with $$S^3$$ is $$w$$, any pair's intersection doesn't intersect $$S^3$$, and hence they are pairwise non-intersecting.

Passing through the standard "thickened stereographic projection" map $$B^4 - \cbr{0} \cup \cbr{(1,0,0) \times I} \simeq \RR^3 \times \RR$$, this yields a collection of pairwise nonintersecting hemispheres in $$\RR^3 \times I$$ who intersection with $$\RR^3 \times \cbr{0}$$ is $$w$$;
this implies that they have the same radius $$r$$, so their sintersection with $$\RR^3 \times \cbr{t}$$ is in $$\cW'_n$$ for $$t < r$$, yielding a path $$h_t$$ in $$\cW'_n$$ beginning at $$w$$.

In fact, $$h_t$$ preserves centers, and as $$\varepsilon \rightarrow 0$$ we have $$\rho(h_{t - \varepsilon}) \rightarrow 0$$.
By Lemma 3, this is unwoven for $$\varepsilon$$ small, so $$h_0 = w$$ is unwoven as well, and we are done.
<span style="float:right;font-size:25px;">
        □
</span>

<br />

Because it will be useful later, we explicitly record the full strength of this argument:
let $$X_\varepsilon \subset \cW'_n$$ be the subspace of realizations such that $$d(c,c') > \varepsilon \rho(w)$$ for all $$c,c'$$.
> **Lemma 5.** The paths $$h_t$$ together form a deformation retract of $$\cW'_n$$ onto $$X_\varepsilon$$ which preserves the centers and normals of each component.

From this perspective, Lemma 3 can be viewed as saying that $$X_\varepsilon$$ is connected, which together with Lemma 5, immediatley proves the proposition.

### How we'll prove the linear case
In the next post, I'll introduce weaves which are preserved by *arbitrary isometric group actions*, recovering linear weaves along the way.
The key insight will be that preservation under isometric group actions depends only on component centers and normals;
hence Lemma 5 continues to apply.
In another post, we'll prove an equivariant version of Lemma 3, hence proving that equivariant linking detects the equivariant unweave.
