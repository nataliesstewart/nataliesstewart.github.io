---
layout: post
title:  "Chainmail math 5: operadic right-modules and toroidal decomposition, the theory"
date:   2022-09-23
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


$$


**This post is under construction.**
See <a href="https://nataliesstewart.github.io/blog/chainmail-math/2022/09/16/atoroidal-decomposition-for-weaves.html"> the previous post</a> in this series for context and content of the following post, or the bottom of the <a href="https://nataliesstewart.github.io/blog/chainmail-math/2022/09/09/the-moduli-space-of-weaves.html">first in the series</a> for a table of contents.


### Symmetric sequences, operads, and free functors
Let $$\Sigma$$ denote the groupoid $$\Sigma := \coprod_{n \in \NN} \Sigma_n$$; this is equivalent to the core of the category of finite sets.
> **Definition 6.** *Fix $$\cC$$ a cocomplete symmetric monoidal closed category*.
> *The *category of symmetric sequences in $$\cC$$* is the functor category $$\cC^\Sigma$$*.
> These possess a symmetric monoidal product called the *composition product*, computed on objects by
> <p align="center">
>   $$\cO \circ \cO'(n) := \coprod_{n_1 + \cdots + n_k = n} \cO(k) \otimes \bigotimes_{i} \cO'(n_i).$$
> </p>
> An *operad* is a monoid in symmetric sequences.

We could have equivalently replaced $$\Sigma$$ with $$\mathbf{Fin}^{\simeq}$$;
we use the skeleton for the sake of the notation $$\cO(n)$$.

I'll cut to the chase;
there is a free forgetful adjunction between pointed symmetric sequences and operads, given by the free monoid construction with respect to $$\circ$$.
There's likewise a free-forgetful adjunction between symmetric sequences and left-modules over a given operad, as well as right-modules.
Left-modules are a generalization of *algebras*, which are precisely left modules concentrated in degree 0.

If we view the weight grading of a symmetric sequence $$X_\bullet$$ as being the "number of elements," then we may view right-modules over $$\cO$$ as an algebraic structure wherein, given an element of $$X_\bullet$$ with $$n$$ elements, and $$n$$ elements of $$\cO$$ with $$n_1,\dots,n_k$$ elements, we produce an element of $$X_\bullet$$ with $$\sum_i n_i$$ elements.

We use this perspective to formalize toroidal composition.
But first, we sketch the notion of a *operadic congruence generated by a sub-symmetric sequences*.

### Congruences, quotients, and operads
This section will be far from self contained.

Let $$\cC$$ be a finitely complete category.
A <href a="https://ncatlab.org/nlab/show/congruence">congruence on $$X$$</a> is an equivalence relation on $$X$$ internal to $$\cC$$;
in particular, such a thing is a subobject $$R \hookrightarrow X \times X$$, which yields a parallel pair $$R \rightrightarrows X$$ by composing with the right and left projection.
Note that the condition of internal reflexivity is precisely that there exists a common section $$\Delta:X \rightarrow R \rightrightarrows X$$.

The *quotient* $$X / R$$ is, if it exists, the coequalizer of the diagram $$R \rightrightarrows X$$. 

In particular, any morphism $$S \rightarrow X$$ has a <a href="https://ncatlab.org/nlab/show/kernel+pair">kernel pair</a>, defined as the pullback of the cospan $$S \rightarrow X \leftarrow S$$, and this supports the structure of a congruence.
If all quotients exist for kernel pairs, then <a href="https://ncatlab.org/nlab/show/regular+category">every coequalizer is expressed as the quotient of its kernel pair</a>;
this is a nonabelian version of the axiom in abelian category that cokernels of kernels agree with kernels of cokernels. 

If in fact the morphism property of *being a coequalizer of some parallel pair* is pullback-stable, then $$\cC$$ is called <a href="https://ncatlab.org/nlab/show/regular+category#properties">regular;</a> 
regular categories are the categories with pullback-stable image factorizations, yielding a form of the first isomorphism theorem:
every morphism $$f:X \rightarrow Y$$ factors canonically as a coequalizer followed by a monomorphism.

> **Claim.** Let $$G \hookrightarrow X \times X$$ be a subobject, for $$X$$ a monoid.
> Then, the poset $$P$$ of congruences on $$X$$ containing $$G$$ (ordered by containment) has a unique minimal element.

It suffices to prove that $$P$$ is <a href="https://en.wikipedia.org/wiki/Directed_set">cofiltered</a> and its opposite poset satisfies the conditions of <a href="https://en.wikipedia.org/wiki/Zorn%27s_lemma">Zorn's lemma.</a>
In fact, we can prove a stronger condition:
we show that $$P$$ has arbitrary nonempty limits, i.e. it has arbitrary nonempty intersections.

### Toroidal composition
There are symmetric sequences $$A^\vee$$ of atoroidal toroidal weaves, $$A^{\Sym}$$ of atoroidal weaves, $$W^\vee$$ of toroidal weaves, and $$W^{\Sym}$$ of weaves, in sets.
Toroidal composition provides two maps of symmetric sequences:
<p align="center">
  $$W^\vee \circ W^\vee \xrightarrow{\mu^\vee}W^\vee.$$
