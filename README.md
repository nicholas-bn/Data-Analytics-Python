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
- Application d'un PCA pour réduire en 2D.
- Application d'un KMeans pour prédire les clusters.
- Visualisation graphique des clusters.

![RésultatsClustering](https://i.imgur.com/MQpvgzg.png)

### 3. Prédiction supervisé d'une catégorie de voiture pour les nouveaux clients.

- Nettoyage des datasets de client d’entraînement et à prédire
- Application d’un StandardScaler
- Jointure des clusters au client d’entrainement via le numéro de plaque d’immatriculation
- Prédiction sur les nouveaux de cluster préférentiel.

### 4. Choix d'un véhicule dans le cluster prédit.

- Random parmi un véhicule dans le cluster.


