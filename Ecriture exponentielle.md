
**Définition** :
Soit $\theta\in\mathbb R$, on pose $e^{i\theta}:=\cos(\theta)+i\sin(\theta)$ 
Soit $z\in\mathbb C^*$,soit $\rho =|z|\in\mathbb R_+^*$
On a donc $z=\rho e^{i\cdot arg(z)}$ 

**Règles de calcul** :
- $zz'=\rho\rho 'e^{i(\theta +\theta ')}$
- $\bar z = \rho e^{-i\theta}$
- $\dfrac{1}{z}= \dfrac{\bar z}{|z|²} = \dfrac {\rho}{\rho ²} e^{-i\theta} = \rho ^{-1}e^{-i\theta}$
- $z^n = (\rho e^{i\theta})^n = \rho ^n e^{in\theta}$ 
- $\cos(\theta)= \dfrac{e^{i\theta} + e^{-i\theta}}{2}$
- $\sin(\theta) = \dfrac{e^{i\theta} - e^{-i\theta}}{2i}$

**Définitions** :
<u>Factorielle</u> : On pose $0!=1$ et $\forall n\in\mathbb N^*, n!=\prod_{k=1}^n k$ 
<u>Coefficient binomiaux</u> : $\dbinom{n}{k} = \dfrac{n!}{k!(n-k)!}$ 


**Formule du triangle de Pascal** :
$$\dbinom{n-1}{k} + \dbinom{n-1}{k-1} = \dbinom {n}{k}$$
*Preuve* :
$\dbinom{n-1}{k} + \dbinom{n-1}{k-1} = \dfrac{(n-1)!}{k!(n-1-k)!} + \dfrac{(n-1)!}{(k-1)!(n-1-(k-1))!}$

$= \dfrac{(n-1)!}{k!(n-1-k)!} \dfrac{n-k}{n-k}+ \dfrac{(n-1)!}{(k-1)!(n-1-(k-1))!}\dfrac{k}{k}$

$=\dfrac{(n-1)!\times (n-k)+k\times (n-1)!}{k!(n-k)!}$

$=\dfrac{(n-1)!(n-k+k)}{k!(n-k)!} =\dfrac{n!}{k!(n-k)!}=\dbinom{n}{k}$


**Binôme de Newton** :
$\forall n\in\mathbb N,\forall (a,b)\in\mathbb C,(a+b)^n = \sum_{k=0}^n \left(\dbinom{n}{k}a^kb^{n-k}\right)$ 
*Preuve* :
Pour $n = 0$ :
$(a+b)⁰=1 \land \sum_{k=0}^{0}\left(\dbinom{0}{k}a^kb^{n-k}\right) = 1$
Pour $n\ge 0$, supposons que au rang $n$ on a $(a+b)^n = \sum_{k=0}^n \left(\dbinom{n}{k}a^kb^{n-k}\right)$ et montrons alors qu'on a $(a+b)^{n=1} = \sum_{k=0}^{n+1} \left(\dbinom{n+1}{k}a^kb^{n+1-k}\right)$
$(a+b)^{n+1} = (a+b)(a+b)^n = (a+b)\times \sum_{k=0}^n \left(\dbinom{n}{k}a^kb^{n-k}\right)$

$=\sum_{k=0}^n\left(\dbinom{n}{k}a^{k+1}b^{n-k}\right) + \sum_{k=0}^{n}\left(\dbinom{n}{k}a^kb^{n+1-k}\right)$ 

$=\sum_{k=1}^{n+1}\left(\dbinom{n}{k-1}a^kb^{n-(k-1)}\right) +\sum_{k=0}^{n}\left(\dbinom{n}{k}a^kb^{n+1-k}\right)$ 
<small>Changement d'indice dans la première somme</small> 

$= a^{n+1} + \sum_{k=1}^{n}\left(\dbinom{n}{k-1}a^kb^{n-(k-1)}\right) +\sum_{k=1}^{n}\left(\dbinom{n}{k}a^kb^{n+1-k}\right) + b^{n+1}$ 
<small>On sort respectivement le dernier terme et le premier terme de la première et de la deuxième somme</small> 

$=a^{n+1} + \sum_{k=1}^n \left( \left[\dbinom{n}{k-1} + \dbinom{n}{k}\right]a^kb^{n+1-k}\right) + b^{n+1}$

$=\dbinom{n+1}{n+1}a^{n+1}b⁰ + \sum_{k=1}^n \left( \dbinom{n+1}{k}a^kb^{n+1-k}\right) + \dbinom{n+1}{0}a⁰b^{n+1}$ 
<small>On utilise la formule du triangle de Pascal</small>

$=\sum_{k=0}^{n+1} \left(\dbinom{n+1}{k}a^kb^{n+1-k}\right)$

On conclut selon le principe de récurrence que $\forall n\in\mathbb N,(a+b)^n = \sum_{k=0}^n \left(\dbinom{n}{k}a^kb^{n-k}\right)$


**Linéarisation de puissance de cos et sin** :

Exemple avec $\cos³(\theta)$ et $\sin³(\theta)$ : 

$\cos³(\theta)=\left(\dfrac{e^{i\theta}+e^{-i\theta}}{2}\right)^{3}=\dfrac{e^{3i\theta}+e^{-3i\theta}+3e^{i\theta}+3e^{-i\theta}}{8}=\dfrac{1}{4}(\cos(3\theta)+3\cos(\theta))$
$\sin³(\theta)=\left(\dfrac{e^{i\theta}-e^{-i\theta}}{2i}\right)^{3}=\dfrac{e^{3i\theta}-e^{-3i\theta}-3e^{i\theta}-3e^{-i\theta}}{-8i}=-\dfrac{1}{4}(\sin(3\theta)-3\sin(\theta))$ 


**Fonction exponentielle complexe** :
On définit $\exp_{\mathbb C} : \mathbb C \longrightarrow \mathbb C$ de la manière suivante :
Soit $z=a+ib\;,(a,b)\in\mathbb R$. On pose $\exp_{\mathbb C}(z) = e^{z} := e^{a}(\cos(b)+i\sin(b)) = re^{i\theta}$
Avec $r=e^{a}$ et $\theta \equiv b \;[2\pi]$.

<u>Remarque</u> :
- Soit $r\in\mathbb R$, $\exp_{\mathbb C} (r)=e^r$
- Soient $z=a+ib$ et $z'=a'+ib'$ alors 
$\exp_{\mathbb C}(z+z') = e^{a+a'}e^{i(b+b')}$
$=e^{a+a'}([(\cos(b)\cos(b')-\sin(b)\sin(b')]+i[\cos(b)\sin(b')-\cos(b')\sin(b)])$
$=e^{a+a'}(\cos(b)(\cos(b')+i\sin(b'))+i\sin(b)(\cos(b')+i\sin(b')))$
$=e^{a+a'}((\cos(b')+i\sin(b'))(\cos(b)+i\sin(b)))$
$=e^{a}e^{a'}e^{b}e^{b'}$
$=\exp_{\mathbb C}(z)\exp_{\mathbb C}(z')$
- $e^{-z}e^{z} = e^{z}e^{-z} = 1$
- $(e^{z})^{n} = e^{nz}$
- $\overline{e^{z}} = e^{\overline z}$

