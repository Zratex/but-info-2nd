Le pointeur est une variable stockant l'[[Adresse|adresse mémoire]] d'une autre variable.

En [[Cpp|C++]], l'[[Opérateur informatique|opérateur]] `*` est utilisé pour faire appel à cette notion de pointeur. Il ne pointe pas vers la valeur en elle même, mais son emplacement.
En sachant son emplacement, on peux manipuler cet élément directement avec le pointeur.
>L'accès à l'emplacement précis de l'[[Adresse|adresse]] se fait avec une [[Référence]]
## Syntaxe
L'[[Opérateurs cpp|opérateur *]] se met devant le nom de la variable. Exemple :
```cpp
int valeur=1;
int *pointeur = &valeur;
```
