---
description: Sfoglia i casi d’uso di Chat con collaboratori e i prompt di esempio, organizzati per area e suddivisi per approfondimenti sui dati, pubblico, percorsi e operazioni sulla piattaforma.
title: Casi di utilizzo della chat del collaboratore
feature_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 261f478d3dec0845c0a5532201ef6ddc81808372
workflow-type: tm+mt
source-wordcount: 3729
ht-degree: 6%

---

# Casi d’uso di Chat con i collaboratori{#use-cases}

Chat con collaboratori consente di eseguire query, analizzare e agire sui dati di [!DNL Experience Platform] utilizzando il linguaggio naturale anziché navigare in più interfacce utente o scrivere query manualmente. Questa pagina cataloga i casi d’uso su cui i professionisti si basano maggiormente, organizzati per area di lavoro: approfondimenti sui dati, tipi di pubblico, percorsi, elementi fondamentali e strumenti sandbox. Ogni voce include l&#39;abilità richiamata, le applicazioni con cui lavora e i prompt di esempio che è possibile copiare, adattare ai propri dati e perfezionare attraverso la conversazione.

>[!NOTE]
>
>In arrivo:
>
>Nuove funzionalità per gli agenti di AEM tramite CX Enterprise Collaborator, progettate per consentire di ottenere di più e più rapidamente.
>
>Tutti i clienti idonei avranno accesso alle funzionalità di agenti Adobe Experience Manager in Coworker, su base continua.
>
>Vedi anche [IA in AEM - Panoramica delle funzionalità agente in AEM](https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/overview).

## Esperienza del marchio

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Aggiornare le pagine di AEM | Esegui azioni quali aggiornamento, rimozione, sostituzione o aggiunta di elementi di contenuto per mantenere le esperienze accurate e correnti. Gli input possono essere annotazioni visive o del linguaggio naturale, ad esempio PDF o screenshot. | `aem-sites-pages-update` | Adobe Experience Manager (AEM) - AEM Sites | Il &lt;URL> aggiorna il titolo a Hello World<br><br>on &lt;URL> cambia il pulsante &quot;Take our Coffee Quiz&quot; (Acquista il quiz sul caffè) in una versione più coinvolgente<br><br>Aggiorna &lt;URL> in base al &lt;URL> allegato<br><br>on. Desidero aggiungere una nuova sezione teaser in fondo alla pagina su una promozione in esecuzione nel mese di agosto: acquistare una macchina da caffè e ottenere 2 sacchi di caffè gratis. Trovi anche l&#39;immagine di amici che bevono caffè e usarlo nel teaser |
| Aggiornare AEM in blocco | Esegui azioni in blocco su più pagine contemporaneamente, ad esempio rimuovi, sostituisci o aggiungi elementi di contenuto per mantenere le esperienze accurate e correnti. | `aem-sites-pages-bulkreplace` | Adobe Experience Manager (AEM) - AEM Sites | in &lt;aem path> aggiorna tutte le pagine che contengono la copia &quot;MyBarista\&quot; in &quot;BrewPass&quot; |
| Passare da Figma a frammento di contenuto visivo | Importare i disegni direttamente da Figma in Adobe Experience Manager utilizzando il linguaggio naturale. L’abilità crea automaticamente il modello di contenuto, il frammento di contenuto, le risorse e il modello di visualizzazione richiesti, consentendo agli utenti aziendali di passare in pochi minuti dalla progettazione ai contenuti pronti per il web senza dover eseguire la configurazione manuale. | `aem-sites-visualcontentfragments-create` | Adobe Experience Manager (AEM) - AEM Sites | Importa da &lt;Figma_URL> |

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Crea modulo | Generare un nuovo modulo adattivo da una descrizione in linguaggio semplice, una descrizione allegata, un’immagine o un PDF | `aem-forms-adaptiveform-create` | Adobe Experience Manager (AEM) - AEM Forms | &quot;Creare un modulo di onboarding per dipendenti&quot;<br><br>&quot;Creare un modulo utilizzando la descrizione allegata (immagine o pdf)&quot;<br><br>&quot;Creare un &lt;tipo di modulo> modulo adattivo&quot; |
| Modifica/aggiorna modulo | Modificare un modulo esistente: aggiungere/modificare campi, modificare un layout semplice, configurare azioni di invio o applicare modifiche da un documento di linee guida allegato | `aem-forms-adaptiveform-edit` | Adobe Experience Manager (AEM) - AEM Forms | &quot;Aggiungi campo Secondo nome sotto campo Nome&quot;<br><br>&quot;Inserisci campi Nome e Cognome in un layout a 2 colonne, 50/50&quot;<br><br>&quot;Configura il modulo per inviare dati a un endpoint REST&quot;<br><br>&quot;Aggiorna il modulo in modo che corrisponda al documento delle linee guida allegato&quot;<br><br>&quot;Aggiungi campo &lt;nome campo> sotto &lt;campo esistente>&quot; |
| Aggiungi logica di business | Creare regole semplici, ad esempio mostrare o nascondere un campo in base al valore di un altro campo | `aem-forms-adaptiveform-edit` | Adobe Experience Manager (AEM) - AEM Forms | &quot;Mostra il campo Società solo quando il tipo di dipendente è Contraente&quot;<br><br>&quot;Mostra il campo &lt;campo> solo quando &lt;altro campo> è &lt;valore>&quot; |
| Incorpora modulo | Inserire un modulo esistente o appena creato in una pagina AEM Sites designata (supportata solo nelle pagine Edge Delivery Services) | `aem-forms-adaptiveform-embed` | Adobe Experience Manager (AEM) - AEM Forms | &quot;Incorpora il modulo nella home page del sito&quot;<br><br>&quot;Incorpora il modulo in &lt;percorso pagina>&quot; |

