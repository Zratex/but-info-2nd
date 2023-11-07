On a une liste d'actions à exécuter qui prend (ou non) des **paramètres**.

En fonction des besoins, une fonction peux retourner quelque chose afin que cet élément de retour soit traité autre part.
# [[Mathématiques]]
## Définition
La structure contient :
- le **nom** de la fonction (souvent une lettre en maths)
- les **paramètres**

Exemple :
$f(x)$
## Utilisation
Admettons $f(x)=x+1$
Si $x=0$ alors $f(x)=0+1=1$
# Informatique
## Python
### Définition
La structure contient :
- le mot `def`
- le **nom** de la fonction
- des parenthèses suite au nom, suivi de `:`
- Non obligatoire :
	- les **paramètres** de la fonction entre les parenthèses
	- Après le `:`, écrire `->` suivi du type de retour attendu

Exemple de définition de fonction :
```python
def f(x):
	x+=1
	return x
```
### Utilisation
Utilisation de la fonction :
```python
x=0
print("X est désormais égal à ",f(x))
```
`X est désormais égal à 1`
## [[Cpp|C++]]
### Définition
La structure contient :
- Le **type** de retour (si il n'y en a pas, il faut écrire `void`)
- Le **nom** de la fonction
- Des parenthèses
- Code de la fonction contenu entre crochets `{}`
- Non obligatoire :
	- les **paramètres** de la fonction entre les parenthèses, contenant :
		- Type du paramètre
		- Pointeur, référence ou aucun des deux
		- Nom du paramètre

Exemple de définition de fonction :
```cpp
int f(int x){
	x=x+1
	return x
}
```
### Utilisation
Utilisation de la fonction :
```cpp
int x=0;
cout << "X est désormais égal à " << 
```
