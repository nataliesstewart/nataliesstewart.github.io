---
layout: base
title: Writings
---

<script type="text/javascript" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"> </script> 

<style>
details {
  border-radius: 4px;
  padding: 0.5em 0.5em 0;
}

summary {
  margin: -0.5em -0.5em 0;
  padding: 0.5em;
  font-size = 15pt;b
}

details[open] {
  padding: 0.5em;
}

details[open] summary {
  margin-bottom: 0.5em;
}
</style>

## Papers
<details> 
<summary>
	<b> An Eckmann-Hilton argument in equivariant higher algebra</b> (2025). <a href="https://arxiv.org/abs/2508.05556">[arxiv]</a>
	</summary>
    If you're familiar with <a href="https://arxiv.org/pdf/1808.06006.pdf">Schlank-Yanovski</a>, this works similarly;
    whereas connectivity of a space is a function on the orbit category, connectivity of a unital \(G\)-operad is most naturally viewed as a function on the poset of unital weak indexing systems (meaning minimum connectivity of \(I\)-admissible \(H\)-sets), and it turns out that connectivity function yields the obvious analog of Schlank-Yanovski's lower bound on Boardman-Vogt tensor products.
    
   We acquire probably the most _algebraic_ intrinsic characterization you can get for (almost unital weak) \(\mathcal{N}_\infty\)-operads:
   they are the targets of \(G\)-\(\infty\)-categorical Eckmann-Hilton arguments, or equivalently, they are the smashing localizations on (almost unital) \(G\)-operads.
</details>


<details> 
<summary>
	<b style="color:#92b99b;">On tensor products with equivariant commutative operads</b> (2025).
	<a href="https://arxiv.org/abs/2504.02143">[arxiv]</a>
    <!--<a href="/files/Ninfty_nightly.pdf">[v1.5]</a>-->
</summary>
	We study cartesian and cocartesian structures in equivariant higher algebra, leading to computations of tensor products of \(G\)-operads with weak \(\mathcal{N}_\infty\)-operads.
	In particular, we find that
	<ul>
	<li>
		The category of (co)cartesian structures on a \(G\)-category with finite indexed (co)products is contractible.
	</li>
	<li>
		Cartesian \(\mathcal{O}\)-algebras can be presented as "\(\mathcal{O}\)-monoids;"
		in particular, \(\mathcal{O}\)-algebras in the catesian structure on coefficient systems are Segal objects over either of the associated algebraic patterns.
	</li>
	<li>
		If \(\mathcal{C}^{\otimes}\) is cocartesian over all arities at which a reduced \(G\)-operad \(\mathcal{O}^{\otimes}\) has nonempty structure spaces and the underlying \(G\)-category of colors of \(\mathcal{O}\) is contractible, then objects of \(\mathcal{C}\) admit <i>contractible</i> moduli of \(\mathcal{O}\)-algbera structures;
		moreover, the converse is true, if you generalize to <i> unital</i> \(I\)-operads.
	</li>
	<li>
		If \(I\) is almost essentially unital and \(\mathcal{O}^{\otimes}\) is almosst essentially reduced, then there is an equivalence \(\mathcal{O} \otimes \mathcal{N}_{I\infty} \simeq \mathcal{N}_{I\infty}\) if and only if \(A\mathcal{O} \leq I\).
		Moreover, the assumptions were necessary:
		if \(I\) is not almost essentially unital, then \(\mathcal{N}_{I\infty}^{\otimes 2}\) is not connected, let alone equivalent to \(\mathcal{N}_{I \infty}^{\otimes}\).
		Hence almost-unital weak \(\mathcal{N}_\infty\)-operads are idempotent algebras, i.e. they classify smashing localizations.
	</li>
	<li>
		There is an equivalence \(\mathcal{O} \otimes \mathcal{N}_{I\infty} \simeq \mathcal{O}\) if and only if the underlying \(I\)-operad of \(\mathcal{O}\) is cocartesian--equivalently, if and only if \(\mathcal{O}\)-algebra \(G\)-spaces have \(I\)-indexed Wirthmüller isomorphisms. 
	</li>
	<li>
		The above point allows you to compute \(\mathcal{N}_{I\infty} \otimes \mathcal{N}_{J \infty} \simeq \mathcal{N}_{I \vee J \infty}\) in the almost-unital setting, affirming the remaining conjecture of <a href="https://arxiv.org/pdf/1309.1750">Blumberg-Hill</a>. 
	</li>
	<li>
		\(\otimes\)-idempotence of \(\mathrm{Comm}^{\otimes}_G\) allows for the <i>sliced</i> equifibered perspective to be symmetric monoidal, leading to an easy construction of a canonical lift of the Boardman-Vogt tensor product to a presentably symmetric monoidal \(G\)-\(\infty\)-category of \(G\)-operads.
	</li>
	<li>
		Lurie's Disintegration and assembly procedure works for \(G\)-space colored \(G\)-operads, on the level of giving natural \(G\)-colimit presentations via one-color \(G\)-operads;
		\(G\)-functorial distributivity of \(\otimes\) allows us to compute tensor products of \(G\)-space colored \(G\)-operads in terms of one-colored \(G\)-operads.
		Put a pin in this--we'll use it for equivariant Dunn additivity with tangential structure.
	</li>
	<li>
		\(A \mapsto \mathrm{RMod}_A\) takes \(\mathcal{O} \otimes \mathbb{E}_1\)-algebras to \(\mathcal{O}\)-monoidal \(\infty\)-categories;
		in particular, right modules over an \(I\)-commutative algebra are given a  natural \(I\)-symmetric monoidal structure when \(I\) is an indexing category.
	</li>
	<li>
		Factorization homology is \(G\)-symmetric monoidal;
		in particular, the above computation lifts \(\mathrm{THR}\) to a natural endofunctor of \(\mathbb{E}_{\infty\sigma}\)-rings.
		As a bit of service, we show how to lift this to a lax \(C_2\)-symmetric monoidal cyclotomic structure, constructing a lax \(C_2\)-symmetric monoidal functor whose induced endofunctor of \(C_2\)-commutative rings is Quigley-Shah's Real topological cyclic homology.
	</li>
	</ul>
