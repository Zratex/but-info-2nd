Cette note décrit l'implémentation des méthodes de [[Classe]] en [[Cpp|C++]], une fois que les [[Prototype|prototypes]] ont été réalisés dans l'[[En-tête]].
Ce qu'il veut dire qu'ici je vais décrire ce que doit contenir un fichier [[Extensions du cpp#Extensions vues en cours|.cc]]
## Etapes par étapes
1) Importation des modules externes utilisés
   Il faudrait logiquement obligatoirement mettre le fichier `.h` avec `#include "NomDeLaClasse.h"`
2) Il faut réaliser le code de chaque [[Fonction|fonctions]] des [[Prototype|prototypes]] présents dans le [[En-tête|.h]]
   Pour l'agencement des [[Fonction|fonctions]], il faut respecter :
   - Le type de retour
     Si il n'y a pas de type défini dans le [[En-tête|.h]], on ne met rien
   - Mettre le nom de la classe suivi de `::`
   - Nom de la [[Classe#^22d486|méthode]]
   - Parenthèses contenant les paramètres de la [[Fonction|fonction]]
## Exemple avec du code
Si on applique ce qui a été listé dans la partie `Etapes par étapes` juste au dessus, le code devrait ressembler à ça :
```cpp
#include "NomDeLaClasse.h"

NomDeLaClasse :: NomDeLaClasse(/*Paramètres de la fonction*/)
{
	//contenu du constructeur
}

void NomDeLaClasse :: Test(/*Paramètres de la fonction*/)
{
	// Contenu de la fonction
}
```
Après les parenthèses, [[const]] peut être placé.