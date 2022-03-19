# Chapitre 23 : Espaces vectoriels
## Prop 5.4 (Caractérisation d'une somme directe)
Deux sous-espaces vectoriels $A$ et $B$ de $E$ sont en somme directe ssi $A\cap B=\{0\}$.

**Démo :**

Si $A\cap B=\{O\}$

$\begin{aligned}
    \text{Soient }
    &a,a'\in A
    \\
    &b,b'\in B
    \\
    &\text{tq } a+b=a'+b'
\end{aligned}
$

$
\begin{aligned}
    \text{Mque }
    &a=a'
    \\
    &b=b'
\end{aligned}
$

Or $a+b=a'+b'$

Donc $a-a'=b-b'$

$\begin{aligned}
    \text{Mais }
    &a-a'\in A \text{ (sev de } E\text{)}
    \\
    &b-b'\in B \text{ (sev de } E\text{)}
\end{aligned}
$

Donc $a-a'\in A\cap B=\{0\}$

Donc $a = a'$ et $b=b'$

**Réciproque :**

Supposons que $A+B$ est une somme directe

Soit $x\in A\cap B$

$
\begin{aligned}
    \text{Alors } x
    &=\underset{\in A}{x}+\underset{\in B}{0}
    \\
    &=\underset{\in A}{0}+\underset{\in B}{x}
\end{aligned}
$

Par unicité de l'écriture, $x=0$

Donc $A\cap B\subset\{O\}$

Mais $0\in A\cap B$ (sev)

Donc $A\cap B=\{O\}$

---
## Prop 5.6 (Famille génratrice d'une somme)
$\begin{aligned}
    \text{Soient }
    &A \text{ et } B \text{ deux sous-espaces vectoriels de } E
    \\
    &\mathcal F\text{ une famille génératrice de }A
    \\
    &\mathcal G\text{ une famille génératrice de }B
\end{aligned}
$

Alors la famille $F\cup G$ est une famille génératrice de $A+B$.

**Démo**

$\begin{aligned}
    \text{Supposons }
    &\mathcal F =(x_i)_{1\le i\le n}
    \\
    &\mathcal G = (y_i)_{1\le j\le p}
\end{aligned}
$

où $n,p\in\mathbb{N}^*$

Soit $u\in A+B$

$
\begin{aligned}
    \text{Alors }
    &\exists a\in A
    \\
    &\exists b\in B
\end{aligned}
$

tq $u=a+b$

$
\begin{aligned}
    \text{Or }
    &\forall i\in [1;n], \exists \lambda_j\in K^n
    \\
    &\forall j\in [1;p], \exists \mu_j\in K^p
\end{aligned}
$

$
\begin{aligned}
    \text{tq }
    &a=\sum_{i=1}^n \lambda_i x_i
    \\
    &b=\sum_{j=1}^n \mu_j y_j
\end{aligned}
$

et $a+b=\sum_{i=1}^n \lambda_i x_i+\sum_{j=1}^n \mu_j y_j\in vect(\mathcal F\cup\mathcal G)$

Donc $A+B\subset vect(\mathcal F\cup\mathcal G)$

Mais $\mathcal F\cup\mathcal G\subset A+B$

Donc $vect(\mathcal F\cup\mathcal G)\in A+B$

(car $A$ et $B$ est un sev de $E$)

$
\begin{aligned}
    \text{Donc }
    &vect(\mathcal F\cup\mathcal G)\in A+B\text{ (car } A\text{ et } B\text{ est un sev de }E\text{)}
    \\
    &A+B=vect(\mathcal F\cup\mathcal G)
\end{aligned}
$