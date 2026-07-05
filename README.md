# Monteur Nation — Site

Ce dossier contient ton site complet, prêt à héberger sur GitHub Pages.

## Fichiers
- `index.html` → page d'accueil
- `monteur-nation-essentiel.html` → page de vente formation Essentiel™ (Premiere Pro)
- `monteur-nation-mobile.html` → page de vente formation Mobile™ (CapCut/VN)

Les 3 pages sont maintenant reliées entre elles :
- Depuis l'accueil, les boutons "Rejoindre la formation" mènent vers chaque page de vente.
- Depuis chaque page de vente, une barre en haut permet de revenir à l'accueil ou d'aller vers l'autre formation.

## Héberger sur GitHub Pages (gratuit)

1. Crée un compte GitHub (github.com) si tu n'en as pas.
2. Crée un nouveau repository, par exemple `monteur-nation` (public).
3. Mets tous les fichiers de ce dossier (`index.html`, `monteur-nation-essentiel.html`, `monteur-nation-mobile.html`) à la racine du repository — soit en les glissant/déposant sur la page GitHub ("Add file" → "Upload files"), soit via git :
   ```
   git init
   git add .
   git commit -m "Premier déploiement du site"
   git branch -M main
   git remote add origin https://github.com/TON-USER/monteur-nation.git
   git push -u origin main
   ```
4. Sur GitHub, va dans **Settings → Pages**.
5. Dans "Build and deployment", choisis **Source: Deploy from a branch**, branche `main`, dossier `/root`.
6. Clique **Save**. Après ~1 minute, ton site sera en ligne à :
   ```
   https://TON-USER.github.io/monteur-nation/
   ```

## À faire avant publication
- Remplace les `PASTE-PHOTO-URL-*.jpg` et `PASTE-PAYMENT-PROOF-*.jpg` par tes vraies images (témoignages, preuves de paiement).
- Remplace les vidéos YouTube `SRC_VIDEO_3` par tes vraies vidéos.
- Vérifie que les liens de paiement (`boutique.dekel-dev.com/checkout?...`) sont corrects.
- Si tu veux un nom de domaine personnalisé (ex. `academy.dekel-dev.com`), ajoute un fichier `CNAME` à la racine contenant ce domaine, puis configure un enregistrement DNS chez ton registrar (CNAME vers `TON-USER.github.io`).
