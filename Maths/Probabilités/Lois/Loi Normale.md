# Enoncé
Si une distribution de données continu est caractérisé par une moyenne ==m==, avec une dispersion des valeurs ==σ== (écart-type) ;
> Alors ==X== suit une loi **Normale** de paramètres `m` et `σ`

$F_X(t)$ représente la répartition de la [[Variables aléatoires|variable aléatoire]] $X$.
C'est donc la [[Probabilités|probabilité]] que $X$ soit inférieur ou égal à ==t==
## Correspondance des paramètres
- ==m== correspond à la moyenne donné dans l'énoncé
- ==σ== correspond à l'écart-type, c'est à dire que :
  - m-σ : valeur minimale pouvant être tirée
  - m+σ : valeur maximale pouvant être tirée

## Implication graphique
Sur une courbe de normale [[Loi Normale#Centrée et réduite|centrée réduite]], 0 coupe le graphique en 2 :
- A gauche : aires A et B
- A droite : aires C et D

Ce qui sépare chaque zone, c'est l'emplacement de la valeur de `t` (et du coup par symétrie il ne faut pas oublier `-t`).

Ces aires ont des propriétés géométriques :
- A=D car symétrie centré sur 0
- B=C car symétrie centré sur 0
- A+B+C+D=1 car c'est la totalité de la surface du graphique, donc ces possibilités que l'on peux avoir
# Formule
Une fois l'énoncé posé, on note  $X \sim \mathcal{N}(m,\sigma^2)$ ; et on a donc :
$$f(x) = \frac{1}{\sigma\sqrt{2\pi}}e^{-\frac{1}{2}\left(\frac{x-m}{\sigma}\right)^2}$$
## Centrée et réduite
Si m=0 et σ=1, on appelle ça une loi normale **centrée-réduite**. 
Cette distribution particulière implique un changement de la formule, en ceci :
$$\frac{X-m}{\sigma}\sim \mathcal{N}(0;1)$$

A savoir que $Z=\frac{X-m}{\sigma}$

Cela implique que :
- $F_X(0) = 0.5$
  Parce que c'est la moitié de σ=1
- $F_X(t)=1-F_X(-t)$
  > ==Je ne comprends pas ce que ça représente==
# Exemples
## Exo 1 : Guérite
Exemple d'exercice de Blanchard :
### Enoncé
```
On envisage de construire à l'entrée d'une caserne une guérite dans laquelle pourra s'abriter la sentinelle en cas d'intempéries.
Les sentinelles sont des appelés dont la taille est approximativement distribuée selon une loi normale de moyenne 175cm et d'écart-type 7cm.

A quelle hauteur minimale doit se trouver le toît de la guérite pour qu'au moins 95% des sentinelles puissent s'y tenir debout ?
```
### Définition des valeurs
$X$ est une [[Variables aléatoires|variable aléatoire]] décrivant la taille d'un individu sélectionné.
- On cherche pas $\mathbb{P}(X<h)$ car on sais que c'est égal à 0.95, mais on cherche surtout ==h==
- $X$ suis une loi normale noté $X \sim \mathcal{N}(m,\sigma^2)$ ; où :
	- ==m== est la moyenne de taille des sentinelles
	  Ici n=**175cm**
	- ==σ== est l'écart type
	  Ici σ=**7cm**
### Calcul
Admettons que $T=\frac{X-175}{7}$ ;
$\mathbb{P}(X<h)=0.95 <=> \mathbb{P}(T<\frac{h-175}{7})=0.95$
> ==Je ne comprends pas pourquoi on remplace :==
>- Entre les 2 proba, $X$ par $T$ 
>- Entre les 2 fractions, $X$ par $h$
>- Entre les 2 proba, $h$ par la fraction

Dans la table des $z$, on doit trouver les coordonnées (x,y) de la valeur qui s'approche le plus de 0.95.
Askip en x c'est 1.64 donc on le met à la place du 0.95 dans la modélisation.

Résolution de l'équation :
- $\frac{h-175}{7}=1.64$
- $h-175=1.64*7$
- $h-175 = 11.48$
- $h = 175+11.48$
- $h=186.48$

Il faudrait donc que la hauteur soit d'environ **186.48cm** pour que 95% des sentinelles puissent passer.