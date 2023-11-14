Ce qui illustre le mieux le concept d'une file est une **file d'attente**.

Il existe des règles à suivre pour les files, similaire aux [[Pile|piles]] :
- Premier rentrée, premier sortie
- Eléments homogènes (càd de même type)
- Linéarité
## Opération
Les règles de la concept de file implique obligatoirement la programmation de certaines [[Opérateur informatique|opérations]] :
- [[Constructeur|Construction]] d'une file vide
- Savoir si la file est vide ou non (`Test de vacuité`)
- Enfiler
- Défiler
- Savoir qui est en **tête** de file (celui qui va sortir)

> Le coût des [[Opérateur informatique|opérations]] doivent être les mêmes peu importe la taille de la file

## Programmation
Concept de programmation en [[Cpp|C++]] :
```
Il faut s'imaginer une liste avec un indice de départ et de fin. Ce qui est en dehors de cet interval sont des valeurs "nulles".
Quand on ajoute un nouvel élément il est (dans cet exemple) indenté à droite.
Ensuite, il faut se représenter cette file comme un cercle, c'est à dire que si on dépasse le dernier élément sur la droite, comme un cycle, on se retrouve sur la gauche.

Cela implique donc qu'une file a un nombre limité d'éléments.
```