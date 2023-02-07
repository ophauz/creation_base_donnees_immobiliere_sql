# Création d'une base de données immobilières avec SQL



## Business tasks

Pour le compte d'un réseau d'agences immoblière, création d'un modèle permettant de mieux prévoir le prix de vente des biens immobiliers.

### 1. Création de la base de données permettant de collecter les transactions immobilières et foncières en France.

A partir des données extraites du site open data des [Demandes de valeurs foncières (DVF)](https://www.data.gouv.fr/fr/datasets/demandes-de-valeurs-foncieres/)


#### - Préparation du dictionnaire des données

![p2_dictionnaire](https://user-images.githubusercontent.com/87067133/217299142-3e745df6-d267-47fb-8cb6-091de83f213d.png)


####  - Préparation du modèle conceptuel des données

Les données peuvent être divisées en 3 tables : 
Celle relative au bien immobilier
Celle relative à l’acte notarié
Celle relative à la commune

On utilise Gitmind pour préparer le modèle conceptuel de données, les trois entités, les associations et cardinalités 
 
![p2_modele_conceptuel](https://user-images.githubusercontent.com/87067133/217298814-28f24746-a0ac-4677-8aa2-5d3161771719.png)

  
####  - Préparation du schéma relationnel normalisé en 3NF de la base de données qui donnera lieu à la création des tables

Il faut définir les clés primaires et étrangères
Pour la table bien immobilier, on choisit un identifiant unique auto-incrémenté
Pour acte notarié, on choisit un identifiant unique auto-incrémenté
Pour commune, on choisit la variable « code ID commune »

Les variables ID commune et ID acte notarié seront également les clés étrangères de la table bien immobilier.

On utilise SQL Power Architect pour dessiner le schéma relationnel
  
  ![p2_schema_relationnel](https://user-images.githubusercontent.com/87067133/217298871-dd31c8d8-13f7-43c3-a5c6-2a97ee4b26c3.png)
  

####  - Implémentation de la base de données (sur PostgreSQL)

SQL Power Architect > export du code SQL du schéma relationnel > PGAdmin > Postgres SQL > import des tables en csv 



  
### 2. Requêtes SQL pour aider les différentes agences à mieux accompagner leurs clients.



####  - Nombre de transactions du premier semestre


![p2_req_1](https://user-images.githubusercontent.com/87067133/217304319-1e76bee8-fc24-491f-a50d-9f766add9e31.png)



####  - Répartition des transactions selon le nb de pièces


![p2_req_2](https://user-images.githubusercontent.com/87067133/217304567-be1a31d1-a898-4dc3-95ce-b014fc91f461.png)



####  - 10 départements où le prix du mètre² est le plus haut


![p2_req_3](https://user-images.githubusercontent.com/87067133/217304757-608f320a-3b74-41c2-9de4-826cab8e5fdc.png)



####  - Prix moyen du mètre² d’une maison en IDF


![p2_req_4](https://user-images.githubusercontent.com/87067133/217304846-c3aaf6d7-79f1-4846-b704-c220547d3ae5.png)



####  - Les 10 appartements les plus chers, avec leur département et leur surface


![p2_req_5](https://user-images.githubusercontent.com/87067133/217305459-2c0ccd25-a5ec-4f7a-aff1-a892006e2412.png)



####  - Evolution du nombre de ventes entre le 1er et le 2nd trimestre


![p2_req_6](https://user-images.githubusercontent.com/87067133/217305529-778b9329-305c-4a89-94d3-53e0f7f42e41.png)



####  - Communes où le nombre de transactions a augmenté de 20% ou plus entre le 1er et le 2nd trimestre


![p2_req_7 1](https://user-images.githubusercontent.com/87067133/217306237-00844a46-2dd5-420b-92f0-6b9cb6302f06.png)
![p2_req_7 2](https://user-images.githubusercontent.com/87067133/217306296-fd5cd4ef-94cd-41d1-9b7a-acc835705030.png)
![p2_req_7 3](https://user-images.githubusercontent.com/87067133/217306314-b95cdcc6-17c5-48d4-b2c3-41aa64a1fc1f.png)


####  - Différence (en %) du prix au mètre² entre les appartements de 2 et 3 pièces


![p2_req_8](https://user-images.githubusercontent.com/87067133/217306541-1a01e435-8dde-4864-86b1-a5590e6d4668.png)



####  - La moyenne des valeurs foncières pour les trois meilleures communes des départements 6, 13, 33, 59 et 69


![p2_req_9 1](https://user-images.githubusercontent.com/87067133/217306722-a7bf6851-d6dc-437e-aa5b-df1d1e94d974.png)
![p2_req_9 2](https://user-images.githubusercontent.com/87067133/217306758-0cfc7654-c805-4080-a3bf-b716a5b76260.png)



##### Environnement technique : UML, SQL Power Architect, PostgreSQL, SQL
