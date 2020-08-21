---
layout: post
title:  "Categorical structures on the l-pieces part 2"
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

\newcommand{\id}{\operatorname{id}}
\newcommand{\STan}{\mathbf{sTAN}}

\newcommand{\bm}{\mathbf{m}}
\newcommand{\bE}{\mathbf{E}}
\newcommand{\bS}{\mathbf{S}}

\newcommand{\cT}{\mathcal{T}}

\newcommand{\NN}{\mathbb{N}}

$$

See <a href="https://nataliesstewart.github.io/blog/geometric-topology/2020/08/20/the-l-pieces-1.html">part 1 here.</a>

# Theory of $$n$$-fold categories
In this post, my goal is to describe the category theory concept underlying the $$\ell$$-pieces.
This is a construct called _$$n$$-fold categories_, the more complicated and less useful cousin of $$n$$-categories.
I'll mostly focus on the $$n=2$$ case of _double categories_, since they generally seem more studied.
Then, I'll give a notion of _sqaure tangles_ which runs parallel to the study of pieces, but is a lot easier to work with.
In a future post, I'll bring $$\ell$$-pieces back.

**This'll mostly be a restatement of $$n$$Lab** plus some personal thoughts.
We'll be mostly concerned with the simple structure of $$n$$-fold categories;
if you're interested, there is some <a href="https://ncatlab.org/nlab/show/double+category#FPPModel">present work being done by Moser, Sarazola, and Verdugo on Quillen model structures on the category of double categories.</a>, but this is irrelevant, so I won't mention it further. 

### What an $$n$$-fold category is
Recall that (modulo size issues) an $$n$$-category is simply a category enriched in the $$(n-1)$$-categories.
We'll give a similar definition for $$n$$-fold categories, but to do so I'll give a little bit of exposition on internal categories.
The notation will follow MacLane's "Categories for the working mathematician."

**Definition.**
Let $$\bE$$ be a category.
A *category  internal to $$\bE$$ is the following data

* an _object of objects_ $$C_0 \in \bE$$,

* an _object of arrows_ $$C_1 \in \bE$$,

* an _identity arrow_ $$i:C_0 \rightarrow C_1$$,

* _domain and codomain arrows_ $$d_0,d_1:C_1 \rightarrow C_0$$, and 

* a _composition arrow_ $$\gamma:C_1 \times_{C_0} C_1 \rightarrow C_1$$ defined on the pullback:

<p align="center">
![the pullback](/assets/lpieces2_1.png =300px)
</p>

such that $$d_0i = \id = d_1i$$ so that identity arrows have the right (co)domain and such that the following diagrams commute, establishing identity, (co)domain of the composite, and associativity of composition.

<p align="center">
![identity](/assets/lpieces2_2.png =300px)
</p>
<p align="center">
![codomain](/assets/lpieces2_3.png =300px)
</p>
<p align="center">
![associativity](/assets/lpieces2_4.png =300px)
</p>


We can define internal functors in exactly the way one expects;
they are pairs of morphisms between the object and arrow objects which are compatible with the above data.
Hence there is a well-defined notion of a _category of internal categories in $$\bE$$_.

This implicitly requires that the pullback $$C_1 \times_{C_0} C_1$$ exists, as well as a few others.
In the case that $$\bE$$ has all pullbacks, an internal category can be shown to be precisely a monad in the bicategory of spans in $$\bE$$, though I won't go into depth (see <a href="https://ncatlab.org/nlab/show/internal+category">nlab</a> for details).

We'll handwave existence of pullbacks away, since we only work with finitely complete categories.  
In fact, the following theorem due to Charles and Andrée Ehresmann (and which appears directly proven in <a href="https://ncatlab.org/nlab/show/internal+category#CartesianClosure">nlab</a>) let's us handwave this away.

**Theorem.**
Suppose $$\bE$$ is finitely complete.
Then, the category of internal categories in $$\bE$$ is also finitely complete.
The same applies for finitely complete cartesian closed categories. 

When $$\bE = \mathbf{Set}$$, these are precisely the cateory axioms;
hence a (small) category is simply a category object in $$\mathbf{Set}$$.
You can probably guess where this is going...

**Definition.** A *1-fold category* is simply a small category.
An *$$n$$-fold category* is a category internal to the category of $$(n-1)$$-fold categories. 

This is neat, but perhaps too neat.
Now, I'll go into detail on how to picture these, with a heavy focus on double categories.

### What an $$n$$-fold category _really_ is

Let's draw a double category $$D_1 \rightrightarrows D_0$$
It may be said to consist of the following:

* *objects* given by the objects of $$D_0$$.

* *vertical morphisms* given by the morphisms of $$D_0$$.

* *horizontal morphisms* given by the objects of $$D_1$$.

* *2-cells* given by the morphisms of $$D_1$$.

This can be pictured via the following square:

