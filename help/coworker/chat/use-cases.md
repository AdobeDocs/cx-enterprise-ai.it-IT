---
description: Sfoglia i casi d’uso di Chat con collaboratori e i prompt di esempio, organizzati per area e suddivisi per approfondimenti sui dati, pubblico, percorsi e operazioni sulla piattaforma.
title: Casi d’uso
source-git-commit: 7907ba48f339a6da4f144c0420d31911e03f5050
workflow-type: tm+mt
source-wordcount: '1136'
ht-degree: 3%

---

# Casi d’uso {#use-cases}

Di seguito sono riportati alcuni casi d&#39;uso e alcuni esempi di prompt utilizzati dai professionisti in Adobe CX Enterprise Chat per collaboratori, organizzati per area di lavoro. Ogni prompt viene creato per essere copiato, adattato con i propri dati e contesto e perfezionato attraverso la conversazione.

## Informazioni sui dati

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Rapporti e metriche pull di CJA | Eseguire query su CJA in tempo reale per estrarre metriche, dimensioni, segmenti e visualizzazioni dati | `cja` | Customer Journey Analytics (CJA) | &quot;Mostra visualizzazioni pagina per gli ultimi 30 giorni&quot; · &quot;Elenca i segmenti principali nella visualizzazione dati master&quot; |
| Analisi comparativa | Confrontare le metriche su canali, periodi di tempo o segmenti affiancati | `cja` | Customer Journey Analytics (CJA) | &quot;Confronto dei ricavi per canale, mese e mese&quot; · &quot;Che aspetto ha la conversione da PC desktop a PC portatili questo trimestre?&quot; |
| analisi funnel | Passaggio ai funnel di conversione con più passaggi con drop-off in ogni fase | `cja` | Customer Journey Analytics (CJA) | &quot;Passami attraverso il funnel di pagamento&quot; · &quot;Mostra funnel di conversione da PDP all&#39;acquisto&quot; |
| Previsione | Progetta valori metrici futuri basati su dati storici CJA | `cja` | Customer Journey Analytics (CJA) | &quot;Sessioni di previsione per i prossimi 30 giorni&quot; · &quot;Siamo sulla buona strada per raggiungere il nostro obiettivo di fatturato?&quot; |
| Analisi della causa principale | Ricercare il motivo per cui una metrica è cambiata: diagnosticare gocce, picchi e anomalie | `cja-root-cause-analysis` | Customer Journey Analytics (CJA) | &quot;Perché le conversioni sono calate la settimana scorsa?&quot; · &quot;Cosa ha causato il picco dei ricavi il 15 gennaio?&quot; |
| Riepiloghi esecutivi e digest dei KPI | Creare riepiloghi delle prestazioni pronti per le parti interessate, consigli prescrittivi e descrizioni della presentazione | `cja-executive-summary` | Customer Journey Analytics (CJA) | &quot;Fornisci un riepilogo esecutivo del mese scorso&quot; · &quot;Crea uno schema della presentazione da dati di questo trimestre&quot; |
| Convalida dei dati AA ↔ CJA | Confrontare, controllare e riconciliare i dati tra Adobe Analytics e Customer Journey Analytics | `aa-cja-validation` | ADOBE ANALYTICS + CJA | &quot;Confrontare la suite di rapporti AA con la visualizzazione dati di CJA&quot; · &quot;Convalidare le visualizzazioni di pagina tra AA e CJA&quot; |
| Serie temporali operative e analisi causale | Eseguire query e analizzare dati storici di serie temporali per tipi di pubblico, set di dati e percorsi con attribuzione causale | `operational-stats-causal-analysis` | Tutte le candidature ammissibili | &quot;Mostra le tendenze delle dimensioni del pubblico negli ultimi 90 giorni&quot; · &quot;Perché la riga del set di dati ha conteggiato un picco il 3 marzo?&quot; |
| Creare abilità CJA personalizzate | Trasforma i modelli analitici in competenze riutilizzabili e ripetibili che persistono nelle sessioni | `cja-skill-creator` | Customer Journey Analytics (CJA) | &quot;Trasforma questa analisi settimanale dei ricavi in un’abilità riutilizzabile&quot; · &quot;Salva come abilità per il reporting mensile di funnel&quot; |

