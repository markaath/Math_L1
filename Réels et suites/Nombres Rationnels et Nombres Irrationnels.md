
$\mathbb Q = \{\frac{b}{c}, (b,c) \in \mathbb Z \times \mathbb N^*\}$ 
$\mathbb R \setminus \mathbb Q :=$ l'ensemble des irrationnels.

**Théorème :**
$\forall p \in \mathcal P,\sqrt{p} \notin \mathbb Q$ 

*Preuve :*
Par l'absurde. 
Supposons que $\sqrt{p} \in \mathbb Q$ ie $\exists (a,n) \in \mathbb Z \times \mathbb N^* : \sqrt{p} = \frac{a}{n}$. 
$\sqrt{p} > 0 => a \in \mathbb N^*$.  Quitte à factoriser par les facteurs communs, on suppose $a\land n = 1$.

$\sqrt{p} = \frac{a}{n} => p = \frac{a²}{n²}$ ie $p|a² => p|a$ car $p\in \mathcal P$
$\Rightarrow \exists b \in \mathbb N : a = pb$
$\Rightarrow p²b²=pn²$
$\Rightarrow pb²=n²$ 
$\Rightarrow p|n² \Rightarrow p|n$ Absurde, $n \land a = 1$ donc $\forall p \in \mathcal P,\sqrt{p} \notin \mathbb Q$. 

Remarque : $+,-,\times,/$ sont des LCI dans $\mathbb Q$

**Définition :**
$A \subseteq \mathbb R$ est dense dans $\mathbb R$ $\Leftrightarrow$ $\forall (a,b) \in \mathbb R², \exists x \in A : a < x < b$

**Théorème :**
$\mathbb Q$ et $\mathbb R \setminus \mathbb Q$ sont denses dans $\mathbb R$

*Preuve :*
Soient $(a,b) \in \mathbb R : a < b$.
- $\mathbb Q$ est dense dans $\mathbb R$ : 
Par Archimède, $\exists n \in \mathbb N^* : \frac{1}{n} < b-a$
$\Rightarrow a < a+\frac{1}{n} < b$
Soit $p:=\lfloor an \rfloor + 1 \in \mathbb Z$, alors $p-1 \le an < p$
$\Rightarrow a < \frac{p}{n} \le a + \frac{1}{n} < b$ et $\frac{p}{n} \in \mathbb Q$

- $\mathbb R \setminus \mathbb Q$ est dense dans $\mathbb R$ : 
Soient $a' = a - \sqrt{2}$ et $b' = b - \sqrt{2}$.
Alors $\exists r \in \mathbb Q : a' < r <b'$ et $r+\sqrt{2} \in \mathbb R \setminus \mathbb Q$.  Supposons que $c:= r +\sqrt{2} \in \mathbb Q$.
Alors $\sqrt{2}=c-r  \in \mathbb Q$, absurde et $a < r + \sqrt{2} < b$ 

**Corollaire :**
Tout intervalle réel contient une infinité de rationnels et une infinité d'irrationnels.

*Preuve :*
Montrons que $\forall (a,b) \in\mathbb R², \forall n \in\mathbb N^*,\forall i\in[\![2,n]\!],\exists x  \in\mathbb Q \;\cap\; ]a,\frac{b}{n}[\;\cap\;]\frac{(i-1)b}{n},\frac{ib}{n}[ \;\land \;\exists y \in\mathbb R\setminus\mathbb Q \;\cap \;]a,\frac{b}{n}[\;\cap\;]\frac{(i-1)b}{n},\frac{ib}{n}[$.
$\forall n\in\mathbb N^*,\forall i\in[\![1,n]\!],$ 
$(a,\frac{ib}{n}) \in\mathbb R²$ donc par la densité de $\mathbb Q$ et $\mathbb R\setminus Q$ dans $\mathbb R$, $\exists x \in\mathbb Q\; \cap\;]a,\frac{ib}{n}[$$\;\land\;\exists y \in\mathbb R\setminus \mathbb Q\; \cap\;]a,\frac{ib}{n}[\;\cap\;]\frac{(i-1)b}{n},\frac{ib}{n}[$
Et pour un $n$ donné,la densité nous donne $n$ rationnels et $n$ irrationnels dans $]a,b[$$=]a,\frac{b}{n}[\;\cup\;\bigcup_{i=1}^n ]\frac{(i-1)b}{n},\frac{ib}{n}[$ .
On pose $A=]a,\frac{b}{n}[\;\cup\;\bigcup_{i=1}^n ]\frac{(i-1)b}{n},\frac{ib}{n}[$.
Donc $card \big\{x \in\mathbb Q \;\cap\;A$$\big\}\underset{n\to +\infty}{\longrightarrow}+\infty$ et $card\big\{y\in\mathbb R\setminus \mathbb Q\; \cap\;A\big\}\underset{n\to +\infty}{\longrightarrow}+\infty$ 