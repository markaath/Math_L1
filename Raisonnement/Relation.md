
**Relations binaires :**
Une relation binaire sur un ensemble $E$ est un sous ensemble $\mathcal R$  de $E²$, $\mathcal R \subseteq E²$ .

On écrit souvent $(x,y) \in \mathcal R$ comme $x\mathcal R y$.
Si $E$ est un ensemble fini, alors on peut représenter graphiquement une relation binaire : 
on dessine un point pour chaque élément de $E$ et on dessine une flèche entre deux points qui sont en relation, avec la pointe de la flèche qui indique l'ordre dans le couple de point.

**Définition :**
Soient $E$ un ensemble et $\mathcal R \subseteq E²$ une relation.
* $\mathcal R$ est réflexive si $\forall x \in E, x\mathcal Rx$
* $\mathcal R$ est antiréflexive si $\forall x \in E, \lnot (x\mathcal R x)$
* $\mathcal R$ est symétrique si $\forall (x,y) \in E², x\mathcal R y \Rightarrow y\mathcal R x$ 
* $\mathcal R$ est antisymétrique si $\forall (x,y) \in E², (x\mathcal R y\land y\mathcal R x) \Rightarrow x=y$ 
* $\mathcal R$ est transitive si $\forall (x,y,z) \in E³, (x\mathcal R y\land y\mathcal R z)\Rightarrow x\mathcal R z$ 
* $\mathcal R$ est totale si $\forall (x,y)\in E²,x \neq y \Rightarrow x \mathcal R y \lor y\mathcal R x$ 
* $\mathcal R$ est asymétrique si $\forall (x,y) \in E², x\mathcal R y \Rightarrow \lnot (y\mathcal R x)$

<u>Remarques</u> :

1) $\mathcal R$ antisymétrique $\land$ $\mathcal R$ antiréflexive $\Rightarrow \mathcal R$ asymétrique
*Preuve* :
$\boxed{\Rightarrow}$ :
Supposons que $\mathcal R$ est antisymétrique et antiréflexive et que $x\mathcal R y, (x,y) \in E²$. 
Supposons que $y\mathcal R x$, alors par antisymétrie, $x=y$. 
Donc $x\mathcal R x$, ce qui contredit l'antiréflexivité, donc $\mathcal R$ est asymétrique.

$\boxed{\Leftarrow}$ :
Supposons que $\mathcal R$ est asymétrique et soit $x\in E : x \mathcal R x$, alors par asymétrie on a $\lnot(x \mathcal R x)$, absurde. Donc $\mathcal R$ asymétrique $\Rightarrow$ $\mathcal R$ antiréflexive.

L'antécédent de l'implication de $\mathcal R$ antisymétrique est toujours faux par l'asymétrie de $\mathcal R$ donc, $\mathcal R$ asymétrique $\Rightarrow \mathcal R$ antisymétrique.

2) 
$\lnot (\mathcal R$ réflexive$)$ $\xcancel{ \Longleftrightarrow} \mathcal R$ antiréflexive
$\lnot(\mathcal R$ symétrique$) \xcancel{\Longleftrightarrow} \mathcal R$ asymétrique
En revanche, on a :
$\mathcal R$ antiréflexive $\Rightarrow \lnot (\mathcal R$ réflexive$)$
$\mathcal R$ asymétrique $\Rightarrow \lnot (\mathcal R$ symétrique$)$

3)  $(\mathcal R$ antiréflexive$)\land (\mathcal R$ transitive$) \Rightarrow (\mathcal R$ asymétrique)$
*Preuve :*
Soit $(x,y) \in E² : x\mathcal R y$. Si on a $y\mathcal R x$, alors comme $\mathcal R$ transitive, on a $x\mathcal R x$, ce qui contredit $\mathcal R$ antiréflexive, donc on a nécessairement $\lnot(y\mathcal Rx)$ donc $\mathcal R$ est asymétrique.

