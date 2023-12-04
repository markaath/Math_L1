
$\mathbb{R}$ est un corps ordonné muni de $+$ et de $\times$ et d'une relation d'ordre compatible.

**Axiome 1 :**  $\forall$ ($x,y,z$) $\in$ $\mathbb{R}$$³$  $x$ $\le$ $y$ $\Rightarrow$ $x+z$ $\le$ $y+z$
	**Axiome 2 :** $\forall$ ($x,y$) $\in$ $\mathbb{R}²$  $x > 0$ $\land$ $y > 0$ $\Rightarrow$ $x \times y$ $>$ $0$ 

**Définition :** Soit $A$ $\subseteq$ $\mathbb R$ , $A$ $\neq$ $\emptyset$
	- $M$ $\in$ $\mathbb R$ est un majorant de $A$ si $\forall x \in A, x \le M$  
	- $A$ est borné supérieurement ou majoré si $\exists M \in \mathbb{R} :  \forall x \in A, x \le M$    
	- $M \in \mathbb{R}$ est le max de $A$ si $M$ est un majorant de $A$ et $M \in A$. Dans ce cas $M = max(A)$.
	- $M \in \mathbb{R}$ est la borne supérieure de $A$ si $M$ est le plus petit majorant de $A$. On écrit alors $M = sup(A)$. 
	- $M = max(A) \Leftrightarrow M = sup(A) \land M \in A$ 
	- On définit de façon analogue le minorant, borné inférieurement (ou minoré), le minimum (noté $min(A)$ )et la borne inférieur (notée $inf(A)$ )
	- $A$ est borné s'il est majoré et minoré

**Axiome 3** : $\forall E \subseteq \mathbb{R} : E \neq \emptyset \land E$ majoré (respectivement minoré), $E$ admet une borne supérieure (respectivement inférieure)

**Théorème d'Archimède :** 
$\forall x \in \mathbb R,  \forall \varepsilon \in \mathbb {R_+^*}, \exists n \in \mathbb N : n\varepsilon > x$ 
En particulier pour $\varepsilon = 1$, on a $\forall x \in \mathbb R, \exists n \in \mathbb N : n > x$.

*Preuve* : 
Par l'absurde : 

Supposons que $\exists (x,\varepsilon) \in \mathbb R \times \mathbb {R_+^*} : \forall n \in \mathbb N n\varepsilon \le x$. 
Donc $A = \left\{n\varepsilon, n\in \mathbb N\right\}$ est majoré par $x$. 
Par la propriété de la borne supérieure (Axiome 3), $\exists M \in \mathbb R : M = sup(A)$. En particulier  $M-\varepsilon$ n'est pas un majorant de $A$ : $\exists n_0 \in \mathbb N : n_0\varepsilon > M - \varepsilon$.
Donc $(n_o + 1 )\varepsilon > M$ et $((n_0 +1)\varepsilon) \in A$.
Donc $M$ n'est pas un majorant de $A$.

**Corollaire :**  
$\forall x \in \mathbb R_+^*, \exists n \in \mathbb N : 0 < \frac{1}{n} < x$

*Preuve* : 
Soit $x \in \mathbb R_+^*$, alors $y = \frac{1}{n} \in \mathbb R_+^*$. 
Donc par le théorème d'Archimède avec $\varepsilon = 1, \exists n \in \mathbb N^* : n > y > 0 \Rightarrow \frac{1}{n} < \frac{1}{y} = x$.

**Corollaire :** 
$\forall x \in \mathbb R, \exists ! N \in \mathbb Z : N \le x < N + 1$ 

*Preuve* :
-<u>Existence</u> :
Supposons que $x > 0$, alors par Archimède, $\exists n_0 \in \mathbb N : n_0 > x$.
Soit $A = \{n \in \mathbb N : n \le n_0 \land n \le x\} \subseteq \mathbb N$.On a $A \neq \emptyset$ car $0 \in A$ et $A$ fini car $A \subseteq [\![0,n_0]\!]$. 
$\Rightarrow \exists N = max(A)$ 
Donc $N \le x$ et $N+1 \notin A$ : soit $N+1 > n_0$, soit $N+1>x$. Donc $\exists N \in \mathbb N : N \le x < N+1$.
On montre la même chose de façon analogue pour $x<0$.

-<u>Unicité</u> : 
Supposons que $\exists (N,N') \in \mathbb Z² :$
$N \le x < N+1 \land N' \le x < N'+1 \land N'>N$
$\Rightarrow N' \le x <N+1$
$\Rightarrow N' < N+1$
$N'\le N$  Absurde donc un tel $N$ est unique.

Remarque : 
Soient $\emptyset \neq A \subseteq B$, $B$ borné.
1) $B$ borné $\Leftrightarrow$ $\exists r \in \mathbb R_+^* : B \subseteq [-r,r]$ 
2) ($A \neq \emptyset$ et $A\subseteq B \Rightarrow B \neq \emptyset$ et $B$ borné) $\land$ $(A \subseteq B \Rightarrow A$ est borné)  
3) Supposons que $max(A),max(B),min(A),min(B)$ existent. Soit $b := max(B)$ 
$\Rightarrow \forall x \in B, x \le b \land b \in B$
$\Rightarrow \forall x \in A, x \le b$
$\Rightarrow max(A) \le max(B)$

De façon analogue, on obtient $min(A) \ge min(B)$. 




