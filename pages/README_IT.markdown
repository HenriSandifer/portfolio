[🇬🇧 **English Version**](../README.md) | [🇫🇷 **Version française**](README_FR.markdown)

# Data Engineer

<div style="display: flex; justify-content: space-between; flex-wrap: wrap;">
  <div style="flex: 1; min-width: 120px; margin-right: 10px;">
    <p>🌍 <strong>Lingue parlate</strong> (fluente)</p>
    <div class="tags">
      <span class="tag">Inglese</span>
      <span class="tag">Francese</span>
      <span class="tag">Italiano</span>
    </div>
  </div>
  <div style="flex: 1; min-width: 120px; margin-right: 10px;">
    <p>🧱 <strong>Stack tecnologico</strong></p>
    <div class="tags">
      <span class="tag">Python</span>
      <span class="tag">Pandas</span>
      <span class="tag">SQL</span>
      <span class="tag">AWS S3/ECS</span>
      <span class="tag">Power BI</span>
      <span class="tag">Streamlit</span>
    </div>
  </div>
  <div style="flex: 1; min-width: 120px;">
    <p>🎯 <strong>Competenze</strong></p>
    <div class="tags">
      <span class="tag">ETL</span>
      <span class="tag">Modellazione dei dati</span>
      <span class="tag">Qualità dei dati</span>
      <span class="tag">Registrazione degli errori</span>
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

## 📺 Presentazione video

⌛ **_Prossimamente_**

_Problem-solver ed ex-microbiologo/agronomo con un'attitudine per la costruzione, manutenzione e ottimizzazione delle infrastrutture dati._

---

## 🎓 Istruzione

* **RNCP 6, Concepteur Développeur d'Applications**  
  *Bootcamp: Data Scientist (DATAROCKSTARS)*  
  *Certificazione prevista per 09/2025*  
  *Bootcamp intensivo di 400 ore in Data Science*

* **M.S., Agricoltura Sostenibile**  
  *Università degli Studi di Padova, Italia - 2022*

* **B.A., Biologia**  
  *Carleton College, USA - 2015*

* **Baccalauréat Francese - Economia e Sociologia (Opzione Internazionale)**  
  *EABJM, Parigi - 2011*

---

## 📌 Progetti

### **🔮 1. Sistema di previsione del consumo elettrico regionale**

![Prediction screenshot](../assets/evaluation.jpeg)

Sistema completo, **end-to-end e automatizzato** per la previsione a breve termine del consumo di elettricità in tutte le regioni della Francia. Pipeline di dati **cloud-native** robusta, scalabile e manutenibile che gestisce l'intero ciclo di vita dei dati, dall'acquisizione automatizzata dei dati di consumo e temperatura in tempo reale tramite API allo storage su cloud, all'addestramento del modello, alla previsione e alla valutazione. Il progetto culmina in un'**applicazione Streamlit live** per la visualizzazione interattiva delle previsioni.

* **Pratiche chiave:** **Acquisizione automatizzata di dati da API esterne**, **implementazione di un data lake su cloud (AWS S3)**, **elaborazione e trasformazione efficiente dei dati** (incluso il ricampionamento di serie storiche e aggiornamenti incrementali), **containerizzazione con Docker** e **orchestrazione automatizzata tramite i servizi AWS**. Flusso di lavoro **MLOps** completo, che include feature engineering, gestione dei modelli con **MLflow** e previsione e valutazione automatizzate a più livelli.

* **Stack tecnologico:** **AWS (S3, ECS, EventBridge)**, **Docker**, **Python** (Pandas, Scikit-learn, XGBoost, Boto3, Plotly), **MLflow**, **Streamlit** e **Render**.

### 👉🌐 Visualizza la **Demo Live**: [https://predi-elec.onrender.com](https://predi-elec.onrender.com)

### 👉📖 Visualizza il **Report di Proggetto Completo** (+ video) : [Report di Proggetto Completo](Predi_Elec_IT.md)

---

### **📊 2. Pipeline ETL e analisi del consumo energetico industriale francese (EACEI)**

![Dashboard screenshot](../assets/eacei.png)

