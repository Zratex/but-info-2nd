On applique ces transformations suivantes avec un couple $(\bar{a},\bar{b})$ :
- <u>Chiffrement :</u> $\bar{c} = \bar{a} * \bar{m} + \bar{b}$
	  - Forme similaire à une [[Fonction]] affine (*d'où son nom*) : $ax+b$
	  -> Vu dans les [[Applications linéaires]]
- <u>Déchiffrement :</u> $\bar{c} = \bar{a}^{-1} * (\bar{c} - \bar{b})$

Où l'on admet donc que :
- ==m== : message en clair
- ==c== : message chiffré
## Calcul
### Chiffrement
Pour réaliser $\bar{a} * \bar{m} + \bar{b}$, il faut réaliser étape par étape :
- <u>Multiplication</u> (via $\bar{a}$) :
- <u>Addition</u> (via $\bar{b}$) : Même chose qu'avec le [[Code César]]
## Déchiffrement
Pour réaliser $\bar{a}^{-1} * (\bar{c} - \bar{b})$, il faut réaliser étape par étape :
- <u>Soustraction</u> (via $\bar{b}$) :
- <u>Division</u> : On ne peut pas diviser par un modulo, donc on utilise la multiplication par son inverse (d'où la notation $\bar{a}^{-1}$). Etape par étape ce que l'on doit faire :
	- Trouver la valeur de $\bar{a}$
	- [[Calcul inverse|Calculer l'inverse]] de $\bar{a}$ pour avoir $\bar{a}^{-1}$
	- Multiplier par $\bar{a}^{-1}$