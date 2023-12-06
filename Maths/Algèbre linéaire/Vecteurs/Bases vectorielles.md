Une base [[Vecteurs|vectorielle]] c'est un **espace** où tout éléments composant une famille de [[Vecteurs]] (exemple : $x$) seront indépendants.
Il faut savoir qu'un vecteur se combinant avec une base aura **qu'une seule** combinaison possible.

> En sachant cela, on peut définir les [[Dimensions]]
## Représentation par calcul
Si on a un plan $(\vec{i};\vec{j})$, tout [[Vecteurs|vecteurs]] du style $\vec{u} = (x,y)$ s'exprimeront de cette manière :
$$\vec{u} = x*\vec{i} + y*\vec{j}$$
### Exemple
Base = $(\vec{i};\vec{j})=((1,0);(0,1))$
Si $\vec{u}=(1,3)$ alors $\vec{u}$ dans notre base sera égal à $1*(1,0) + 3*(0,1)$
> C'est avec ça que l'on construit des [[Coordonnées]]
## Base canonique
C'est la base par défaut d'un [[Ensembles mathématiques#^fef7da|ensemble]] $\mathbb{R}^n$.

| Ensemble $\mathbb{R}^n$ | Base canonique | Représentation par calcul |
| :-: | :-: | :-: |
| $\mathbb{R}^1$ | `1` | $x*1$ |
| $\mathbb{R}^2$ | `{(1,0);(0,1)}` | $x*(1,0) + y*(0,1)$ |
| $\mathbb{R}^3$ | `{(1,0,0);(0,1,0);(0,0,1)}` | $x*(1,0,0)+y*(0,1,0)+z*(0,0,1)$
| $...$ | $...$ | $...$ |