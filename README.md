# Seed · Data Sport

Tableau de bord sportif et page de paramétrage des fournisseurs, en français.

## Développement

Node.js 22.12+ (validé avec Node.js 24).

```sh
npm ci
npm run dev
```

## Production

```sh
npm run build
npm run preview
```

Navigation : tableau de bord à `/`, paramètres à `/#parametres`.

Cette version affiche des états vides, sans données fictives. Les filtres de période et la navigation sont opérationnels. Les connecteurs Garmin, iGPSPORT et Zwift ne sont pas encore implémentés : aucun identifiant n'est collecté ou stocké. La prochaine étape nécessite un serveur pour le stockage sécurisé et la validation des modes d'accès autorisés par chaque fournisseur. Les polices Google sont optionnelles, avec des polices système en repli.

## GitHub Pages

La publication est automatisée par `.github/workflows/pages.yml` à chaque envoi sur `main`.
Dans les paramètres GitHub du dépôt, ouvrir **Pages**, puis sélectionner **GitHub Actions** comme source.
Le site est prévu pour https://maximiliendbrx.github.io/Data-Sport/ ; Vite utilise donc la base `/Data-Sport/`.
Le workflow peut également être relancé depuis **Actions → Publish Seed to GitHub Pages → Run workflow**.
