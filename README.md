# MLflow

Une plateforme de gestion de cycle de vie de modèle de machine learning inventé par le créateur de spark.

Globalement MLflow c'est une techno qui va nous permettre de pouvoir bien collaborer au sein de notre team data. Mais aussi à titre personnel sur nos machines, MLflow nous permettra d'organiser toutes nos modèles que nous avons entrainé afin de pouvoir choisir l'un de ces modèles plus facilement.

Donc c'est une techno qui va nous permettre de travailler avec plusieurs librairies de machine learning et d'utiliser nos modèles via une api ou une interface graphique.
MLflow facilite le partage entre collaborateur au sein d'une équipe et s'installe assez facilement.

Aujourd'hui Sur le github de MLflow [ici](https://github.com/mlflow/mlflow) on a plus de 8000 étoiles et il y a pas mal de contributeur sur ce projet.

# Problematique

MLflow répond à un problème de management des modèles.
Exple: Vous bossez dans une grande boite avec 3, 4 data scientists mais chacun va entrainer plusieurs modèles qui vont avoir des performences differentes, avec des hyper-paramètres différents. Comment garder une trace de toutes ces expériences ?

# Mlflow Tracking
## Tracking API
Ceci est le premier composant de MLflow. Il nous aidera a sauvegarder, requéter tous nos modèles de machine learning que nous avons entrainé. On peut accéder a ce composant soit via une API en ligne de commande ou une interface graphique.
Dans cette interface graphique on trouvera les infos sur nos modèles entrainés (date, utilisateurs,métriques , hyperparamètres, nom du modèle, taille des données,...)

En cliquant sur un run, on obtient plus d'info. Notamment pour les modèles de deep learning on peut avoir l'évolution des métriques à travers le temps.
Et sur un modèle on peut voir les Artifacts, qui sont des fichiers qui vont permettre de sauvegarder par exemple des images, des modèles, des fichiers de données

![image5](https://user-images.githubusercontent.com/48319188/113626126-0f255b80-9662-11eb-8d6e-e3550e5254cf.jpg)

<img width="1107" alt="oss_registry_1_register" src="https://user-images.githubusercontent.com/48319188/113626319-4bf15280-9662-11eb-91b0-3362d1a05b20.png">

# Mlflow Projects

C'est une convention pour pouvoir organiser et décrire le code afin de pouvoir le rendre reproductible.

L'idée est de pouvoir partager le code aux autres data scientist au sein de l'équipe, le rendre réutilisable soit via un dossier comportant tous les fichiers ou via un repo git.

Dans le fichier yaml qui represente le projet on trouvera:

- le nom du projet
- l'environnement ( soit une image docker)
- les entry_points


![MLproject](https://user-images.githubusercontent.com/48319188/113754265-587fb480-970f-11eb-8131-5288f1fdffdd.png)

# MLflow Models

Cette composante nous permet de packager les modèles de machine learning pour pouvoir les utiliser via des services API ou sur les clusters pour faire des prédictions.

# MLflow Model Registry

C'est un endroit ou on va stocker  des modèles pour manager leur cycle de vie. 
- Cela permet une gestion centralisée de tous les modèles en production au sein de l'entreprise. 
- On a une meilleure gestion du versionning
- On peut faire un staging qui nous permet de connaitre l'étape actuelle du modèle

<img width="1107" alt="registry" src="https://user-images.githubusercontent.com/48319188/113754562-a72d4e80-970f-11eb-97c5-64edd193725f.png">

<img width="1106" alt="registry2" src="https://user-images.githubusercontent.com/48319188/113754825-ebb8ea00-970f-11eb-9831-99b27653a9aa.png">

<img width="1105" alt="registry3" src="https://user-images.githubusercontent.com/48319188/113755142-43efec00-9710-11eb-810b-d6330026b1d4.png">


![registry5](https://user-images.githubusercontent.com/48319188/113755368-887b8780-9710-11eb-92c9-fd43916353b6.png)
