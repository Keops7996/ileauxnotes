# L’Île aux Notes

Jeu d'entraînement musical pour toute la famille : violoncelle, piano et guitare.

- Les notes tombent dans les couloirs des cordes (ou des touches) ; le micro écoute l'instrument, ou on joue au toucher.
- Deux affichages : « Chute » (les notes tombent dans les couloirs) et « Partition » (vraie portée avec clé, armure, mesures, la note à jouer colorée et les notes jouées en vert).
- Modes Douceur (sans points, pour apprendre sans pression), Entraînement (le jeu attend la bonne note) et Défi (en rythme), tempo réglable, métronome.
- Profils par musicien (avatar, couleur, un ou plusieurs instruments), points (total et de la semaine), étoiles, rangs et badges.
- Piano : main droite ou main gauche au choix, avant l'exercice ou pendant (bouton ✋), avec import des deux portées (MusicXML) ou séparation automatique des mains (MIDI).
- Duo : deux musiciens à l'écran, chacun son tour ou ensemble ; ou sur deux appareils avec le « Départ synchronisé » (même heure de départ, horloges réglables, bip test).
- Bibliothèque « Partitions » depuis le menu (sans choisir de musicien) : ajout, modification, suppression, catégories, recherche, filtre par instrument et tri.
- Éditeur pour entrer ses propres partitions, partagées par toute la famille, avec import de fichiers MusicXML (.musicxml, .mxl) et MIDI (.mid).
- Réglages (roue dentée du menu, protégés par un petit calcul) : historique des performances, ajout ou retrait d'une performance, remise à zéro des scores avec confirmation, sauvegarde dans un fichier et synchronisation avec un dépôt GitHub privé.

## Jouer

Tout tient dans `index.html` (aucune installation). Pour utiliser le micro, la page doit être servie en HTTPS, par exemple avec GitHub Pages :

1. Sur GitHub : **Settings → Pages → Build and deployment → Deploy from a branch**, branche `main`, dossier `/ (root)`.
2. Ouvrir l'adresse indiquée dans Safari sur l'iPhone ou l'iPad.
3. **Partager → Sur l'écran d'accueil** pour l'installer comme une app (orientation paysage).
4. Pour la télé : recopie de l'écran via AirPlay.

Les profils et les scores sont enregistrés dans le navigateur de l'appareil.

## Sauvegarde privée sur GitHub (optionnel)

1. Créer un dépôt **privé** vide, par exemple `ileauxnotes-data`.
2. Créer un jeton : GitHub → Settings → Developer settings → Personal access tokens → **Fine-grained tokens** → *Generate new token* ; *Repository access* : uniquement `ileauxnotes-data` ; *Permissions* → *Contents* : **Read and write**.
3. Dans l'app : roue dentée → Sauvegarde → dépôt `Keops7996/ileauxnotes-data` + jeton → **Connecter**. À faire une fois sur chaque appareil de la famille.

La progression est alors envoyée après chaque partie et récupérée à l'ouverture de l'app.