**Définition :** 
Soient $E$ un ensemble et  $\mathcal R \subseteq E²$ une relation. Alors :
	-$\mathcal R$ est une relation d'équivalence si $\mathcal R$ est réflexive, symétrique et transitive
	-$\mathcal R$ est une relation d'ordre large si $\mathcal R$ est réflexive, antisymétrique et transitive. Si de plus $\mathcal R$ est totale, on parle de relation d'ordre large totale
	-$\mathcal R$ est une relation d'ordre stricte si $\mathcal R$ est antiréflexive et transitive, donc antisymétrique et asymétrique également. Si de plus $\mathcal R$ est totale, on parle de relation d'ordre stricte totale.

*Notation :*
On note souvent les relations d'équivalence par $\backsim$ au lieu de $\mathcal R$ :
$x\backsim y$ veut dire $x\mathcal R y$ avec $\mathcal R$ une relation d'équivalence.

**Définition :**
Soit $x\in E$. La classe d'équivalence de $x$ est l'ensemble : $$\left[ x \right] = {\left[ x \right]}_\backsim = \bar{x} = \{ y \in E : y \backsim x\}$$ Un élément z de $\bar{x}$ est un <u>représentant</u> de $\bar{x}$.

**Théorème :** Soient $E$ un ensemble et $\backsim \subseteq E²$ une relation d'équivalence.
1) $\forall (x,y) \in E², \bar{x} = \bar{y} \Leftrightarrow x\backsim y$
2) $\forall (x,y) \in E²$, soit $\bar{x} = \bar{y}$ soit $\bar{x} \cap \bar{y} = \emptyset$ 
3) $E$ est l'union de ses classes d'équivalences par rapport à $\backsim$ 

*Preuve :* 
1) $\Rightarrow$ :
$\forall (x,y) \in E², x\backsim y \Rightarrow y \in \bar{x} \land x\in \bar{y}$
$\Rightarrow \bar{x}=\bar{y}$

$\Rightarrow$ :
$\forall (x,y) \in \bar{x}\in\bar{y} => y \in \bar{x} \land x \in \bar{y}$
$\Rightarrow y\backsim x \land x\backsim y$
2) On veut montrer que $\lnot(\bar{x} = \bar{y}) \Rightarrow \bar{x} \cap \bar{y} = \emptyset$
$\bar{x} \neq \bar{y} \Rightarrow \forall (x_i,y_i) \in \bar{x} \times \bar{y}, x_i \notin \bar{y} land y_i \bar{y}$
$\Rightarrow \bar{x} \cap \bar{y}$
Par contraposée, on a $\lnot (\bar{x}\cap\bar{y}=\emptyset) \Rightarrow \bar{x}=\bar{y}$

3) Soit $(\overline{x_i})_{i \in [\![1,n]\!]}$ l'ensemble de toutes les classes d'équivalence de $E$ par rapport à $\backsim$. Soit $y\in E : \forall i \in [\![1,n]\!], y \in \overline{x_i}$. Alors $y\in \overline{y} = \{y\}$ et $\bar{y} \in (\overline{x_i})_{i \in [\![1,n]\!]}$ . Absurde.

**Définition** :
Soit $E$ un ensemble, $\mathcal R \subseteq E²$ une relation d'ordre large (partiel à priori). Souvent on écrit $\mathcal R$ comme $\ge$ ou $\succcurlyeq$. On dit que $E$ muni de $\mathcal R$ est un ensemble ordonné.

<u>Remarque</u> : 
Si $\mathcal R$ est une relation d'ordre strict, on peut définir $\mathcal R'$ par 
$x\mathcal R' y \Longleftrightarrow x \mathcal R y \lor x = y$
Inversement, si $\mathcal R$ est une relation d'ordre large, on peut définir $\mathcal R'$ par
$x\mathcal R' y \Longleftrightarrow x \mathcal R y \land x \neq y$

**Définition** : 
Soit $(E, \succcurlyeq)$ un ensemble ordonné, $S\subseteq E, (a,b) \in E²$.
On dit que $a$ est un minorant de $S$ si $\forall x \in S, x \succcurlyeq a$ 