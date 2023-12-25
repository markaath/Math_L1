
Soient $a\in\mathbb Z^{*}, c\in\mathbb Z, b\in\mathbb N^{*}$
On cherche à résoudre dans $\mathbb Z$ la congruence $(D) : ax\equiv c \;[b]$
On considère l'équation diophantienne $(E)$ associée à $(D)$ : $$(E) : ax+by=c$$

1) Existence de solutions
$(D)$ admet des solutions $\Leftrightarrow \exists x\in\mathbb Z : ax\equiv c\;[b]$
$\Leftrightarrow \exists x\in\mathbb Z : \exists y \in\mathbb Z : c = ax+by$
$\Leftrightarrow$ $(E)$ admet des solutions
$\Leftrightarrow (a\land b)|c$

2) Simplification 
$x$ est solution de $(D)$ ssi $x$ est solution de $(D') : a'x \equiv c' \;[b']$, avec $d=a\land b, a=da', b=db', c=dc'$ 

3) Solution particulière
$(x_{0},y_{0})$ est solution de $(E') \Rightarrow x_0$ est solution de $(D')$
Une méthode pour trouver $(x_0,y_0)$ est de trouver les coefficients de Bézout $(u,v)$ pour $(a',b')$ et de poser $x_{0}= uc'$ et $y_{0}= vc'$

4) Trouver toutes les solutions
Soit $x_0$ une solution de $(D')$. Alors
$\{x\in\mathbb Z : ax\equiv c\;[b]\} = \{x\in\mathbb Z : x\equiv x_0 \;[b']\}$
*Preuve* :
$\Rightarrow$ :
Soit $x_{1}$ une solution de $(D') \Rightarrow \exists y\in\mathbb Z : (x_{1},y_{1})$ est solution de $(E')$
$\Rightarrow \exists k\in\mathbb Z : x_{1}= x_{0}+kb'$ et $y_{1}=y_{0}-kb'$
$\Rightarrow x_{1}\equiv x_{0}\;[b']$
$\Leftarrow$ :
Soit $x_{1}\equiv x_0\;[b']$ alors
$a'x_{1}\equiv a'x_{0}\;[b']$
$\Rightarrow a'x_{1}\equiv c'\;[b']$ car $x_0$ est solution de $(D')$ et $x_1$ est bien solution de $(D')$.

<u>Remarques</u> :
1) $ax\equiv 0\;[b]$ a toujours des solutions et $\mathcal S=\{x\in\mathbb Z : x\equiv 0\;[b]\}$
2) $ax\equiv 1\;[b]$ a des solutions ssi $a\land b = 1$
3) Stratégie alternative pour résoudre $(D') : a'x\equiv c'\;[b']$ :
Quand $b'$ n'est pas trop grand.
- On cherche un inverse multiplicatif de $a'\mod b'$
- Soit $g$ un tel inverse multiplicatif alors $a'g\equiv 1\;[b']$
et $ga'x\equiv c'g\;[b'] \Leftrightarrow x\equiv c'g\;[b']$ et les solutions de $(D')$ sont $\{x\in\mathbb Z : x\equiv c'g\;[b']\}$
