
### wiki_scraper.py
- Gère le scraping des articles Wikipedia
- Utilise BeautifulSoup et requests pour l'extraction de contenu
- Implémente le multithreading pour optimiser la collecte de données
- Fonctions principales :
  - `collect_links()` : Collecte récursivement les liens Wikipedia
  - `check_link_exists()` : Vérifie si un lien est déjà dans la base
  - `save_links_to_json()` : Sauvegarde les liens dans un fichier JSON

### data_processor.py
- Traite les données extraites des articles Wikipedia
- Nettoie et formate le texte pour le stockage
- Fonctions principales :
  - `extract_article_content()` : Extrait le contenu d'un article
  - `format_data()` : Formate les données pour la base de données
  - `update_database()` : Insère ou met à jour les données dans SQLite
  - [pourquoi pas d'abord faire le nlp_processor puis sauvegarder ]

### nlp_processor.py
- Implémente les fonctionnalités de traitement du langage naturel
- Utilise spaCy pour la tokenization et la lemmatisation

