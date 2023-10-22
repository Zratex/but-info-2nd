# Enoncé
Si il y a ==n== tirages **sans remise** dans une urne de ==N== boules, ==X== est la [[Variables aléatoires|variable aléatoire]] comptant le nombre de bonnes boules piochées ;
> Alors c'est une loi **hypergéométrique** de paramètres `N`, `n`, `p`
## Correspondance des paramètres
Ce segment est pour faire en sorte de référencer les paramètres, afin que quand on passera la souris sur un paramètre dans les formules qui suivront, sa description apparaîtra.

==n== correspond au **nombre de répétions** ^06a7a3

==p== correspond à la **probabilité** que l'événement recherché **se réalise.** Calcul : `N1/N` ^9a53b9

==k== correspond au **nombre de tirages requis pour réussir** ^ab957f
### Représentations de N
==N== correspond au **nombre de boules** dans l'urne.
- ==N1== : nombre de boules **gagnante**
  - Calcul : `p*N`
- ==N2== : nombre de boules **perdante**
  - Calcul : `(1-p)*N`
  - Autre propriété : `N2/N = 1-p`
# Formule
Une fois l'énoncé posé, on note $X \sim \mathcal{H}(n,p,N)$ ; et on a donc :
- $\Omega_X =$ {max(0 ; [[Loi hypergéométrique#^06a7a3|n]] - [[Loi hypergéométrique#Représentations de N|N2]]), ... , min([[Loi hypergéométrique#^06a7a3|n]] ; [[Loi hypergéométrique#Représentations de N|N1]])}
- $\displaystyle\forall$ [[Loi hypergéométrique#^ab957f|k]] $\in \Omega_X, \quad \mathbb{P}(X=k) = \frac{\binom{N_1}{k}\binom{N_2}{n-k}}{\binom{N}{n}}$

A savoir que :
- $\Omega$ = [[Univers]]
- le calcul avec les parenthèses correspond à des [[Coefficient binomiale|coefficients binomiaux]]
## Autres formules
- <u>Espérance :</u> $\mathbb{E}(X) =$ [[Loi hypergéométrique#^06a7a3|n]] * [[Loi hypergéométrique#^9a53b9|p]]
- <u>Variance :</u> $\mathbb{V}(X) =$ [[Loi hypergéométrique#^06a7a3|n]] $*$ [[Loi hypergéométrique#^9a53b9|p]] $*$ (1-[[Loi hypergéométrique#^9a53b9|p]]) $*\frac{N-n}{N-1}$
# Exemples
Exemple d'utilisation de la loi hypergéométrique dans le cadre d'un exercice.
## Exo 1 : GPT
Je viens de faire un test, et je pensais pas que ChatGPT (3.5) pouvait rédiger lui même des exercices.
### Enoncé
```
Dans un sac contenant 20 boules, 8 sont rouges et 12 sont vertes.
On souhaite tirer 5 boules du sac sans les remettre.

Quelle est la probabilité que parmi les 5 boules tirées, exactement 3 soient rouges ?
```
### Définition des valeurs
$X$ est une [[Variables aléatoires|variable aléatoire]] décrivant la probabilité de tirer **3 boules rouges sur 5 tirées**. Ce qu'il veux dire que :
- On cherche $\mathbb{P}(X=3)$
  Donc dans la formule, ==k== sera égal à 3
- $X$ suis une loi Hypergéométrique noté $X \sim \mathcal{H}(n,p,N)$ ; où :
	- ==n== est le nombre de boules tirées
	  Ici n=**5**
	- ==N== est le nombre de boules totales
	  Ici N=**20**
	- ==N1== représente le nombre de boules gagnantes
	  Ici N1=**8**
	- On admet donc que ==N2== = N-N1 = **12**
### Calcul
$\displaystyle\forall$ [[Loi hypergéométrique#^ab957f|k]] $\in \Omega_X, \quad \mathbb{P}(X=3) = \frac{\binom{8}{3}\binom{12}{5-3}}{\binom{20}{5}}$
- $\mathbb{P}(X=3) = \frac{56*\binom{12}{2}}{\binom{20}{5}}$
- $\mathbb{P}(X=3) = \frac{56*\binom{12}{2}}{15504}$
- $\mathbb{P}(X=3) = \frac{56*66}{15504}$
- $\mathbb{P}(X=3) = \frac{3696}{15504}$
- $\mathbb{P}(X=3) \approx 0.238$

(détail du calcul des [[Coefficient binomiale|coefficients binomiaux]] ici : [[Calcul coef binomiale]])