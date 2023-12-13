Soit $f$ une fonction réelle de domaine $\mathbb R$ ou une fonction réelle telle que $\mathcal I_f \subseteq \mathcal D_f$.
On défini une suite par récurrence à l'aide de $f$ : 
- On choisit $\alpha\in\mathcal D_f$ et on pose $u_0 = \alpha$
- On définit par récurrence $u_{n+1} = f(u_{n})$ 
Autrement dit : 
- $u_{0}=\alpha$
- $u_{1}= f(\alpha)$
- $u_{2}= f\circ f(\alpha)$
- $u_{n}= f\circ\underset{n \;fois}{...}\circ f(\alpha)$ 

<u>Quelques remarques et méthodes</u> :
Soient $I$ un intervalle et $f:I\longrightarrow I$ une fonction réelle.
Soit $(a_n)_{n\in\mathbb N}$ définie par : $a_0=\alpha\in I,\; a_{n+1}=f(a_n)$
1) Supposons $\mathcal I_f$ majoré : $\exists M\in\mathbb R : \forall x\in I, f(x)\le M$ et $M_{0}= \max\{\alpha,M\}$. On va montrer par récurrence que $\forall n\in\mathbb N, u_{n}\le M_0$
*Preuve* :
Pour $n=0$ : 
$a_0 = \alpha \le M_0$
Pour $n\ge 0$ :
Si $a_{n} \le M_0$ alors $a_{n+1}=f(u_n)$ or $f$ est majorée par $M_{0}\ge M$ donc $a_{n+1}\le M\le M_0$
Donc si $\mathcal I_f$ est majorée, alors $(a_n)_{n\in\mathbb N}$ l'est aussi
<u>Attention</u> : La réciproque est fausse.
2) Supposons $f \nearrow (\nearrow)$ . Alors $\forall \alpha\in I$, la suite $u_{0}=  \alpha, a_{n+1} = f(a_n)$ est soit monotone (strictement) soit constante.
*Preuve* :
Soit $\beta = u_{1} = f(u_{0})=f(\alpha)$
1- Supposons que $\beta = \alpha,\; f(\beta) = a_{2}=f(a_1)=f(\alpha)=\alpha$ donc $(u_n)_{n\in\mathbb N}$ est constante.
2- Supposons que $\beta > \alpha$ 
Alors $a_{1}> a_0$ et $a_{2}= f(\beta) \ge f(\alpha)$ par $\nearrow$ de $f$.
Par récurrence : 
Pour $n=0$ : 
On a bien $a_1>a_0$
Pour $n \ge 0$ : 
$a_n\le a_{n+1} \Rightarrow a_{n+1}\le a_{n+2}$ par $\nearrow$ de $f$

<u>Remarque</u> : 
Soit $A\subseteq \mathbb R$ borné, supposons qu'il existe $(a_n)_{n\in\mathbb N}$ telle que $\mathcal I_{a_n}\subseteq A$ et la suite converge ver $l\in\mathbb R$
- Si $l$ est un majorant de $A$, alors $l=\sup(A)$ 
- Si $l$ est un minorant de A, alors $l=\inf(A)$
*Preuve* :
Supposons que $l$ major $A$.
$\forall x\in A,\; x\le l$ soit $(a_n)_{n\in\mathbb N}$ une suite qui converge vers $l$ telle que l'image de la suite est inclues dans $A$.
Par la définition de limite on a : 
$\forall\varepsilon >0,\exists n_0\in\mathbb N : \forall n \ge n_{0,}|a_{n}- l| <\varepsilon$ ie $\forall n\ge n_{0}, \;-\epsilon + l < u_{n}< l + \varepsilon$
Donc si $l'$ est un autre majorant de $A$ et $l'<l$ alors 
$\exists \varepsilon > 0 : l' = l -\varepsilon$
Et on a alors : $\exists n_0\in\mathbb N : \forall n\ge n_0, a_n > l'$
En particulier, $\exists a\in A (a= a_{n_{0}}): a > l'$ donc $l'$ n'est pas majorant.
Donc $l$ est le plus petit majorant donc $l=\sup(A)$
De façon analogue on montre $l=\inf(A)$ si $l$ minore $A$.
