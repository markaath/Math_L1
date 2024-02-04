
<u><b>Ouverts</b></u> :

**Définition** :
Soient $a\in\mathbb R$ et $r>0$. On défini la boule ouverte de centre $a$ et de rayon $r$ comme :
$\mathcal B(a,r) = \{x\in\mathbb\ R : |x-a|<r\} = ]a-r;a+r[$

<u>Remarque</u> :
$r\leq s \Leftrightarrow \mathcal B(a,r)\subseteq\mathcal B(a,s)$

**Définition** :
Soient $a\in\mathbb R$ et $V\subseteq\mathbb R$. On dit que $V$ est un voisinage de $a$ si :
$\exists r>0 : \mathcal B(a,r)\subseteq V$
**Proposition** :
Si $V$ est un voisinage de $a$ et $V\subseteq W$ alors $W$ est un voisinage de $a$.

**Définition** :
Un ensemble $U\subseteq\mathbb R$ est dit ouvert si c'est un voisinage de tous ses points
- ie $\forall a\in U, \exists r>0 : \mathcal B(a,r)\subseteq U$
- ie $\forall  a\in\mathbb U, \exists r>0 : \forall x\in\mathcal B(a,r), x\in U$

**Théorème** :
Une union quelconque (même infinie), d'ensembles ouverts est ouverte :
- ie $U=\bigcup _{i\in I} U_i$ est ouvert (avec les $U_i$ ouverts, pour tout $i\in I$)
**Preuve** :
Soit $x\in U=\bigcup _{i\in I} U_i$ quelconque.
$x\in U \Rightarrow \exists i_{0}\in I : x\in U_{i_{0}}$
Comme $U_{i_{0}}$ est ouvert c'est un voisinage de $x$.
Donc $\exists r>0 : \mathcal B(x,r)\subseteq U_{i_{0}}$
Donc $\exists r>0 : \mathcal B(x,r)\subseteq U$
Donc $\forall x\in U, \exists r>0 : \mathcal B(x,r)\subseteq U$
Donc $U$ est ouvert.

**Corollaire** : 
Tout ensemble ouvert est une union d'intervalles.
**Preuve** :
Soit $U$ ouvert.
Etant donné $x\in U, \exists r_{x}>0 : \mathcal B(x,r_{x})\subseteq U$
Alors $U=\bigcup _{x\in U}\mathcal B(x,r_{x})=\bigcup _{x\in U} ]x-r_{x};x+r_{x}[$

**Théorème** :
Une intersection finie d'ouverts est ouverte.
**Preuve** :
Soient $U = \bigcap _{i\in I} U_i$ et $x\in U$
Alors $\forall i\in I, x\in U_{i}\Rightarrow\exists r_{i}>0 : \mathcal B(x,r_{i})\subseteq U_{i}$
On pose $r=\min{r_{i},i\in I}>0$.
Alors $\mathcal B(x,r)\subseteq\mathcal B(x,r_{i})\subseteq U_{i}, \forall i\in I$
$\Rightarrow \mathcal B(x,r)\subseteq U$

<b><u>Fermés</u></b> :

**Définition** :
Un sous ensemble $A\subseteq\mathbb R$ est dit fermé si $A^{C}=\mathbb R\setminus A$ est ouvert. En d'autres termes, $A$ est fermé si $\forall x\notin A, \exists r>0 : \mathcal B(x,r) \subseteq \mathbb R\setminus A$ ie $\mathcal B(x,r)\cap A = \emptyset$


**Théorème** :
Soit $(F_{i})_{i\in I}$ une famille d'ensembles fermés.
- $\bigcap _{i\in I} F_{i}$ est fermé
- Si $I$ est fini, alors $\bigcup _{i\in I} F_{i}$ est fermé
**Preuve** :
$\mathbb R\setminus \bigcap _{i\in I} F_{i} = \bigcup _{i\in I} (\mathbb R\setminus F_{i})$ est ouvert comme union d'ouverts. En effet $F_{i}$ fermé $\Rightarrow \mathbb R\setminus F_{i} = F_{i}^{C}$ ouvert.
Si $I$ est fini :
$\mathbb R\setminus\bigcup _{i\in I} F_{i} = \bigcap _{i\in I} (\mathbb R\setminus F_{i})$ est ouvert comme intersection finie d'ouverts.