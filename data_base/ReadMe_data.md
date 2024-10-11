## /data_base
Ce dossier contient la base de données et les fichiers liés aux données.
### wikipedia_links.json
- Stocke tous les liens Wikipedia collectés
- Format : `{"url": "...", "title": "...", "date_added": "..."}`

### wiki_articles.db
- Base de données SQLite contenant les articles traités
- Tables :
  - `articles` : Stocke le contenu des articles
   - `titres` : Stocke le contenu des titres
  - `categories` : Stocke les catégories des articles
  - [ Trouver un moyen de se debarasser des liens deja sauvegader dans la base ]
  - [ Pourquoi pas parcourir wikipedia categorie par categorie ]

