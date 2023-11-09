`const` est un mot-clé en [[Cpp|C++]] permettant d'indiquer au système que l'élément (que ce soit une variable, un [[Pointeur]], une [[Référence]] ou une [[Fonction]]) d'origine ne doit pas être modifiée.
On dit que l'élément est **constant**.

## Variable
Pour qu'une variable soit constante, il suffit juste de mettre l'attribut `const` devant sa déclaration.
Exemple :
```cpp
const int value = 10;
```
La valeur `value` ne pourra donc pas être modifiée, et sera toujours égal à 10
## [[Fonction]]
Il y a 2 cas où `const` peut être utilisé dans une [[Fonction|fonction]]. Ces 2 cas peuvent être utilisés en même temps
### 1 - Paramètres d'une [[Fonction]]
Un élément d'entrée, donc un paramètre, peut avoir l'attribut `const`
Exemple :
```cpp
void Exemple(const char nom){
	//Contenu de la fonction
}
```
### 2 - [[Fonction]] constante
Un fonction constante est une fonction avec l'attribut `const` à la fin de sa déclaration.
Exemple :
```cpp
void Exemple() const {
	//Contenu de la fonction
}
```
### Implémentation [[Objet]]
En objet, si l'on veut qu'une [[Classe#^22d486|méthode]] soit constante, il faut ajouter l'attribut `const` au niveau de son [[Prototype]] :
- fichier [[En-tête|.h]]
- et dans le fichier [[Méthodes cpp|.cc]]