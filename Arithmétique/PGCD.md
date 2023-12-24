
Soient $a\in\mathbb Z^{*},b\in\mathbb Z, D = \{d\in\mathbb Z : d|a \land d|b\}$.
$D\neq\emptyset$ car $1\in\mathbb Z$ en effet $a\neq 0 \land d|a \Rightarrow d\;\big|\left|a\right|$ 
donc $-|a|\le d\le |a|, \forall d\in D$
D'où $D$ est fini et non vide donc il admet un maximum et $\max(D)\ge 1$ car $1\in D$

**Définition** :
Soient $(a,b)\in\mathbb Z² : a\neq 0$ ou $b\neq 0$
$PGCD(a,b) = a \land b : = \max(D)$

**Propriétés** :
- $a\land b = b\land a = (\pm a)\land (\pm b) \ge 1$
- $0\land b = |b|$
- $1\land b = 1$
**Lemme** :
Soient $a\in\mathbb N^{*}, b\in\mathbb Z : b = aq+r$ avec $0\le r < a$
Alors $a\land b = a\land r$
**Corollaire** :
Soient $a\in\mathbb N^{*}, (b,c)\in\mathbb Z², 0\le r < a$
Alors :
1) $b$ et $c$ ont le même reste $r$ dans la DE par $a$ $\Leftrightarrow b\equiv c \;[a]$
2) $b\equiv c\;[a] \Leftrightarrow a\land b = a\land c$
*Preuves* :
1) 
$\Rightarrow$ :
Soient $(q,q')\in\mathbb Z² : b = qa+r \land c = q'a+r$
Donc $b-c = qa+r -q'a -r = a(q-q')$
et $b-c\equiv 0\;[a] \Rightarrow b\equiv c\;[a]$
$\Leftarrow$ :
$b\equiv c\;[a] \Rightarrow \exists k \in\mathbb Z : b-c \equiv b-c= ka$
$\Rightarrow \begin{cases} b=qa+r\\ c=q'a+r'\end{cases}$ 
$\Rightarrow \exists k\in\mathbb Z : ka=a(q-q') + (r-r')$
$\Rightarrow a(k-q+q')= r-r'$
$\Rightarrow r\equiv r'\;[a]$
$\Rightarrow \exists l\in\mathbb r=r'+la$
Or on a :
$\begin{cases} 0\le r < a\\0\le r' <a\end{cases}$ 
$\Rightarrow \begin{cases} 0\le r'+la<a\\0\le r'<a\end{cases}$
$\Rightarrow \begin{cases} la\le r'+\lambda< a\\-r'>a\end{cases}$
$\Rightarrow \begin{cases} la< a \\la>-a\end{cases}$ car $la\ge -r'>a$
$\Rightarrow -a < la <a \overset{a\neq 0}{\Rightarrow} -1<l<1 \Rightarrow l=0$
D'où $r=r'+0\times a = r'$

2) Montrons que $b\equiv c\;[a] \Rightarrow a\land b= a\land c$
$b\equiv c\;[a] \Rightarrow \exists (q,q')\mathbb Z² : b=aq+r \land c=aq'+r, 0\le r<a$
Le lemme précédent nous donne $b\land a = r\land a= c\land a$