## Tipi di pubblico

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Creare tipi di pubblico dal linguaggio naturale | Orchestrare la creazione di tipi di pubblico dettagliati con l’approvazione dell’utente in ogni fase | `audience-creation-flow` | Real-Time CDP (RTCDP) | &quot;Crea un pubblico di utenti che hanno acquistato negli ultimi 30 giorni&quot; · &quot;Crea un segmento per i membri fedeltà di alto valore in California&quot; |
| Creare definizioni di PQL | Assembla le definizioni del pubblico da proprietà XDM, eventi comportamentali o tipi di pubblico esistenti; supporta l’aggregazione e le finestre temporali | `segment-definition-assembly` | Real-Time CDP (RTCDP) | &quot;Crea un PQL per le persone che hanno visualizzato più di 3 prodotti ma non hanno acquistato&quot; · &quot;Aggiungi una finestra temporale di 7 giorni alla condizione dell’evento&quot; |
| Cerca e trova tipi di pubblico | Trova i tipi di pubblico per ID, nome, ricerca semantica; rileva i duplicati e analizza le sovrapposizioni | `audience-search` | Real-Time CDP (RTCDP) | &quot;Trova tutti i tipi di pubblico fidelizzati&quot; · &quot;Esiste un duplicato del segmento &quot;Acquirenti festivi&quot;?&quot; |
| Stimare la dimensione del pubblico | Stimare la portata del profilo per un’espressione PQL utilizzando l’API di anteprima AEP con polling | `audience-size-estimate` | Real-Time CDP (RTCDP) | &quot;Quanto è grande questo pubblico?&quot; · &quot;Stimare la portata di questa espressione PQL&quot; |
| Cascata dimensione pubblico | Scomporre un PQL in sottopredicati e mostrare in che modo ogni condizione contribuisce alla dimensione finale del pubblico | `audience-size-waterfall` | Real-Time CDP (RTCDP) | &quot;Mostrami la cascata per questo PQL&quot; · &quot;Suddividi in che modo ogni condizione riduce il pubblico&quot; |
| Scopri i campi XDM per il targeting | Cerca i campi per nome, descrizione o valore dei dati; scopri dove si trovano e dove sono già utilizzati | `field-discovery` | Real-Time CDP (RTCDP) | &quot;Quali campi posso utilizzare per eseguire il targeting dei clienti fidelizzati?&quot; · &quot;Trova campi relativi alla cronologia acquisti&quot; |
| Pubblicare/salvare tipi di pubblico | Mantenere le definizioni del pubblico in AEP Segmentation Service con convenzioni di denominazione e controlli di conformità | `audience-publish` | Real-Time CDP (RTCDP) | &quot;Salva come bozza&quot; · &quot;Pubblica il pubblico con il nome &quot;Venditori primaverili&quot;&quot; |

## Percorsi

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Creazione di percorsi dal linguaggio naturale | Orchestrare la creazione di percorsi in AJO da un prompt di testo o da un’immagine o un diagramma di flusso caricati | `journey-create` | Adobe Journey Optimizer (AJO) | &quot;Crea un percorso di benvenuto che invia un’e-mail dopo l’iscrizione, attende 3 giorni, quindi invia un follow-up&quot; · &quot;Crea un percorso da questa immagine di diagramma di flusso caricata&quot; |
| Analizzare i conflitti di percorso | Rilevare sovrapposizioni di pubblico, conflitti di pianificazione e problemi di deduplicazione tra percorsi attivi | `journey-analyze-conflict` | Adobe Journey Optimizer (AJO) | &quot;Il mio percorso di abbandono del carrello è in conflitto con altri percorsi?&quot; · &quot;Verificare la sovrapposizione del pubblico tra i miei percorsi attivi&quot; |

