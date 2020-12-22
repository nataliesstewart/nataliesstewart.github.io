---
layout: post
title:  "Toposes, presheaves, and free categories 1"
date:   2020-12-19
categories: applied-category-theory
---
<script type="text/javascript" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"> </script> 
<link rel="stylesheet" type="text/css" href="https://tikzjax.com/v1/fonts.css">
<script src="https://tikzjax.com/v1/tikzjax.js"></script>
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

\newcommand{\id}{\operatorname{id}}
\newcommand{\STan}{\mathbf{sTAN}}

\newcommand{\bm}{\mathbf{m}}
\newcommand{\by}{\mathbf{y}}
\newcommand{\bC}{\mathbf{C}}
\newcommand{\bE}{\mathbf{E}}
\newcommand{\bS}{\mathbf{S}}

\newcommand{\cT}{\mathcal{T}}

\newcommand{\NN}{\mathbb{N}}

\newcommand{\Poly}{\mathbf{Poly}}

\newcommand{\Sub}{\operatorname{Sub}}

\newcommand{\Set}{\mathbf{Set}}

\newcommand{\op}{\text{op}}

\def\Nat{\operatorname{Nat}}
\def\Free{\operatorname{Free}}
$$

Please ignore this, which hopefully should be a circle.
<script type="text/tikz">
   \begin{tikzpicture}
     \node (A) at (0,1) {$A$};
     \node (1) at (1,1) {$1$};
     \node (X) at (0,0) {$X$};
     \node (O) at (1,0) {$\Omega$};
     \path[draw,white] (A) -- (X);
     \path[draw,white] (A) -- (1);
     \path[draw,white] (1) -- (O);
     \path[draw,white] (X) -- (O);
   \end{tikzpicture}
</script>

**this is incomplete!**

This post will largely consist of information which exists at nlab, and I will be a bit terse.
My goal here is to summarize the notions of a *presheaf topos* and a *free category* so as to use them later to do more interesting and original stuff.

I will assume basic knowledge of category theory, and will only give a handwavy sketch of basics of topos theory.
Refer to <a href="https://www.springer.com/gp/book/9781461298397">*Categories for the Working Mathematician* by Mac Lane</a> for the free category things and <a href="https://www.springer.com/gp/book/9780387977102">*Sheaves in Geometry and Logic* by Mac Lane and Moerdijk</a> for the topos theory things.

*(last updated: December 22, 2020)*

### Toposes at a glance

Let $$\bC$$ be a category.
The *category of presheaves on $$\bC$$* is $$\Set^{\bC^{\op}}$$, i.e. the category of contravariant functors $$\bC^{\op} \rightarrow \Set$$ and natural transformations between them.
The *yoneda embedding* is the functor $$\by:\bC \rightarrow \Set^{\bC^{\op}}$$ sending $$X \mapsto \bC(-,X)$$, and a functor in the essential image of the yoneda embedding is called *representable*.
Yoneda's lemma implies that $\by$ is fully faithful.

For $$X \in \bC$$, the *category of subobjects of $$\bC$$*, called $$\Sub_\bC(X)$$ is the full subcategory of the slice category $$\bC/X$$ of bundles over $$X$$, whose objects are the monics $$A \rightarrowtail X$$.
Some elementary arguments yield that this is a poset, and morphisms correspond with factorization of monics $$A \rightarrowtail B \rightarrowtail X$$.
In the case that $$\bC$$ is locally small, taking the underlying set of this poset yields a presheaf $$\Sub:\bC^{\op} \rightarrow \Set$$.

Suppose that $$\bC$$ has a terminal object $$1$$.
We say that a *subobject classifier* of $$\bC$$ is a morphism $$\top:1 \rightarrow \Omega$$ such that every monic $$A \rightarrowtail X$$ is expressed as the pullback of a unique morphism along $$\top$$;
diagramatically, this is expressed as

<p align="center">
<a href="/assets/freetopos1_1.png"><img src="/assets/freetopos1_1.png" align="center" height="100" ></a>
</p>

Now supposing that $$\bC$$ is finitely cocomplete and locally small, this is equivalent to $$\Omega$$ being a representing element for $$\Sub$$, i.e. it is equivalent to requiring that there exists a natural isomorphism
<p align="center">
  $$\Sub(-) \simeq \bC(-,\Omega).$$
</p>
This is unique up to isomorphism by Yoneda's lemma.