**Informazioni correlate**

* [Funzionalità Agentic in AEM: Esperienza del marchio - Produzione di esperienze - Sites](https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/experience-production/use-cases#use-cases-sites)

* [Funzionalità Agentic in AEM: Esperienza del marchio - Produzione di esperienze - Forms](https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/experience-production/use-cases#use-cases-forms)

### Sviluppo

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Gestire le pipeline di Cloud Manager | Creare, eseguire e monitorare le pipeline di AEM Cloud Manager, inclusi registri, artefatti, variabili e impostazioni | `cloud-manager-pipeline-management` | Adobe Experience Manager (AEM) | &quot;Elencare le pipeline per il programma 12345&quot;<br><br>&quot;Qual è lo stato della pipeline più recente?&quot; |
| Gestire gli ambienti Cloud Manager | Creazione, configurazione e manutenzione di ambienti AEM Cloud Manager, inclusi RDE, variabili di ambiente, registri e backup | `cloud-manager-environment-management` | Adobe Experience Manager (AEM) | &quot;Elencare gli ambienti personali per il programma 12345&quot;<br><br>&quot;Reimpostare il codice RDE&quot; |
| Gestire i programmi Cloud Manager | Elencare, ispezionare ed eliminare programmi AEM Cloud Manager, incluse pipeline e ambienti | `cloud-manager-program-management` | Adobe Experience Manager (AEM) | &quot;Elenca i miei programmi Cloud Manager&quot;<br><br>&quot;Ottieni dettagli per 12345 programma&quot; |
| Gestire le pianificazioni degli aggiornamenti delle versioni di AEM | Configura le ore di pausa giornaliere e i periodi di disponibilità dell&#39;aggiornamento per la manutenzione automatica e visualizza le finestre di blocco del codice globali di Adobe | `cloud-manager-release-management` | Adobe Experience Manager (AEM) | &quot;Qual è la finestra delle ore non interattive corrente?&quot;<br><br>&quot;Pianificazione di un periodo senza aggiornamento dal 20 dicembre al 2 gennaio&quot; |

**Informazioni correlate**

* [Funzionalità Agentic in AEM: Esperienza del marchio - Sviluppo](https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/development/use-cases)

### Formazione iniziale

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Onboarding end-to-end guidato | Orchestrazione dell’intero ciclo di vita di onboarding, selezione dell’archivio, delega alla cartella, tag, metadati, importazione e ricerca di sottocompetenze, se non conosci l’attività di onboarding specifica necessaria. | `aem-onboarding-workflow` | Adobe Experience Manager (AEM) - AEM Assets | &quot;Eseguire l&#39;onboarding del team in AEM Assets&quot;<br><br>&quot;Passare all&#39;onboarding di AEM DAM&quot; |
| Progettare e creare gerarchie di cartelle | Consiglia e crea strutture di cartelle scalabili in AEM Assets (in `/content/dam`) in base alle esigenze aziendali o agli input CSV. | `aem-folder-management` | Adobe Experience Manager (AEM) - AEM Assets | &quot;Consigliare una struttura di cartelle per le risorse di marketing lifestyle&quot;<br><br>&quot;Creare cartelle in base a questo file CSV&quot; |
| Progettare e creare tag | Progetta e crea vocabolari di tag controllati in `/content/cq:tags`, spazi dei nomi, tag gerarchici e operazioni batch tag. | `aem-tag-taxonomy` | Adobe Experience Manager (AEM) - AEM Assets | &quot;Progettare una tassonomia dei tag con spazi dei nomi per le categorie di prodotti &quot;<br><br>&quot;Importare tag da questo CSV&quot;<br><br>&quot;Creare questi tag gerarchici in AEM&quot; |
| Creare e assegnare moduli di metadati | Progetta e crea moduli di metadati personalizzati, utilizzati dagli autori di contenuti dell’interfaccia utente di creazione, da un CSV, una tabella, un documento sui requisiti o una descrizione, e facoltativamente li assegna alle cartelle. | `aem-metadata-form` | Adobe Experience Manager (AEM) - AEM Assets | &quot;Creare un modulo metadati da questo elenco di campi&quot;<br><br>&quot;Assegnare il modulo alla cartella `campaigns`&quot; |

**Informazioni correlate**

* [Funzionalità di Agentic in AEM: Esperienza del marchio - Onboarding](https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/onboarding/use-cases)

## Contenuto verificato

### Individuazione dei contenuti

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Ricerca per tema semantico | Trova le risorse per concetto, umore o tema visivo utilizzando la corrispondenza semantica basata sull’intelligenza artificiale. | `aem-assets-discovery` | Adobe Experience Manager (AEM) - AEM Assets | &quot;Trovami immagini di vita del caffè mattutino&quot; |
| Ricerca per metadati personalizzati | Filtra le risorse in base ai campi di metadati personalizzati (ad esempio, Coffee Blend, Brand, Roast Level). | `aem-assets-discovery` | Adobe Experience Manager (AEM) - AEM Assets | &quot;Trova risorse in cui `Coffee Blend` è `Morning Muse`&quot;<br><br>&quot;Ottieni risorse la cui licenza non è scaduta&quot;<br><br>&quot;Trova risorse il cui nome campagna non è impostato (la proprietà deve essere indicizzata per ottenere risultati appropriati).&quot; |
| Cerca per stato di approvazione | Filtra le risorse in base allo stato di approvazione. Ad esempio, stato approvato, in revisione, rifiutato o mancante. | `aem-assets-discovery` | Adobe Experience Manager (AEM) - AEM Assets | &quot;Mostra tutte le risorse approvate nella cartella `Campaign`&quot; |
| Cerca per cartella/percorso | Per identificare le risorse, interpreta i prompt del linguaggio naturale che fanno riferimento ai nomi delle cartelle in AEM. Puoi semplicemente menzionare la cartella nel loro prompt, senza navigare manualmente nell’archivio, riducendo in modo significativo il numero di clic necessari per individuare il contenuto corretto. | `aem-assets-discovery` | Adobe Experience Manager (AEM) - AEM Assets | &quot;Nella cartella `WKND`&quot;?<br><br>&quot;Mostra le risorse modificate dopo l&#39;1 novembre 2025 nella cartella `WKND`&quot; |

**Informazioni correlate**

* [Funzionalità Agentic in AEM: Contenuto verificato - Individuazione dei contenuti](https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/content-advisor/discovery/use-cases)

### Ottimizzazione dei contenuti

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Creazione di rendering ad alta risoluzione e rendering ottimizzati per il canale | Genera nuove rappresentazioni di una risorsa a una risoluzione e a un livello di qualità specifici, semplificando la preparazione di varianti pronte per il canale senza modifiche manuali. Puoi anche produrre rappresentazioni personalizzate in base ai requisiti specifici della piattaforma, come ad esempio Instagram Stories, garantendo che le risorse soddisfino automaticamente il formato, il rapporto di trasmissione e le linee guida sulla qualità. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) - AEM Assets | &quot;Crea una rappresentazione `2000px` come `JPEG` con `80% quality`&quot;<br><br>&quot;Crea una rappresentazione per una storia Instagram&quot; |
| Sovrapposizioni con marchio e generazione composita | Applica grafici promozionali, sovrapposizioni o badge alle risorse esistenti con un posizionamento preciso, per supportare la creazione rapida di composizioni pronte per la campagna. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) - AEM Assets | &quot;Sovrapponi l&#39;immagine con gli elementi grafici dello sconto `30%` sul banner promozionale, posizionandolo `100px` dal centro&quot; |
| Miglioramenti alle immagini, regolazioni del colore di sfondo, trasformazioni di orientamento | Applica miglioramenti visivi (nitidezza delle immagini), sostituisci i colori di sfondo ed esegui trasformazioni di orientamento. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) - AEM Assets | &quot;Cambia il colore di sfondo di `PNG` in `#ff8932`&quot;<br><br>&quot;Contrasta l&#39;immagine&quot;<br><br>&quot;Specchia l&#39;immagine orizzontalmente&quot; |

