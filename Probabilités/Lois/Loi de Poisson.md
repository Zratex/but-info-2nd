# Enoncé
Quand un énoncé admet ==X== occurrences sur une certaine intervalle de temps, on admet que $\lambda$ est la moyenne sur un intervalle de temps prédéfini.
# Formule
On note $X \sim \mathcal{P}(\lambda)$ ; On a donc :
- $\Omega_X$ = {0 ,1 , $\cdots$ }
- $\forall k \in \Omega_X , \mathcal{P}(X=k) = \frac{\lambda^k*e^{-\lambda}}{k!}$

A savoir que :
- $\Omega$ = [[Univers]]
- $\lambda$ = moyenne sur un intervalle de temps prédéfini
- e = fonction exponentielle
## Autres formules
- <u>Espérance :</u> $\mathbb{E}(X) =$ $\lambda$
- <u>Variance :</u> $\mathbb{V}(X)=$ $\lambda$ 

# Exemple
## Exo 1 : GPT (nul)
Encore un exo par ChatGPT (3.5). Vraiment très intéressant cette fonctionnalité
### Enoncé
```
Dans une usine de production de pièces électroniques, on observe en moyenne 2 défaillances de composants par jour. Les défaillances surviennent de manière aléatoire et suivent une distribution de Poisson.

Quelle est la probabilité qu'il n'y ait aucune défaillance de composants en une journée ?
```
### Définition des valeurs
$X$ est une [[Variables aléatoires|variable aléatoire]] décrivant la probabilité qu'il n'y ait aucune défaillance sur une journée.
- On cherche $\mathbb{P}(X=0)$
  Donc ==k== sera égal à **0**
- $X$ suis une loi de poisson noté $X \sim \mathcal{P}(\lambda)$ ; où :
	- $\lambda$ est le nombre moyen de défaillances par jour
	  Ici $\lambda=2$
### Calcul
$\forall k \in \Omega_X , \mathcal{P}(X=k) = \frac{\lambda^k*e^{-\lambda}}{k!}$
- $\mathcal{P}(X=0) = \frac{2^0*e^{-2}}{0!}$
- $\mathcal{P}(X=0) = \frac{e^{-2}}{1}$
- $\mathcal{P}(X=0) = e^{-2}$
## Exo 2 : GPT (non-nul)
Même énoncé que l'exo précédent, mais on cherche autre chose :
### Enoncé
```
Dans une usine de production de pièces électroniques, on observe en moyenne 2 défaillances de composants par jour. Les défaillances surviennent de manière aléatoire et suivent une distribution de Poisson.

Quelle est la probabilité qu'il y ait au moins 3 défaillances de composants en une journée ?
```
### Définition des valeurs
$X$ est une [[Variables aléatoires|variable aléatoire]] décrivant la probabilité qu'il n'y ait aucune défaillance sur une journée.
- On cherche $\mathbb{P}(X<3)$
  A savoir que $\mathbb{P}(X<3)=\mathbb{P}(X=0)+\mathbb{P}(X=1)+\mathbb{P}(X=2)$
- $X$ suis une loi de poisson noté $X \sim \mathcal{P}(\lambda)$ ; où :
	- $\lambda$ est le nombre moyen de défaillances par jour
	  Ici $\lambda=2$
### Calcul
$\forall k \in \Omega_X , \mathcal{P}(X=k) = \frac{\lambda^k*e^{-\lambda}}{k!}$
- Calcul de $\mathbb{P}(X=0)$ :
	(valeur reprise dans l'exo précédent)
	$\mathbb{P}(X=0) = e^{-2}$
- Calcul de $\mathbb{P}(X=1)$ (on remplace donc **k** par 1 dans la formule) :
	- $\mathbb{P}(X=1) = \frac{2^1*e^{-2}}{1!}$
	- $\mathbb{P}(X=1) = 2*e^{-2}$
- Calcul de $\mathbb{P}(X=2)$ (on remplace donc **k** par 2 dans la formule) :
	- $\mathbb{P}(X=2) = \frac{2^2*e^{-2}}{2!}$
	- $\mathbb{P}(X=2) = \frac{4*e^{-2}}{2}$
	- $\mathbb{P}(X=1) = 2*e^{-2}$

Calcul de $\mathbb{P}(X<3)=\mathbb{P}(X=0)+\mathbb{P}(X=1)+\mathbb{P}(X=2)$ :
- $\mathbb{P}(X<3)= e^{-2} + 2*e^{-2} + 2*e^{-2}$ 