</details>

<details> 
<summary>
	<b>Equivariant operads, symmetric sequences, and Boardman-Vogt tensor products</b> (2025).
	<a href="https://arxiv.org/abs/2501.02129">[arxiv]</a>
	<a href="/files/1n_nightly.pdf">[v1.5]</a>	
</summary>
	The purpose of this paper is to set the stage to study the homotopy theory of \(G\)-operads and their Boardman-Vogt tensor products.
	The important constructions are the <i> underlying \(G\)-symmetric sequence</i> and the <i>Boardman-Vogt tensor product of \(G\)-operads</i>.
	The important facts are the following:
	<ul>
		<li>
			The underlying \(G\)-symmetric sequence is monadic.
		</li>
		<li>
			There is a well-behaved localizing subcategory of \(G\)-\(d\)-operads (whose structure spaces are \((d-1)\)-truncated), compatible with all of the constructions.
		</li>
		<li>
			The \(\mathcal{O}\)-\(G\)-coefficient systems functor \(\mathcal{O} \mapsto \mathrm{Alg}_{\mathcal{O}}(\mathrm{Coeff}^G\mathcal{C})\) detects equivalences on the base change of the underlying \(G\)-symmetric sequence to \(\mathcal{C}\);
			in particular, evaluation on \(n\)-truncated \(G\)-spaces detects \(n\)-equivalences of \(G\)-operads and evaluation on \(G\)-spaces is conservative. 
		</li>
		<li>
			The equivariant operadic nerve intertwines everything in sight, so it has a conservative right-derived functor; moreover, it's only the coherences that make things annoying, so it's easy to verify that it's an equivalence on one-color \(G\)-1-operads.
		</li>
		<li>
			The Boardman-Vogt tensor product works as you expect it to and intertwines with the Day convolution structure on \(G\)-symmetric monoidal \(\infty\)-categories via the envelope.
		</li>
	</ul>
	This is not yet submitted; <a href="/files/1n_nightly.pdf">click here for v1.5.</a>
</details>

<details>
<summary>
<!--	<b style="color:#92b99b;">On tensor products of equivariant commutative operads</b> (2024). -->
    <b >Orbital categories and weak indexing systems</b> (2024).
    <a href="https://arxiv.org/abs/2409.01377">[arxiv]</a>
</summary>
    This paper is an exposé on weak indexing systems, the combinatorics behind weak \(\mathcal{N}_\infty\) operads.
    The main point here is to show that, even though it's somewhat more complicated, you can run some version almost all of the homotopical combinatorics you know and love in the more general setting of subterminal \(G\)-operads, perhaps under mild unitality assumptions.

<p>    Submitted.</p>
</details>

<details> 
<summary> <b>Lower Bounds on Volumes of Hyperbolic 3-Manifolds via Decomposition</b> (2021) with <a href="https://sites.williams.edu/cadams/">Colin Adams</a> et al. 
<a href="https://arxiv.org/abs/2111.06319">[arxiv]</a>
</summary>
<p>
Lower bounds on the volumes of hyperbolic link complements are given via a new construction:
  a <i> bracelet link</i> is a link in \(S^3\) decomposed as a cycle of interconnected tangles, and it is proved that a bracelet link of \(2n\) tangles, such that each individual tangle may be <i>replicated</i> into a hyperbolic bracelet link of \(2n\) copies of the tangle, is hyperbolic, with volume at least the average of the replicated links.
