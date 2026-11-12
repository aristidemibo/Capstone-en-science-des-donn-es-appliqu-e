# Capstone-en-science-des-donn-es-appliqu-e
🚀 Prédiction de l'atterrissage du premier étage de Falcon 9
Projet Capstone – IBM Applied Data Science (Coursera) Dernier cours du IBM Data Science Professional Certificate et de la spécialisation Applied Data Science with Python.
📌 Contexte et problématique

SpaceX propose des lancements Falcon 9 à environ 62 millions de dollars, alors que les autres fournisseurs facturent à partir de 165 millions de dollars. Cette différence s'explique en grande partie par la réutilisation du premier étage de la fusée.

Dans ce projet, j'endosse le rôle d'un·e Data Scientist travaillant pour une startup qui souhaite concurrencer SpaceX. L'objectif : prédire si le premier étage de Falcon 9 atterrira avec succès. Cette prédiction permet d'estimer le coût réel d'un lancement et d'aider l'entreprise à formuler des offres plus éclairées face à SpaceX.

🎯 Objectifs
Collecter des données réelles sur les lancements de Falcon 9 (API REST et web scraping)
Nettoyer et préparer les données (data wrangling)
Mener une analyse exploratoire (SQL et visualisation)
Construire des tableaux de bord et des cartes interactives
Entraîner, optimiser et comparer plusieurs modèles de classification
Communiquer les résultats aux parties prenantes
🧭 Méthodologie
Étape	Description	Outils
1. Collecte des données	Récupération via l'API SpaceX et scraping des pages Wikipédia des lancements Falcon 9	requests, BeautifulSoup, pandas
2. Data wrangling	Gestion des valeurs manquantes, création de la variable cible (Class : succès / échec de l'atterrissage)	pandas, numpy
3. EDA avec SQL	Requêtes exploratoires sur les sites de lancement, les charges utiles, les résultats de mission	SQL, sqlite
4. EDA avec visualisation	Relations entre numéro de vol, site, charge utile, orbite et taux de réussite	matplotlib, seaborn
5. Analyse géospatiale	Carte interactive des sites de lancement et de leur proximité (côtes, villes, voies de transport)	Folium
6. Dashboard interactif	Exploration des lancements par site et par charge utile	Plotly Dash
7. Modélisation prédictive	Classification, recherche d'hyperparamètres et comparaison des modèles	scikit-learn
8. Restitution	Rapport / présentation des résultats	PowerPoint / PDF
🤖 Modèles de machine learning

Les modèles suivants ont été entraînés et optimisés avec GridSearchCV sur un jeu d'entraînement, puis évalués sur un jeu de test :

Régression logistique
Machine à vecteurs de support (SVM)
Arbre de décision
K plus proches voisins (KNN)
