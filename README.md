# Création d'une base de données immobilières avec SQL

## Business tasks

Pour le compte d'un réseau d'agences immoblière, création d'un modèle permettant de mieux prévoir le prix de vente des biens immobiliers.

### 1. Création de la base de données permettant de collecter les transactions immobilières et foncières en France.

  - Données extraites du site open data des Demandes de valeurs foncières (DVF). Il faut que tu prépares le dictionnaire des données en respectant le template en PJ pour répertorier et décrire les données importantes à stocker.

  - Modèle conceptuel des données ? Ça nous permettra de bien visualiser les différentes entités, associations et cardinalités de la base de données. Pour le formalisme, choisis ce que tu veux entre UML ou MERISE
  
    
  ![Capture d’écran 2023-02-07 à 17 04 13](https://user-images.githubusercontent.com/87067133/217298002-3600eddf-bf68-4b95-8a20-4826384d69e3.png)
  
  
  - Schéma relationnel normalisé en 3NF de la base de données qui donnera lieu à la création des tables.
  
  
  ![Capture d’écran 2023-02-07 à 17 05 30](https://user-images.githubusercontent.com/87067133/217298214-68533896-3732-43cf-a92f-67a2b1cc0206.png)

  
  
  - implémentation de la BDD
  
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