</p>
<p>
  This replication is generalized to arbitrary 3-manifolds via a construction called <i>starbursts</i>, which separate the manifold into <i>pieces</i>, which have a well defined \(2n\)-<i>replicant</i>;
  if the resulting pieces from removing a regular neighborhood of a starburst have hyperbolic replicants, then the 3-manifold is hyperbolic, with volume at least the average of the volumes of the replicants. 
</p>
<p>
  Applications are presented to hyperbolicity of links in thickened surfaces and in the solid torus.
</p>
</details>

<details> <summary> 
	<b>Augmented cellular alternating links in thickened surfaces are hyperbolic </b>(2021) with <a href="https://sites.williams.edu/cadams/">Colin Adams</a> et al.
	<a href="https://arxiv.org/abs/2107.05406">[arxiv]</a>
   	<a href="https://link.springer.com/article/10.1007/s40879-023-00692-3">[EJM]</a>
    </summary>
    Work of <a href="https://arxiv.org/abs/1506.03026v1">Colin Adams</a> concerning hyperbolicity of generalized augmented alternating links in the 3-sphere is extended to hyperbolicity of such links in \(I\)-bundles over a surface other than the Klein bottle or \(\mathbf{RP}^2.\)
  This is used to prove hyperbolicity class of links in thickened orientable surfaces called <i> rubber band links </i>, which are generated by graphs.
  Both lower and upper bounds are provided for the volumes of rubber band links, both depending linearly on the number of edges in the graph.
</details>

<br/><br/>  

## In-progress projects to look out for



<details> 
<summary>
<!--	<b style="color:#92b99b;">On tensor products of equivariant commutative operads</b> (2024). -->
	<b>Connectivity of equivariant configuration spaces and \(\mathbb{E}_V\)-algebraic Wirthmüller maps</b>.
	<a style="color:#DEB0FF;" href="/files/Conf_draft.pdf">[draft]</a>
</summary>
    The results in this draft keep getting stronger, and the dependencies heavier;
    as of right now, the _point_ is that you can lift the Fadell-Neuwirth fibration to equivariant configurations, reducing connectivity statements for configurations in \(G\)-manifolds to connectivity and dimension statements in their strata with fixed isotropy. 
    In the case of orthogonal representations, this itself is completely determined by the dimensions of various fixed point spaces;
    surprisingly, this means that the collection of arities \(S\) for which \(\mathbb{E}_V(S)\) is \(n\)-connected is closed under self-indexed coproducts and restruction, i.e. it's a _unital weak indexing system_.
    As a consequence, an easy dimension-counting condition completely classifies the connectivity of the fibers of semiadditive norm maps in the \(G\)-category of \(\mathbb{E}_V\)-\(G\)-spaces, quantifying how close these things are to \(G\)-semiadditivity (and hence how close \(\mathbb{E}_V\)-algebras are to weak \(\mathcal{N}_\infty\)-algebras).
</details>

<details> 
<summary>
	Dimension-shifting multiplicative norms in equivariant homotopy theory.
</summary>
    <p>
        In ongoing work with <a href="https://brankoj.gitlab.io/">Branko Juran</a>, we hope to use equivariant higher algebra to fulfill the conjectures of <a href="https://arxiv.org/abs/2212.11404">Blumberg-Hill-Mandell</a> in the \(\infty\)-categorical setting, replacing strictly commutative algebras with normed algebras (having finite-index norms).
    </p>
</details>

<details> 
<summary>
<b style="color:#92b99b;">Homotopical additivity of equivariant little disk operads</b>.
	<a style="color:#DEB0FF;" href="/files/dunn.pdf">[rough draft]</a>
</summary>
</summary>
   	A not-quite-complete draft which nevertheless does what it says on the tin: we prove \(\mathbb{E}_V \otimes \mathbb{E}_W \simeq \mathbb{E}_{V \oplus W}\).
</details>

<details> 
<summary>
    Modules and cotangent complexes in equivariant higher algebra.
</summary>
    I hope to relitigate Higher Algebra chapter 7 in the setting of \(G\)-operads;
    the aim is to lift the characterization of cotangent complexes from <a href="https://arxiv.org/pdf/1007.5315.pdf">Basterra-Mandell</a> in the setting \(G = C_2\) using the (dihedral) Bar construction of e.g. <a href="https://arxiv.org/pdf/2111.06970.pdf">Knoll-Gerhardt-Hill</a>, in preparation for computations in Real deformation theory. 
    This is ongoing joint work with <a href="https://research-portal.uu.nl/en/persons/ryan-quinn">Ryan Quinn</a>.
