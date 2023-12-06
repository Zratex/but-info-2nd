Une Matrice linéaire est la représentation [[Matrices|matricielle]] d'une [[Applications linéaires]] (se référer à [[Comparaison Linéaire-Matrice]]).
Il existe donc des méthodes de conversions entre les 2 domaines.
## Application linéaire vers Matrice
Le modèle de transformation à suivre :

| Coordonnées en paramètres de $f$ | valeur de $x$ | valeur de $y$ | $...$ |
| :-: | :-: | :-: | :-: |
| valeur de $x$ dans le paramètre $f(x)$ | `Fonction[x][x]` | `Fonction[y][x]` | $...$ |
| valeur de $y$ dans le paramètre $f(y)$ | `Fonction[x][y]` | `Fonction[y][y]` | $...$ |
| $...$ | $...$ | $...$ | $...$ |
Si un élément pour une coordonnée n'est pas explicitée dans la forme linéaire, dans la matrice il faut le mettre égal à ==0==.
### Exemple
Admettons que l'on ait une [[Fonction]] $f$ définie comme ceci : $f(x,y)=(2x+y,y-x)$
Sa [[Matrices|matrice]] se formera comme ceci :
$$\begin{matrix} 2 & 1 \\ -1 & 1 \end{matrix}$$
#### Décomposition
| Parenthèses à regarder| valeurs de $x$ | valeurs de $y$ |
| :-: |:-: | :-: |
| **Première** | Nous avons $2x$, donc:<br><br>$x=2$ | Nous avons $+y$, soit $1*y$, donc:<br><br>$y=1$ |
| **Seconde** | Nous avons $-x$, ce qui revient à $-1*x$, donc:<br><br>$x=-1$ | Nous avons simplement $y$, soit $1*y$, donc:<br><br>$y=1$ |