Questo progetto consiste in una **pipeline ETL robusta e multi-stadio** progettata per ingerire, pulire e strutturare **164 file di dati grezzi altamente eterogenei** (XLS, XLSX) sul consumo energetico industriale francese dal 2010 al 2023. L'obiettivo principale era trasformare questo complesso set di dati in un **database con schema a stella** pulito, unificato e pronto per l'analisi, che è poi servito come base per una **dashboard interattiva di Power BI** per analizzare le tendenze energetiche.

* **Pratiche chiave:** Questo progetto mette in mostra una **gestione avanzata della qualità dei dati** (gestione di formati di file variabili, standardizzazione di dimensioni diverse come settori di attività, regioni e dimensioni delle aziende, e gestione dei dati soppressi), **modellazione dei dati con uno schema a stella**, **modularità**, **configurazione come codice (JSON)** e una **gestione robusta degli errori** durante tutto il processo ETL.

* **Stack tecnologico:** **Python**, **Pandas**, **JSON**, output CSV e **Microsoft Power BI**.

### 👉🌐 Visualizza la **Dashboard Live**: [Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiZTE4YjVhMjctZjFmZS00YjRjLThlOTctNDAyOGI0ZTNiNGNiIiwidCI6ImJlOTNmMTc4LTA5NjQtNDcwOS1hMDZjLTY4ZThhZjBhODM1NSJ9&pageName=f779d68dcac6fc795d20)

### 👉📖 Visualizza il **Report di Proggetto Completo** (+ video) : [Report di Proggetto Completo](EACEI_IT.md)

---

### **💻 3. Piattaforma di analisi in tempo reale per l'e-commerce (in corso)**

Questo progetto **in corso**, incentrato sui concetti di **Big Data**, simula una piattaforma di analisi e-commerce end-to-end, elaborando eventi di interazione degli utenti sia in batch che in streaming, archiviandoli in un data lake, caricandoli in un data warehouse e trasformandoli per l'analisi. La piattaforma pone l'accento su **scalabilità**, **qualità dei dati**, **gestione degli errori** e **resilienza in condizioni reali**.

* **Pratiche chiave:** Il progetto amplifica gli aspetti **Big Data** attraverso la simulazione di volume/velocità, il partizionamento e lo streaming. Incorpora **robusti controlli di qualità dei dati (Great Expectations)**, una **gestione e monitoraggio degli errori migliorati**, **idempotenza**, **evoluzione dello schema** e un **semplice livello di interrogazione/servizio** per una completezza end-to-end. Include anche le basi di **CI/CD** e una **dimostrazione di scalabilità** per mostrare pratiche di ingegneria ponderate.

* **Stack tecnologico:** **Kafka**, **Spark**, **Airflow**, **Snowflake**, **PostgreSQL**, **DBT**, **Great Expectations**, **S3**, **Docker**, **FastAPI** e **GitHub Actions**.

### 👉📝 Visualizza la Documentazione del Proggetto in Corso : [Documentazione del Proggetto](E_commerce_IT.md)

---

## 🧰 Esperienza professionale

### **Ingegnere di Progetti Agronomici - Agrivoltaico**

*SOLVEO Energies (sviluppatore di energie rinnovabili) - Tolosa*  
*Luglio 2024 - Gennaio 2025*

- Interfaccia agronomica per i team di sviluppo sul campo: conduzione di diagnosi aziendali e redazione di note tecniche di supporto decisionale
- Redazione delle specifiche funzionali per lo sviluppo del software di gestione agrivoltaica dell'azienda
- Creazione di un database di riferimento sui fabbisogni di luce per 17 colture, basato su una sintesi di oltre 70 articoli scientifici

### **Business Engineer**

*MYCOPHYTO SAS (startup French Tech) - Grasse (PACA)*  
*Agosto 2023 - Novembre 2023*

- Gestione delle relazioni con i clienti dalla prospezione all'implementazione sul campo: presentazioni tecniche, proposte commerciali e monitoraggio agronomico (campionamento, produzione di report)
- Miglioramento degli strumenti di supporto alle vendite e di reporting: riprogettazione dello strumento di pricing (formule Excel avanzate) e sviluppo di uno strumento di visualizzazione cartografica (QGIS) per i deliverable ai clienti

### **Account Manager / Proprietario**

*Domaine La Tourbeille // Taverne du Belvédère - Regione di Bordeaux*  
*2017 - 2023*

- Vendite B2B, gestione del budget, strategia commerciale
- Gestione delle operazioni di ristorazione
- Implementazione di pratiche agroecologiche nel vigneto
