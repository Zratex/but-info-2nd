C'est un enchainement d'éléments (appelés **nœuds**) avec une partie dédiée à son information, et une autre destinée à pointer le prochain nœud.

Il y a un pointeur en début de chaîne, et ce pointeur est en général décrit par le fonctionnement des [[Pile|piles]].
De ce fait, ce pointeur pointe vers le premier nœud, ce qu'il fait que ce nœud est la [[Pile#^2d3680|tête]] de la [[Pile|pile]].
## Exemple
Exemple d'implémentation en [[Cpp|C++]] d'un nœud (ici on réalise une [[Classe]] dédiée):

```cpp
class Noeud
{
	private:
		char x;
		Noeud * p;
}
```
