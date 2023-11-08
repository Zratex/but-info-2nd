Un destructeur en [[POO]] est une [[Classe#^22d486|méthode]] appelée lors de la destruction d'un [[Objet]]. L'idée est de libérer l'espace mémoire que prends l'[[Objet]].

## En [[Cpp|C++]]
Le destructeur doit être programmé :
- Soit quand un [[Classe#^e5375d|attribut]] est un pointeur
- Soit dans le cas de la règle du [[Trio]]
### Implémentation
Voici comment est ce que le destructeur doit être implémenté :
#### Fichier [[En-tête|.h]]
Le [[Prototype]] doit tout simplement être défini de cette manière :
```cpp
public:
	~NomDeLaClasse();
```
#### Fichier [[Méthodes cpp|.cc]]
Si l'on veux qu'un simple destructeur, il suffit d'écrire ceci :
```cpp
~NomDeLaClasse(){
}
```
La destruction de l'[[Objet]] est automatiquement géré.
> Si un des [[Classe#^e5375d|attribut]] est un pointeur, ou que l'on veux que la destruction se fasse d'une manière spécifique, on peux mettre des instructions dans cette [[Fonction]]
##### Pointeur
Si un [[Classe#^e5375d|attribut]] est un [[Pointeur]], il faudra utiliser l'[[Opérateur informatique|opérateur]] [[Delete]] pour le supprimer.
Exemple de code :
```cpp
~NomDeLaClasse(){
	delete[] AttributTypeTableau;
}
```