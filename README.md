# ImageHunt

## Liste des fonctionalités à implémenter

### Comptes
- Possibilité de créer un compte au démarrage
- Modifier le compte
- Le compte contient :
  - Modifiable
    - Pseudo
    - (Photo)
    - (Stocker les amis)
  - Non modifiable
    - Partie actuelle
    - (partie précédente)
- configurer pour qu'on puisse utiliser la montre
- l'id du compte est stocké sur le téléphone pour ne pas avoir à rentrer le mot de passe à chaque fois
- (Possibilité d'avoir des amis)
- (Possibilité de supprimer le compte)

### Partie/Groupe
- Création de la partie par le game master(/l'administrateur)
  - Donner un nom à la partie
  - (Donner un logo à la partie)
  - Rajouter des personnes en connaissant leur pseudo
  - Les personnes rajoutées recoivent une notification et peuvent l'accepter
  - (nominer le game master dans le groupe)
  -  le statut de chaque personne est stocké : joueur, game master, admin
  - game mode setting : temp limité ou pas
  - rajouter des photos
- même si la partie n'est pas lancée, tout est stocker sur firebase pour pouvoir éditer la partie plus tard 
- le game master peut rajouter des photos pendant la partie
- les joueurs sont notifiés quand une nouvelle photo est disponible
- les joueurs envoient leur résultat au game master pour une mission donnée
  - cela déclenche l'appareil photo
  - le joueur envoie la photo
  - (le game master voit la position gps du joueur)
  - (le joueur peut rajouter un commentaire)
- Le game master est notifié quand une personne submit son résultat
- (game master peut suivre la position des joueurs)
- (le game master peut communiquer avec tous le monde)
- le game master décide si la photo est valide ou pas
  - le game master peut communiquer avec l'envoyeur
  - (si le game master est trop lent, l'application décide par elle même si c'est configuré comme tel)
- les scores sont mis à jours automatiquement
- Possibilités pour terminer la mission
  - le game master termine la mission
  - la mission se termine quand x joueurs ont trouvé la photo
  - temps limite
- Fin de la partie
  - game master (administrateur) termine la partie
  - la temps de la partie est écoulé
- Possibilité de quitter la partie
- Possibilité de supprimer la partie
- (Avoir la possibilité de relancer une partie déjà jouer, le jeu se souvient des photos, hints)

### Définition d'une mission/photo à trouver
- Deux modes pour rajouter une photo:
  - La photo est prise par l'application, on prend aussi la position gps
  - la photo vient de la galerie, on accepte la photo si il y a une pos gps sinon on demande d'activer la position gps sur les photos
- photo
- etat programmable : cacher, temps avant de démarrer la mission
- hint programmable : temps d'envoi depuis le lancement de la partie
 - photo
 - message
 - lieu gps, idéalement un cercle de grandeur configurable
- stocker qui est en attente de décision du game master
- (stocker qui a trouver la photo)

### intégration de la watch
- Quand une notification est envoyée, elle apparait aussi sur la montre
- on peut voir les photos de la partie
- on peut selectionner une photo
- on peut afficher pour la mission
  - la boussole
  - le hint text
  - les hint photos

### life cycle
- a l'ouverture pour la première fois, on a accés à une activité où l'on peut creer un compte
- possibilité de se connecter à un compte déjà existant
- une fois connecté, l'appli se connecte automatiquement
- lorsqu'on ouvre l'application on arrive sur la page de la dernière image hunt ouverte, page d'accueil sinon
- possibilité de naviguer entre les images hunts
- lorsqu'on ferme l'application, l'appli enregistre sur quelle partie nous étions

## Graphical User Interface
see dedicated file

## Classes
see dedicated file