**Informazioni correlate**

* [Funzionalità Agentic in AEM: Contenuto verificato - Ottimizzazione dei contenuti](https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/content-advisor/content-optimization/use-cases)

## Governance del brand

| Caso d&#39;uso | Descrizione | Competenza | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Linee guida e ricerca dei segmenti | Recuperare le linee guida dettagliate del brand, definite per segmento, mercato o categoria | enterprise-context | Adobe Experience Manager (AEM) | &quot;Quali sono le linee guida per il tono di voce per questo marchio?&quot;<br>&quot;Elencare le categorie di attestazioni utilizzate nel settore verticale dell&#39;integrità&quot; |
| Valutare i contenuti in base alle linee guida del brand | Valutare una pagina, un blocco di testo o un’immagine pubblicati/creati in base ai controlli del marchio configurati | aem-governance | Adobe Experience Manager (AEM) | &quot;Valutare questa pagina di destinazione in base alle linee guida di SecurBank&quot;<br>&quot;Questa tagline supera i controlli del tono di voce?&quot; |
| Eseguire il debug delle autorizzazioni di AEM | Eseguire il debug/comprendere i criteri di autorizzazione, gli ACL e le regole di ereditarietà. | aem-governance | Adobe Experience Manager (AEM) | &quot;Perché l&#39;amministratore dell&#39;entità può scrivere `/content/folder/us` su `https://author/` ?&quot;<br>&quot;Perché non è possibile scrivere l&#39;autore campione in `/content/dam` su `https://author`&quot; |

