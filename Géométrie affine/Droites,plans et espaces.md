Soit $(O,\vec{i},\vec{j},\vec{k})$ un ROND.

**Plan affine :**
On le note souvent $\mathbb R²$. 

<u>Droites dans le plan </u> :

1) On se donne un point $P \in \mathbb R²$ est un vecteur directeur $\vec{u} \in \mathbb R² : \vec{u} \neq \vec{0}$. L'équation paramétrique de la droite passant par $P = (a,b)$ et de vecteur directeur $\vec{u} = \begin{pmatrix} u_1 \\ u_2 \end{pmatrix}$ est : $$D=\{ (x,y) \in \mathbb R² : \exists \lambda \in \mathbb R : x = a+\lambda u_1 \land y = b + \lambda u_2\}$$ $(P,\vec{u})$ est un repère de la droite $D$.
2) On se donne $(a,b,c)\in \mathbb R³ : (a,b) \neq (0,0)$. Une équation cartésienne d'une droite dans le plan est de la forme : $$ax+by+c=0$$
3) Étant donné $P\neq P'$ avec $(P,P')\in {(\mathbb R²)}²$, il existe une unique droite qui passe par ces deux points.

**Espace fixe affine :**
On le note souvent $\mathbb R³$.

<u>Plans dans l'espace</u> :

1) Soient $(\vec{u},\vec{v}) \in \mathbb (R³)²\setminus \{(\vec{0},\vec{0})\} : \vec{u} \bcancel{\parallel} \vec{v}$ et $P\in\mathbb R³$ un point de coordonnées $(a,b,c)$. $(P,\vec{u},\vec{v})$ est un repère du plan d'équation paramétrique : $$\begin{cases}
x = a+\lambda u_x + \mu v_x \\ y = b+ \lambda u_y + \mu v_y \\ z= c+ \lambda u_z + \mu v_z \end{cases} \quad,((\lambda,\mu) \in \mathbb R²)$$
2) Soient $(a,b,c,d)\in \mathbb R⁴ : (a,b,c) \neq (0,0,0)$. Une équation cartésienne d'un plan est de la forme $$ax+by+cz+d=0$$
3) Étant donné trois points de l'espace $P,P',P''$ il existe un unique plan passant par les trois points.

<u>Droites dans l'espace</u> :

1) Soient $\vec{u}\in \mathbb R³\setminus\{\vec{0}\}$ et un point $P \in \mathbb R³ : \vec{u} = \begin{pmatrix} u_1 \\ u2 \\ u3 \end{pmatrix}$ et $P=(a,b,c)$. $(P,\vec{u})$ nous donne un repère pour la droite d'équation paramétrique : $$\begin{cases} x = a+ \lambda u_1 \\ y=b+ \lambda u_2 \\ z=c+\lambda u_3\end{cases} \quad ,(\lambda \in \mathbb R)$$
2) Soient $(a,b,c,d,a',b',c',d') \in \mathbb R⁸ : ((a,b,c),(a',b',c')) \neq ((0,0,0),(0,0,0))$ et $\begin{pmatrix} a \\b\\c \end{pmatrix} \bcancel{\parallel} \begin{pmatrix} a'\\b'\\c'\end{pmatrix}$. Le système suivant définit l'équation cartésienne d'une droite dans l'espace : $$\begin{cases}ax+by+cz+d=0\\a'x+b'y+c'z+d'=0\end{cases}$$
3) Étant donné deux points de l'espace $P\neq P',(P,P')\in\mathbb (R³)²$, il existe une unique droite passant par ces deux points.

<u>Dans un super-espace</u> :

Soient $D$ une droite, $(P,\vec{u})$ un repère pour $D$, avec $P\in R⁴, \vec{u}\in \mathbb R⁴ \setminus{\vec{0}}$ et $$D=\{Q\in\mathbb R⁴ : \exists \lambda \in\mathbb R⁴ : Q=P+\lambda \vec{u}\}$$
Soient $(a_{ij})_{j\in[1,4]}^{i\in[1,3]} \in R¹²,(b_1,b_2,b_3)\in \mathbb R³ : (a_{1j})_{j\in[1,4]} \bcancel{\parallel} (a_{2j})_{j\in[1,4]} \bcancel{\parallel} (a_{3j})_{j\in[1,4]}$ et $\forall j\in [\![1,4 ]\!], (a_{1j}),(a_{2j}),(a_{3j})$ sont non simultanément nuls. Une équation paramétrique de $D$ est :$$\begin{cases}a_{11}x_1+a_{12}x_2+a_{13}x_3+a_{14}x_4 = b_1 \\ a_{21}x_1+a_{22}x_2+a_{23}x_3+a_{24}x_4 =b_2\\a_{31}x_1+a_{32}x_2+a_{33}x_3+a_{34}x_4 =b_3\end{cases}$$
