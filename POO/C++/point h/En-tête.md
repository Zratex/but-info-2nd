L'en-tête contient la définition de la [[Classe]] en [[Cpp|C++]].

## Structure d'en-tête
### Etapes par étapes
1) Définition `.h`
   Il faut intégrer `#ifndef __NomDeLaClasse_H__` suivi de `#define __NomDeLaClasse_H__`
2) Importation des modules externes utilisés.
   ça se fait avec `#include <NomDuModule>`
3) `class NomDeLaClasse{`
4) [[Prototype]]
5) `};` et `#endif`

### Exemple avec du code
Si on applique ce qui a été listé dans la partie `Etapes par étapes` juste au dessus, le code devrait ressembler à ça :
```cpp
#ifndef __NomDeLaClasse_H__
#define __NomDeLaClasse_H__

#inclue <NomDuModule>

class NomDeLaClasse{
	private:
		//Attributs de la classe
	public:
		//Constructeur
		//Trio (si besoin)
		//Méthodes de la classe
};

#endif
```