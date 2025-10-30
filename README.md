# visite-ens-lyon-sophia-2025.github.io

Visite de l'ENS Lyon aux laboratoires I3S, INRIA et LEAT à Sophia Antipolis 4-5 novembre 2025

## À propos

Ce site web statique est construit avec Jekyll et utilise des fichiers Markdown pour le contenu. Il est automatiquement déployé sur GitHub Pages.

## Structure du site

- `index.md` - Page d'accueil
- `programme.md` - Programme détaillé de la visite
- `infos-pratiques.md` - Informations pratiques (lieu, transport, etc.)
- `_layouts/default.html` - Layout HTML principal
- `_config.yml` - Configuration Jekyll

## Modification du contenu

Pour modifier le contenu du site :

1. Éditez les fichiers `.md` dans le dépôt
2. Utilisez la syntaxe Markdown standard
3. Commitez et pushez vos modifications
4. GitHub Pages reconstruira automatiquement le site (peut prendre 1-2 minutes)

## Ajouter une nouvelle page

1. Créez un nouveau fichier `.md` dans le dépôt
2. Ajoutez l'en-tête YAML au début :
   ```markdown
   ---
   layout: default
   title: Titre de la page
   ---
   ```
3. Ajoutez votre contenu en Markdown
4. Liez la page depuis d'autres pages avec `[Texte du lien](nom-de-la-page.md)`

## Développement local (optionnel)

Pour tester le site localement avant de pousser :

```bash
# Installer les dépendances
bundle install

# Lancer le serveur de développement
bundle exec jekyll serve

# Visiter http://localhost:4000
```

## Site en ligne

Le site est accessible à l'adresse : https://etiloz.github.io/visite-ens-lyon-sophia-2025.github.io/

