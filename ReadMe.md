
# WikiSearchAI - Moteur de Recherche Intelligent pour Wikipedia

Ensemble, nous levons l'ancre, avec cette immense mer de connaissances à explorer. Le cap est fixé, mais, tout navigateur le sait bien, c'est le vent qui nous guidera.

L'aventure que nous entamons avec **WikiSearchAI** ressemble à un voyage en haute mer. Ce plan, bien tracé, est comme la carte d'un vaste océan : une esquisse des côtes que nous espérons atteindre, mais entre les vagues, les marées et les courants imprévisibles, il y aura forcément des détours, des îles surprises et peut-être même quelques tempêtes (mais rien de trop effrayant, promis !).

On risque de se faire un peu secouer de temps en temps, mais après tout, que serait une bonne aventure sans quelques vagues pour épicer le tout ? L’océan est vaste et n’attend que nous pour le conquérir.

## Description du Projet
WikiSearchAI est un moteur de recherche intelligent qui utilise le traitement du langage naturel pour faire des recherches dans les articles Wikipedia. Le projet combine le scraping web, le traitement de données, le NLP et une interface utilisateur en R Shiny.

## Structure du Projet
```
wiki_search_ai/
├── data_base/
│   ├── processed_data.db      
│   ├── ReadMe_data.md          
│   └── wiki_links.json         
│
├── python_scripts/
│   ├── data_extractor.py      
│   ├── nlp_processor.py        
│   ├── ReadMe_python.md        
│   └── wiki_scraper.py         
│
├── R_scripts/
│   ├── app.R                  
│   └── ReadMe_R.md             
├── main.py   
├── ReadMe.md                 
└── ReadMe_main.md       
```      
 # Guide général du projet


## Liste des Tâches à Accomplir

### Phase 1 : Configuration Initiale
- [x] Créer la structure du projet
- [x] Initialiser l'environnement virtuel Python
```bash
python -m venv env
source env/bin/activate  # Sur Windows : .\env\Script\Activate
```
- [x] Installer les dépendances Python
```bash
pip install -r requirements.txt
```
- [x] Installer les dépendances R
On se réfèrera à l'article : https://rstudio.github.io/renv/

### Phase 2 : Développement du Scraper Wikipedia
- [ ] Développer la fonction de collecte des liens Wikipedia
  - [ ] Développer la fonction qui vérifie si un lien est déjà ajouté ou pas
  - [ ] Implémenter la sauvegarde des liens dans le fichier JSON
  - [ ] Implémenter le multithreading [avec le module asynchrone]
  - [ ] Ajouter un système de reprise en cas d'interruption

### Phase 3 : Extraction et Stockage des Données
- [ ] Développer le système d'extraction de contenu via les liens Wikipedia
  - [ ] Extraire le titre, le contenu et les catégories
  - [ ] Formater les données extraites
- [ ] Créer la base de données SQLite
  - [ ] Implémenter les fonctions d'insertion/mise à jour
- [ ] Implémenter un système de logging [si nécessaire]
- [ ] Ajouter la gestion des erreurs et des exceptions

### Phase 4 : Traitement NLP
- [ ] Développer le modèle NLP
  - [ ] Implémenter la tokenization et la lemmatisation
  - [ ] Créer le système de vectorisation TF-IDF
  - [ ] Développer le système de scoring des résultats

### Phase 5 : Développement de l'Interface R Shiny
- [ ] Développer l'interface utilisateur
  - [ ] Créer la page de recherche
  - [ ] Implémenter l'affichage des résultats
- [ ] Implémenter la communication avec le backend Python
- [ ] Ajouter des fonctionnalités de filtrage et de tri des résultats [pour le fun !]

### Phase 6 : Intégration et Tests
- [ ] Développer des tests d'intégration
- [ ] Effectuer des tests de performance
- [ ] Optimiser les requêtes et le temps de réponse [si possible]

### Phase 7 : Déploiement
- [ ] Déployer les scripts Python sur le serveur
- [ ] Déployer l'application R Shiny sur GitHub [un site web accessible]

### Phase 8 : Documentation et Finalisation
- [ ] Créer un PDF LaTeX avec le package zestedesavoir pour documenter tout le projet
- [ ] Créer un guide d'utilisation [pourquoi pas l'intégrer au site web !]
- [ ] Documenter le processus de déploiement
- [ ] Préparer une présentation du projet avec beamer [c'est une blague !]

## Utilisation
1. Assurez-vous que le backend Python est en cours d'exécution
2. Lancez l'application R Shiny
3. Utilisez la barre de recherche pour effectuer des requêtes
4. Explorez les résultats et utilisez les filtres [si disponibles]

## Contribution
Les contributions sont les bienvenues ! Veuillez suivre ces étapes :
1. Forkez le projet
2. Créez une nouvelle branche (`git checkout -b append_feature`)  
3. Committez vos changements (`git commit -m 'description du commit'`)
4. Poussez vers la branche (`git push origin append_feature`)
5. Ouvrez un Pull Request

## Ressources Utiles
- [Documentation de BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
- [Documentation de spaCy](https://spacy.io/usage)
- [Guide R Shiny](https://shiny.rstudio.com/tutorial/)
- [API Wikipedia](https://pypi.org/project/wikipedia/)
