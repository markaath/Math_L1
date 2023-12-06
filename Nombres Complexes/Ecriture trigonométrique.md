<u>Rappel de trigonométrie</u> :

- $\sin(\alpha + \beta) = \sin(\alpha)\cos(\beta)+\sin(\beta)\cos(\alpha)$ 
- $\cos(\alpha + \beta)= \cos(\alpha)\cos(\beta)-\sin(\alpha)\sin(\beta)$
- $\left|\sin\left( \dfrac{\beta}{2} \right)\right|=\sqrt{\dfrac{1-\cos(\beta)}{2}}$
- $\left|\cos\left(\dfrac{\alpha}{2}\right)\right| = \sqrt{\dfrac{1+\cos(\alpha)}{2}}$

**Nombres complexes de module 1** :
Soient $(z=a+ib,z'=a'+ib')\in\mathbb C² : |z|=|z'|=1$.
Alors $|zz'|=|z||z'|=1$ et $\dfrac{1}{z}=\dfrac{\overline z}{|z|²}=\overline z$
On note $\mathbb U = \{z\in \mathbb C\ : |z| = 1\}$

<u>Remarque</u> :
$\forall z \in\mathbb C^*,\exists(r,z_0)\in\mathbb R_+^*\times\mathbb U : z = r\cdot z_0$ et $z=|z|(\cos(\alpha)+i\cdot \sin(\alpha))$

**Définition** :
$\alpha$ est une argument de $z$, noté $arg(z)$

<u>Remarque</u> :
Tout $\alpha ' \equiv \alpha \;[2\pi]$ est aussi un argument de $z$.

**Définition** :
$\forall z \in\mathbb C^*, z=|z|(\cos(arg(z))+i\cdot \sin(arg(z)))$. On appelle cette écriture l'écriture trigonométrique. Tout $z\in\mathbb C^*$ est identifié par le couple $(|z|,arg(z))$

<u>Remarque</u> :
Avec cette écriture on peut écrire $\forall (z,z')\in\mathbb (C^*)²$,
$z=|z|\cdot z_0, z' = |z'|\cdot z'_0$ avec $(z_0,z'_0)\in\mathbb U$ et 
$z_0 = \cos(arg(z))+i\cdot \sin(arg(z))$
$z'_0= \cos(arg(z'))+i\cdot \sin(arg(z'))$
Et on a : $zz'=|z||z'|\left[(\cos(arg(z)\cos(arg(z'))-\sin(arg(z))\sin(arg(z')))\right]+i\cdot\left[\cos(arg(z))\sin(arg(z'))+\cos(arg(z'))\sin(arg(z))\right]$ $\quad\; =|z||z'|\left[\cos(arg(z)+arg(z'))+i\sin(\sin(arg(z)+arg(z'))\right]$
Et on obtient $|zz'|=|z||z'|$ et $arg(zz')=arg(z)+arg(z')$

**Propriété** :
Soit $z\in\mathbb C^*$
- $arg(-z)= \pi + arg(z)$
- $arg(\bar z) = -arg(z)$
- $arg\!\left(\dfrac{1}{z}\right)=-arg(z)$
- $arg(z^n)=n\cdot arg(z)$

**Formule de Moivre** :
$(\cos(\theta)+i\cdot\sin(\theta))^n=\cos(n\theta)+i\cdot\sin(n\theta)$ 
*Preuve* :
Soit $z = \cos(\theta) + i\sin(\theta) \in\mathbb U$, donc $z^n\in\mathbb U$ et $arg(z^n)=n\cdot arg(z)$
Donc $z^n = \cos(arg(z^n))+i\sin(arg(z^n))$ 
$=\cos(n\cdot arg(z)) + i\sin(n\cdot arg(z))$
$=\cos(n\theta) + i\sin(n\theta)$

