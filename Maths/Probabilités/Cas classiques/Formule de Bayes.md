# Enoncé
Cette formule permet d'établir un lien entre $\mathbb{P}(A)$ et $\mathbb{P}_B(A)$
>Pour le calcul de $\mathbb{P}_B(A)$, se référer à la note sur les [[Conditionnelle|probabilité conditionnelles]]

Il faut donc admettre qu'on a bien un événement $A$ et $B$
# Formule
La formule ressemble à ça :
$$\mathbb{P}_B(A) = \frac{\mathbb{P}_A(B) \times \mathbb{P}(A)}{\mathbb{P}(B)}$$
Si on admet que $B$ est sur un [[Univers]] défini par {$A,\bar{A}$}, on obtiens cette formule :
$$\mathbb{P}_B(A) = \frac{\mathbb{P}_A(B) \times \mathbb{P}(A)}{\mathbb{P}_A(B)\times \mathbb{P}(A) + \mathbb{P}_{\bar{A}}(B)\times \mathbb{P}(\bar{A})}$$
> Ne pas oublier le calcul sur les [[Conditionnelle|probabilités conditionnelles]]

# Exemples
## Exo 1 : GPT
Exercice donné par ChatGPT (3.5) pour m'entraîner :
```
Un test médical a été développé pour détecter une maladie rare, appelée Maladie X. Le test a été évalué comme suit :

- Le test est positif chez 99% des patients atteints de la Maladie X.
- Le test est négatif chez 98% des personnes en bonne santé.
- La Maladie X affecte 1% de la population.

Un patient se présente avec un test positif. Quelle est la probabilité que ce patient soit réellement atteint de la Maladie X ?
```
## Définition des valeurs
- $A$ événement `est malade`
	$\mathbb{P}(A)=0.01$
- $B$ événement `positif au test`
On cherche donc $\mathbb{P}_B(A)$

On en déduis aussi que :
- $\mathbb{P}(\bar{A})$ événement `n'est pas malade`
	$\mathbb{P}(\bar{A}) = 1-\mathbb{P}({A}) = 1-0.01 = 0.99$
- $\mathbb{P}_A(B)$ événement `positif sachant qu'il est malade`
	$\mathbb{P}_A(B)=0.99$
- $\mathbb{P}_\bar{A}(B)$ événement `positif sachant qu'il n'est pas malade`
	$\mathbb{P}_\bar{A}(B) = 0.02$
> A savoir que $\mathbb{P}_\bar{A}(B)$ revient au même que `1- (la probabilité de négatif et pas malade)`

On a besoin de savoir ce que vaut $\mathbb{P}_\bar{A}(B)$ et $\mathbb{P}(\bar{A})$ pour la formule
## Calcul
$$\mathbb{P}_B(A) = \frac{\mathbb{P}_A(B) \times \mathbb{P}(A)}{\mathbb{P}_A(B)\times \mathbb{P}(A) + \mathbb{P}_{\bar{A}}(B)\times \mathbb{P}(\bar{A})}$$
- $\mathbb{P}_B(A) = \frac{0.99 \times 0.01}{0.99\times 0.01 + 0.02\times 0.99}$
- $\mathbb{P}_B(A) \approx \frac{0.0099}{0.0099 + 0.0198}$
- $\mathbb{P}_B(A) \approx \frac{0.0099}{0.0297}$
- $\mathbb{P}_B(A) \approx 0.33333$
