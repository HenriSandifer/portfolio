[🇬🇧 **English Version**](../README.md) | [🇮🇹 **Versione Italiana**](./README_IT.md)

# Data Engineer

<div style="display: flex; justify-content: space-between; flex-wrap: wrap;">
  <div style="flex: 1; min-width: 120px; margin-right: 10px;">
    <p>🌍 <strong>Langues parlées</strong> (courant)</p>
    <div class="tags">
      <span class="tag">Anglais</span>
      <span class="tag">Français</span>
      <span class="tag">Italien</span>
    </div>
  </div>
  <div style="flex: 1; min-width: 120px; margin-right: 10px;">
    <p>🧱 <strong>Stack technique</strong></p>
    <div class="tags">
      <span class="tag">Python</span>
      <span class="tag">Pandas</span>
      <span class="tag">SQL</span>
      <span class="tag">AWS S3/ECS</span>
      <span class="tag">Kafka</span>
      <span class="tag">Spark</span>
      <span class="tag">Airflow</span>
      <span class="tag">Snowflake</span>
      <span class="tag">Power BI</span>
      <span class="tag">Streamlit</span>
    </div>
  </div>
  <div style="flex: 1; min-width: 120px;">
    <p>🎯 <strong>Compétences</strong></p>
    <div class="tags">
      <span class="tag">ETL</span>
      <span class="tag">Modélisation des données</span>
      <span class="tag">Qualité des données</span>
      <span class="tag">Enregistrement des erreurs</span>
    </div>
  </div>
</div>

<style>
  .tags {
    margin-top: 8px;
  }
  .tag {
    display: inline-block;
    background-color: #f1f1f1;
    color: #333;
    padding: 4px 8px;
    margin: 2px;
    font-size: 0.85em;
    border-radius: 12px;
    border: 1px solid #ccc;
  }
</style>

<p></p>

---

## 📺 Présentation vidéo

### ⌛ Bientôt disponible

_Problem-solver et ancien microbiologiste/agronome avec un talent pour la construction, la maintenance et l'optimisation des infrastructures de données._

---

## 🎓 Formation

* **RNCP 6, Concepteur Développeur d'Applications**  
  *Bootcamp : Data Scientist (DATAROCKSTARS)*  
  *Certification attendue le 09/2025*  
  *Bootcamp intensif de 400 heures en Data Science*

* **M.S., Agriculture Durable**  
  *Università degli Studi di Padova, Italie - 2022*

* **B.A., Biologie**  
  *Carleton College, États-Unis - 2015*

* **Baccalauréat Français - Économie et Sociologie (Option Internationale)**  
  *EABJM, Paris - 2011*

---

## 📌 Projets

### **🔮 1. Système de prévision de la consommation régionale d'électricité**

![Prediction screenshot](./assets/evaluation.jpeg)

Système complet, **de bout en bout et automatisé** pour la prévision à court terme de la consommation d'électricité dans toutes les régions de France. Pipeline de données **cloud-native** robuste, évolutif et maintenable qui gère le cycle de vie complet des données, de l'acquisition automatisée des données de consommation et de température en temps réel via des API au stockage dans le cloud, à la formation du modèle, à la prévision et à l'évaluation. Le projet aboutit à une **application Streamlit en direct** pour la visualisation interactive des prévisions.

* **Pratiques clés :** **Acquisition automatisée de données à partir d'API externes**, **mise en œuvre d'un data lake dans le cloud (AWS S3)**, **traitement et transformation efficaces des données** (y compris le rééchantillonnage de séries chronologiques et les mises à jour incrémentielles), **conteneurisation avec Docker** et **orchestration automatisée via les services AWS**. Workflow **MLOps** complet, comprenant l'ingénierie des fonctionnalités, la gestion des modèles avec **MLflow**, et une prédiction et une évaluation automatisées à plusieurs niveaux.

* **Stack technique :** **AWS (S3, ECS, EventBridge)**, **Docker**, **Python** (Pandas, Scikit-learn, XGBoost, Boto3, Plotly), **MLflow**, **Streamlit** et **Render**.

### 👉🌐 Voir la **Démo en direct** : [https://predi-elec.onrender.com](https://predi-elec.onrender.com)

[📁 Voir le rapport de projet complet](./pages/project_1.md)

---

### **📊 2. Pipeline ETL & Analyse de la consommation d'énergie industrielle française (EACEI)**

![Dashboard screenshot](./assets/eacei.png)

