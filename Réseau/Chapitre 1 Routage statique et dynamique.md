# Chapitre 1 : Routage statique et dynamique
## I - Adressage des paquets IP par hôtes terminaux
### 1) choisir sa route (suite)
Principe de [[Routage]]
### 2) Tables de routage des hôtes
Un équipement peux envoyer un paquet :
- A lui même (loopback)
- Un destinataire sur le même réseau local
- A un destinataire distant

Réseau :
- local : via un switch ou un accesspoint wifi ou directement par cable
- distant : passerelle par défaut requise

## II - Fonctionnement des routeurs
### 1) choisir sa route (fin)
En fonction de l'adresse de destination, le routeur transmet le paquet sur l'interface correspondante.
### 2) Routage statique et dynamique
Problématique : Comment le routeur peut il connaître les différents chemins le reliant aux autres routeurs ?
- par config ([[Routage Statique|Statique]])
- par apprentissage ([[Routage dynamique|Dynamique]])
### 4) Table de routage
Pour un routeur, elle regroupe :
- Des adresses réseaux
- Leur masque associé
- Le moyen de les atteindre avec l'adresse IP du premier routeur situé sur la route

Elle est inutile pour les réseaux directement connectés au routeur.
## III - Protocoles de routage dynamique
### 2) but du [[Routage dynamique]]
- Rechercher le chemin le plus court ou le plus rapide parmi plusieurs routes possibles.
- Protocoles distribuées : chaque routeur choisit le chemin
- Protocoles itératifs : exécutés en boucle -> mise à jour à chaque intération
### 3) Deux familles de protocoles
#### 1 - Protocoles à vecteur de distance
- Basés sur le nombre de sauts à parcourir (Routeurs)
- Echange d'informations avec les voisins : chacun s'annonce à ses voisins, qui diffusent à leur tour `Schéma d'un réseau classique avec des sauts, comme au Bac par exemple`
#### 2 - Protocoles à l'état de lien
- prise en compte de la bande passante
- envoi de messages **Link State Update** (LSU) (Adresse IP + Bande passante) : table de voisinage
- Tables transmises aux voisins : chaque routeur connaît la topologie du réseau
## IV
### 1 - Mises à jour
Il y a différentes méthodes de màj :
- Envoyées uniquement en cas de changement
- Màj incrémentielles (seulement les nouveautés)
- réparties en zones, contraire au màj globales
## V
