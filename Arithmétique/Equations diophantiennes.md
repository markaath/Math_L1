Le but est de trouver tous les couples $(x,y)\in\mathbb Z²$ tels que $ax+by = c := (E)$

1) Existence de solutions 
$(E)$ admet des solutions dans $\mathbb Z$ ssi $a\land b |c$
*Preuve* :
$\Rightarrow$ :
Soient $d=a\land b, (a',b')\in\mathbb Z² : a=da', b=db'$
Alors $c=ax+by = d(a'x+b'y)$, donc $d|c$
$\Leftarrow$ :
Si $d|c$ alors soit $c' : c = dc'$
$a'\land b' = 1 \Rightarrow \exists (u,v)\in\mathbb Z² : a'u+b'v=1$
$a'u+b'v=1\Rightarrow a'dc'u + b'dc'v = dc' = c$
$\Rightarrow ac'u + bc'u = c$
Alors $x=c'u$ et $y=c'v$ sont des solutions de $(E)$.

2) Simplification
Supposons que $d|c$. Alors $(x,y)$ est une solution de $(E)$ ssi $(x,y)$ est solution de $$(E') := a'x + b'y = c'$$
3) Une méthode pour trouver des solutions particulières
On trouve des coefficients de Bézout pour $(a',b')$ et on pose $x_0=uc'$ et $y_{0} = vc'$
*Preuve* :
Si $a'u +b'v = 1$ alors $a'c'u + b'c'v = c'$ et $(x_0,y_0)$ est solution de $(E')$

4) Trouver toutes les solutions
Soit $(x_0,y_0)$ une solution particulière, alors $$\{(x,y)\in\mathbb Z² : ax+by = c\} = \{(x,y)\in\mathbb Z² : \exists k\in\mathbb Z : x = x_{0}+kb' \land y=y_{0}-ka'\}$$
*Preuve* : 
Soit $k\in\mathbb Z$ et soient $x_{1}= x_{0}+ kb'$ et $y_{1}= y_{0}-ka'$
$\Rightarrow$ :
Montrons que $(x_1,y_1)$ est solution de $(E)$
$a'x_1 + b'y_{1}= a'x_{0}+a'kb' + b'y_{0} - b'ka' = a'x_{0} + b'y_{0}$
Or on a posé $(x_0,y_0)$ solution de $(E)$ donc $a'x_{1}+b'y_{1}=ax_{0}+b'y_{0}=c'$
