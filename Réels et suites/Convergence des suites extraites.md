
**Lemme** :
Soit $$\begin{matrix}\varphi : & \mathbb N & \longrightarrow \mathbb N \\ & n & \longmapsto & \varphi (n) \end{matrix} \nearrow\nearrow$$Alors $\forall n\in\mathbb N, \varphi(n) \ge n$.
*Preuve* :
Pour $n=0$, on a $\varphi (0) \ge 0$ car $\varphi (0)\in\mathbb N$
Pour $n \ge 0$, supposons que $\varphi (n) \ge n$.
On a $\varphi (n+1) > \varphi (n)$ car $\varphi \nearrow\nearrow$ et $\varphi (n) \ge n$
$\Rightarrow \varphi (n+1) > n \Rightarrow \varphi (n+1) \ge n$
On conclut selon le principe de récurrence que $\forall n\in\mathbb N, \varphi (n) \ge n$

**Proposition** :
Toute sous suite d'une suite (réelle ou complexe) convergente vers $l\in\mathbb C$ converge également vers $l$.
*Preuve* :
Supposons que $(u_n)_{n\in\mathbb N}$ converge vers $l\in\mathbb C$ et, soient $\varphi : \mathbb N \longrightarrow \mathbb N \nearrow\nearrow$ et $(v_n)_{n\in\mathbb N} = (u_{\varphi (n)})_{n\in\mathbb N}$
Soit $\varepsilon > 0$.
$\lim\limits_{n\to +\infty} u_n= l \Rightarrow \exists n_0 \in\mathbb N : \forall n \ge n_0, |u_n - l| < \varepsilon$
$\varphi (n) \ge n \Rightarrow \forall n\ge n_0, \varphi (n) \ge \varphi (n_0) \ge n_0$ 
et $|u_ {\varphi (n)} - l | < \varepsilon, \forall n \ge n$ ie $\lim\limits_{n\to +\infty} u_{\varphi (n)} = l$ 

**Corollaire** : 
Si $(u_n)_{n\in\mathbb N}$ admet deux sous suites qui ne convergent pas vers la même limite, alors $(u_n)_{n\in\mathbb N}$ n'a pas de limite