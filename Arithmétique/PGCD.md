
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

**Algorithme d'Euclide** :
Comme $a\land b = a\land (-b)$ et $a\land 0 = |a|$, on va supposer, sans perte de généralité, $(a,b)\in\mathbb {(N^*)}²$

On fait la DE de $b$ par $a$ :
$b=aq_{1}+ r_1$
On sait que $a\land b = a\land r_1$ donc si $r_{1}= 0$ alors $a\land b = a\land 0 = a$ et si $r_{1}>0$ alors on fait le DE de $a$ par $r_1$ :
$a=r_1q_{2}+ r_2$ idem

$\forall i\in[\![1,(n+1)]\!]$ on a $b>a>r_1>r_2>...>r_{n+1}\ge 0$
Alors $\exists n\in\mathbb N : r_{n}\neq 0$ et $r_{n+1} = 0$
Et par construction on a $a\land b= a\land r_{1}= r_{1\land}r_2=...=r_{n}\land 0 = r_n$

**Définition** :
Soient $(a,b)\in\mathbb Z$ $a$ et $b$ sont premiers entre eux $\Leftrightarrow a\land b = 1$

**Lemme** :
Soient $(a,b)\in\mathbb {(Z^{*)}²,}d:=l a\land b$ ie $\exists (a',b')\in\mathbb Z² : a= da'$ et $b=db'$
Alors $a'\land b' = 1$
*Preuve* :
Soit $d'=a'\land b'$ et soient $(a'',b'')\in\mathbb Z² : a'=da''$ et $b'=db''$
Donc $a=da'=dd'a''$ et $b=db'=dd'b''$
Donc $dd'\le d$ par définition du $PGCD$ 
Donc $d'\le1$ mais $d'\ge 1$ car $d'=a'\land b'$
Donc $d'=1$

**Théorème de Bézout** :
$\forall (a,b)\in(\mathbb Z^*)²,\exists (u,v)\in\mathbb Z : a\land b = au+bv$
On dit que $u$ et $v$ sont des coefficients de Bézout pour $a$ et $b$.

**Algorithme d'Euclide étendu** :
*Exemple* :
$60\land 14$ On cherche $(u,v)\in\mathbb Z² : a\land b = au+bv$
$60 = 14 \times 4 + 4$ $\qquad r_1=4=60\times 1 - 14\times 4$
$14 = 4 \times 3 + 2$ $\qquad r_{2}= 2 = 14 \times 1 - 3 \times 4 = 14 \times 1 - 3\times (60\times 1 - 14 \times 4)= -3 \times 60 + 13\times 14$

Et $60\land 14 = -3  \times 60 + 13 \times 14= 2$

**Conséquence du théorème de Bézout** :
1) Soient $(a,b,d)\in\mathbb {(N^*)}³$
$d|a$ et $d|b \Rightarrow d|a\land b$
*Preuve* :
Par Bézout, $\exists (u,v)\in\mathbb Z² : au+bv = a\land b$
$d|a \Rightarrow d|au$ et $d|b\Rightarrow d|bv$ donc $d|au+bv=a\land b$
2) Soient $(a,b)\in\mathbb (N^*)³, a\land b = 1 \Leftrightarrow \exists(u,v)\in\mathbb Z:au+bv=1$

**Lemme de Gauss** :
Soit $a,b,c\in\mathbb N^*$
Si $a|bc$ et $a\land b = 1$ alors $a|c$
*Preuve* : 
Par Bézout $\exists (u,v)\in\mathbb Z² : au+bv = 1$
$\Rightarrow auc+bvc = c$ et $a|auc$ et $a|bc$
$\Rightarrow a|bvc$
$\Rightarrow a|auc+bvc=c$

**Corollaire au lemme de Gauss** :
Soient $a,b,c\in\mathbb N^{*}: a\land b = 1$
Si $a|c$ et $b|c$ alors $ab|c$
*Preuve* :
$b|c \Rightarrow \exists c_1\in\mathbb N : c= bc_1$
$a|c=bc_{1}$ et $a\land b = 1 \Rightarrow a|c1$
$\Rightarrow \exists c_{2}\in\mathbb N : c1 = ac_2$
$\Rightarrow c = bc_1=abc_{2}\Rightarrow ab|c$