Ce projet est une **pipeline ETL robuste à plusieurs étapes** conçue pour ingérer, nettoyer et structurer **164 fichiers de données brutes très hétérogènes** (XLS, XLSX) sur la consommation d'énergie industrielle française de 2010 à 2023. L'objectif principal était de transformer cet ensemble de données complexes en une **base de données en schéma en étoile** propre, unifiée et prête pour l'analyse, qui a ensuite servi de base à un **tableau de bord Power BI interactif** pour analyser les tendances énergétiques.

* **Pratiques clés :** Ce projet met en avant une **gestion avancée de la qualité des données** (gestion de formats de fichiers variés, standardisation de dimensions diverses comme les secteurs d'activité, les régions et la taille des entreprises, et traitement des données masquées), **la modélisation des données avec un schéma en étoile**, **la modularité**, **la configuration sous forme de code (JSON)** et une **gestion robuste des erreurs** tout au long du processus ETL.

* **Stack technique :** **Python**, **Pandas**, **JSON**, sorties CSV et **Microsoft Power BI**.

### 👉🌐 Voir le **Tableau de bord en direct** : [Tableau de bord Power BI](https://app.powerbi.com/view?r=eyJrIjoiZTE4YjVhMjctZjFmZS00YjRjLThlOTctNDAyOGI0ZTNiNGNiIiwidCI6ImJlOTNmMTc4LTA5NjQtNDcwOS1hMDZjLTY4ZThhZjBhODM1NSJ9&pageName=f779d68dcac6fc795d20)

[📁 Voir le rapport de projet complet](./pages/project_2.md)

---

### **💻 3. Plateforme d'analyse en temps réel pour l'e-commerce (en cours)**

Ce projet **en cours**, axé sur les concepts du **Big Data**, simule une plateforme d'analyse de bout en bout pour l'e-commerce, traitant à la fois les événements d'interaction des utilisateurs par lots et en streaming, les stockant dans un data lake, les chargeant dans un data warehouse et les transformant pour l'analyse. La plateforme met l'accent sur **l'évolutivité**, **la qualité des données**, **la gestion des erreurs** et **la résilience en conditions réelles**.

* **Pratiques clés :** Le projet amplifie les aspects **Big Data** par la simulation de volume/vélocité, le partitionnement et le streaming. Il intègre des **contrôles de qualité des données robustes (Great Expectations)**, une **gestion et une surveillance améliorées des erreurs**, **l'idempotence**, **l'évolution du schéma** et une **couche simple de requêtes/services** pour une complétude de bout en bout. Il inclut également les bases du **CI/CD** et une **démonstration de l'évolutivité** pour présenter des pratiques d'ingénierie réfléchies.

* **Stack technique :** **Kafka**, **Spark**, **Airflow**, **Snowflake**, **PostgreSQL**, **DBT**, **Great Expectations**, **S3**, **Docker**, **FastAPI** et **GitHub Actions**.

[📁 Voir la documentation du projet en cours](./pages/project_3.md)

---

## 🧰 Expérience professionnelle

### **Ingénieur de Projets Agronomiques - Agrivoltaïsme**

*SOLVEO Energies (développeur d'énergies renouvelables) - Toulouse*  
*Juillet 2024 - Janvier 2025*

- Interface agronomique pour les équipes de développement sur le terrain : réalisation de diagnostics d'exploitation et rédaction de notes techniques d'aide à la décision
- Rédaction des spécifications fonctionnelles pour le développement du logiciel de gestion agrivoltaïque de l'entreprise
- Création d'une base de données de référence sur les besoins en lumière de 17 cultures, basée sur une synthèse de plus de 70 articles scientifiques

### **Ingénieur d'Affaires**

*MYCOPHYTO SAS (startup de la French Tech) - Grasse (PACA)*  
*Août 2023 - Novembre 2023*

- Gestion de la relation client de la prospection au déploiement sur le terrain : présentations techniques, propositions commerciales et suivi agronomique (échantillonnage, production de rapports)
- Amélioration des outils d'aide à la vente et de reporting : refonte de l'outil de tarification (formules Excel avancées) et développement d'un outil de visualisation cartographique (QGIS) pour les livrables clients

### **Gérant de comptes / Propriétaire**

*Domaine La Tourbeille // Taverne du Belvédère - Région de Bordeaux*  
*2017 - 2023*

- Ventes B2B, gestion budgétaire, stratégie commerciale
- Gestion des opérations de restauration
- Mise en place de pratiques agroécologiques dans le vignoble
