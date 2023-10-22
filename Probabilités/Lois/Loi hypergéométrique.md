# Enoncé
Si il y a ==n== tirages **sans remise** dans une urne de ==N== boules, ==X== est la variable aléatoire comptant le nombre de bonnes boules piochées ;
> Alors c'est une loi **hypergéométrique** de paramètres `N`, `n`, `p`
## Correspondance des paramètres
Ce segment est pour faire en sorte de référencer les paramètres, afin que quand on passera la souris sur un paramètre dans les formules qui suivront, sa description apparaîtra.

==n== correspond au **nombre de répétions** ^06a7a3

==p== correspond à la **probabilité** que l'événement recherché **se réalise.** Calcul : `N1/N` ^9a53b9
### Représentations de N
==N== correspond au **nombre de boules** dans l'urne.
- ==N1== : probabilité boule **gagnante**
  - Calcul : `p*N`
- ==N2== : probabilité boule **perdante**
  - Calcul : `(1-p)*N`
  - Autre propriété : `N2/N = 1-p`
# Formule
Une fois l'énoncé posé, on note $X \sim \mathcal{H}(n,p,N)$ ; et on a donc :
- $\Omega_X =$ {max(0 ; [[Loi hypergéométrique#^06a7a3|n]] - [[Loi hypergéométrique#Représentations de N|N2]]), ... , min([[Loi hypergéométrique#^06a7a3|n]] ; [[Loi hypergéométrique#Représentations de N|N1]])}
- $\displaystyle\forall k \in \Omega_X, \quad \mathbb{P}(X=k) = \frac{\binom{N_1}{k}\binom{N_2}{n-k}}{\binom{N}{n}}$

A savoir que :
- $\Omega$ = [[Univers]]
- le calcul avec les parenthèses correspond à des [[Coefficient binomiale|coefficients binomiaux]]
## Autres formules
- <u>Espérance :</u> $\mathbb{E}(X) =$ [[Loi hypergéométrique#^06a7a3|n]] * [[Loi hypergéométrique#^9a53b9|p]]
- <u>Variance :</u> $\mathbb{V}(X) =$ [[Loi hypergéométrique#^06a7a3|n]] $*$ [[Loi hypergéométrique#^9a53b9|p]] $*$ (1-[[Loi hypergéométrique#^9a53b9|p]]) $*\frac{N-n}{N-1}$
# Exemple
Exemple d'utilisation de la loi hypergéométrique dans le cadre d'un exercice.