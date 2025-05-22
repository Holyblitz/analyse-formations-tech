# analyse-formations-tech
Analyse des formations tech de France à partir des données publiques disponibles (Python, Sql, Power Bi, scrapping)
Cette analyse a pour objectifs de permettre la comparaison entre les centres de formation en France métropolitaine pour des publics différents.

Méthodologie:
1.Scraping Python (BeautyfullSoup) sur Mon compte formation et Trustpilot
2.Nettoyage des données (Sql et Python)
3.Analyse (SQL)
4.Visualisation (power bi)

| Source               | Type d’information                                |
| -------------------- | ------------------------------------------------- |
| Mon Compte Formation | Titre de formation, organisme, localisation, etc. |
| Trustpilot / Google  | Notes des utilisateurs, avis, ambiance, etc.      |
| Autres (en cours)    | Données publiques ou semi-publiques               |

Exemple d'indicateurs produits

    Moyenne des avis par centre de formations (Trustpilot)

    Nombre de formations proposées par technologie (Python, SQL, etc.)

    Estimations de performance (retour à l’emploi, satisfaction)

    Cartographie des offres par région

Travail en cours

Scraping de données sur plusieurs métiers tech

Structuration dans PostgreSQL

Intégration des notes d’organismes

Création de tableaux de bord

Rédaction de cas d'usage concrets pour publication

------------------------------------------------------------------------------------------------------------------------------------------------------

MAJ V.1 achevée
    V.1 complete

# Comparatif des centres de formation tech en France 🇫🇷  
## Tech Training Centers Comparison – France 🇫🇷

## 🎯 Objectif / Goal

Ce projet vise à aider les recruteurs du secteur tech à mieux comprendre le paysage des formations techniques en France.  
This project aims to help tech recruiters better understand the French tech training landscape.

## 🗂️ Sources de données / Data Sources

- **Mon Compte Formation** : pour les informations sur les formations, métiers, technologies, organismes.  
  Mon Compte Formation: to gather training titles, associated jobs, technologies, and institutions.
- **Trustpilot** : pour les avis utilisateurs sur les organismes de formation.  
  Trustpilot: to collect user reviews about training centers.

## 🧹 Traitement des données / Data Processing

- Nettoyage et normalisation des données.  
  Cleaning and normalization of raw data.
- Suppression de la majorité des doublons.  
  Most duplicate entries were removed.
- Création de deux tables principales :  
  Two main tables were built:
  - Avis par organisme / Reviews per training center.
  - Pertinence des technologies par métier / Relevance of technologies per job.

## 📊 Résultats / Results

- Tableau comparatif des avis par organisme.  
  Comparative table of user reviews per training center.
- Classement des technologies enseignées selon leur adéquation métier.  
  Ranking of taught technologies based on job relevance.
- Tableau final : **Top 5 des meilleures formations par métier**.  
  Final table: **Top 5 best trainings per job**.

## ❌ Limites / Limitations

L’absence de données centralisées sur le **taux de retour à l'emploi** nous a empêchés d'intégrer cette dimension.  
Lack of centralized data on **employment return rates** made it impossible to include that metric.

## 🛠️ Technologies utilisées / Technologies Used

- Python (Selenium, BeautifulSoup, Pandas)
- PostgreSQL
- Excel (préparation des données) / for data preparation
- Power BI (visualisation prévue) / planned for data visualization
