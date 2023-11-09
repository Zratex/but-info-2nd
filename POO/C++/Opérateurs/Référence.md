Une référence est une notion dérivée du [[Pointeur]]. C'est tout simplement l'emplacement exacte en [[Adresse|mémoire]] de la variable.

En [[Cpp|C++]], l'[[Opérateur informatique|opérateur]] `&` est utilisé pour retourner la référence d'une variable.
> Une référence ne peux pas :
> - être réassigner, car c'est une [[const|constante]]
> - être nulle

## Syntaxe
L'[[Opérateurs cpp|opérateur &]] se met devant le nom de la variable. Exemple :
```cpp
int valeur=1;
int &ref=valeur;
```
