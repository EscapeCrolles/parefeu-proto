# Protocole Pare-feu – prototype de repérage

Une seule page web pour relever les lieux, monter un parcours test et le jouer avec validation GPS sur place. Rayon par défaut : 20 m.

## Mettre la page en ligne (GitHub Pages, une fois)

Faisable depuis Chrome sur Android, en mode « Version pour ordinateur » si les menus sont trop serrés.

1. Sur github.com, crée un dépôt **public** (Pages gratuit l'exige), par exemple `parefeu-proto`.
2. Dans le dépôt : **Add file → Upload files**, envoie `index.html`, puis **Commit changes**.
3. **Settings → Pages** : Source = *Deploy from a branch*, Branch = `main`, dossier `/ (root)`, **Save**.
4. Après une à deux minutes, la page est en ligne à `https://TON-PSEUDO.github.io/parefeu-proto/`.
5. Ouvre ce lien dans Chrome, accepte la localisation **précise**. Menu ⋮ → « Ajouter à l'écran d'accueil » pour l'avoir comme une appli.

Le dépôt ne contient que le code. Tes lieux, questions et réponses restent dans le téléphone : rien n'est public.

## Relever (pendant le repérage)

- Attends que la pastille en haut à droite passe au vert (précision de 10 m ou mieux) ou au jaune (25 m ou mieux).
- Donne un nom et une remarque (ce qu'on peut exploiter sur place), puis **Enregistrer ce lieu**. Reste immobile 10 secondes : la position est moyennée.
- Si le message signale une précision faible, refais le relevé un peu plus à découvert. Avec un rayon de 20 m, un relevé à ± 30 m ne tiendra pas.

## Parcours

- L'ordre de la liste est l'ordre de la partie (boutons Monter / Descendre).
- Par lieu : rayon, énigme de destination, question sur place, réponses acceptées séparées par `/`, indice.
- Les réponses ignorent majuscules, accents, tirets et espaces : « Mil huit cent quatre-vingt-dix-sept » = « mil huit cent quatre vingt dix sept ».
- Une étape sans réponse se valide d'un bouton, une fois sur place : pratique pour tester juste les zones.
- La pastille à droite du nom donne ta distance au lieu, en vert quand tu es dans le rayon.
- **Export tableur** : la liste à m'envoyer. **Sauvegarde** / **Importer** : copie complète du parcours, pour la garder ou la charger sur un autre téléphone.

## Jouer

- **Ouvrir la sacoche** lance le chrono de 1 h 30. La partie copie le parcours au départ : modifier le parcours pendant une partie ne la change pas.
- L'étape se débloque en entrant dans le rayon (le téléphone vibre). La réponse n'est acceptée que dans la zone.
- **Indice** : +5 minutes, une fois par étape. **Je suis sur place** : débloque sans GPS, noté dans le journal.
- Option « Compter la marge d'erreur du GPS » : la zone est atteinte si la distance moins la précision est sous le rayon. Plus tolérant, à essayer si 20 m bloque trop souvent.
- Garde l'écran allumé et la page ouverte : le navigateur ne suit pas la position en arrière-plan.

## Journal

Par étape : heure d'arrivée et de validation (comptées depuis le départ), temps passé sur place, distance et précision au moment de valider, essais, indice, secours. **Export tableur** pour me l'envoyer après chaque test.

## À savoir

- Les données sont stockées dans Chrome. Vider les données du navigateur les efface : fais une **Sauvegarde** après chaque repérage.
- Testé avec un GPS simulé dans Chrome. Le comportement réel du GPS de ton téléphone en ville reste à vérifier sur le terrain : c'est le but du prototype.
