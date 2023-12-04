**Définition** :
Un ensemble est une collection d'objets mathmatiques

<u>Caractérisation d'un ensemble</u> :

*Définition extensive* : On liste tout les éléments de l'ensemble
*Définition par compréhension* : On donne une propiété qui caractérise les éléments de l'ensemble

**Définition** : 
Soit $U$ un ensemble, $A(x)$ un énoncé avec une variable libre x.

On défini $V=\{x \in U : A(x)\}$, qui est un sous-ensemble de $U$. La variable x est maintenant  mutifiée par {}.

**Définition** : 
Soient $U$ un ensemble, $A(x)$ un énoncé avec $x$ une variable libre.
- $\{x \in U : A(x)\} = \emptyset \Leftrightarrow \forall x \in U, ¬A(x)$
- $\{x \in U : A(x)\} = U \Leftrightarrow \forall x \in U, A(x)$
- Soient $V_i  = \{x \in U : A_i(x)\}, i \in [\![1,2]\!]$, alors 
	- $V_1 \cap V_2 = \{x \in U : A_1(x) \land A_2(x)\}$
	- $V_1 \cup V_2 = \{x \in U : A_1(x) \lor A_2(x)\}$ 
	- $V_1 \setminus V_2 = \{x \in U : A_1(x) \land ¬A_2(x)\}$
	- $V_1 \times V_2 = \{(x,y) \in U² : A(x) \land A(y)\}$

**Définition** : 
Soit $A \subseteq U$, $\mathcal P (A) = \{X \subseteq U : X \subseteq A\}$ est l'ensemble des partie de A.

**Propriété** : 
Soient $A,B \subseteq E$, $A=B \Leftrightarrow A\cap B = A\cup B$
*Preuve* : 
Supposons que $A\cap B = A \cup B$ 
$\Rightarrow \Bigl[\forall x \in E, x \in A\cup B \Rightarrow x \in A \cap B\Bigl]$ 

Donc $\forall x \in A, x \in A\cup B \Rightarrow x \in A\cap B \Rightarrow x \in B$.
Supposons maintenant que $A=B$.
Alors $A\cap B = A \land A\cup B = A$ et on a bien $A\cap B = A\cup B$.

<u>Fonctions</u> :
$f : A \longrightarrow B$ est une loi qui $\forall x \in A$ associe au plus un élément de $B$.

Si à $x \in A$, $f$ associe $y\in B$ on note $f(x)=y$ et$\underset{\qquad\quad x \;\;\longmapsto\; y = f(x)}{f : A \longrightarrow B}$ 

**Définition** : 
Soit $f : A \longrightarrow B$ une fonction.
- $f$ est une application si $\mathcal D_f = A$
- $f$ est injective si $\forall (x,y) \in \mathcal D_f f(x)=f(y) \Rightarrow x=y$
- $f$ est surjective si $\mathcal I_f = B$ 
- $f$ est bijective $\Leftrightarrow$ $f$ est injective $\land$ $f$ surjective 

**Définition** :
Soient $f : A  \longrightarrow B$ une fonction, $x \in A, y \in B : f(x) = y, A_0 \subseteq A, B_0 \subseteq B$.
- $x$ est un antécédent de $y$ par $f$, $y$ est l'image de $x$ par $f$
- $f(A_0) = \{y\in B : \exists A_0 : f(x) = y\} \subseteq \mathcal I_f$ est l'image direct de $A_0$ par $f$
- $f^{-1}(B_0) = \{x \in \mathcal D_f : f(x) \in B_0\} \subseteq \mathcal D_f$ est l'image réciproque de $B_0$ par $f$

<u>Composition</u> :
Soient $f : A \longrightarrow B,\; g: C \longrightarrow D$ avec $A,B,C,D$ des ensembles et $f,g$  des fonctions.

$\mathcal D_{g\circ f} = \{x \in \mathcal D_f : f(x) \in \mathcal D_g\}$ 
$g\circ f$ est définie si $f^{-1}(\mathcal D_g \neq \emptyset$. Dans ce cas, $\forall x \in f^{-1}(\mathcal D_g)$, on a : $g\circ f(x) = g(f(x))$

