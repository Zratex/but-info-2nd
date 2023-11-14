Avant le tableau, il faut définir :
- prix = prix de l'objet à l'achat hors taxes
- valeur résiduelle = ?
- Base amortissable = prix-valeur résiduelle

Ensuite, il faut définir :
- Le temps : ça va être notre nombre de lignes dans le tableau
- Mode d'amortissement : ici linéaire

| Exercice (année) | Base amortissable | Calculs | Amortissements dotations | Amortissements cumulés | Valeur Nette Comptable |
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| N | BA | (nb jours restants dans l'année/360)$*BA*$TVA| Résultat calcul | $AD_N=$Amortissement dotations | BA-Amortissements cumulés |
| N+1 | BA | BA$*$TVA | Résultat calcul | $AD_{N}+$ Résultat Calcul| BA-Amortissements cumulés |
| N+2 | BA | BA$*$TVA | Résultat calcul | $AD_{N1}+$ Résultat Calcul | BA-Amortissements cumulés |
| N+3 | BA | BA$*$TVA | Résultat calcul | $AD_{N2}+$ Résultat Calcul | BA-Amortissements cumulés |
| N+n | BA |(nb jours entre anniversaire achat et début d'année/360)$*BA*$TVA | Résultat du calcul | $AD_{N-1}$ Résultat Calcul | Valeur résiduelle = BA-Amortissements cumulés |

Pourquoi 360 : [[Année lombarde]]
## Extrait de bilan après inventaire au $N+n$
| Actif | Brut | Amortissements | Net |
| :-: | :-: | :-: | :-: |
| Immobilisation corporelles : (nom du produit) | Prix d'achat HT | Amortissements cumulés de l'année | VNC de l'année |
