```mermaid
sequenceDiagram
create actor A as Alice
create actor B as Bob
	Note over A,B: Chiffrement par Alice via clé privée
	A->>B: c
	Note over A,B: Déchiffrement par Bob via clé privée
```

| Avantages | Inconvénients |
| :--: | ---- |
| Très rapide | Comment transmettre la clé sans quelle se fasse interceptée |
## Méthodes de calcul
Il y a différentes méthodes d'application du [[Chiffrement]] symétrique :
- [[Code César]]
- [[Chiffrement affine]]
- [[Chiffrement Vigenère]]
	- [[Chiffrement Vernam]]