**Informazioni correlate**

* [Funzionalità Agentic in AEM: Governance del brand](https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-governance/use-cases)

## Informazioni sui dati

| Caso d&#39;uso | Descrizione | Competenza | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| [Recuperare i report e le metriche di CJA](data-insights/analytics-chat.md) | Eseguire query su CJA in tempo reale per estrarre metriche, dimensioni, segmenti e visualizzazioni dati | `cja` | Customer Journey Analytics (CJA) | &quot;Mostra visualizzazioni pagina per gli ultimi 30 giorni&quot; <br> &quot;Elenca segmenti principali nella visualizzazione dati master&quot; |
| Analisi comparativa | Confrontare le metriche su canali, periodi di tempo o segmenti affiancati | `cja-root-cause-analysis`, `cja`, `dx-api`, `knowledge-graph` | Customer Journey Analytics (CJA) | &quot;Confrontare i ricavi per canale, mese e mese&quot; <br> &quot;Come si presenta la conversione da PC portatile a desktop in questo trimestre?&quot; |
| Prestazioni della campagna | Misura il modo in cui le campagne, i canali e le proprietà web vengono eseguiti in un determinato periodo di tempo. | `cja`, `dx-api`, `knowledge-graph` | | &quot;Quali sono state le prestazioni delle campagne web di Acrobat il mese scorso?&quot; |
| analisi funnel | Passaggio ai funnel di conversione con più passaggi con drop-off in ogni fase | `cja` | Customer Journey Analytics (CJA) | &quot;Visualizza il funnel di pagamento&quot; <br> &quot;Mostra funnel di conversione da PDP all&#39;acquisto&quot; |
| Previsione | Progetta valori metrici futuri basati su dati storici CJA | `cja` | Customer Journey Analytics (CJA) | &quot;Sessioni di previsione per i prossimi 30 giorni&quot; <br> &quot;Siamo sulla buona strada per raggiungere il nostro obiettivo di fatturato?&quot; |
| [Analisi causa principale](data-insights/root-cause-analysis.md) | Ricercare il motivo per cui una metrica è cambiata: diagnosticare gocce, picchi e anomalie | `cja-root-cause-analysis` | Customer Journey Analytics (CJA) | &quot;Perché le conversioni sono diminuite la settimana scorsa?&quot; <br> &quot;Cosa ha causato il picco delle entrate il 15 gennaio?&quot; |
| Riepiloghi esecutivi e digest dei KPI | Creare riepiloghi delle prestazioni pronti per le parti interessate, consigli prescrittivi e descrizioni della presentazione | `cja-executive-summary`, `cja-bacom-anomaly-tracker-v2`, `cja-cno-weekly-pulse`, `cja-reporting`, `cja`, `dx-api` | Customer Journey Analytics (CJA) | &quot;Assegnami un riepilogo esecutivo del mese scorso&quot; <br> &quot;Creare una struttura della presentazione di diapositive dai dati di questo trimestre&quot; |
| [AA ↔ convalida dati CJA](data-insights/data-validation-aa-cja.md) | Confrontare, controllare e riconciliare i dati tra Adobe Analytics e Customer Journey Analytics, in particolare durante l’aggiornamento da Adobe Analytics a Customer Journey Analytics | `aa-cja-validation`, `cja`, `dx-api` | ADOBE ANALYTICS + CJA | &quot;Confronta la suite di rapporti AA con la visualizzazione dati di CJA&quot; <br> &quot;Convalida le visualizzazioni di pagina tra AA e CJA&quot; |
| Serie temporali operative e analisi causale | Eseguire query e analizzare dati storici di serie temporali per tipi di pubblico, set di dati e percorsi con attribuzione causale | `operational-stats-causal-analysis` | Tutte le candidature ammissibili | &quot;Mostra tendenze dimensioni pubblico negli ultimi 90 giorni&quot; <br> &quot;Perché la riga del set di dati ha conteggiato un picco il 3 marzo?&quot; |
| Creare abilità CJA personalizzate | Trasforma i modelli analitici in competenze riutilizzabili e ripetibili che persistono nelle sessioni | `cja-skill-creator` | Customer Journey Analytics (CJA) | &quot;Trasforma questa analisi settimanale dei ricavi in un&#39;abilità riutilizzabile&quot; <br> &quot;Salva come abilità per il reporting mensile di funnel&quot; |

