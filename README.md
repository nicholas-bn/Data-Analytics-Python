# Data-Analytics-Python
Application de plusieurs modèles de Machine Learning à partir de véhicules immatriculés et de clients pour prédire le véhicule le plus adapté.


## Différentes étapes pour la prédiction de véhicules pour les clients

1. Préparation et Analyse de la data.
2. Clustering des types de véhicules depuis le fichier Immatriculations.csv et ajout sur la colonne de train clients.
3. Prédiction supervisé d'une catégorie de voiture pour les nouveaux clients.
4. Choix d'un véhicule dans le cluster prédit.


### 1. Préparation et Analyse de la data

- Les données sont fragmentées en plusieurs fichiers CSV.
- Etude des différents modéles a appliqué.

### 2. Clustering des types de véhicules depuis le fichier Immatriculations.csv et ajout sur la colonne de train clients.

- Analyse graphique/textuelle des datas.
- Nettoyage de la data de Immatriculations.csv.
- Application d’un StandardScaler
- Application d'un PCA pour réduire en 2D.
- Application d'un KMeans pour prédire les clusters.
- Visualisation graphique des clusters.

![RésultatsClustering](https://i.imgur.com/MQpvgzg.png)

### 3. Prédiction supervisé d'une catégorie de voiture pour les nouveaux clients.

- Nettoyage des datasets de client d’entraînement et à prédire
- Application d’un StandardScaler
- Jointure des clusters au client d’entrainement via le numéro de plaque d’immatriculation
- KFold + Catboostclassifier pour prédire les nouveaux clusters

### 4. Choix d'un véhicule dans le cluster prédit.

- Random parmi un véhicule dans le cluster.


## Lancement des notebooks

- Nécessite Jupyter Notebook (via Anaconda par exemple), de quelques package python (sklearn, numpy, missingno, etc.)
- Lancer le notebook _"cluster_vehicule_EDA.ipynb"_ en premier pour produire le CSV _"immatriculation_and_cluster.csv"_ en amont nécessaire à _"Client_EDA.ipynb"_ qui contient les plaques et leur cluster respectifs.
