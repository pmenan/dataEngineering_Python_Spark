# dataEngineering_Python_Spark
Ce repo contient un script de traitement de données avec python + Spark (PySpark) 
Ce traitement tourne sur cluster Amazone EMR crée en amont du traitement.

Objectif :
- Récupérer un fichier depuis Redfin (https://redfin-public-data.s3.us-west-2.amazonaws.com/redfin_market_tracker/city_market_tracker.tsv000.gz)
- le stocker dans un aws s3 bucket source : s3://store-raw-data-123-yml)
- Explorer le fichier, faire des transformations (ajout de colonnes calculées, suppression des valeurs en doubles et lignes avec valeurs manquantes)
- Chargement des données au format parquet après transformation dans aws 3 bucket cible : s3://redfin-transform-zone-123-yml

volume de donnée : 1.1GB
