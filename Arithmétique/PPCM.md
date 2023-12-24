Soient $a,b\in\mathbb Z^*$ et $M = \{d\in\mathbb N^{*}: a|d \land b|d\}$
$M\neq \emptyset$ car $|ab|\in M$
Donc $M$ a un plus petit élément et $\min(M)=PPCM(a,b)=a\lor b > 0$

**Propriété** :
Soient $a,b,c \in\mathbb N^{*}, d = a\land b$
1) Soient $a',b' : a'\land b' = 1$ et $a=a'd$ et$b=b'd$
Alors $a\lor b= a'b'd$
2) $(a\lor b)(a\land b) = ab$
3) $a|c$ et $b|c \Rightarrow (a\lor b)|c$
*Preuve* :
1) Soit $m=a'b'd$, montrons que $m=a\lor b$
$b|m$ et $a|m$, donc m est un multiple commun. Soit $n$ un autre multiple commun (ie $a|n$ et $b|n$)
Soit $n' : n= an' = a'dn'$
On a $b=b'd|n=a'dn'$ donc par Gauss $b'|n'$
Soit $n'' : n' = b'n''$ alors
$n=an'=a'db'n''=mn''$ donc $m|n$ en particulier $m\le n$
2) $(a\lor b)(a\land b) = a'b'dd= a'db'd=ab$
3) $a\lor b = da'b', a|c \Rightarrow \exists c' : c=ac', b=b'd|c=ac'=a'dc'$
$\Rightarrow b'|a'c'$ 
Et comme $a'\land b' = 1$, Gauss nous donne $b'|c'$ ie $\exists c'' : c'=b'c''$
Donc $c=ac'=a'db'c''=(a\lor b)c' \Rightarrow (a\lor b)|c$