</p>
<p align="center">
  $$W^{\Sym} \circ W^\vee \xrightarrow{\mu} W^{\Sym}.$$
</p>

We'd like to realize the first as the composition map of an operad, and the second as a structure map of an operadic right module.
To do the first, we need to choice a unit.
This is not too hard: 

> **Proposition 1.** $$\cW^{\vee}(1)$$ is contractible;
> that is, there is a contractible space of one-component toroidal weaves.

To prove this, note that there is a deformation retract of $$\cW^{\vee}(1)$$ onto the realization given by the core curve of the solid torus;
this is a translation followed by a rotation.

Let $$\eta \in \Hom(\cO_{\operatorname{triv}}, W^\vee) \simeq W^{\vee}(1) \simeq *$$ be the for $$W^\vee$$.

> **Proposition 2.**
> The maps $$\mu^\vee, \eta$$ endow on $$W^{\vee}$$ the structure of an operad.

This is more-or-less obvious, so I'll skip it.
The following proposition is also obvious, and I'll also skip it

> **Proposition 3.**
> The map $$\mu$$ endows $$W^{\Sym}$$ with the structure of a right module over $$W^\vee$$.

These summarize the existence of algebraic structure on weaves;
there's both an operadic composition within toroidal weaves, and an operadic right-action of toroidal weaves on weaves.
We next describe toroidal decomposition, which amounts to giving presentations of $$W$$ and $$W^\vee$$ as quotients of free objects.

### Toroidal decomposition
Note that $$\cA^\vee$$ is contractible by Proposition 1, so $$A^\vee$$ is uniquely pointed.
There is a free operad $$\Fr_{\Op}\prn{A^\vee}$$ on $$A^\vee$$ as a pointed object;
this is the operad parameterizing trees labelled with atoroidal toroidal weaves, modulo the one-component weave $$O$$ acting as unit.
The operad structure on $$W^\vee$$ is given by a structure map $$\Fr_{\Op}\prn{W^\vee} \rightarrow W^\vee$$.
This induces a map
<p align="center">
    $$\Fr_{\Op}\prn{A^\vee} \rightarrow \Fr_{\Op}\prn{W^\vee} \rightarrow W^\vee.$$
</p>
In the other direction, the previous discussion of toroidal decomposition yields a map of operads $$W^\vee \rightarrow \Fr_{\Op}\prn{A^\vee}$$, after choosing a (non-canonical) decomposition of each fully toroidal weave into a tree of 2-component weaves.
We'd like to realize these as maps within a split coequalizer diagram in operads;
to do so, we need the technology of operadic congruence envelopes.

**TODO: put discussion of operadic congruence envelopes here.**

Now, let $$r^\vee_{M} \in \Fr_{\Op}\prn{A^\vee}^{\times 2}$$ be the relation between the two realizations of $$M_3$$ within $$\Fr_{\Op}\prn{A^\vee}$$;
these are both trees of height 2 with one leaf node $$M_2$$ and the other $$O$$, with the first making one choice of position for the $$M_2$$ and the other making the other.
Similarly, let $$r^\vee_O \in \Fr{|Op}\prn{A^\vee}^{\times 2}$$ be the relation between the two realizations of $$3 \cdot O$$.

Toroidal decomposition for toroidal weaves can be phrased as follows:

> **Theorem 4.**
> The operadic cofork diagram
> <p align="center">
>   $$\langle r_M, r_O \rangle \rightrightarrows \Fr_{\Op}(A^\vee) \rightarrow \cW^\vee$$
> </p>
> is split by toroidal decomposition;
> hence $$\cW^\vee$$ is the quotient of the operad of trees labelled by $$A^\vee$$ by the realizations of $$M_3$$ and $$3 \cdot O$$.

Similarly, note that $$A \circ W^\vee$$ is the free right $$W^\vee$$-module on $$A$$.
Let $$r_M$$ and $$r_0$$ be the relations in $$A \circ W^\vee$$ corresponding with the realizations of $$M_3$$ and $$3 \cdot O$$.
Toroidal decomposition for weaves can be phrased as follows:

> **Theorem 5.**
> The right $$W^\vee$$-module cofork diagram
> <p align="center">
>   $$\langle r_M, r_O \rangle \rightrightarrows A \circ W^\vee \rightarrow W^\Sym$$
> </p>
> is split by toroidal decomposition;
> hence $$W^{\Sym}$$ arises by affixing a single atoroidal weave to a toroidal weave, modulo the pairs of such decompositions for $$M_3$$ and $$3 \cdot O$$.

We then may pass from $$W^{\Sym}$$ to $$W$$ by taking $$\Sigma$$-orbits.

The various functors employed in this construction are summarized in the following chart:
<div align="center">
	<a href="/assets/toroidal decomposition.png"><img src="/assets/toroidal decomposition.png" align="center" weight="800" ></a>
	<p align="center">
    <font size="2"> This illustration is color coded for clarity; red describes the free operad construction, green the free module construction, orange the structure of toroidal weaves, and blue the structure of weaves. Each cofork diagram is a (split) coequalizer.</font>
  </p>
</div>


