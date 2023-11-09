std en [[Cpp|C++]] permet de gérer quelques trucs assez sympa.
Il faut importer les modules à utiliser. On en a vu 3 :
- `iostream`
  Afficher une chaîne de charactères dans la console de commande
- `invalid_argument`
  Permet de retourner une erreur du type argument invalide
- `string`
  Littéralement les chaînes de charactères

## Exemple
```cpp
#include <iostream>
#include <string>
#include <stdexcept>

int main(){
	std::string Chaine;
	std::cout << "Entrez une chaine : ";
	std::cin >> Chaine;
	if (Chaine==""){
		throw std::invalid_argument("Chaine vide");
	} else {
		std::cout << Chaine << std:endl
	}
}
```