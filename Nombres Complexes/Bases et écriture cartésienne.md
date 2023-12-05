
**Définition** : 
On introduit un nouvel objet mathématique appelé $i$ tel que : 
- $i \notin \mathbb R$ 
- $i² = -1$
Donc $i$ est une solution de $x² + 1 = 0$

**Définition** : 
Un nombre complexe est un objet de la forme $a+ib, (a,b) \in \mathbb R²$.
$\mathbb C = \{a + ib, (a,b) \in \mathbb R²\}$

**Définition** : Opération sur $\mathbb C$ 
Soient $z = a + ib$ et $z' = a' +ib', \;(z,z' \in \mathbb C)$.
- $z+z' = (a+ib)+(a'+ib') = (a + a') + i(b+b')$
- $z\cdot z' = (a+ib)(a'+ib') = (a\cdot a' - b \cdot b') + i(b\cdot a' + a\cdot b')$ 

**Propriété** : 
$+$ et $\cdot$ ont les mêmes propriétés que dans $\mathbb R, \mathbb Q, \mathbb Z, \mathbb N$ 

**Définition** : 
Soit $z = a + ib$ 
- $a$ est la partie réelle de $z$, notée $Re(z)$
- b est la partie imaginaire de $z$, notée $Im(z)$

**Propriété** : 
Le produit $z\cdot z' = 0 \Leftrightarrow z = 0 \lor z'= 0$ 

**Définition** : 
Soit $z = a+ib \in \mathbb C$ 
- $-z = -a -ib$ est l'opposé de $z$ et $z+(-z) = 0$ et $-1\cdot z = -z$
- si $r\in \mathbb R$, on défini $r\cdot z = ra + irb$ 
- $a-ib = \bar z$ est le conjugué de $z$

<u>Remarque</u> : 
$z \cdot \bar z = (a+ib)(a-ib)= a² + b² = Re(z)² + Im(z)²$

**Définition** : 
$\sqrt{a²+b²} = |z|$ est le module de $z$ et $z\cdot\bar z = |z|²$
De plus $|\bar z| = |z|$

<u>Remarque</u> : 
Soit $z\in \mathbb C^*$
On considère le nombre complexe $\bar z \cdot \dfrac{1}{|z|²}= \dfrac{a-ib}{a² + b²}$ et comme $z\cdot \bar z = |z|²$, on a $\dfrac{1}{z} = \dfrac{\bar z}{|z|²}$. 
Donc tout nombre complexe différent de $0$ a un inverse multiplicatif.

**Définition** : 
$\forall z \in \mathbb C, z'\in\mathbb C^*$
$\dfrac{z}{z'} = \dfrac{z\cdot \overline {z'}}{|z|²}$ 

**Règles de calcul** :
- $\overline {z_1 + z_2} = \bar z_1 + \bar z_2$ 
- $\overline {z_1\cdot z_2} = \bar z_1\cdot \bar z_2$ 
- $|\bar z| = |z|$
- $|z_1 \cdot z_2| = |z_1|\cdot|z_2|$

**Théorème** : Inégalité triangulaire
$\forall (z,z')\in\mathbb C², |z+z'| \le |z| +|z'|$ 
*Preuve* :
$|z+z'|² = (z+z')(\overline{z+z'})$
$=z\overline {z} + z\overline {z'}+ z'\overline {z}+z'\overline {z'}$ 
$=|z|² + |z'|² + z\overline {z'} + z'\overline{z}$
$=|z|² + |z'|² + \overline{z\overline{z'}} + z\overline{z'}$
$=|z|² + |z'|² +2Re(z\overline{z'})$
Or on a $Re(z\overline{z'})\le |z\overline{z'}|$, d'où 
$|z+z'|² \le |z|² + |z'|² +2|z\overline{z'}| \Longleftrightarrow |z+z'|² |z|² + |z'|² + 2|z||z'|$
$\Longleftrightarrow |z + z'|² \le (|z|+|z'|)²$
$\Longleftrightarrow |z+z'| \le |z| + |z'|$

**Corollaire** : 
En particulier, l'inégalité triangulaire est vraie dans $\mathbb R$ : 
$\forall (x,y)\in \mathbb R², |x+y| \le |x|+|y|$