A *topos* is a cartesian closed, finitely cocomplete category possessing a subobject classifier.
We will care primarily about toposes as generalizations of $$\Set$$ for doing logic, in a way which will become clear later.
We will give the relevant example of toposes now.

### The presheaf topos
One early example of a topos is the presheaf category $$\Set^{\bC^{\op}}$$.
This category is bicomplete and cartesian closed, as (co)limits and exponentials may be computed pointwise.
We will soon give the subobeject classifier for $$\Set^{\bC^{\op}}$$ to verify that it is a topos, first characterizing what it *must* be in order for $$\Set^{\bC^{\op}}$$ to have a subobject classifier.

Suppose such a subobject classifier $$\Omega$$ exists;
then,
<p align="center">
  $$ \Sub_{\bC^{\op}}(\by X) \simeq \Nat(\by X,\Omega) \simeq \Omega(X) $$
</p>
by Yoneda's lemma, naturally in $$X$$.
Hence characterizing subobjects reduces to characterizing subfunctors of $$\by X$$.

Say that a *sieve on $$X$$* is a set of arrows $$S$$ having codomain $$X$$ such that, whenever $$g \in S$$ and $gf$ is defined, we have $$gf \in S$$.
This is sort of like a *right ideal* on the arrows with codomain $$X$$.

There is a natural correspondence between sieves on $$X$$ and subfunctors of $$\by X$$, which gives the object map of the presheaf $$\Omega$$.
Naturality gives that the restriction map of $$\Omega(X)$$ is given by the *pushforward map* on $$\by X$$, which is realized by the corresponding map of sieves.

### Free categories
To consider a presheaf category, we need a category.
Why not choose a free one?

Let $$G:A \rightrightarrows N$$ be a graph (by which, of course, I mean a quiver).
Then, the *free category* $$\Free(G)$$ has as objects $$N$$ and as morphisms $$\Free(G)(X,Y)$$ the paths of finite (possibly zero) length from $$X$$ to $$Y$$ in $$G$$, with composition given by concatenation.
The free category construction forms a left adjoint to the forgetful functor from categories to graphs.
Note that $$\Free(G)^{\op} \simeq \Free(G^{\op})$$, where the latter graph has arrows reversed.

These are nicely structured;
for instance, note that every morphism in a free category is both epic and monic.
I'm more interested, however, in considering the *presheaf topos* on a free category.

Note that, presheaves on $$\Free(G)$$ are equivalent to graphs homomorphisms $$G^{\op} \rightarrow \Set$$;
that is, it is a set $$N(X)$$ for each node $$X$$ and a map $$N(Y) \rightarrow N(X)$$ for each morphism $$f:X \rightarrow Y$$ which is functorial.

We can come up with some examples;
note that $$\Set^{\Free\prn{\prn{\bullet \rightrightarrows \bullet}^{\op}}} = \Set^{\bullet \rightrightarrows \bullet}$$ is the category of pairs of sets $$A,N$$ with parallel arrows $$A \rightrightarrows N$$;
that is, it forms the category of graph.
This was explored in <a href="http://vigna.di.unimi.it/ftp/papers/ToposGraphs.pdf">this paper by Sebastiano Vigna</a>.

For a similar feeling example, let $$\omega$$ be the first countable ordinal, i.e. the natural numbers under the usual order $$\leq \subset \NN\times \NN$$.
Note that $$\omega$$ is a free category on the graph with nodes $$\NN$$ and arcs $$i \rightarrow i+1$$.
Using this, a presheaf on $$\omega$$ corresponds with an $$\NN$$-indexed collection of sets $$(X_i)_{i \in \NN}$$ with morphisms $$p_i:X_i \rightarrow X_{i-1}$$.

There is an equivalence of categories between $$\Set^{\omega^{\op}}$$ and the category of *forests of potentially infinite height*;
the nodes at height $$i$$ are given by $$X_i$$, and the parent of a node $$x \in X_i$$ is $$p(x_i)$$.
For details, see <a href="https://content.iospress.com/articles/fundamenta-informaticae/fi32-1-02">this paper by Stefano Kasangian and Sebastiano Vigna.</a>

---

On the next episode, I'll go more in depth on some examples of what *being a topos* buys us for presheaves on particular free graphs. 
In particular I'll work some examples of topologies on presheaf toposes on free graphs, and we'll see what those buy us. 