## Elementi fondamentali

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Conoscenza del prodotto e documentazione | Rispondi alle domande pratiche, concettuali, sulla risoluzione dei problemi e sulle best practice contenute nei documenti ufficiali di Adobe | `product-knowledge` | Tutte le candidature ammissibili | &quot;Come si imposta una destinazione di streaming?&quot; · &quot;Qual è la differenza tra segmentazione in batch e segmentazione in streaming?&quot; |
| Query di entità AEP/AJO | Funge da punto di ingresso principale per domande sulle entità della piattaforma; passa a KG, all’individuazione dei campi o alle API in base alle esigenze | `operational-insights` | Tutte le candidature ammissibili | &quot;Quanti set di dati ho?&quot; · &quot;Mostra tutti i percorsi attivi&quot; · &quot;Elenca le destinazioni&quot; |
| Query di Knowledge Graph | Conteggi aggregati, join tra entità, ricerche di relazioni ed esplorazione dei metadati tramite singole query SQL | `knowledge-graph` | Tutte le candidature ammissibili | &quot;Quali tipi di pubblico utilizzano questo set di dati?&quot; · &quot;Mostra relazioni tra schemi e set di dati&quot; |
| Operazioni API AEP/AJO/CJA | Fornisci un gateway API diretto per mutazioni, controlli dello stato in tempo reale e tipi di entità non inclusi nel Knowledge Graph | `cxo-api` | Tutte le candidature ammissibili | &quot;Elimina set di dati X&quot; · &quot;Controlla lo stato del processo di acquisizione batch&quot; |
| Risoluzione entità e collegamento | Utilizza la ricerca semantica e lessicale per risolvere le menzioni di entità nelle entità AEP effettive e individuare i campi XDM | `entity-linking` | Adobe Experience Platform (AEP) | &quot;Risolvi &#39;Acquirenti di vacanze&#39; a un pubblico effettivo&quot; · &quot;Trovami campi relativi alla cronologia degli acquisti&quot; |
| Creare un contesto personale | Generare un profilo utente personalizzato dai registri di attività di AEP, CJA e/o Workfront | `build-my-context` | Tutte le candidature ammissibili | &quot;Creare il contesto dall’attività di AEP e CJA&quot; · &quot;Chi sono io in questa organizzazione?&quot; |
| Contesto organizzazione distillata | Estrarre conoscenze a livello di organizzazione da un documento nel wiki di contesto dell&#39;organizzazione condiviso | `distill-org-context` | Tutte le candidature ammissibili | &quot;Distilla questo documento nel wiki dell’organizzazione&quot; · &quot;Aggiungi questo file al contesto dell’organizzazione&quot; |
| Contesto utente Distil | Estrarre il contesto di lavoro personale da un documento nel wiki del contesto utente | `distill-user-context` | Tutte le candidature ammissibili | &quot;Aggiungi questo file al mio contesto utente&quot; · &quot;Estrai il mio contesto di lavoro da questo documento&quot; |
| Gestire le abilità personalizzate | Salva, modifica o elimina le abilità riutilizzabili di proprietà dell&#39;utente che persistono nelle sessioni | `manage-skill` | Tutte le candidature ammissibili | &quot;Salva il flusso di lavoro come un’abilità&quot; · &quot;Elimina l’abilità di reporting settimanale&quot; · &quot;Trasforma questa in un’abilità riutilizzabile&quot; |

## Strumenti sandbox

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Spostare i metadati degli oggetti tra sandbox | Migra facilmente schemi, tipi di pubblico e altre configurazioni di oggetti tra sandbox, con le dipendenze risolte automaticamente | `sandbox-tooling-workflow` | Adobe Experience Platform (AEP) | &quot;Sposta lo schema Luma Loyalty Members Platinum dalla sandbox corrente alla sandbox di produzione&quot; · &quot;Promuovi il pubblico US Gold Loyalty Members allo stage&quot; |
