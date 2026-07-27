# French Market Concepts

Cinq maquettes statiques et autonomes :

1. LnkFlow
2. CrawlRaven
3. Migma AI
4. Skippr
5. ACME.BOT

## Prévisualisation GitHub Pages

URL de publication : https://jeanjean59800.github.io/french-market-previews/

Pages individuelles :

- `/lnkflow/`
- `/crawlraven/`
- `/migma/`
- `/skippr/`
- `/acmebot/`

La branche de publication dédiée est `gh-pages`, dossier `/ (root)`.

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

Un fichier `robots.txt` est également présent sur la branche de publication pour demander aux moteurs de ne rien explorer. Ces mesures réduisent l’indexation, mais les URL GitHub Pages restent publiques.
