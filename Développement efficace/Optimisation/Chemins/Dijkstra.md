On prend tout les chemins possibles pour prendre le plus court du POV de Dijkstra.

On doit se munir de :
- liste des points non visités
- dictionnaire point adjacent à l'actuel, avec un coût correspondant
## Fonctionnement
Quand on sélectionne un [[Arbre#POV Informatique|Noeud]] :
- On le retire de la liste des points non visités
	- Sauf si il n'est pas dans la liste, dans ce cas là on n'exécute pas la suite
- On réalise le dictionnaire d'adjacence
	- Si un point n'est pas joignable, on attribue une valeur infinie
- On sélectionne le [[Arbre#POV Informatique|Noeud]] avec le moins d'adjacences
	- En vérifiant qu'il est bien dans la liste des points non visités
- On met à jour le dictionnaire d'adjacence par rapport au nouveau Noeud :
	- On retire le nouveau Noeud de la liste des points joignables, et on retire le nouveau noeud de la liste des points non visités
	- Pour mettre à jour, on additionne distances du nouveau noeud, par rapport à la distance qu'on a déjà franchie
		- On fait ce process sur toute la liste seulement si de nouveaux points sont joignables
