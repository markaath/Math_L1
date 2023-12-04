
**Définition** :
Soit $(a_n)_{n \in \mathbb N} \in \mathbb K$ et soit $l \in \mathbb C$.
On dit que $(a_n)_{n\in \mathbb N}$ tend vers $l$ et on écrit $\lim\limits_{n \to +\infty} a_n$, si $\forall \varepsilon \in \mathbb R_+^*, \exists n_0 \in \mathbb N : \forall n \ge n_0, |a_n - l| < \varepsilon$. 
$(a_n)_{n \in \mathbb N}$ converge si $\exists l \in \mathbb C : \lim\limits_{n \to +\infty} a_n = l$
Si $(a_n)_{n\in \mathbb N}$ est à valeurs dans $\mathbb R$, 
$(a_n)_{n \in \mathbb N} \underset{n \longrightarrow + \infty} {\longrightarrow} + \infty$ si $\forall M > 0, \exists n_0 \in \mathbb N : \forall n \ge n_0, a_n > M$ 
$(a_n)_{n \in \mathbb N} \underset{n \longrightarrow - \infty} {\longrightarrow} + \infty$ si $\forall M > 0, \exists n_0 \in \mathbb N : \forall n \ge n_0, a_n > M$ 

**Théorème** :
1) Si $(a_n)_{n\in\mathbb N}$ converge, alors la limite est unique
2) Si $(a_n)_{n\in\mathbb N}$ converge, alors elle est bornée
3) Si $\lim\limits_{n \longrightarrow + \infty} a_n = l \in \mathbb C$ et $\lim\limits_{n \longrightarrow + \infty} b_n = l' \in \mathbb C$ alors :
	- $(a_n + b_n)_{n\in\mathbb N}   \underset{n \longrightarrow + \infty} {\longrightarrow} l + l'$
	- $(a_n - b_n)_{n\in\mathbb N}   \underset{n \longrightarrow + \infty} {\longrightarrow} l - l'$
	- -$(a_n \cdot b_n)_{n\in\mathbb N}   \underset{n \longrightarrow + \infty} {\longrightarrow} l \cdot l'$ 
	- Si $l' \neq 0$, alors ultimement $b_n \neq 0$ et $(\frac{a_n}{b_n})_{n\in\mathbb N} \underset{n \longrightarrow + \infty}{\longrightarrow} (\frac{l}{l'}$

*Preuve* :
1) à faire
2) Soit $(a_n)_{n\in\mathbb N}$ convergente. 
Alors $\exists l \in \mathbb C : \forall \varepsilon>0, \exists n_0 \in \mathbb N : \forall n \ge n_0, |a_n - l| < \varepsilon$ *(1)*
Soient $\varepsilon = 1$ et $n_0(1)$ l'indice correspondant à $\varepsilon=1$ dans *(1)*.
Donc $\forall n \ge n_0(1), |a_n -l| < 1$
Donc $\forall n \ge n_0(1), |a_n| = |a_n - l + l| \le |a_n - l| + |l| < 1 + |l|$
Soit $M = max\{1 + |l|, |a_i|_{i \in [\![0, n_0(1)-1]\!]}\}$. Alors, $\forall n \in \mathbb N, |a_n| \le M$ ie $-M \le a_n \le M$ .
Donc $(a_n)_{n\in\mathbb N}$ est bornée, et on a également montré que $(a_n)_{n\in\mathbb N}$ ultimement bornée $\Rightarrow$ $(a_n)_{n \in\mathbb N}$ bornée

**Propriété** :
Soit $f$ une fonction réelle et soit $(a_n)_{n \in\mathbb N}$ la suite définie par $a_n := f(n)$.
Si $f$ vérifie une propriété $P$ au voisinage de $+\infty$ alors $(a_n)_{n\in\mathbb N}$ vérifie ultimement $P$.

*Preuve* :
$P(f)$ vraie au voisinage de $+\infty$ veut dire $\exists M \in \mathbb R : \forall x \ge M, P(f)$ vraie.
Soit $N= max\{0, \lfloor M \rfloor + 1\}$. Alors $\forall n \ge N$, on a que $n \ge M$ et donc $P(f(n))$ vraie.
On a montré que $\exists n_0(=N) \in \mathbb N : \forall n \ge n_0, P(a_n)$ vraie également.

