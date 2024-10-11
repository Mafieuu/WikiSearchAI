
## /R_script
Ce dossier contient l'application R Shiny pour l'interface utilisateur.

### app.R
- Point d'entrée de l'application Shiny
- Définit l'UI et le serveur
- Composants principaux :
  - Barre de recherche et bouton
  - Filtres de résultats [si possible]
  - Affichage des résultats paginés

### helpers.R
- Fonctions utilitaires pour l'application Shiny
- Gère la communication avec le backend Python
- Fonctions principales :
  - `query_backend()` : Envoie des requêtes au backend Python
  - `format_results()` : Formate les résultats pour l'affichage
  - [La base et le wiki_link vont dans le serveur ]
  - [pourquoi pas sauvegarder si necessaire le resultat du backend ]
  - [dans un .csv accesible depuis le server Github]

## Notes de Développement
- Suivez PEP 8 pour le style de code Python [**Super important**]
- Documentez toutes les fonctions avec des docstrings [**Super important**]
- Communiquer [**Super important**]