</details>

<details> 
<summary>
	All models for \(G\)-operads agree.
</summary>
    <p>
        In ongoing work with <a href="https://www.ru.nl/en/people/marc-g">Gregoire  Marc</a>, we hope to show that the Nardin-Shah and Bonventre-Pereira models for \(G\)-operads agree, ultimately verifying that one can use "monoids in \(G\)-symmetric sequences" in equivariant higher algebra arguments exactly when it's convenient.
    </p>
</details>

<details>
<summary>
	Canonical indexed tensor products of homotopical Mackey functors.
</summary>
	This is ongoing work with <a href="https://sites.google.com/view/bastiaan-cnossen">Bastiaan Cnossen</a>, <a href="https://t-lenz.github.io/">Tobias Lenz</a>, and <a href="https://www.math.uni-bonn.de/people/linskens/webpage.htmpl">Sil Linskens</a>. 
</details>








<br/><br/>  

## Topics I intend to dive into within the next few years





<details> 
<summary>
    The multiplication on \(\mathrm{BP}_{\mathbb{R}}\) and \(\mathrm{BP}_{\mathbb{R}} \langle n \rangle\).
</summary>
    <p>
        I hope to construct canonical lifts of \(\mathbb{E}_{2n}-\mathrm{MU}\)-algebra structures on \(\mathrm{BP}\) to \(\mathbb{E}_{n \rho}-\mathrm{MU}_{\mathbb{R}}\)-algebra structures on \(\mathrm{BP}_{\mathbb{R}}\) using the cellularity results announced in <a href="https://arxiv.org/pdf/1806.11033.pdf">Hill-Hopkins</a> as well as the above conjectures concerning change of group functors applied to equivaraint operadic cotangent complexes.
    </p>

    <p>
    After doing so, I hope to add \(\mathbb{R}\) and \(C_2\), as well as replace \(3\) with \(2 \rho - 1\), in section 2 of <a href="https://arxiv.org/pdf/2012.00864.pdf">Hahn-Wilson</a> and claim the new result as my own.
    </p>
</details>

<details> 
<summary>
    Infinite loop space theory for equivariant associative operads?
</summary>
    <p>
    Lately, I've started to believe that some \(\mathcal{N}_\infty\)-operads are "exotic" in the sense that they do not arise as a filtered colimit of operads satisfying recognition principles in equivariant algebraic topology. 
    I hope to either exhibit some such examples, or (more likely) verify that no such examples exist.
    </p>
</details>





<br/><br/>  

## Notes and other things
<details>
<summary> 
Slides: 
<b> Homotopy-coherent interchange and equivariant little disk operads</b>
<a href="/files/dunn_archive.zip">[source]</a>
<a href="/files/dunn_handout.pdf">[handout]</a>
</summary>
	Slides for a talk in Belfast.
</details>

<details>
<summary> 
<b> A directory of higher G-algebra.</b>
<a href="https://www.overleaf.com/read/pryjbtypsgph#4c3fcc">
[overleaf]</a> <a href="/files/higher_galgebra.pdf">[pdf]</a>
</summary>
a living document intended to serve as a companion to <a href="https://people.math.harvard.edu/~lurie/papers/HA.pdf">Higher algebra</a>, giving citations to equivariant lifts of its greatest hits.
</details>

<details>
<summary> 
<a href="/files/ninftynotes.pdf">
    You can construct G-commutative algebras one norm at a time
</a>
</summary>
    a draft of some <a href="https://zygotop.github.io/">Zygotop</a> lecture notes, complete with many errors, about the additivity of \(N_\infty\)-operads.
</details>

<details>
<summary> 
<a href="/files/borromean.pdf">You can't make the Borromean rings out of chainmail</a>
</summary>
 lecture notes for a talk at Harvard's "trivial notions" seminar.
</details>


<details> <summary> <a href="https://math.mit.edu/research/undergraduate/spur/documents/2019Johnson-Stewart.pdf">Some graphical realizations of two-row Specht modules of Iwahori-Hecke algebras of the symmetric group (2019).</a> Joint with Miles Johnson.
    </summary>
  Studies a generalization of Khovanov's "crossingless matchings" representation of an Iwahori-Hecke Algebra of the symmetric group to include a particular number of endpoints on the "bottom" and "top";
  in the generic case, such a representation is proven to be isomorphic to a two-row Specht module whose young partition corresponds with the number of endpoints.
  Some heuristics are given towards existence of such an isomorphism in all cases.
  In the characteristic-5 case, some irreducible subrepresentation of Jordan-Shor's Fibonacci representation are given, and these are proven to be isomorphic to the irreducible quotients of two-row Specht modules whose rows differ by length at most 3.
</details>
