# Mon suivi muscu

Petite app web pour suivre deux séances full body par semaine : répétitions à cocher, exercices terminés, charges semaine par semaine et images d'exécution.

## Mettre l'app en ligne avec GitHub Pages

1. Crée un nouveau dépôt sur GitHub (par exemple `suivi-muscu`).
2. Ajoute les fichiers à la racine du dépôt : `index.html`, `README.md` et le dossier `images/`.
3. Dans le dépôt, ouvre **Settings → Pages**.
4. Sous **Build and deployment**, choisis **Deploy from a branch**, puis la branche `main` et le dossier `/ (root)`, puis enregistre.
5. Après une minute ou deux, l'app est disponible à l'adresse `https://TON-PSEUDO.github.io/suivi-muscu/`.

Sur téléphone, ouvre le lien puis utilise « Ajouter à l'écran d'accueil » pour l'avoir comme une vraie app.

## Ajouter les images

Place une image par exercice dans le dossier `images/`, avec exactement ces noms (formats acceptés : `.jpg`, `.png`, `.webp`, `.jpeg`, `.gif`) :

| Exercice | Nom du fichier |
|---|---|
| Hip thrust | `hip-thrust` |
| Presse à cuisses | `presse-cuisses` |
| Abduction à la machine | `abduction` |
| Développé machine pectoraux | `developpe-pectoraux` |
| Élévations latérales | `elevations-laterales` |
| Planche | `planche` |
| Soulevé de terre roumain | `souleve-terre-roumain` |
| Fentes / split squat bulgare | `fentes-split-squat` |
| Pont fessier une jambe / kickback | `pont-kickback` |
| Tirage vertical | `tirage-vertical` |
| Rowing machine | `rowing` |
| Crunch à la poulie | `crunch-poulie` |

Exemple : `images/hip-thrust.jpg`. Tant qu'une image est absente, l'app affiche un lien de recherche d'images pour cet exercice.

## Données

Les coches et les charges sont enregistrées dans le navigateur (`localStorage`), sur l'appareil utilisé. L'onglet **Suivi** propose un export et un import en JSON pour sauvegarder ou transférer les données.

## Modifier le programme

Les exercices, les séries et les répétitions se trouvent dans l'objet `PROGRAM` au début du script de `index.html`.

