# Chapitre 23 : Espaces vectoriels
## Prop 5.4 (Caractérisation d'une somme directe)

Soit $A$ et $B$ 2 sev de $E$.

Alors $A$ et $B$ sont en somme directe ssi $A\cap B=\{0\}$.

**Démonstration :**

$\text{Si }A\cap B=\{O\}$

$
\begin{aligned}
    \text{Soient }
    &a,a'\in A
    \\
    &b,b'\in B
    \\
    &\text{tq }a+b=a'+b'
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

$\text{Or }a+b=a'+b'$

$\text{Donc }a-a'=b-b'$

$
\begin{aligned}
    \text{Mais }
    &a-a'\in A \text{ (sev de } E\text{)}
    \\
    &b-b'\in B \text{ (sev de } E\text{)}
\end{aligned}
$

$\text{Donc }a-a'\in A\cap B=\{0\}$

$\text{Donc }a = a' \text{et } b=b'$

**Réciproque :**

$\text{Supposons que }A+B\text{ est une somme directe}$

$\text{Soit }x\in A\cap B$

$
\begin{aligned}
    \text{Alors } x
    &=\underset{\in A}{x}+\underset{\in B}{0}
    \\
    &=\underset{\in A}{0}+\underset{\in B}{x}
\end{aligned}
$

$\text{Par unicité de l'écriture, }x=0$

$\text{Donc }A\cap B\subset\{O\}$

$\text{Mais }0\in A\cap B$ (sev)

$\text{Donc }A\cap B=\{O\}$

---
## Prop 5.6 (Famille génratrice d'une somme)
$
\begin{aligned}
    \text{Soient }
    &A \text{ et } B \text{ 2 sev de } E
    \\
    &\mathcal F\text{ une famille génératrice de }A
    \\
    &\mathcal G\text{ une famille génératrice de }B
\end{aligned}
$

$\text{Alors la famille }F\cup G\text{ est une famille génératrice de }A+B$.

**Démonstration :**

$\begin{aligned}
    \text{Supposons }
    &\mathcal F =(x_i)_{1\le i\le n}
    \\
    &\mathcal G =(y_j)_{1\le j\le p}
\end{aligned}
\text{ où }n,p\in\mathbb{N}^*$

$\text{Soit }u\in A+B$

$
\begin{aligned}
    \text{Alors }
    &\exists a\in A
    \\
    &\exists b\in B
\end{aligned}
\text{ tq }u=a+b$

$
\begin{aligned}
    \text{Or }
    &\forall i\in [1;n], \exists \lambda_i\in K^n
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

$\text{et }\displaystyle a+b=\sum_{i=1}^n\lambda_i x_i+\sum_{j=1}^n\mu_j y_j\in vect(\mathcal F\cup\mathcal G)$

$\text{Donc }A+B\subset vect(\mathcal F\cup\mathcal G)$

$\text{Mais }\mathcal F\cup\mathcal G\subset A+B$

$
\begin{aligned}
    \text{Donc }
    &vect(\mathcal F\cup\mathcal G)\subset A+B\text{ (car } A\text{ et } B\text{ sont sev de }E\text{)}
    \\
    &A+B=vect(\mathcal F\cup\mathcal G)
\end{aligned}
$

---
## Prop 5.7 (Famille libre d'une somme directe)
$
\begin{aligned}
    \text{Soient }
    &A\text{ et }B\text{ 2 sev de }E\text{ en somme directe}
    \\
    &\mathcal F\text{ une famille génératrice de }A
    \\
    &\mathcal G\text{ une famille génératrice de }B
\end{aligned}
$

$\text{Alors la famille }\mathcal F\cup\mathcal G\text{ est une f.l de }A\oplus B$.

**Démonstration :**

$\begin{aligned}
    \text{Supposons }
    &\mathcal F =(x_i)_{1\le i\le n}
    \\
    &\mathcal G =(y_j)_{1\le j\le p}
\end{aligned}
\text{ où }n,p\in\mathbb{N}^*$

$
\begin{aligned}
    \text{Soient }
    &\forall i\in [1;n], \lambda_i\in K^n
    \\
    &\forall j\in [1;p], \mu_j\in K^p
\end{aligned}
\text{ tq }\displaystyle\sum_{i=1}^n\lambda_i x_i+\sum_{j=1}^n\mu_j y_j=0$

$\begin{aligned}
    \text{Donc }
    &\underset{\in A}{\sum_{i=1}^n\lambda_i x_i}=\underset{\in B}{-\sum_{j=1}^n\mu_j y_j}
    \\
    &A\cap B=\{0\}
\end{aligned}
$

$\text{Donc } \displaystyle\sum_{i=1}^n\lambda_i x_i+\sum_{j=1}^n\mu_j y_j=0$

$\text{Or }\mathcal F \text{ et }\mathcal G\text{ sont libres}$

$
\begin{aligned}
    \text{Donc }
    &\forall i\in [1;n], \lambda_i=0
    \\
    &\forall j\in [1;p], \mu_j=0
    \\
    &\mathcal F\cup\mathcal G\text{ est libre}
\end{aligned}
$

---
## Théo 6.3
Soit $E$ un espace vectoriel de dimension finie.
            
Alors :
1. $E$ admet une base finie
2. Toutes les bases de $E$ sont finies, et ont le même nombre d'éléments

**Démonstration :**

$\text{On suppose } E\not ={\{0\}}$

1. $\text{Par hypothèse, } E\text{ admet une f.g finie }(u_i)_{1\le i\le n}$

   $\text{Où }n\in N^* (n\not ={0}\text{ car }E\not ={\{0\}})$
   
   $\text{Si }(u_i)_{1\le i\le n}\text{ est libre : c'est une base finie}$

   $\text{Sinon, par 4.11, un des }u_i\text{ est c.l des autres}$
   
   $\text{Par exemple }u_n\in vect((u_i)_{1\le i\le n-1}(\text{et donc }n\ge 2\text{ car }E\not ={\{0\})}$

   ...

2. $
\begin{aligned}
    \text{Soient }
    &B\text{ une base finie de }E
    \\
    &B'\text{ une autre base finie de }E
\end{aligned}
$

    $
\begin{aligned}
    \text{Or }
    &B\text{ est libre}
    \\
    &B'\text{ est génératrice}
\end{aligned}
$

    $\text{Donc par 6.2, } card(B)\le card(B')\text{ ie }B\text{ est fini}$

    $\text{Donc }card(B')=card(B)$