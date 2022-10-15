---
layout: post
title:  "Chainmail math 4: kinging/möbiusing and toroidal decomposition, the praxis"
date:   2022-09-22

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
See <a href="https://nataliesstewart.github.io/blog/chainmail-math/2022/09/15/level-2.html"> the previous post</a> in this series for context, or the bottom of the <a href="https://nataliesstewart.github.io/blog/chainmail-math/2022/09/09/the-moduli-space-of-weaves.html">first in the series</a> for a table of contents

### On kinging and Möbiusing
In chainmail, we often refer to a process called *kinging*, wherein every circle in a weave is replaced with two adjacent circles.
For instance, <a href="https://www.mailleartisans.org/weaves/weavedisplay.php?key=8">King's maille</a> is a common weave which is created by kinging <a href="https://www.mailleartisans.org/weaves/weavedisplay.php?key=6">European 4 in 1</a>.
We sometimes concieve of partial kinging, e.g. in <a href="https://www.mailleartisans.org/weaves/weavedisplay.php?key=223"> Poor King's Scale</a> (up to ring rescaling), a partial kinging of European 4 in 1, and a sheet variant of the titular <a href="https://www.joshuadiliberto.com/JD_newWebPages/tutorial_vertebrae4in1chain.php">Vertebrae weave</a>.

We may understand this one ring at a time;
one may reach a (partially or fully) kinged weave by repeatedly replacing components in a weave with $$O+O$$, where $$O$$ is the one component weave.
Hnce we may understand kinging hopefully as a process $$\cW_*^+ \rightarrow \cW_{*+1}$$, where $$\cW_*^+$$ refers to the graded space of weaves with a distinguished component.

There are other practical analogues to this process;
we may Möbius a weave by replacing a component with <a href="https://nataliesstewart.github.io/blog/chainmail-math/2022/09/15/level-2.html">the</a> prime 2-component weave.

These are each gotten by substituting a weave into a solid torus surrounding a component of a weave.
We'll refer to this process as *toroidal composition*.

Just as how supplying the obvious additive structure on $$W$$ allowed us to decompose weaves into primes, we can ask if there's a similar decomposition into atoroidals;
this turns out to be much more complicated, as our decription of toroidal composition allowed us only to substitute weaves with a distinguished (implicit) embedding into a solid torus.
This will lead us astray from actual content, so we largely sweep it under the rug in this post, which is aimed at addressing only the actual content.

In this post, we first make sense of what a toroidal or atoroidal (sub)weave is.
We then collect these in a hypergraph invariant of weaves, called the *toroidal hypergraph*;
following this, we give several workhorse lemmas about the structure of the toroidal hypergraph, which allow us to make sense of decomposition, in the language of *atoroidal quotients* and *fully toroidal quotients*.
We perform a classification of fully toroidal weaves, reducing the class of indecomposable weaves for this decomposition to only the atoroidal weaves.
We end with a sketch of the toroidal decomposition of each of the 4-component weaves appearing in the RIM.


### Toroidal subweaves, quotients, and the contraction lemma
By convention, we refer to a subweave as *trivial* if it has size 1, i.e. it has one compoent.

> **Definition 1.** *A subweave $$t \hookrightarrow w$$ is * toroidal * if there is an isometrically embedded solid torus $$T \hookrightarrow \RR^3$$ of core radius 1 such that $$T \cap w = t$$*.

A nontrivial toroidal subweave $$t \hookrightarrow w$$ is a witness to the fact that $$w$$ can be built from weaves of size $$< \abs{w}$$.
To establish this precisely, we need a way to reverse this building, which we develop via the following definition.

> **Definition 2.** A *toroidal partition* of a weave $$w$$ is a partition of $$\abs{w}$$ such that the subweave consisting of the each part is toroidal.

