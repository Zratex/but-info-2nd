Noté ${\binom{n}{k}}$ se disant "k parmi n".
A calculer, cela revient à faire $\frac{n!}{k!(n-k)!}$
## Méthode de calcul
Tableau représentant comment calculer un coefficient binomiale.
Il faut se dire que le tableau est représenté par la fonction C, et que ses paramètres correspond aux coordonnées du tableau.

| ${\binom{n}{k}}$ | **0** | **1** | **2** | $...$ | $k$ |
| :-: | :-: | :-: | :-: | :-: | :-: |
| **0** | 1 | | | | |
| **1** | `1` | ==1== | | | |
| **2** | 1 | C(2,1)=`C(1,0)`+==C(1,1)== = 2 | 1 | | |
| $...$ | | | | | |
| $n$ | | | | | |
A savoir que :
- quand un paramètre est à 0, le résultat est 0
- Le dernier élément de la ligne sera toujours égal à 1, car il n'existe pas de valeur de même coordonnée `k` en `n-1`
- La formule autrement est $C(n,k)=C(n-1,k-1)+C(n-1,k)$
> Pour faire simple, un élément `x` du tableau est égal à l'élément au dessus + l'élément en haut à gauche de `x`
