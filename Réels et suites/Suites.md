
Une suite est une fonction de $\mathbb N$ dans $\mathbb K$ : $$u : \mathbb N \longrightarrow \mathbb K$$ Si u est une suite et $n \in \mathbb N$, ont note $u_n := u(n)$, et on l'appelle le terme de rang n, ou n-ième terme ou terme général de la suite.

Plus généralement, soit $n_0 \in \mathbb N$ et $\mathbb N_{\ge n_0} := \{n \in \mathbb N : n \le n0\}$, on appelle aussi suite une fonction de $\mathbb N_{\ge n_0}$ dans $\mathbb K$.

**Définition :**
Une suite complexe $(a_n)_{n\in \mathbb N}$ est bornée si l'ensemble $\{|a_n|,n\in \mathbb N\}\subseteq \mathbb R$ est bornée.

<u>Suites Réelles</u> :

**Définition :**
	-Une suite réelle $(a_n)_{n \in \mathbb N}$ est majorée/minorée/bornée si l'image de la suite est respectivement majorée/minorée/bornée.
	Donc $(a_n)_{n\in\mathbb N}$ est majorée/minorée/bornée si $\exists M \in \mathbb R : \forall n \in \mathbb N, a_n \le M$ / $a_n \ge M$ / $|a_n| \le M$.
	-Une suite réelle ou complexe $(a_n)_{n\in\mathbb N}$ est constant si $\exists \alpha \in \mathbb K : \forall n\in \mathbb N, a_n = \alpha$.
	-Une suite réelle est $\nearrow$ si $\forall n \in \mathbb N, a_n \le a_{n+1}$, $\nearrow\nearrow$ si $\forall n \in \mathbb N, a_n < a_{n+1}$, 
	$\searrow$ si $\forall n \in \mathbb N, a_n \ge a_{n+1}$, $\searrow\searrow$ si $\forall n \in \mathbb N, a_n > a_{n+1}$.
	-Une suite est (strictement) monotone si elle est (strictement) $\nearrow$ ou (strictement) $\searrow$ 

**Définition :**
On dit que $(a_n)_{n\in\mathbb N}$ a une propriété $P$ à partir d'un certain rang ou ultimement si $\exists n_0 \in \mathbb N : (a_n)_{n\ge n_0}$ à la propriété

**Définition :**
Soient $(a_n)_{n\in\mathbb N}$ une suite et $\varphi : \mathbb N \longrightarrow \mathbb N$ une fonction $\nearrow\nearrow$.
On considère $(b_k)_{k\in\mathbb N}$ définie par $b_k = a_{\varphi (k)}$. On dit que $(b_k)_{k\in\mathbb N}$ est une sous-suite (ou suite extraite) de  $(a_n)_{n\in\mathbb N}$ et $\varphi$ une extractrice. On peut noter $(a_{\varphi (k)})_{k\in\mathbb N}$.

<u>Remarque</u> : 
Pour montrer qu'une suite n'est pas ultimement constante, il suffit d'extraire de suites qui n'ont pas la même image.

