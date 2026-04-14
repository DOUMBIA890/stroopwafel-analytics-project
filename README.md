Projet d’Analyse des Ventes Stroopwafel

📌 Vue d’ensemble

Ce projet est un pipeline de données de bout en bout conçu pour analyser la performance des ventes d’une entreprise de distribution.

Il couvre :

Ingestion des données avec Python
Stockage des données dans PostgreSQL
Transformation des données avec dbt
Visualisation avec Power BI

🏗️ Architecture

Fichiers CSV → Python → PostgreSQL (raw) → dbt (staging & marts) → Dashboard Power BI

🧰 Stack technique
Python (pandas, SQLAlchemy)
PostgreSQL
dbt (transformation des données)
Power BI (visualisation)

📊 Modèle de données
Table de faits : fct_sales
Dimensions :
dim_products
dim_employees
dim_promotions
dim_shifts

📈 Principaux insights
Identification des produits les plus performants
Analyse de l’impact des promotions
Suivi de la performance des employés
Analyse des tendances de ventes dans le temps

🚀 Comment exécuter le projet
pip install -r requirements.txt
python scripts/load_data.py
dbt run
dbt test

⚠️ Variables d’environnement

Créer un fichier .env :

DB_HOST=localhost
DB_PORT=5432
DB_USER=postgres
DB_PASSWORD=your_password
DB_NAME=stroopwafelshop

📌 Auteur

Aboubacar Doumbia

📊 Dashboard Power BI

Le dashboard permet de visualiser les performances des ventes à travers plusieurs KPI :

- Chiffre d’affaires total
- Quantité vendue
- Top produits
- Performance des employés
- Impact des promotions

### Aperçu du dashboard

![Dashboard Power BI](images/dashboard.png)
