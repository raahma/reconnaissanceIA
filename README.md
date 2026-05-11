# reconnaissanceIA

Interface **Scan IA** DirectAlu (reconnaissance produit par image).

- Fichier principal : `index.html` (hébergement statique ou [GitHub Pages](https://pages.github.com/)).
- Données catalogue : `product-links.json`.
- Ressources : dossier `assets/`.

## Mettre à jour le site après changements sur `front_v5.html`

À la racine du dossier parent (`Version_5`, un niveau au-dessus) :

```bash
node scripts/sync-reconnaissanceIA-repo.mjs
```

Puis dans ce dossier (`reconnaissanceIA`) :

```bash
git add .
git commit -m "Update scanner"
git push origin main
```

Le dossier `reconnaissanceIA` est le clone Git lié à [github.com/raahma/reconnaissanceIA](https://github.com/raahma/reconnaissanceIA).

## Bouton « Scanner ma pièce » sur directalu.com

Le dépôt Git **ne change pas** le site tout seul. Il faut :

1. **Activer GitHub Pages** sur le repo (Settings → Pages → branche `main`, dossier `/ (root)`).
2. Noter l’URL du type `https://raahma.github.io/reconnaissanceIA/`.
3. Dans WordPress / le thème DirectAlu, faire pointer le bouton **Scanner ma pièce** vers cette URL (ou vers une page du même domaine qui redirige vers cette URL).

Tant que l’étape 3 n’est pas faite sur le site, le bouton continuera d’ouvrir l’ancienne page (`/fr/scanner-ma-piece`).
