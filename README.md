# reconnaissanceIA

Interface **Scan IA** DirectAlu (reconnaissance produit par image).

- Fichier principal : `index.html` (hébergement statique ou [GitHub Pages](https://pages.github.com/)).
- Données catalogue : `product-links.json`.
- Ressources : dossier `assets/`.

## Mettre à jour depuis le dépôt de développement

À la racine du projet parent (`Version_5`) :

```bash
node scripts/sync-reconnaissanceIA-repo.mjs
```

Puis commit et push depuis ce dossier.

## Git

```bash
git add .
git commit -m "Update scanner"
git push origin main
```