> **Lemma 1.** *(the contraction lemma)* Fix some $$0 < \varepsilon' < \varepsilon$$.
> Suppose $$t \hookrightarrow w$$ is a toroidal subweave witnesed by some $$T_\varepsilon \hookrightarrow \RR^3$$ of core diameter $$\varepsilon$$.
> Then, there exists a witness $$T_{\varepsilon'}$$ of $$t$$ with core diameter $$\varepsilon'$$.

A toroidal partition supplies an equivalence relation on the set of weaves.
This should suggest the notion of a quotient:

> **Definition 3.** *Given a toroidal partition* $$\cbr{t_i}$$ of $$w$$, the *quotient* $$w / \cbr{t_i}$$ is formed by replacing each part with the core circle of a solid torus containing each part. 


Given a toroidal partition $$\cbr{t_i}$$ of $$w$$, we can reconstruct $$w$$ by substituting $$\cbr{t_i}$$ into the rings of $$w / \cbr{t_i}$$;
to make good use of this, we need to describe the extent of this reconstruction procedure.
We'd like to give a *canonical decomposition* of each weave $$w$$ such that $$w$$ is indecomposable if and only if this decomposition is trivial.
To develop this, we need to define the notion of indecomposability.

> **Definition 4.** 
> *A toroidal subweave $$t \hookrightarrow w$$ is * atoroidal * if it is of size $$\geq 2$$ and every proper subweave of $$t$$ of size $$ \geq 2$$ is not toroidal in $$w$$.*
> *A weave is atoroidal if it is atoroidal as a subweave of itself.

We denote by $$\cA_* \hookrightarrow \cW_*$$ the summand consisting of atoroidal weaves, and $$\cA_*^\vee := \cW_*^\vee \cap \cA_*$$.
The atoroidal subweaves are minimal among the sub-poset of $$P(w)$$ of toroidal subweaves of size at least 2.
We will formalize this perspective via hypergraphs:

### Some structure of the toroidal hypergraph 
> **Definition 5.** 
> *Given a weave $$w$$, the *toroidal hypergraph* $$H(w)$$ is the hypergraph corresponding with the subset of $$P(\abs{w}) - \cbr{\varnothing}$$ of toroidal weaves.*
> *The weave $$w$$ is *toroidally connected* if $$H(w)$$ is connected.*
> *The weave $$w$$ is *fully toroidal* if the hypergraph is fully connected, i.e. every subweave is toroidal.*


A toroidal partition of $$w$$ is equivalent to a partition of $$\abs{H(w)}$$ by edges, and $$H(w / \cbr{t_i})$$ is given by contracting the corresponding edges, i.e. as $$H(w)/\cbr{t_i}$$.
The following lemma is clear;

> **Lemma 2**. A toroidal partition $$\cbr{t_i}$$ of $$w$$ has atoroidal quotient $$w / \cbr{t_i}$$ iff each part is a union of connected components of $$H(w)$$.

We hope to construct a maximal atoroidal quotient;
a natural choice for such a thing is the connected component partition of $$H(w)$$.
Luckily for us, this works:

> **Proposition 3.** Every connected component $$t$$ of $$H(w)$$ corresponds with a toroidal weave;
hence there is a unique maximal atoroidal quotient of $$w$$.

To prove this, we use the following lemma:
> **Lemma 4.** Suppose $$s,t \subset w$$ are toroidal subweaves such that $$s \cap t \neq \emptyset$$. Then, the following subweaves of $$w$$ are toroidal: 
> 1. $$s \cup t$$,
> 2. $$s \cap t$$,
> 3. $$s \cup t - s \cap t$$,  and 
> 4. $$s - s \cap t$$. 

This is a simple application of the contraction lemma:
for the first, we fix a solid torus $$T_t$$ about $$t$$ and realize a small enough solid torus $$T_s$$ around $$s$$ so that $$T_s \subset T_t$$.
Then, $$T_t$$ realizes $$s \cup t$$ as a toroidal subweave.
The others are simple.
Proposition 3 follows quickly from Lemma 4.

Another use of Lemma 4.1 characterizes fully toroidal weaves:
> **Proposition 5.** A weave is fully toroidal if and only if every subweave of size 2 is toroidal.

A weave is atoroidal iff it is equivalent to its maximal atoroidal quotient.
A weave is toroidally connected iff its maximal atoroidal quotient is one ring.
Together, we see that the indecomposable pieces with respect to maximal atoroidal quotients are the atoroidal and toroidally connected weaves.

We may visualize this by drawing a labelled tree with one root node labelled by $$w / \cbr{t_i}$$ and $$\abs{\cbr{t_i}}$$-many leaf nodes labelled by $$\cbr{t_i}$$.
We induct this visualization by replacing $$t_i$$ with a tree of a similar form unless it is the one-component weave.
This yields an isomorphism between the symmetric sequence of toroidal weaves and the symmetric sequence of trees whose nonleaf nodes are labelled by atoroidal toroidal weaves of size corresponding with the out-degree of the nodes and whose leaves are labelled by toroidally connected weaves.
Similarly, this yields an isomorphism between the weaves and a similar symmetric sequence, where the root node is simply an atoroidal weave.

One familiar with the technology of operads may recognize this;
we work this out in the language of free operads and free left modules over operads in the next post.

### Further decomposition of toroidally connected weaves
> **Proposition 6.** Suppose $$\abs{w} \geq 3$$. Then, the following are equivalent:
> * $$w$$ has a fully toroidal quotient of size at least 3
> * $$w$$ is toroidally connected.
>
> In the case that $$w$$ is toroidally connected, the partition $$M(w)$$ whose nontrivial partitions are the minimal toroidal subweaves of size at least 3 yields the unique maximal fully toroidal quotient of $$w$$.

First note that $$M(w)$$ has fully toroidal quotient;
to see this, suppose that $$m,m' \subset w$$ are parts.
Since the hypergraph of the quotient is gotten by contracting the hypergraph of the total weave along the parts,  by Lemma 5 it suffices to show that $$m \cup m'$$ is toroidal.
By toroidal connectedness, there is some toroidal subweave $$t$$ such that $$t \cap m$$ and $$t \cap m'$$ are nontrivial.
By minimality, $$m \cup m' \subset t$$.
If $$t \neq m \cup m'$$, then $$\prn{t \cap m} \cup \prn{t \cap m'} \neq \varnothing$$, so Lemma 4.3 implies that $$m \cup m'$$ is toroidal. 