## Tipi di pubblico

| Caso d&#39;uso | Descrizione | Competenza | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| [Crea tipi di pubblico dal linguaggio naturale](audiences/create-audience-from-natural-language.md) | Orchestrare la creazione di tipi di pubblico dettagliati con l’approvazione dell’utente in ogni fase | `audience-creation-flow` | Real-Time CDP (RTCDP) | &quot;Crea un pubblico di utenti che hanno acquistato negli ultimi 30 giorni&quot; <br> &quot;Crea un segmento per i membri fedeltà di alto valore in California&quot; |
| Creare definizioni di PQL | Assembla le definizioni del pubblico da proprietà XDM, eventi comportamentali o tipi di pubblico esistenti; supporta l’aggregazione e le finestre temporali | `segment-definition-assembly` | Real-Time CDP (RTCDP) | &quot;Crea un PQL per gli utenti che hanno visualizzato più di 3 prodotti ma non hanno acquistato&quot; <br> &quot;Aggiungi una finestra temporale di 7 giorni alla condizione evento&quot; |
| Cerca e trova tipi di pubblico | Trova i tipi di pubblico per ID, nome, ricerca semantica; rileva i duplicati e analizza le sovrapposizioni | `audience-search` | Real-Time CDP (RTCDP) | &quot;Trova tutti i tipi di pubblico fedeltà&quot; <br> &quot;Esiste un duplicato del segmento &quot;Acquirenti festivi&quot;?&quot; |
| Stimare la dimensione del pubblico | Stimare la portata del profilo per un’espressione PQL utilizzando l’API di anteprima Adobe Experience Platform con polling | `audience-size-estimate` | Real-Time CDP (RTCDP) | &quot;Quanto è grande questo pubblico?&quot; <br> &quot;Stimare la portata di questa espressione PQL&quot; |
| Cascata dimensione pubblico | Scomporre un PQL in sottopredicati e mostrare in che modo ogni condizione contribuisce alla dimensione finale del pubblico | `audience-size-waterfall` | Real-Time CDP (RTCDP) | &quot;Mostra la cascata per questo PQL&quot; <br> &quot;Suddividi in base a come ogni condizione riduce il pubblico&quot; |
| Scopri i campi XDM per il targeting | Cerca i campi per nome, descrizione o valore dei dati; scopri dove si trovano e dove sono già utilizzati | `field-discovery` | Real-Time CDP (RTCDP) | &quot;Quali campi posso utilizzare per eseguire il targeting dei clienti fidelizzati?&quot; <br> &quot;Trova campi relativi alla cronologia acquisti&quot; |
| Pubblicare/salvare tipi di pubblico | Mantenere le definizioni del pubblico in Experience Platform Segmentation Service con convenzioni di denominazione e controlli di conformità | `audience-publish` | Real-Time CDP (RTCDP) | &quot;Salva come bozza&quot; <br> &quot;Pubblica il pubblico con il nome &quot;Venditori primaverili&quot;&quot; |

## Percorsi

