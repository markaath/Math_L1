
**Définition** : 
Soit $p\in\mathbb N : p \ge 2$ On dit que $p$ est premier si les seuls diviseurs positifs de $p$ sont $1$ et $p$. On notera $\mathcal P$ l'ensemble des nombres premiers dans toutes la suite.

**Lemme** :
$\forall a\in\mathbb N : a\ge 2, \exists p\in\mathcal P : p|a$

**Lemme d'Euclide** :
Soient $(a,b)\in\mathbb Z, p\in\mathcal P$
$p|ab \Rightarrow \left[p|a \lor p|b\right]$ 
*Preuve* :
Supposons que $p|ab$ et $p\cancel{|}a$ et montrons que $p|b$
$p\cancel{|}a \Rightarrow p\land a = 1$ et par le lemme de Gauss, nécessairement $p|b$.
De façon analogue on montre que $p|ab \land p\cancel{|}b \Rightarrow p|a$

**Théorème** :
Soit $n\in\mathbb N, n\ge 2$
Alors , $\exists r\in\mathbb N^{*}, (\alpha_i)_{i\in [1,r]}\in \mathbb ({N^{*}})^{r}, p_1<p_2<..<p_{r} \in\mathcal P^{r}: n = \prod _{i=1}^{r}p_{i}^{{\alpha _i}}$ 
De plus $r,\alpha _{i}, p_i$ sont uniques

**Lemme** : 
Soit $n\in\mathbb N^*$ 
Si $n$ non premier, alors $\exists p\in\mathcal P : p\le \sqrt{n}$ et $p|n$
