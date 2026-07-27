# French Market Concepts

Cinq maquettes statiques et autonomes :

1. LnkFlow
2. CrawlRaven
3. Migma AI
4. Skippr
5. ACME.BOT

## Ouvrir localement

Ouvrir `index.html` directement dans un navigateur, ou lancer :

```bash
python3 -m http.server 8080 --directory .
```

Puis visiter `http://localhost:8080`.

## Déployer sur un VPS

Copier le dossier dans un répertoire servi par Nginx ou Caddy. Aucun build, aucune dépendance et aucune API ne sont nécessaires.

Toutes les pages contiennent :

```html
<meta name="robots" content="noindex,nofollow">
```

Elles peuvent donc servir de prévisualisations privées avant tout accord du prospect.

## Publier avec GitHub Pages

Le dépôt peut être publié directement depuis la branche `main`, dossier `/ (root)`.

Après avoir créé un dépôt public vide :

```bash
git init
git add .
git commit -m "Publish French market concepts"
git branch -M main
git remote add origin https://github.com/Jeanjean59800/french-market-concepts.git
git push -u origin main
```

Dans GitHub : `Settings` → `Pages` → `Deploy from a branch` → `main` → `/ (root)`.
