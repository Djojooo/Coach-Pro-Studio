# Coach Pro Studio

Cahier de séances d'entraînement de football : tableau tactique à l'échelle, animation par étapes, exemples d'exercices et de séances, fiche PDF A4.

Application web installable (PWA) : elle fonctionne hors connexion après la première ouverture et enregistre les séances **sur l'appareil**.

## Mise en ligne sur GitHub Pages

1. Crée un dépôt sur GitHub (par exemple `coach-pro-studio`).
2. Dépose **tout le contenu de ce dossier** à la racine du dépôt : `index.html`, `manifest.webmanifest`, `sw.js`, `.nojekyll` et le dossier `icons/`.
   - Depuis le site GitHub : *Add file → Upload files*, glisse les fichiers et le dossier `icons`, puis *Commit changes*.
3. Dans le dépôt : *Settings → Pages → Build and deployment*. Source : *Deploy from a branch*, branche `main`, dossier `/ (root)`, puis *Save*.
4. Après une à deux minutes, l'app est en ligne à l'adresse `https://<ton-pseudo>.github.io/coach-pro-studio/`.

Tu peux aussi la mettre dans un sous-dossier d'un dépôt existant (par exemple `studio/` dans `coach-pro`) : tous les chemins sont relatifs, l'app sera alors à `…/coach-pro/studio/`.

## Installer l'app

- **Android (Chrome)** : ouvre l'adresse, puis le bouton *Installer l'app* en haut, ou menu ⋮ → *Installer l'application*.
- **iPhone / iPad (Safari)** : bouton Partager → *Sur l'écran d'accueil*.
- **Ordinateur (Chrome, Edge)** : bouton *Installer l'app* ou l'icône d'installation dans la barre d'adresse.

## Données

- Les séances et les exercices de ta bibliothèque sont enregistrés dans le navigateur de l'appareil. Elles ne passent pas d'un appareil à l'autre.
- *Tout exporter* (en bas de la liste des séances) crée un fichier `.json` avec toutes tes séances ; *Importer* le restaure sur n'importe quel appareil. Fais-le régulièrement.
- Effacer les données du site dans le navigateur supprime les séances : garde une sauvegarde.

## Mettre à jour l'app

Remplace `index.html` dans le dépôt. Si tu modifies aussi les icônes ou le manifeste, change `VERSION` en haut de `sw.js` (par exemple `cps-v2`). La nouvelle version s'affiche à la prochaine ouverture avec connexion.
