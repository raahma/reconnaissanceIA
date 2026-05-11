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
