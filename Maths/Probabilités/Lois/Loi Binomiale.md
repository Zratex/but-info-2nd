# Enoncé
Quand on répète ==n== fois, <u>indépendamment</u> dans de <u>mêmes conditions</u>, avec ==p== la probabilité de se produire, ==X== le nombre de fois que l'événement est réalisé ;
> Cela suit une loi **Binomiale** de paramètre `n` et `p`

A noter qu'il faut impérativement que l'énoncé suive un schéma de [[Loi de Bernoulli|Bernouilli]], c'est à dire qu'il y a une réponse vrai ou fausse.
## Correspondance des paramètres
Ce segment est pour faire en sorte de référencer les paramètres, afin que quand on passera la souris sur un paramètre dans les formules qui suivront, sa description apparaîtra.

==n== correspond au **nombre de répétions** ^bd9df8

==p== correspond à la **probabilité** que l'événement recherché **se réalise** ^8cbbd5
# Formule
Une fois l'énoncé posé, on note $X \sim {\sf Binom}(n,p)$ ; et on a donc :
- $\Omega_X$ = {0 ,1 , $\cdots$ , [[Loi Binomiale#^bd9df8|n]]}
- $\forall k \in \Omega_X , P(X=k) = \binom{n}{k} *$ [[Loi Binomiale#^8cbbd5|p]]<sup>k</sup> $(1-p)^{n-k}$

A savoir que :
- $\Omega$ = [[Univers]]
- Le calcul avec les parenthèses correspond à un [[Coefficient binomiale]]

## Autres formules
- <u>Espérance :</u> $\mathbb{E}(X) =$ [[Loi Binomiale#^bd9df8|n]] $*$ [[Loi Binomiale|p]]
- <u>Variance :</u> $\mathbb{V}(X)=$ [[Loi Binomiale#^bd9df8|n]] $*$ [[Loi Binomiale|p]] $*$ (1-[[Loi Binomiale|p]])

# Exemple
## Exo 1 : GPT
Enoncé donné par ChatGPT (3.5)
### Enoncé
```
Une entreprise fabrique des ampoules électriques, et 95 % de ces ampoules sont de bonne qualité. Cependant, 5 % des ampoules sont défectueuses. Vous achetez un paquet de 10 ampoules.

Quelle est la probabilité que parmi les 10 ampoules achetées, exactement 8 soient de bonne qualité ?
```
### Définition des valeurs
$X$ est la [[Variables aléatoires|variable aléatoire]] décrivant la probabilité que 8 ampoules soient de bonne qualité sur 10 achetées.
- On cherche $\mathbb{P}(X=8)$
  Donc ==k== sera égal à 8
- $X$ suis une loi binomiale noté $X \sim {\sf Binom}(n,p)$ ; où :
	- **n** est le nombre de tira
	  Ici n=**10**
	- **p** est la probabilité d'avoir une ampoule de bonne qualité
	  Ici p=**0.95**
### Calcul
$\forall k \in \Omega_X , P(X=k) = \binom{n}{k} *$ [[Loi Binomiale#^8cbbd5|p]]<sup>k</sup> $(1-p)^{n-k}$
- $\mathbb{P}(X=8) = \binom{10}{8} * 0.95^8 * (1-0.95)^{10-8}$
- $\mathbb{P}(X=8) = 45 * 0.95^8 * 0.05^2$
- $\mathbb{P}(X=8) \approx 0.0745$

Détail du calcul pour $\binom{10}{8}$ dans [[Calcul coef binomiale]]