| Caso d&#39;uso | Descrizione | Competenza | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| [Crea percorsi dal linguaggio naturale](journeys/create-journey-from-natural-language.md) | Orchestrare la creazione di percorsi in AJO da un prompt di testo o da un’immagine o un diagramma di flusso caricati | `journey-create` | Adobe Journey Optimizer (AJO) | &quot;Crea un percorso di benvenuto che invia un&#39;e-mail dopo l&#39;iscrizione, attende 3 giorni, quindi invia un follow-up&quot; <br> &quot;Crea un percorso da questa immagine di diagramma di flusso caricata&quot; |
| Analizzare i conflitti di percorso | Rilevare sovrapposizioni di pubblico, conflitti di pianificazione e problemi di deduplicazione tra percorsi attivi | `journey-analyze-conflict` | Adobe Journey Optimizer (AJO) | &quot;Il percorso di abbandono del carrello è in conflitto con altri percorsi?&quot; <br> &quot;Verifica la sovrapposizione del pubblico tra i miei percorsi attivi&quot; |
| Analizzare l’abbandono del percorso | Identifica dove e perché i clienti abbandonano durante un percorso e rileva pattern di comportamento che portano al disimpegno | `journey-analyze-fallout` | Adobe Journey Optimizer (AJO) | &quot;Dove vengono inviate le persone nel percorso di ricoinvolgimento?&quot; <br> &quot;Quali nodi nel percorso X hanno il fallout più elevato?&quot; |
| Analizzare gli errori delle azioni personalizzate | Identifica quando le azioni personalizzate hanno esito negativo o i tassi di errore si sono impennati all’interno di un percorso e diagnostica le cause principali prima che gli errori si trasformino in interruzioni più ampie | `journey-analyze-custom-action` | Adobe Journey Optimizer (AJO) | &quot;Perché le azioni personalizzate non riescono nel percorso di registrazione fedeltà?&quot; <br> &quot;Visualizza la frequenza di errori per l&#39;azione personalizzata ExternalPush nel percorso di benvenuto.&quot; |
| [Creare, modificare e gestire le sfide relative alla fedeltà](journeys/create-loyalty-challenge.md) | Semplificare e accelerare la gestione dei programmi fedeltà | `loyalty` | Adobe Journey Optimizer (AJO) | &quot;Crea una sfida che incoraggia i membri a provare una nuova bevanda stagionale&quot; <br> &quot;Mostra le sfide di fedeltà con i tassi di abbandono dei membri più elevati.&quot; |

## Elementi fondamentali

