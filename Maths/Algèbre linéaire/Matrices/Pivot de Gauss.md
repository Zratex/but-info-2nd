L'objectif du pivot de Gauss est de trouver la [[Matrice de passage]] d'une [[Matrices|matrice]] donnée.
Le principe est qu'à chaque étape, on exerce une opération sur une des lignes de la [[Matrices|matrice]] donnée, et l'objectif est d'obtenir la [[Matrices unitaire|matrice identité]] de même [[Dimensions]].
## Procédé
D'une part, nous mettons notre [[Matrices|matrice]] d'origine à gauche, puis nous mettons la [[Matrices unitaire|matrice identité]] de même taille à droite.

Ensuite, quand on va réaliser une opération sur la partie de gauche, on va aussi la réaliser dans la partie de droite.

Une fois la [[Matrices unitaire|matrice identité]] obtenue à gauche, le contenu de celle de droite sera la [[Matrice de passage]].

> **Important :** Si le premier élément de la matrice est un `0`, il faut inverser sa ligne avec une autre
### Exemple
Prenons comme exemple cette matrice :
$$\begin{matrix} 2 & 5 \\ 6 & 1 \end{matrix}$$
Le détail du calcul du Pivot de Gauss sera :
```
Etape 1 : Placer les matrices
-------          ---------
2 | 5 |          | 1 | 0 |
6 | 1 |          | 0 | 1 |
Etape 2 : Réaliser les calculs
---------          ----------
2 | 5   |          | 1  | 0 |
0 | -14 | L2=L2-3L1| -3 | 1 |
---------          ----------

-------            ----------------
2 | 5 |            |   1  |   0   |
0 | 1 | L2=L2/(-14)| 3/14 | -1/14 |
-------            ----------------

-------        -----------------
2 | 0 | L1-5L2 | 15/14 | 5/14  |
0 | 1 |        | 3/14  | -1/14 |
-------        -----------------

-------      -----------------
1 | 0 | L1/2 | 15/28 | 5/28  |
0 | 1 |      | 3/14  | -1/14 |
-------      -----------------
```
Donc la [[Matrice de passage]] de $\begin{matrix} 2 & 5 \\ 6 & 1 \end{matrix}$ est :
$$\begin{matrix} \frac{15}{28} & \frac{5}{18} \\ \frac{3}{14} & -\frac{1}{14} \end{matrix}$$
