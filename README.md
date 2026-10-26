# Skyjo · ChadGangGames

Le Skyjo pour le hub ChadGangGames : un seul `index.html`, aucune dépendance à installer.

## Modes
- **En ligne** (depuis le hub) : créer une salle ou rejoindre avec un code, jusqu'à 8 joueurs, bots possibles. L'hôte (premier arrivé) fait tourner la partie et les bots ; s'il part, le suivant prend le relais. Un joueur déconnecté est remplacé par un bot au bout de 30 s (ou tout de suite via le bouton de l'hôte) et reprend la main à son retour.
- **Contre des bots** : 1 à 7 bots.
- **Même écran** : plusieurs joueurs se passent l'appareil (+ bots si on veut).

## Hub
- `ChadGang.me()` pour le pseudo et l'avatar, `ChadGang.room()` pour les invitations, `ChadGang.join()` pour les salles (état complet versionné envoyé avec `keep`).
- `ChadGang.finPartie({ gagne, partie })` est appelé par chaque joueur en fin de partie en ligne (le plus petit total gagne).
- Avatars marqués avec `data-chadgang-id` pour les caméras.

## Tester en local
Ouvrir `index.html` dans un navigateur : le menu propose les modes bots et même écran. Ajouter `?fast` à l'adresse accélère les animations (pratique pour tester).
