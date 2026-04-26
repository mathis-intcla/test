# Workstories by Mélissa

Site vitrine one-page inspiré de la direction artistique Workstories (palette chaleureuse, univers aventureux, ton éditorial orienté podcast/voix).

## Aperçu du projet

- **Stack**: HTML + CSS (sans framework)
- **Objectif**: landing page claire, rapide à charger, facile à maintenir
- **Fichiers principaux**:
  - `index.html`
  - `styles.css`

## Lancer le projet en local

### Option 1 (recommandée)

```bash
python3 -m http.server 8000
```

Puis ouvrir: [http://localhost:8000](http://localhost:8000)

### Option 2

Ouvrir directement `index.html` dans un navigateur (moins fiable pour certains assets externes selon les navigateurs).

## Structure

```txt
.
├── index.html
├── styles.css
├── LICENSE
├── .gitignore
├── README.md
└── .github/
    └── workflows/
        └── ci.yml
```

## Workflow GitHub conseillé

1. Créer une branche:
   ```bash
   git checkout -b feat/ma-modif
   ```
2. Modifier les fichiers.
3. Tester en local (`python3 -m http.server 8000`).
4. Commit:
   ```bash
   git add .
   git commit -m "feat: ma modification"
   ```
5. Push + Pull Request sur GitHub.

## CI (GitHub Actions)

Un workflow est inclus (`.github/workflows/ci.yml`) pour:
- vérifier que `index.html` et `styles.css` existent,
- signaler rapidement une régression structurelle sur les pushes/PR.

## Déploiement GitHub Pages (optionnel)

Tu peux publier le site en activant **Settings → Pages** sur la branche `main` (root).

## Licence

Ce projet est distribué sous licence **MIT**. Voir [`LICENSE`](./LICENSE).
