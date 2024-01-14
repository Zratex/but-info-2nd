Se principe se base sur l'existence de la [[Matrice Inverse]], mais nous l'appliquons ici seulement pour le [[Chiffrement]].
## Calcul
On défini :
- $n$ : valeur dont on cherche l'inverse
- $x$ : itération de l'opération
- Tout les nombres doivent être sur un [[Modulo]] précis

Le principe est que l'on avance dans le tableau temps que l'on a pas trouvé $\bar{1}$ dans les résultats.
> $\bar{x}$ où $\bar{n}*\bar{x}=\bar{1}$ sera donc l'inverse de $\bar{n}$, càd $\bar{n}^{-1}$
### Exemple
On cherche l'inverse de $\bar{n}=\bar{7}$ en [[Modulo 26]] :

| $\bar{x}$ | $\bar{0}$ | $\bar{1}$ | $\bar{2}$ | $\bar{3}$ | $\bar{4}$ | $\bar{5}$ | $\bar{6}$ | $\bar{7}$ | $\bar{8}$ | $\bar{9}$ | $\bar{10}$ | $\bar{11}$ | $\bar{12}$ | $\bar{13}$ | $\bar{14}$ | $\bar{15}$ |
| :--: | :--: | :--: | :--: | :--: | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| $\bar{7} * \bar{x}$ | $\bar{0}$ | $\bar{7}$ | $\bar{14}$ | $\bar{21}$ | $\bar{28} = \bar{2}$ | $\bar{9}$ | $\bar{16}$ | $\bar{23}$ | $\bar{30}=\bar{4}$ | $\bar{11}$ | $\bar{18}$ | $\bar{25}$ | $\bar{32}=\bar{6}$ | $\bar{13}$ | $\bar{20}$ | $\bar{27}=\bar{1}$ |
Donc l'inverse de $\bar{7}$ est $\bar{15}$ en [[Modulo 26]], ce qu'il fait que $\bar{n}^{-1}=\bar{15}$