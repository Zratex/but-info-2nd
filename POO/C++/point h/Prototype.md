Le prototype correspond au contenu de la [[Classe]] qui est défini en avance dans le ficher [[En-tête|.h]]. Pour ce qu'il faut mettre dans le fichier en lui même, se référer à la note sur l'[[En-tête]]

## Attributs
Définition des attributs. Avant la définition des attributs, il est important d'indiquer `private:`

Ensuite, chaque attribut devra contenir :
1) Type
2) Pointeur ou référence ou aucun des deux
3) Nom de l'attribut

### Exemple
```cpp
private:
	char test;
```
## [[Classe#^22d486|Méthodes]]
On défini le prototype de chaque [[Fonction#Cpp C++|fonction]]. Leurs fonctionnement sera décrit plus tard dans le fichier [[Extensions du cpp#Extensions vues en cours|.cc]].
Pour le prototype d'une [[Fonction#Cpp C++|fonction]], il faut respectivement :
1) Le type de retour.
   -> Si il n'y a pas de type de retour, il faut mettre `void`
2) Le nom de la fonction (avec une parenthèse après)
3) Les paramètres de la fonction (pas obligatoire).
   Il faut savoir que pour un paramètre, il faut y mettre :
   - Son type
   - Si c'est un pointeur, une référence, ou aucun des deux

Mis à part cela, il faudrait définir le [[Constructeur#En Cpp C++|constructeur]] (exemple d'implémentation dans la note dédiée)
### Exemple
```cpp
public:
	char getTest();
	void setTest(char);
```
### [[Trio]]
Il ne faut surtout pas oublier de vérifier si le [[Trio]] n'est pas à implémenter dans cette [[Classe]]