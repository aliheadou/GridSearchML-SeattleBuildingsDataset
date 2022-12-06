# GridSearchML-SeattleBuildingsDataset

## Notebook Nettoyage

Pour atteindre l'objectif de ville neutre en émissions de carbone en 2050, la ville de Seattle s’intéresse de près aux émissions des bâtiments non destinés à l'habitation. La mesure de la consommation énergétique, ainsi que des émissions en gaz à effet de serre, est la première étape de toute démarche d'amélioration de l’efficacité énergétique d’un bâtiment.

Pour ce faire, des relevés minutieux ont été effectués en 2015 et en 2016. Les relevés sont en effet des indicateurs performants qui permettent de comprendre le fonctionnement des systèmes d’énergie des bâtiments (électricité, chauffage, climatisation, ventilation etc..). Cependant, ces relevés sont coûteux à obtenir, et à partir de ceux déjà réalisés, nous devons tenter de prédire les émissions de CO2 et la consommation totale d’énergie de bâtiments pour lesquels elles n’ont pas encore été mesurées.

Dans ce premier notebook, après avoir nettoyé les deux jeux de données, nous allons sélectionner et créer de nouvelles variables pertinentes pour la prédiction des deux quantités d'intérêts. Dans un second temps, nous chercherons à mesurer l’intérêt de l’ENERGY STAR Score qui a été défini par le Portfolio Manager pour évaluer l'éfficacité thermique sur une échelle de 1 à 100.


## Notebook Prediction

Dans ce notebook, nous allons utiliser quelques modèles de machine learning dans le but de prédire nos deux variables cibles, SiteEnergyUse(kBtu) et TotalGHGEmissions, grâce au feature engineering réalisé dans le notebook de nettoyage précédent.

Dans un second temps, on cherchera à évaluer l’intérêt de l’ENERGY STAR Score pour la prédiction. Pour ce faire, on va intégrer cette variable comme nouvelle variable indépendante de notre modélisation et observer son effet sur les métriques de performances. On verra que le score des modèles ensemblistes devient nettement meilleur lorsque l'on tient compte de cette variable.
