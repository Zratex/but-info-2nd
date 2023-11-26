Ce sont des signes assez souvent utilisés en [[Mathématiques]].

**∀** x ∈ E, P(x) -> se lit : "**Quelque soit** x appartenant à E, P(x) est vrai"
**∃** x ∈ E, P(x) -> se lit : "**il existe (au moins)** un x appartenant à E tel que P(x) soit vrai" ^98f953
## Négation d'une phrase quantifiée
- `\(∀ x ∈ E, P(x)) = ∃ x ∈ E, \(P(x))`
- `\(∃ x ∈ E, P(x)) = ∀ x ∈ E, \(P(x))`
<u>Exemple :</u>
```
E = {Etudiants}
G(x) : x est grand
Aucun n'est grand <=> ∀ x ∈ E, \(G(x)) <=> \(∃ x ∈ E, G(x))
```
## A propos de l'ordre des quantificateurs :
```
E={étudiants}
A(x,y) : x et y sont amis
∀ x ∈ E, ∃ y ∈ E, A(x,y)
Tout le monde a au moins un ami
∃ y ∈ E, V x ∈ E, A(x,y)
Il y a au moins un étudiant ami avec tout le monde
```