Next note that every toroidal partition with fully toroidal quotient must be coarser than $$M(w)$$; indeed, if $$m \subset w$$ is a nonrivial part which lands in multiple parts of a toroidal partition, then the image of $$m$$ in its quotient is a toroidal subweave of size $$\abs{m} \geq 3$$ whose proper nontrivial subweaves are non-toroidal, preventing full toroidality.

Last, suppose that $$w$$ possesses a fully toroidal quotient of size at least 3;
if $$m,m' \in M(w)$$ are parts, then the image of $$m \cup m'$$ in $$w / M(w)$$ is toroidal, so $$m \cup m'$$ is a (nontrivial proper) toroidal subweave.
Hence $$w$$ is toroidally connected.
This concludes the proof.

The wording of Proposition 6 is a bit weird;
this is because every two component weave is simultaneously fully toroidal and atoroidal, as both conditions are satisfied vacuously.

We can now make a canonical process for decomposition:
you first iterate atoroidal quotients until this halts, in which case you have toroidally connected weaves of size at least 3;
then you iterate maximal fully toroidal quotients until this halts, at which case you have toroidally disconnected weaves of size at least 3.
The indecomposable objects in this decomposition are precisely the atoroidal and fully toroidal weaves.
Luckily, these objects are easy to classify:


### What are the fully toroidal weaves, anyway?
> **Proposition 7.** Suppose $$w$$ is a fully toroidal weave. Then $$w$$ is equivalent to either Möbius $$n$$ or $$n \cdot O$$.

The first step in this proposition is the following definition:
> **Definition 6.** * Given a weave $$w$$, the *linking graph* $$L(w)$$ is the undirected graph whose vertices are $$\abs{w}$$, such that $$c$$ and $$c'$$ are adjacent iff the linking number of $$c$$ and $$c'$$ is nonzero.

The following Lemma is useful for recognizing toroidality.

> **Lemma 8.** Suppose $$t \subset w$$ is a toroidal subweave and $$c,c' \in t$$ are components.
> Then, there is an isomorphism of the linking graph $$L(w)_{/c} \simeq L(w)_{/c'}$$ which sends $$c$$ to $$c'$$ and sends every other vertex to itself. 

We use this to prove Proposition 8.

By the level 2 classification, the two (atoroidal) weaves of size 2 are $$M_2$$ and $$2 \cdot O$$. 
Since every size-2 subweave of a fully toroidal weave is toroidal, such a weave can be generated by repeatedly kinging and Möbiusing $$O$$.

Note that any sequence which includes both kinging and Möbiusing generates a weave who is neither discrete nor fully connected;
by Lemma 8, every fully toroidal weave must then be generated under only kinging or only Möbiusing 
Then, Proposition 7 follows by noting that every $$n$$-component weave generated by kinging is $$n \cdot O$$ and every $$n$$-component weave generated by Möbiusing is $$M_n$$.


### Some worked out examples.
The elements of the <a href="https://docs.google.com/spreadsheets/d/1O0weIB9KkCSFKIvFKhsnYluknzou5wXFCilfTZXy4wQ/edit?usp=sharing">RIM</a> which are realizable with a single ring size appear on first glance to have no redundancy, they cover all of the elements of $$\widetilde W_{\leq 4}$$ that I'm aware of, and they agree with our computation of $$W_{\leq 2}$$.
Our examples will primarily be pulled from this, or generated by RIM elements under toroidal composition.
We will use their naming convention.

This is harder to write than draw, so here's a big drawing:

<div align="center">
	<a href="/assets/RIM atoroidal.png"><img src="/assets/RIM atoroidal.png" align="center" height="2000" ></a>
</div>

### The next step
In the <a href="https://nataliesstewart.github.io/blog/chainmail-math/2022/09/23/operadic-atoroidal-decomposition.html">next post</a>, we will sum up our perspective in terms of operads, and conjecture a topological version of the toroidal decomposition laid out here.
