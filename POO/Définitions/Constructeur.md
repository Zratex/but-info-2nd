Le constructeur est une [[Classe#^22d486|Méthode]] de classe [[Classe]] décrivant comment est ce que la machine doit construire une nouvelle [[Instance]].

Il peux contenir des paramètres et ne retourne 
## En [[Cpp|C++]]
### [[Prototype]] du [[En-tête|.h]]
Il doit être compris dans les [[Prototype#Classe 58f4c5 Méthodes|Méthodes]] du prototype sous cette forme :
```cpp
public:
	NomDeLaClasse(/** Paramètres **/);
```
### Implémentation dans le fichier [[En-tête|.cc]]
```cpp
NomDeLaClasse :: NomDeLaClasse(/** Paramètres **/){
	//Contenu du constructeur
}
```