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

Ceci est le premier composant de MLflow. Il nous aidera a sauvegarder, requéter tous nos modèles de machine learning que nous avons entrainé. On peut accéder a ce composant soit via une API en ligne de commande ou une interface graphique.
Dans cette interface graphique on trouvera les infos sur nos modèles entrainés (métriques , hyperparamètres, nom du modèle, taille des données,...)

![image5](https://user-images.githubusercontent.com/48319188/113626126-0f255b80-9662-11eb-8d6e-e3550e5254cf.jpg)