| Caso d&#39;uso | Descrizione | Competenza | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Conoscenza del prodotto e documentazione | Rispondi alle domande pratiche, concettuali, sulla risoluzione dei problemi e sulle best practice contenute nei documenti ufficiali di Adobe | `product-knowledge` | Tutte le candidature ammissibili | &quot;Come si imposta una destinazione di streaming?&quot; <br> &quot;Qual è la differenza tra segmentazione in batch e segmentazione in streaming?&quot; |
| Query di entità Experience Platform/Journey Optimizer | Funge da punto di ingresso principale per domande sulle entità della piattaforma; passa a KG, all’individuazione dei campi o alle API in base alle esigenze | `operational-insights` | Tutte le candidature ammissibili | &quot;Quanti set di dati ho?&quot; <br> &quot;Mostra tutti i percorsi attivi&quot; <br> &quot;Elenca le mie destinazioni&quot; |
| Query di Knowledge Graph | Conteggi aggregati, join tra entità, ricerche di relazioni ed esplorazione dei metadati tramite singole query SQL | `knowledge-graph` | Tutte le candidature ammissibili | &quot;Quali tipi di pubblico utilizzano questo set di dati?&quot; <br> &quot;Mostra relazioni tra schemi e set di dati&quot; |
| Operazioni API per Experience Platform/Journey Optimizer/Customer Journey Analytics | Fornisci un gateway API diretto per mutazioni, controlli dello stato in tempo reale e tipi di entità non inclusi nel Knowledge Graph | `cxo-api` | Tutte le candidature ammissibili | &quot;Elimina set di dati X&quot; <br> &quot;Controlla lo stato del processo di acquisizione batch&quot; |
| Risoluzione entità e collegamento | Utilizza la ricerca semantica e lessicale per risolvere le menzioni di entità nelle entità Experience Platform effettive e individuare i campi XDM | `entity-linking` | Adobe Experience Platform | &quot;Risolvi gli &quot;acquirenti per vacanze&quot; a un pubblico effettivo&quot; <br> &quot;Trovami i campi relativi alla cronologia acquisti&quot; |
| Gestire le abilità personalizzate | Salva, modifica o elimina le abilità riutilizzabili di proprietà dell&#39;utente che persistono nelle sessioni | `manage-skill` | Tutte le candidature ammissibili | &quot;Salva il flusso di lavoro come abilità&quot; <br> &quot;Elimina abilità report settimanale&quot; <br> &quot;Trasforma questa in un&#39;abilità riutilizzabile&quot; |
| Monitorare la capacità di streaming e le violazioni | Controlla l’utilizzo dello streaming, la capacità e lo stato di violazione correnti e storici nelle sandbox | `observability-streaming-capacity`, `observability-streaming-usage`, `observability-capacity-breaches` | Adobe Experience Platform | &quot;Qual è la capacità di streaming corrente nella sandbox corrente?&quot; <br> &quot;La mia sandbox attuale ha superato i limiti di capacità nell’ultima settimana?&quot; |
| [Visualizza i risultati della valutazione dello stato](https://experienceleague.adobe.com/it/docs/experience-platform/run-and-operate/health-checks/overview) | Visualizzare la valutazione più recente dello stato di integrità per la sandbox, eseguire il drill-in di un controllo non riuscito e visualizzare le entità interessate | `rao-view-latest-health-checks-assessment` | Adobe Experience Platform | &quot;Cosa c&#39;è che non va nella sandbox?&quot; <br> &quot;Informazioni sulla valutazione del controllo di integrità più recente&quot; <br> &quot;Quali sono i problemi per il controllo di descrizione dello spazio dei nomi personalizzato?&quot; |
| Correggi problemi di verifica stato | Correggi i problemi relativi a spazio dei nomi, criteri di unione e schema delle identità contrassegnate direttamente dalla chat, con la tua approvazione prima di apportare qualsiasi modifica | `rao-remediate-identity-namespace-description`, `rao-remediate-merge-policy-duplicate-name`, `rao-remediate-missing-audit-field-group`, `rao-remediate-default-merge-policy-naming` | Adobe Experience Platform | &quot;Correggere le descrizioni dello spazio dei nomi delle identità&quot; <br> &quot;Correggere i nomi dei criteri di unione duplicati&quot; <br> &quot;Correggere gli schemi senza il gruppo di campi di controllo&quot; <br> &quot;Correggere la denominazione dei criteri di unione predefiniti&quot; |

## Strumenti sandbox

| Caso d&#39;uso | Descrizione | Competenza | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| [Spostamento di oggetti tra sandbox](/help/agents/sandbox-tooling.md) | Migra facilmente schemi, tipi di pubblico e altre configurazioni di oggetti tra sandbox, con le dipendenze risolte automaticamente | `sandbox-tooling-workflow` | Adobe Experience Platform | &quot;Sposta lo schema Luma Loyalty Members Platinum dalla sandbox corrente alla sandbox di produzione&quot; <br> &quot;Promuovi il pubblico US Gold Loyalty Members allo stage&quot; |

## Avvisi cliente

| Caso d&#39;uso | Descrizione | Competenza | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Gestire gli abbonamenti agli avvisi | Visualizza e gestisci gli abbonamenti agli avvisi tramite conversazioni in linguaggio naturale. | `alerts-subscribe` | Adobe Experience Platform | &quot;A quali avvisi sono abbonato?&quot;<br><br>&quot;Sottoscrivi questo avviso.&quot;<br><br>&quot;Rimuovi l&#39;abbonamento a questo avviso.&quot; |
| Rivedi attività di avviso | Esaminare lo stato corrente dell&#39;avviso e l&#39;attività cronologica dell&#39;avviso per un periodo di tempo specificato. | `alerts-list` | Adobe Experience Platform | &quot;Cosa è successo nelle ultime 24 ore?&quot;<br><br>&quot;Quali avvisi sono stati attivati nelle ultime 24 ore?&quot;<br><br>&quot;Mostra gli avvisi attivi degli ultimi sette giorni.&quot; |
| Identificare i pattern ricorrenti degli avvisi | Analizza la cronologia degli avvisi per identificare i tipi di avvisi attivati di frequente e le tendenze operative. | `alerts-list` | Adobe Experience Platform | &quot;Visualizza i primi 3 tipi di avviso attivati.&quot;<br><br>&quot;Quali tipi di avviso si sono verificati più frequentemente in questo mese?&quot;<br><br>&quot;Quali modelli di avviso vengono visualizzati negli ultimi sette giorni?&quot; |
| Concentrarsi su questioni ad alta priorità | Filtra l’attività di avviso in base alla gravità per assegnare la priorità agli sforzi di indagine. | `alerts-list` | Adobe Experience Platform | &quot;Mostra solo gli avvisi con priorità elevata.&quot;<br><br>&quot;Quali avvisi critici sono stati attivati questa settimana?&quot;<br><br>&quot;Mostra gli avvisi critici degli ultimi 30 giorni.&quot; |
| Comprendere il raggio di impatto degli avvisi | Identificare gli oggetti più interessati dagli avvisi e determinare dove iniziare l&#39;indagine. | `alerts-list` | Adobe Experience Platform | &quot;Quali sono i primi 5 oggetti interessati?&quot;<br><br>&quot;Quali oggetti sono associati agli avvisi con maggiore gravità?&quot; |
| Connettere i tipi di avviso agli oggetti interessati | Analizzare le relazioni tra i tipi di avviso e le risorse interessate. | `alerts-list` | Adobe Experience Platform | &quot;Quali tipi di avviso hanno interessato più frequentemente questo set di dati?&quot;<br><br>&quot;Mostra la relazione tra i tipi di avviso e gli oggetti interessati.&quot;<br><br>&quot;Quale tipo di avviso ha interessato più frequentemente l&#39;oggetto interessato più frequentemente?&quot; |
| Concentrati sugli avvisi personali | Analizza gli avvisi a cui sei abbonato e sei responsabile del monitoraggio. | `alerts-list` | Adobe Experience Platform | &quot;Mostra gli avvisi ad alta gravità a cui sottoscrivo.&quot;<br><br>&quot;Quali avvisi sono stati attivati questa settimana?&quot;<br><br>&quot;È necessario prestare attenzione a uno degli avvisi sottoscritti?&quot; |

## Flusso di lavoro e pianificazione

| Caso d&#39;uso | Descrizione | Competenza | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Gestisci area di lavoro di Planning | Creare ed evolvere aree di lavoro, sezioni, tipi di record e campi di Workfront Planning per organizzare i programmi e tenere traccia del lavoro | `manage-workfront-planning`, `wf-planning-solution-architect` | Pianificazione Workfront | &quot;Creare un&#39;area di lavoro denominata MKG Hub e impostare tipi di record per tenere traccia dei programmi per area&quot; <br> &quot;Impostare i tipi di record e le relazioni necessari per tenere traccia dei programmi MKG per i diversi canali e area&quot; |
| Gestisci record di Planning | Crea e aggiorna i record di pianificazione (campagne, resoconti) e i relativi valori dei campi in un’area di lavoro | `manage-workfront-planning` | Pianificazione Workfront | &quot;Crea una descrizione della campagna di lancio Autunno Brand con l&#39;obiettivo, il pubblico di destinazione e i messaggi chiave&quot; <br> &quot;Aggiorna la descrizione di lancio Autunno Brand con il budget e i canali principali&quot; |
| Creare e gestire i progetti | Progetti spin up e struttura: applicazione di modelli, impostazione di priorità e budget, sequenziamento di attività, aggiunta di fasi e dipendenze e assegnazione di persone o ruoli | `manage-workfront-workflow` | Flusso di lavoro Workfront | &quot;Crea una campagna primaverile, impostala ad alta priorità con un budget di 200.000 dollari e metti in sequenza le attività&quot; <br> &quot;Crea un piano di progetto Workfront denominato [nome progetto] da [modello progetto]&quot; <br> &quot;Crea un piano di progetto per Autunno lancio - Campagna social con attività per la concezione, la progettazione, la copia e la revisione&quot; <br> &quot;Aggiungi una nuova attività di e-mail marketing e assegnala a Rachel Smith&quot; |
| Accelera revisioni e approvazioni | Impostare approvazioni in più fasi, applicare modelli di approvazione, aggiungere/rimuovere approvatori, inviare promemoria ed eseguire aggiornamenti in blocco | `manage-workfront-workflow` | Flusso di lavoro Workfront | &quot;Crea un&#39;approvazione in più fasi - copia, progettazione, legale - e ricorda a chiunque non abbia approvato&quot; <br> &quot;Rimuovi Chris Smith da tutte le approvazioni aperte e sostituisci con Jane Francis&quot; |
| Aggiorna stato attività e lavoro | Contrassegnare le attività come completate, aggiornare la percentuale di completamento e chiudere il lavoro | `manage-workfront-workflow` | Flusso di lavoro Workfront | &quot;Contrassegna l&#39;attività &#39;Produce elemento chiave&#39; in Autunno Launch come completata&quot; <br> &quot;Chiudi l&#39;attività di copia Autunno Launch al 100%&quot; |
| Approfondimenti lavoro superficie | Domande esplorative per individuare il lavoro a rischio, le attività non assegnate, le questioni aperte e lo stato tra i progetti | `query-workfront` | Flusso di lavoro Workfront | &quot;Trova attività incomplete sui progetti correnti che non sono assegnati a nessuno e scadono questa settimana&quot; <br> &quot;Quanti problemi aperti ci sono tra i progetti correnti?&quot; |
| Riepilogo progetti e attività | Elenchi pull, tabelle e conteggi di progetti, attività, problemi e assegnazioni | `query-workfront` | Flusso di lavoro Workfront | &quot;Visualizza una tabella delle attività pronte per l&#39;avvio, con il nome del progetto, la data di scadenza dell&#39;attività e l&#39;utente assegnato&quot; <br> &quot;Ottieni tutte le attività assegnate a [nome utente]&quot; |
| Tracciare lo stato di approvazioni e portfolio | Controlla lo stato delle approvazioni e riepiloga il lavoro incompleto per portfolio | `query-workfront` | Flusso di lavoro Workfront | &quot;Mostra lo stato delle mie approvazioni&quot; <br> &quot;Mostra una tabella con problemi incompleti che fanno parte del portfolio [Portfolio name]&quot; |
