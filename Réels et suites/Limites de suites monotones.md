

1) Soit $(a_n)_{n\in\mathbb N}$ une suite réelle croissante.
	a. Si $(a_n)_{n\in\mathbb N}$ est majorée alors elle converge et $\lim\limits_{n\to +\infty} a_n = sup\{a_n, n\in\mathbb N\}$
	b. Si $(a_n)_{n\in\mathbb N}$ n'est pas majorée alors $\lim\limits_{n\to +\infty} a_n = +\infty$
2) Soit $(a_n)_{n\in\mathbb N}$ une suite réelle décroissante.
	a. Si $(a_n)_{n\in\mathbb N}$ est minorée alors elle converge et $\lim\limits_{n\to +\infty} a_n = inf\{a_n, n\in\mathbb N\}$
	b. Si $(a_n)_{n\in\mathbb N}$ n'est pas minorée alors $\lim\limits_{n\to +\infty} a_n = -\infty$

*Preuves* :
1) 
	a.
	Supposons que $\exists M\in\mathbb R : \forall n\in\mathbb N, a_n \le M$.
	Alors $\{a_n, n\in\mathbb N\} \subseteq \mathbb R$ est majorée et admet une borne supérieure. Soit $a = sup\{a_n, n\in\mathbb N\}$. Alors $\forall \varepsilon > 0, \exists n_0 \in\mathbb N : a-\varepsilon < a_{n_0} \le a$
	Comme $a_n \nearrow$, on a $\forall n\ge n_0, a-\varepsilon < a_{n_0} \le a_n\le a < a+\varepsilon$
	Donc $\forall \varepsilon < 0, \exists n_0 \in\mathbb N : \forall n\ge n_0 -\varepsilon < a_n -a < \varepsilon$ ie $|a_n - a|< \varepsilon$
	Donc $\lim\limits_{n\to +\infty} a_n = a$.
	b.
	Supposons que $(a_n)_{n\in\mathbb N} \nearrow$ mais non majorée.
	Alors $\forall M \in\mathbb R, \exists n_M \in\mathbb N : a_{n_M} > M$
	Comme $(a_n)_{n\in\mathbb N} \nearrow, \forall n\ge n_M, a_n \ge a_{n_M}>M$ et $\lim\limits_{n\to +\infty} a_n = +\infty$
2) 
	a.
	Supposons que $(a_n)_{n\in\mathbb N} \searrow$ minorée, alors $inf\{a_n, n\in\mathbb N \}$ est un minorant donc $(-a_n)_{n\in\mathbb N} \nearrow$ majorée par $-inf\{a_n, n\in\mathbb N\}$ et par 1a $\lim\limits_{n\to\ +\infty} -a_n = -inf\{a_n, n\in\mathbb N\} \Rightarrow \lim\limits_{n\to\ +\infty} a_n = inf\{a_n, n\in\mathbb N\}$ 
	b.
	Supposons que $(a_n)_{n\in\mathbb N} \searrow$ non minorée, alors $(-a_n)_{n\in\mathbb N} \nearrow$ non majorée et par 1b $\lim\limits_{n\to +\infty} -a_n = + \infty \Rightarrow \lim\limits_{n\to +\infty} a_n = -\infty$


