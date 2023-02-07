# Création d'une base de données immobilières avec SQL

## Business tasks

Pour le compte d'un réseau d'agences immoblière, création d'un modèle permettant de mieux prévoir le prix de vente des biens immobiliers.

### 1. Création de la base de données permettant de collecter les transactions immobilières et foncières en France.

A partir des données extraites du site open data des Demandes de valeurs foncières (DVF)

source données : https://www.data.gouv.fr/fr/datasets/demandes-de-valeurs-foncieres/


- Préparer le dictionnaire des données en respectant le template en PJ pour répertorier et décrire les données importantes à stocker.

![p2_dictionnaire](https://user-images.githubusercontent.com/87067133/217299142-3e745df6-d267-47fb-8cb6-091de83f213d.png)


  - Préparer le modèle conceptuel des données.
 
![p2_modele_conceptuel](https://user-images.githubusercontent.com/87067133/217298814-28f24746-a0ac-4677-8aa2-5d3161771719.png)

  
  - Préparer le schéma relationnel normalisé en 3NF de la base de données qui donnera lieu à la création des tables.
  
  ![p2_schema_relationnel](https://user-images.githubusercontent.com/87067133/217298871-dd31c8d8-13f7-43c3-a5c6-2a97ee4b26c3.png)
  

  - Implémenter la base de données (sur PostgreSQL)
  
### 2. Requêtes SQL pour aider les différentes agences à mieux accompagner leurs clients.

(Pour ne pas influencer les étudiants suivant le même parcours, seuls les résultats seront affichés et le code SQL caché)

  - Nombre total d’appartements vendus au 1er semestre 2020.
  - Proportion des ventes d’appartements par le nombre de pièces.
  - Liste des 10 départements où le prix du mètre carré est le plus élevé.
  - Prix moyen du mètre carré d’une maison en Île-de-France.
  - Liste des 10 appartements les plus chers avec le département et le nombre de mètres carrés.
  - Taux d’évolution du nombre de ventes entre le premier et le second trimestre de 2020.
  - Liste des communes où le nombre de ventes a augmenté d'au moins 20% entre le premier et le second trimestre de 2020
  - Différence en pourcentage du prix au mètre carré entre un
appartement de 2 pièces et un appartement de 3 pièces.
  - Les moyennes de valeurs foncières pour le top 3 des communes des départements 6, 13, 33, 59 et 69


Environnement technique : UML, SQL, PostgreSQL
