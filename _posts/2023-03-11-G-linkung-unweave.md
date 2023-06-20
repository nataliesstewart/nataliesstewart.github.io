---
layout: post
title:  "Chainmail math 10: linking detects the G-unweave"
date:   2023-06-20
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
Let $$G$$ be a group acting on $$\RR^3$$ through isometries.
This note serves to note that <a href="/blog/chainmail-math/2023/03/17/linking-unweave.html"> the previous post concerning linking </a> is naturally $$G$$-equivariant:
the (non-equivariant) linking graph, which is weaker than the $$G$$-equivariant linking graph, detects the $$G$$-equivariant unweave.

See the bottom of the <a href="https://nataliesstewart.github.io/blog/chainmail-math/2022/09/09/the-moduli-space-of-weaves.html">first post in the series on chain mail mathematics</a> for a table of contents.

### The linking graph is equivariant and graded
Our construction of the <a href="/blog/chainmail-math/2023/03/17/linking-unweave.html">linking graph</a> was manifestly equivariant;
that is, we supplied a function $$\cW \rightarrow \cbr{\mathrm{Graphs \; in \; } \RR^3}$$, which happens to be equivariant for the evident $$\GG$$-action on the target space.

By Elmendorf's theorem, this data is equivalent to a natural transformation 
<p align="center">
    $$L^G:\cW^G \rightarrow \cbr{G\mathrm{-equivariant\;graphs\;in\;}\RR^3}.$$
</p>
To provide a grading to this graph is equivalent to upgrading this to a natural transformation over $$\pi_0 \Set^{BG}$$.
In fact, this is easy;
the map $$|-|:\cbr{G\mathrm{-equivariant\;graphs\;in\;}\RR^3} \rightarrow \pi_0 \Set^{BG}$$ is given by taking the underlying set of vertices and associated $$G$$-action, which is evidently natural and makes the required diagram commute.



### (Non-equivariant) linking detects the $$G$$-unweave
> **Theorem 1.** Let $$X$$ be the space of $$G$$-weaves of component set $$S$$ such that $$L(w)$$ is trivial, i.e. no pairs of components are linked.
> Then, $$X$$ is connected. 

The first step is already done:
let $$\iota: X_\varepsilon \hookrightarrow X$$ denote the subspace of weave realizations such that the radius $$\rho(w)$$ is at most $$\varepsilon d(c,c')$$ for all components $$c,c'$$.
Then, the non-equivariant proof constructed paths from weave relizations in $$X$$ to those in $$X_\varepsilon$$;these paths preserve centers and normals, hence they are $$G$$-equivariant.
Together, these form a deformation retract of $$X$$ onto $$X_\varepsilon$$, so $$\iota$$ is a homotopy equivalence, and we can just prove that $$X_\varepsilon$$ is connected.

The proof that $$X_\varepsilon$$ is connected is not too hard:
first note that, by separately orienting the rings within their respective $$\varepsilon \operatorname{min}_{c,c'} d(c,c')$$ balls, we have the following:
> **Lemma 2.** There is an equivalence $$X_\varepsilon \simeq \prn{\RRP^2}^n \times \Map(S,\RR^3)^G$$.

Having proved this, the first factor is obviously connected, so we just have to prove the same for the second.
This is the key geometric input: 
for an orbit $$G/H \simeq \langle s \rangle \subset S$$, write $$R := S \backslash \prn{\langle s \rangle}$$, so that
<p align="center">
    $$\begin{align*}
        \Map(S,\RR^3)^G &\simeq \Map(\langle s \rangle, \RR^3 - R)^G\\
        &\simeq \prn{\RR^3 - R}_H\\
        &\simeq \RR^3_H - R_H.
    \end{align*}$$
</p>
Hence it is sufficient to prove that the complement of a discrete set of points in the 3-manifold $$\RR^3_H$$ is (path-)connected.
This is true for any manifold of dimension 2 or higher;
indeed, *any* path in $$\RR^3_H$$ can be isotoped to one which doesn't intersect $$R_H$$, by a routine general position argument.
<span style="float:right;font-size:25px;">
        □
</span>
