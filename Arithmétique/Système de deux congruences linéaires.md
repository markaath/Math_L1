
Soient $(a_{1},a_{2})\in\mathbb {Z^{*}}², (b_{1},b_{2})\in\mathbb {N^{*}}², (c_{1},c_{2})\in\mathbb Z²$
On supposera sans perte de généralité que $a_{1}\land b_{1}=a_{2}\land b_{2}=1$

On cherche à résoudre $(S) : \begin{cases}a_{1}x\equiv c_{1}\;[b_{1}]\quad (l_{1})\\ a_{2}x\equiv c_{2}\;[b_{2}]\quad (l_{2})\end{cases}$
Une condition <u>nécessaire</u> (pas suffisante) pour que $(S)$ ait des solutions est : $[(a_{1}\land b_{1})|c_{1}]\;\land\; [(a_{2}\land b_{2})|c_{2}]$

Dans ce cas on simplifie $(l_{1})$ par $a_{1}\land b_{1}$ et $(l_{2})$ par $a_{2}\land b_{2}$. Ici, on supposera sans perte de généralité que $a_{1}\land b_{1}=a_{2}\land b_{2}=1$

On résout séparément les deux congruences : $$(S) \Longleftrightarrow \begin{cases}x\equiv x_1\;[b_{1}]\\ x\equiv x_{2}\;[b_{2}]\end{cases}$$
**Si $b_{1}\land b_{2} = 1$** :
	Alors $\exists (u,v)\in\mathbb Z² : ub_{1}+vb_{2}=1$
	Donc $b_{1}u \equiv 1\;[b_{2}]$ et $b_{2}v\equiv 1\;[b_{1}]$
	Soit $x_{0}= b_{1}ux_{2}+b_{2}vx_{1}$ alors
	$x_{0}\equiv b_{1}ux_{2}\equiv x_{2}\;[b_{2}]$ et $x_{0}\equiv b_{2}vx_{1}\equiv x_1 \;[b1]$
	D'où $x_0$ est solution de $(S)$ et 
	$(S)\Longleftrightarrow \begin{cases}x\equiv x_{0}\;[b_{1}]\\ x\equiv x_{0}\;[b_{2}]\end{cases} \Longleftrightarrow x\equiv x_{0}\;[b_{1}b_{2}]$
	$\Leftrightarrow \mathcal S = \{x\in\mathbb Z : x\equiv x_{0}\;[b_{1}b_{2}\}$

**Si $b_{1}\land b_{2}\neq 1$** :
	$(S)$ a des solutions ssi $(b_{1}\land b_{2})|(x_{2}-x_{1})$
	On pose $d=b_{1}\land b_{2},\; b_{1}= db'_{1},\; b_{2}=db'_{2},\; b'_{1}\land b'_{2} = 1$
	On cherche des coefficients de Bézout pour $(b'_{1},b'_{2})$ :
	Soient $(u,v) \in\mathbb Z² : ub'_{1}+ vb'_{2} = 1$
	Alors $x_{0}=ub'_{1}x_{2}+vb'_{2}x_{1}$ est solution de $(S)$ et l'ensemble des solutions est :
	$\{x\in\mathbb Z : x\equiv x_{0}\;[b_{1}\lor b_{2}\}$
