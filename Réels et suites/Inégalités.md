
Soient $(u_n)_{n\in\mathbb N}, (v_n)_{n\in\mathbb N}, (w_n)_{n\in\mathbb N}$ des suites réelles.
1) Si ultimement $u_n \le v_n$ et si $u_n \underset{n\to +\infty}{\longrightarrow} l \in\mathbb R$ et $v_n \underset{n\to +\infty}{\longrightarrow} l' \in\mathbb R$, alors $l \le l'$
2) Si ultimement $u_n \le v_n$ alors :
	- $u_n \underset{n\to +\infty}{\longrightarrow} +\infty \Rightarrow v_n \underset{n\to +\infty}{\longrightarrow} +\infty$
	-  $v_n \underset{n\to +\infty}{\longrightarrow} -\infty \Rightarrow u_n \underset{n\to +\infty}{\longrightarrow} -\infty$
3) Théorème de gendarmes : 
Si ultimement $u_n \le w_n \le v_n$ et $u_n\underset{n\to +\infty}{\longrightarrow} l$ et $v_n\underset{n\to +\infty}{\longrightarrow} l$ alors $w_n\underset{n\to +\infty}{\longrightarrow} l$
*Preuves* :
1) à faire
2) à faire
3) Soient $u_n\underset{n\to +\infty}{\longrightarrow} l$, $v_n\underset{n\to +\infty}{\longrightarrow} l$ et $u_n \le w_n\le v_n$. Montrons que $w_n\underset{n\to +\infty}{\longrightarrow} l$.
Soit $\varepsilon > 0$
$w_n\le v_n \Rightarrow w_n -l \le v_n -l \le |v_n-l|$
$w_n \ge u_n \Rightarrow -w_n \le -u_n$
$\qquad\qquad\Rightarrow -(w_n -l) \le -(u_n -l) \le |u_n -l|$
$\qquad\qquad \Rightarrow |w_n -l| \le max\{ |v_n -l|,|u_n -l|\}$
Soient $(n_1,n_2) \in\mathbb N² : \forall n \ge n_1, |u_n -l| < \varepsilon \land \forall n\ge n_2, |v_n - l| < \varepsilon$.
On pose $n_0 = max\{n_1,n_2\}$ et $\forall n \ge n_0, |u_n -l| < \varepsilon \land |v_n-l|<\varepsilon$
$\Rightarrow \forall n \ge n_0, |w_n-l|\le max\{|u_n-l|,|v_n-l|\} < \varepsilon$
Et on a bien $\lim\limits_{n\to +\infty} w_n = l$.

**Conséquences** :

1) Soit $(a_n)_{n\in\mathbb N} \in\mathbb C^{\mathbb N}$. S'il existe deux suites réelles $(b_n)_{n\in\mathbb N}$ et $(c_n)_{n\in\mathbb N}$ telles que, ultimement $b_n \le |a_n|\le c_n$ et $b_n \underset{n\to +\infty}{\longrightarrow} 0 \land c_n \underset{n\to +\infty}{\longrightarrow} 0$ alors $\lim\limits_{n\to + \infty}a_n = 0$
*Preuve* :
Par le théorème des gendarmes, la suite $(|a_n|)_{n\in\mathbb N}$ tend vers 0.
Donc $\forall \varepsilon > 0, \exists n_0  \in\mathbb N : \forall n \ge n_0 ||a_n| -0| < \varepsilon$ 
$\Rightarrow \forall \varepsilon, \exists n_0 \in\mathbb N : \forall n \ge n_0, |a_n| < \varepsilon$
$\Rightarrow a_n \underset{n\to +\infty}{\longrightarrow} 0$

2) Soient $(a_n)_{n\in\mathbb N}$ et $(b_n)_{n\in\mathbb N}$ suites complexes telles que $a_n \underset{n\to +\infty}{\longrightarrow} 0$ et $(b_n)_{n\in\mathbb N}$ ultimement bornée. Alors $\lim\limits_{n\to +\infty} a_n\cdot b_n = 0$
*Preuve* :
Soit $M \in\mathbb R_+^* : \exists n_0 \in\mathbb N : \forall n\ge n_0, |b_n| \le M$
Donc $0 \le |b_n|\le M$
$\Rightarrow 0 \le |b_n|\cdot |a_n| \le M\cdot |a_n|$
Or $a_n\underset{n\to +\infty}{\longrightarrow} 0$
$\Rightarrow |a_n| \underset{n\to\infty}{\longrightarrow}0$
$\Rightarrow M\cdot |a_n| \underset{n\to +\infty}{\longrightarrow} 0$
Donc, par le théorème des gendarmes, $|a_n\cdot b_n| \underset{n\to +\infty}{\longrightarrow}0 \Rightarrow a_n\cdot b_n \underset{n\to\infty}{\longrightarrow}0$
