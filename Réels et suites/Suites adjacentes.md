
Soient $(a_n)_{n\in\mathbb N}$ et $(b_n)_{n\in\mathbb N}$ deux suites réelles telles que $(a_n)_{n\in\mathbb N} \nearrow$ et $(b_n)_{n\in\mathbb N} \searrow$ et $\lim\limits_{n\to +\infty} a_n - b_n = 0$. On dit  que $(a_n)_{n\in\mathbb N}$ et $(b_n)_{n\in\mathbb N}$ sont adjacentes. Dans ce cas, $\exists l \in\mathbb R : a_n \underset{n\to +\infty}{\longrightarrow} l \land b_n \underset{n\to +\infty}{\longrightarrow} l \land \forall n\in\mathbb N, a_n \le l \le b_n$.
*Preuve* :
Montrons que $(a_n)_{n\in\mathbb N}$ est majorée
Supposons que $(a_n)_{n\in\mathbb N}$ n'est pas majorée. Alors $a_n \underset{n\to + \infty}{\longrightarrow} +\infty$ et $b_n =b_n-a_n + a_n \underset{n\to +\infty}{\longrightarrow} + \infty$ donc $b_n \underset{n\to +\infty}{\longrightarrow} +\infty$, absurde car $(b_n)_{n\in\mathbb N}  \searrow$.
Donc $(a_n)_{n\in\mathbb N}$ est majorée, et par un argument symétrique, on montre que $(b_n)_{n\in\mathbb N}$ est minorée.
Alors, $\exists (a,b)\in\mathbb R² : a_n\underset{n\to +\infty}{\longrightarrow}a \land b_n\underset{n\to +\infty}{\longrightarrow}b$. 
Mais $0=\lim\limits_{n\to +\infty}(a_n -b_n)=\lim\limits_{n\to +\infty}a_n -\lim\limits_{n\to +\infty}b_n = a-b$ ie $a=b$.
Or $a=sup\{a_n,n\in\mathbb N\}$ donc $\forall n\in\mathbb N, a_n \le a$ et $b=inf\{b_n,\in\mathbb N\}$ donc $\forall n\in\mathbb N, b_n \ge b$
$\Rightarrow \forall n\in\mathbb N, a_n \le a=b\le b_n$.