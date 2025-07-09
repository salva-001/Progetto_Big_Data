# **Analisi dei Dati di previsione della personalità | introverso estroverso**

Questo progetto analizza un dataset relativo a dati comportamentali e psicologici di diversi individuo, con l'obiettivo di esplorare, pulire e visualizzare i dati per dimostrare che il comportamento sociale (eventi frequentati, tempo passato da solo, post pubblicati...) varia in modo significativo tra introversi ed estroversi, e che certi pattern sociali possono predire la personalità di un individuo.

## **Dati utilizzati**

Il dataset analizzato si chiama **"personality_dataset.csv"** e contiene dati comportamentali e psicologici volti a classificare gli individui come introversi o estroversi

### **Principali colonne del dataset**:

- `Time_spent_Alone`: Tempo medio che un individuo trascorre da solo (in ore).
- `Stage_fear`: Indica se l'individuo sperimenta la paura del palcoscenico.
- `Social_event_attendance`: Numero di eventi sociali partecipati di recente.
- `Going_outside`: Frequenza di uscire per motivi non essenziali.
- `Drained_after_socializing`: Mostra se la persona si sente mentalmente esausta dopo l'interazione sociale.
- `Friends_circle_size`: Conteggio degli amici intimi nella cerchia sociale dell'individuo.
- `Post_frequency`: Frequenza della pubblicazione sui social media.
- `Personalità`: Classificazione della personalità basata sui tratti osservati.

## **Obiettivi del progetto**

1. **Caricamento ed esplorazione dei dati**: verificare la struttura del dataset e individuare eventuali valori mancanti.
2. **Pulizia dei dati**: eliminare colonne non necessarie e gestire i dati nulli.
3. **Analisi statistica**: osservare le principali statistiche descrittive dei dati.
4. **Visualizzazione dei dati**: creare grafici per analizzare distribuzioni e pattern comportmantali sociali.

## **Tecnologie utilizzate**

- **pandas** per la manipolazione e pulizia dei dati
- **numpy** per le operazioni numeriche
- **matplotlib** e **seaborn** per la visualizzazione grafica dei dati
- **scikit-learn** per la modellazione e l'analisi predittiva.


## **Passaggi principali dell'analisi**

1. **Caricamento dei dati**: lettura del file CSV in un DataFrame Pandas.
2. **Pulizia dei dati**:
   - Rimozione di colonne inutili (Stage_fear)
   - Eliminazione di eventuali valori nulli
3. **Esplorazione del dataset**:
   - Utilizzo di `df.info()` e `df.describe()` per analizzare la struttura e le statistiche dei dati
4. **Visualizzazione dei dati**:
   - Creazione di grafici per osservare la distribuzione del tempo passato da soli, della partecipazione agli eventi sociali, del numero degli amici intimi nella cerchia sociale dell'individuo, per la frequenza di uscita per motivi non essenziali, e la frequenza di post pubblicati, con lo scopo di poter visualizzare un patter che mostri come il comportamento sociale varia in modo significativo tra introversi ed estroversi.
5. **Modellazione Predittiva:**
   - Implementazione di modelli di **Regressione Logistica** per dimostrare come certi pattern sociali possono predire la personalità di un individuo.
   **K-means clustering** per per individuare cluster di persone con comportamenti simili.

## **Risultati ottenuti**

Dall'analisi dei dati emergono alcune tendenze chiave:

- Gli introversi mostrano una maggiore tendenza alla **stanchezza dopo interazioni sociali**
- Gli estroversi pubblicano **più frequentemente sui social media**, coerentemente con una “estroversione digitale”.
- Il tempo trascorso in solitudine e il numero di eventi sociali partecipati anche se presi singolarmente sono dei buoni **predittore della personalità**, secondo la regressione logistica.
- I cluster non supervisionati (KMeans) hanno ricostruito gruppi coerenti con i profili psicologici.

## **Conclusioni**

L’analisi ha evidenziato come i comportamenti sociali — dal tempo trascorso da soli alla frequenza delle interazioni, dalla pubblicazione sui social alla risposta emotiva dopo l’interazione, siano fortemente correlati con il profilo di personalità. Gli approcci statistici, cosi come i modelli predittivi applicati hanno permesso di cogliere pattern coerenti con la letteratura psicologica, dimostrando che anche dati quantitativi semplici possono riflettere dinamiche profonde come la gestione dell’energia mentale.

#### **Fonte Dataset**

https://www.kaggle.com/datasets/shalmamuji personality-prediction-data-introvert-extrovert

#### **Versione python utilizzata:**

3.12.7
