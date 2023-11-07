Pour réaliser un scénario, il faut :
## 1) Titre
Titre du scénario
## 2) Préconditions
Liste des préconditions à respecter avant de démarrer le scénario
## 3) Postconditions
Les des postconditions à respecter une fois que le scénario est réalisé sans aucune erreurs
## 4) Tableau
| N° | Acteur : `Nom de l'acteur` | Système |
| :-: | :-: | :-: |
| 1 | ... | |
| 2 | | ... |
Une action par ligne.
> Si l'action est du côté de l'acteur, la case côté système doit être vide.
> Et inversement

# Exemple
## Exo : Panier
Exercice par Prevost, où le sujet est un site d'E-commerce avec un système de panier
### Validation du panier
### - Préconditions
- Le panier est préparé
- Les articles sont disponibles
- L’utilisateur est connecté
- Le site est en ligne et fonctionne
### - Postconditions
- Le panier est vide
- La commande est validée
- Le stock est mis à jour

### Tableau
| N° | Acteur : mimi51 | Système |
| :-: | :-: | :-: |
| 1 | mimi51 valide son panier et choisit un mode de livraison | |
| 2 | | Le système crée la commande |
| 3 | mimi51 confirme la commande | |
| 4 | | Le système demande le paiement |
| 5 | mimi51 paye la commande | |
| 6 | Le système vérifie le paiement et affiche la facture |