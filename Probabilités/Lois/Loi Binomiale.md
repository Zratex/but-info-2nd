# Enoncé
Quand on répète ==n== fois, <u>indépendamment</u> dans de <u>mêmes conditions</u>, avec ==p== la probabilité de se produire, ==X== le nombre de fois que l'événement est réalisé ;
> Cela suit une loi **Binomiale** de paramètre `n` et `p`
## Correspondance des paramètres
Ce segment est pour faire en sorte de référencer les paramètres, afin que quand on passera la souris sur un paramètre dans les formules qui suivront, sa description apparaîtra.

==n== correspond au **nombre de répétions** ^bd9df8

==p== correspond à la **probabilité** que l'événement recherché **se réalise** ^8cbbd5
# Formule
Une fois l'énoncé posé, on note $X \sim {\sf Binom}(n,p)$ ; et on a donc :
- $\Omega_X$ = {0 ,1 , $\cdots$ , [[Loi Binomiale#^bd9df8|n]]}
- $\forall k \in \Omega_X , P(X=k) = \binom{n}{k} *$ [[Loi Binomiale#^8cbbd5|p]]<sup>k</sup> $(1-p)^{n-k}*(p\in[0,1])$

A savoir que :
- $\Omega$ = [[Univers]]
- Le calcul avec les parenthèses correspond à un [[Coefficient binomiale]]

## Autres formules
- <u>Espérance :</u> $\mathbb{E}(X) =$ [[Loi Binomiale#^bd9df8|n]] $*$ [[Loi Binomiale|p]]
- <u>Variance :</u> $\mathbb{V}(X)=$ [[Loi Binomiale#^bd9df8|n]] $*$ [[Loi Binomiale|p]] $*$ (1-[[Loi Binomiale|p]])