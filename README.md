🏥 Système Décisionnel de Santé (Healthcare BI Project)
Ce projet consiste en la conception et la mise en œuvre d'une solution décisionnelle complète dédiée au secteur de la santé. Il permet de centraliser, nettoyer, transformer et analyser des volumes importants de données hétérogènes (admissions, facturations, patients, hôpitaux, médecins) afin d'améliorer la prise de décision stratégique et opérationnelle.

🏗️ Architecture du Projet & Pipeline ETL
Le pipeline de données repose sur les étapes clés suivantes :
1.Sources de Données : Fichiers plats et sources hétérogènes (données relatives aux patients, services cliniques et établissements de santé).
2.Extraction, Transformation et Chargement (ETL) : Développé sous Talend Open Studio, incluant :
Le nettoyage, le filtrage et la déduplication (tUniqRow, tMap).
La gestion et l'alimentation des dimensions (Dim_Patient, Dim_Hospital, Dim_Doctor, Dim_ClinicalService, Dim_AdmissionInfo, Dim_DateAdmission, Dim_DateDischarge).
Le chargement des tables de faits (Fact_Admission, Fact_Billing).
3.Data Warehouse : Stockage des données modélisé selon un modèle en constellation (Star/Constellation Schema) sous une base de données MySQL.
4.Restitution & Reporting : Tableaux de bord interactifs et dynamiques développés sous Power BI.

📊 Structure du Dépôt

Le dossier du projet contient les éléments suivants :
  A.Jobs Talend (.item, .properties) :
importationData & NettoyageETL : Traitement initial, intégration et nettoyage des flux de données.
Dim_* : Jobs d'alimentation des différentes dimensions du Data Warehouse.
Fact_Admission & FactBilling : Jobs de chargement des tables de faits.
  B.Modélisation & Conception : Schémas du modèle en constellation.
  C.Documentation : Présentation globale de la démarche méthodologique (ex. alignement des besoins métiers avec la BI).

🛠️ Technologies Utilisées
-ETL (Integration) : Talend Open Studio for Data Integration
-Base de Données / DW : MySQL (Modélisation dimensionnelle en constellation)
-Visualisation / Business Intelligence : Power BI (Dashboards de facturation et d'admissions)
-Méthodologie : Approche décisionnelle structurée (analyse des besoins, conception, ETL, restitution)

🚀 Fonctionnalités des Tableaux de Bord Power BI
-Dashboard Fact Billing (Facturation) : Analyse du chiffre d'affaires, suivi du montant total de facturation par mois, par hôpital (Top 5), par médicament et par médecin (Top 10).
-Dashboard Fact Admission (Admissions) : Suivi analytique des admissions par année, par genre, par type d'établissement et analyse approfondie des durées de séjour (LongStay) des patients.

👤 Auteur
Projet réalisé par Maram Ben Kilani

Système Décisionnel de Santé - Projet Académique / Ingénierie des données