<p align="center">
![square](/assets/lpieces2_5.png =300px)
</p>

The data of a double category may be summarized by horizontal and vertical "edge categories," as well as horizontal and vertical "2-cell categories" which are compatible with the edge categories and satisfy the *interchange law* specifying that the following composite is well-defined.

<p align="center">
![interchange](/assets/lpieces2_6.png =300px)
</p>

We will prefer this type of description, as it shows symmetry;
there is an evident *transpose double category* given by interchanging the vertical and horizontal direction. 
There exists a Poincaré dual calculus of <a href="https://arxiv.org/pdf/1612.02762.pdf">string diagrams for double categories, due to Myers</a>, but we won't think too hard about that, in part because I'm not sure the same exists for $$n$$-fold categories.

The reader can take it upon themself to work through an analogous construction of $$n$$-fold categories being built up from $$n$$-dimensional hypercubes, where a pair of opposing $$m$$-dimensional facets in an $$(m+1)$$-dimensional face describes an $$m$$-fold category;
i haven't formalized this, but I'm fairly certain that any permutation on $$n$$ letters can transform an $$n$$fold category into another one by permuting the opposin pairs of facets.
This is not the relevant kind of abstract nonsense, so I mention it only in passing.

### The square tangles as an double category with one object
There's some extra niceness that comes along with higher category theory for whom most of the structure is simple;
for instance, a category with one object is a (small) monoid, and a 2-category with one object is a (small, strict) monoidal category.

There's an analogous but unfamiliar structure to a one-object double category, which appears as a pair of *horizontal and vertical monoids* and a set of *crossed morphisms* with horizontal and vertical composition which are compatible with the horizontal and vertical monoids, which are each monoidal, and which satisfy an interchane law.
This structure was described in this <a href="https://math.stackexchange.com/questions/2395428/whats-a-double-category-with-one-object">this math exchange post,</a>

The square tangles will be defined with precisely this structure, and later the $$\ell$$-pieces will be defined with a similar triviality for $$\ell$$-fold categories.

**Definition.**
Let $$R$$ be the square, and let $$\partial R = \bigcup_{i=1}^{2} F_{1i} \cup F_{2i}$$ be the decomposition of the boundary of the square into two pairs of opposing edges.
We define a *square tangle* to be a tangle in $$(R,\bigcup F_{ij} - \bigcup F_{ij} \cap F_{kl})$$.
Doubling this individually across each pair of faces yields a link in a thickened torus;
if this link is hyperbolic, we say that the square tangle is *hyperbolic.*

Two square tangles with the same number of endpoints on opposing edges have a clear notion of *vertical* or *horizontal* composition done by gluin, depending on which edges are being glued together. 

It's a consequence of the main theorem of the forthcoming paper that a link which subdivides into a hyperbolic square tangle is hyperbolic, and a square tangle which decomposes into two hyperbolic square tangles is hyperbolic.
There are lower bounds on volumes going along with that, but we won't worry to much.
I'd rather give a double category.

**Definition.**
We define the double category $$\STan$$ by the following data:

* there is a single object $$*$$.

* the horizontal and vertical edge monoids are each given by $$\NN$$ under addition.

* the set of 2-cells is given by the square tangles, where the top and bottom edges are given by the number of endpoints on $$F_{11}$$ and $$F_{21}$$, and similarly the left and right edges are given by the number of endpoints on $$F_{12}$$ and $$F_{22}$$.
  
* composition of 2-cells is given by the composition of square tangles.

Interchange is clear, as it follows by associativity of "topoloical gluing."
The vertical identity $$2$$-cell $$\id_n^\cdot$$ is given by the square tangle with $$n$$ uncrossing vertical strands;
the horizontal identity $$2$$-cell $$\id_n^\circ$$ is the transpose of this.

### The double sub-category of hyperbolic square tangles and braids
Unfortunately, none of the identity $$2$$-cells are hyperbolic;
since they constitute $$4n$$ parallel loops in a thickened torus, and hence have an essential annulus made by a thickened parallel loop in the same direction.
However, there is something we can say:

**Definition.**
We say that a square tangle is a *braid* if it has endpoints only on two opposing faces, and the (classical) tangle formed by only considering those two faces is a braid. 

These work well with composition:

**Proposition.**
Suppose $$\mathcal{T}$$ is a square tangle and $$\mathcal{T'}$$ is a vertical braid such that the vertical composition $$\cT \cdot \cT'$$ is defined.
Then, the quadruple of $$\cT$$ is identical to the quadruple of $$\cT \cdot \cT'$$;
hence $$\cT$$ is hyperbolic if and only if $$\cT \cdot \cT'$$ is hyperbolic.

Hence we may define a double sub-category of the square tangles, with the same 0- and 1-cells, and 2-cells given by those square tangles who are either braids or hyperbolic.


