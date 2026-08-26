---
description: Sfoglia i casi d’uso di Chat con collaboratori e i prompt di esempio, organizzati per area e suddivisi per approfondimenti sui dati, pubblico, percorsi e operazioni sulla piattaforma.
title: Casi di utilizzo della chat del collaboratore
feature_v2: id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 74c7d4e455b0b7079b5fe85d2b5325e32fe6642e
workflow-type: tm+mt
source-wordcount: 3050
ht-degree: 7%

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
>Vedi anche [IA in AEM - Panoramica delle funzionalità agente in AEM](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/overview).

## Esperienza del marchio

### Produzione di esperienze - Casi di utilizzo di Sites

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Aggiornare le pagine di AEM | Esegui azioni quali aggiornamento, rimozione, sostituzione o aggiunta di elementi di contenuto per mantenere le esperienze accurate e correnti. Gli input possono essere annotazioni visive o del linguaggio naturale, ad esempio PDF o screenshot. | `aem-sites-pages-update` | Adobe Experience Manager (AEM) | Il &lt;URL> aggiorna il titolo a Hello World<br><br>on &lt;URL> cambia il pulsante &quot;Take our Coffee Quiz&quot; (Acquista il quiz sul caffè) in una versione più coinvolgente<br><br>Aggiorna &lt;URL> in base al &lt;URL> allegato<br><br>on. Desidero aggiungere una nuova sezione teaser in fondo alla pagina su una promozione in esecuzione nel mese di agosto: acquistare una macchina da caffè e ottenere 2 sacchi di caffè gratis. Trovi anche l&#39;immagine di amici che bevono caffè e usarlo nel teaser |
| Aggiornare AEM in blocco | Esegui azioni in blocco su più pagine contemporaneamente, ad esempio rimuovi, sostituisci o aggiungi elementi di contenuto per mantenere le esperienze accurate e correnti. | `aem-sites-pages-bulkreplace` | Adobe Experience Manager (AEM) | in &lt;aem path> aggiorna tutte le pagine che contengono la copia &quot;MyBarista\&quot; in &quot;BrewPass&quot; |
| Passare da Figma a frammento di contenuto visivo | Importare i disegni direttamente da Figma in Adobe Experience Manager utilizzando il linguaggio naturale. L’abilità crea automaticamente il modello di contenuto, il frammento di contenuto, le risorse e il modello di visualizzazione richiesti, consentendo agli utenti aziendali di passare in pochi minuti dalla progettazione ai contenuti pronti per il web senza dover eseguire la configurazione manuale. | `aem-sites-visualcontentfragments-create` | Adobe Experience Manager (AEM) | Importa da &lt;Figma_URL> |

**Informazioni correlate**

* [Funzionalità Agentic in AEM: Esperienza del marchio - Produzione di esperienze - Sites](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/experience-production/use-cases#use-cases-sites)

### Produzione di esperienze - Casi di utilizzo di Forms

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Crea modulo | Generare un nuovo modulo adattivo da una descrizione in linguaggio semplice, una descrizione allegata, un’immagine o un PDF | `aem-forms-adaptiveform-create` | Adobe Experience Manager (AEM) | &quot;Creare un modulo di onboarding per dipendenti&quot;<br><br>&quot;Creare un modulo utilizzando la descrizione allegata (immagine o pdf)&quot;<br><br>&quot;Creare un &lt;tipo di modulo> modulo adattivo&quot; |
| Modifica/aggiorna modulo | Modificare un modulo esistente: aggiungere/modificare campi, modificare un layout semplice, configurare azioni di invio o applicare modifiche da un documento di linee guida allegato | `aem-forms-adaptiveform-edit` | Adobe Experience Manager (AEM) | &quot;Aggiungi campo Secondo nome sotto campo Nome&quot;<br><br>&quot;Inserisci campi Nome e Cognome in un layout a 2 colonne, 50/50&quot;<br><br>&quot;Configura il modulo per inviare dati a un endpoint REST&quot;<br><br>&quot;Aggiorna il modulo in modo che corrisponda al documento delle linee guida allegato&quot;<br><br>&quot;Aggiungi campo &lt;nome campo> sotto &lt;campo esistente>&quot; |
| Aggiungi logica di business | Creare regole semplici, ad esempio mostrare o nascondere un campo in base al valore di un altro campo | `aem-forms-adaptiveform-edit` | Adobe Experience Manager (AEM) | &quot;Mostra il campo Società solo quando il tipo di dipendente è Contraente&quot;<br><br>&quot;Mostra il campo &lt;campo> solo quando &lt;altro campo> è &lt;valore>&quot; |
| Incorpora modulo | Inserire un modulo esistente o appena creato in una pagina AEM Sites designata (supportata solo nelle pagine Edge Delivery Services) | `aem-forms-adaptiveform-embed` | Adobe Experience Manager (AEM) | &quot;Incorpora il modulo nella home page del sito&quot;<br><br>&quot;Incorpora il modulo in &lt;percorso pagina>&quot; |

**Informazioni correlate**

* [Funzionalità Agentic in AEM: Esperienza del marchio - Produzione di esperienze - Forms](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/experience-production/use-cases#use-cases-forms)

### Sviluppo

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Diagnosticare e correggere le pipeline di Cloud Manager con errori | Analizzare un’esecuzione non riuscita della pipeline, identificare la causa principale e generare una correzione (con una diff) per la revisione | `cloud-manager-pipeline-troubleshooting` | Adobe Experience Manager (AEM) | &quot;Perché la pipeline di compilazione non riesce?&quot;<br><br>&quot;Suggerisci una correzione per la pipeline di produzione interrotta&quot; |
| Gestire le pipeline di Cloud Manager | Creare, eseguire e monitorare le pipeline di AEM Cloud Manager, inclusi registri, artefatti, variabili e impostazioni | `cloud-manager-pipeline-management` | Adobe Experience Manager (AEM) | &quot;Elencare le pipeline per il programma 12345&quot;<br><br>&quot;Perché l&#39;esecuzione della pipeline di sviluppo non è riuscita?&quot; |
| Gestire gli ambienti Cloud Manager | Creazione, configurazione e manutenzione di ambienti AEM Cloud Manager, inclusi RDE, variabili di ambiente, registri e backup | `cloud-manager-environment-management` | Adobe Experience Manager (AEM) | &quot;Elencare gli ambienti personali per il programma 12345&quot;<br><br>&quot;Reimpostare il codice RDE&quot; |
| Gestire i programmi Cloud Manager | Elencare, ispezionare ed eliminare programmi AEM Cloud Manager, incluse pipeline e ambienti | `cloud-manager-program-management` | Adobe Experience Manager (AEM) | &quot;Elenca i miei programmi Cloud Manager&quot;<br><br>&quot;Ottieni dettagli per 12345 programma&quot; |
| Gestire le pianificazioni degli aggiornamenti delle versioni di AEM | Configura le ore di pausa giornaliere e i periodi di disponibilità dell&#39;aggiornamento per la manutenzione automatica e visualizza le finestre di blocco del codice globali di Adobe | `cloud-manager-release-management` | Adobe Experience Manager (AEM) | &quot;Qual è la finestra delle ore non interattive corrente?&quot;<br><br>&quot;Pianificazione di un periodo senza aggiornamento dal 20 dicembre al 2 gennaio&quot; |

**Informazioni correlate**

* [Funzionalità Agentic in AEM: Esperienza del marchio - Sviluppo](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/development/use-cases)

### Onboarding - Casi di utilizzo di AEM Assets

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Onboarding end-to-end guidato | Orchestrazione dell’intero ciclo di vita di onboarding, selezione dell’archivio, delega alla cartella, tag, metadati, importazione e ricerca di sottocompetenze, se non conosci l’attività di onboarding specifica necessaria. | `aem-onboarding-workflow` | Adobe Experience Manager (AEM) Assets | &quot;Eseguire l&#39;onboarding del team in AEM Assets&quot;<br><br>&quot;Passare all&#39;onboarding di AEM DAM&quot; |
| Progettare e creare gerarchie di cartelle | Consiglia e crea strutture di cartelle scalabili in AEM Assets (in `/content/dam`) in base alle esigenze aziendali o agli input CSV. | `aem-folder-management` | Adobe Experience Manager (AEM) Assets | &quot;Consigliare una struttura di cartelle per le risorse di marketing lifestyle&quot;<br><br>&quot;Creare cartelle in base a questo file CSV&quot; |
| Progettare e creare tag | Progetta e crea vocabolari di tag controllati in `/content/cq:tags`, spazi dei nomi, tag gerarchici e operazioni batch tag. | `aem-tag-taxonomy` | Adobe Experience Manager (AEM) Assets | &quot;Progettare una tassonomia dei tag con spazi dei nomi per le categorie di prodotti &quot;<br><br>&quot;Importare tag da questo CSV&quot;<br><br>&quot;Creare questi tag gerarchici in AEM&quot; |
| Creare e assegnare moduli di metadati | Progetta e crea moduli di metadati personalizzati, utilizzati dagli autori di contenuti dell’interfaccia utente di creazione, da un CSV, una tabella, un documento sui requisiti o una descrizione, e facoltativamente li assegna alle cartelle. | `aem-metadata-form` | Adobe Experience Manager (AEM) Assets | &quot;Creare un modulo metadati da questo elenco di campi&quot;<br><br>&quot;Assegnare il modulo alla cartella `campaigns`&quot; |

**Informazioni correlate**

* [Funzionalità di Agentic in AEM: Esperienza del marchio - Onboarding](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/onboarding/use-cases)

## Contenuto verificato - Casi di utilizzo di AEM Assets

### Individuazione dei contenuti

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Ricerca per tema semantico | Trova le risorse per concetto, umore o tema visivo utilizzando la corrispondenza semantica basata sull’intelligenza artificiale. | `aem-assets-discovery` | Adobe Experience Manager (AEM) Assets | &quot;Trovami immagini di vita del caffè mattutino&quot; |
| Ricerca per metadati personalizzati | Filtra le risorse in base ai campi di metadati personalizzati (ad esempio, Coffee Blend, Brand, Roast Level). | `aem-assets-discovery` | Adobe Experience Manager (AEM) Assets | &quot;Trova risorse in cui `Coffee Blend` è `Morning Muse`&quot;<br><br>&quot;Ottieni risorse la cui licenza non è scaduta&quot;<br><br>&quot;Trova risorse il cui nome campagna non è impostato (la proprietà deve essere indicizzata per ottenere risultati appropriati).&quot; |
| Cerca per stato di approvazione | Filtra le risorse in base allo stato di approvazione. Ad esempio, stato approvato, in revisione, rifiutato o mancante. | `aem-assets-discovery` | Adobe Experience Manager (AEM) Assets | &quot;Mostra tutte le risorse approvate nella cartella `Campaign`&quot; |
| Cerca per cartella/percorso | Per identificare le risorse, interpreta i prompt del linguaggio naturale che fanno riferimento ai nomi delle cartelle in AEM. Puoi semplicemente menzionare la cartella nel loro prompt, senza navigare manualmente nell’archivio, riducendo in modo significativo il numero di clic necessari per individuare il contenuto corretto. | `aem-assets-discovery` | Adobe Experience Manager (AEM) Assets | &quot;Nella cartella `WKND`&quot;?<br><br>&quot;Mostra le risorse modificate dopo l&#39;1 novembre 2025 nella cartella `WKND`&quot; |

**Informazioni correlate**

* [Funzionalità Agentic in AEM: Contenuto verificato - Individuazione dei contenuti](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/content-advisor/discovery/use-cases)

### Ottimizzazione dei contenuti

| Caso d&#39;uso | Descrizione | Abilità | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Creazione di rendering ad alta risoluzione e rendering ottimizzati per il canale | Genera nuove rappresentazioni di una risorsa a una risoluzione e a un livello di qualità specifici, semplificando la preparazione di varianti pronte per il canale senza modifiche manuali. Puoi anche produrre rappresentazioni personalizzate in base ai requisiti specifici della piattaforma, come ad esempio Instagram Stories, garantendo che le risorse soddisfino automaticamente il formato, il rapporto di trasmissione e le linee guida sulla qualità. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) Assets | &quot;Crea una rappresentazione `2000px` come `JPEG` con `80% quality`&quot;<br><br>&quot;Crea una rappresentazione per una storia Instagram&quot; |
| Sovrapposizioni con marchio e generazione composita | Applica grafici promozionali, sovrapposizioni o badge alle risorse esistenti con un posizionamento preciso, per supportare la creazione rapida di composizioni pronte per la campagna. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) Assets | &quot;Sovrapponi l&#39;immagine con gli elementi grafici dello sconto `30%` sul banner promozionale, posizionandolo `100px` dal centro&quot; |
| Miglioramenti alle immagini, regolazioni del colore di sfondo, trasformazioni di orientamento | Applica miglioramenti visivi (nitidezza delle immagini), sostituisci i colori di sfondo ed esegui trasformazioni di orientamento. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) Assets | &quot;Cambia il colore di sfondo di `PNG` in `#ff8932`&quot;<br><br>&quot;Contrasta l&#39;immagine&quot;<br><br>&quot;Specchia l&#39;immagine orizzontalmente&quot; |

**Informazioni correlate**

* [Funzionalità Agentic in AEM: Contenuto verificato - Ottimizzazione dei contenuti](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/content-advisor/content-optimization/use-cases)

## Governance del brand

| Caso d&#39;uso | Descrizione | Competenza | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Linee guida e ricerca dei segmenti | Recuperare le linee guida dettagliate del brand, definite per segmento, mercato o categoria | enterprise-context | Adobe Experience Manager (AEM) | &quot;Quali sono le linee guida per il tono di voce per questo marchio?&quot;<br>&quot;Elencare le categorie di attestazioni utilizzate nel settore verticale dell&#39;integrità&quot; |
| Valutare i contenuti in base alle linee guida del brand | Valutare una pagina, un blocco di testo o un’immagine pubblicati/creati in base ai controlli del marchio configurati | aem-governance | Adobe Experience Manager (AEM) | &quot;Valutare questa pagina di destinazione in base alle linee guida di SecurBank&quot;<br>&quot;Questa tagline supera i controlli del tono di voce?&quot; |
| Eseguire il debug delle autorizzazioni di AEM | Eseguire il debug/comprendere i criteri di autorizzazione, gli ACL e le regole di ereditarietà. | aem-governance | Adobe Experience Manager (AEM) | &quot;Perché l&#39;amministratore dell&#39;entità può scrivere `/content/folder/us` su `https://author/` ?&quot;<br>&quot;Perché non è possibile scrivere l&#39;autore campione in `/content/dam` su `https://author`&quot; |

**Informazioni correlate**

* [Funzionalità Agentic in AEM: Governance del brand](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-governance/use-cases)

## Informazioni sui dati

| Caso d&#39;uso | Descrizione | Competenza | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| [Recuperare i report e le metriche di CJA](data-insights/analytics-chat.md) | Eseguire query su CJA in tempo reale per estrarre metriche, dimensioni, segmenti e visualizzazioni dati | `cja` | Customer Journey Analytics (CJA) | &quot;Mostra visualizzazioni pagina per gli ultimi 30 giorni&quot; · &quot;Elenca i segmenti principali nella visualizzazione dati master&quot; |
| Analisi comparativa | Confrontare le metriche su canali, periodi di tempo o segmenti affiancati | `cja-root-cause-analysis`, `cja`, `dx-api`, `knowledge-graph` | Customer Journey Analytics (CJA) | &quot;Confronto dei ricavi per canale, mese e mese&quot; · &quot;Che aspetto ha la conversione da PC desktop a PC portatili questo trimestre?&quot; |
| Prestazioni della campagna | Misura il modo in cui le campagne, i canali e le proprietà web vengono eseguiti in un determinato periodo di tempo. | `cja`, `dx-api`, `knowledge-graph` | | &quot;Quali sono state le prestazioni delle campagne web di Acrobat il mese scorso?&quot; |
| analisi funnel | Passaggio ai funnel di conversione con più passaggi con drop-off in ogni fase | `cja` | Customer Journey Analytics (CJA) | &quot;Passami attraverso il funnel di pagamento&quot; · &quot;Mostra funnel di conversione da PDP all&#39;acquisto&quot; |
| Previsione | Progetta valori metrici futuri basati su dati storici CJA | `cja` | Customer Journey Analytics (CJA) | &quot;Sessioni di previsione per i prossimi 30 giorni&quot; · &quot;Siamo sulla buona strada per raggiungere il nostro obiettivo di fatturato?&quot; |
| [Analisi causa principale](data-insights/root-cause-analysis.md) | Ricercare il motivo per cui una metrica è cambiata: diagnosticare gocce, picchi e anomalie | `cja-root-cause-analysis` | Customer Journey Analytics (CJA) | &quot;Perché le conversioni sono calate la settimana scorsa?&quot; · &quot;Cosa ha causato il picco dei ricavi il 15 gennaio?&quot; |
| Riepiloghi esecutivi e digest dei KPI | Creare riepiloghi delle prestazioni pronti per le parti interessate, consigli prescrittivi e descrizioni della presentazione | `cja-executive-summary`, `cja-bacom-anomaly-tracker-v2`, `cja-cno-weekly-pulse`, `cja-reporting`, `cja`, `dx-api` | Customer Journey Analytics (CJA) | &quot;Fornisci un riepilogo esecutivo del mese scorso&quot; · &quot;Crea uno schema della presentazione da dati di questo trimestre&quot; |
| [AA ↔ convalida dati CJA](data-insights/data-validation-aa-cja.md) | Confrontare, controllare e riconciliare i dati tra Adobe Analytics e Customer Journey Analytics, in particolare durante l’aggiornamento da Adobe Analytics a Customer Journey Analytics | `aa-cja-validation`, `cja`, `dx-api` | ADOBE ANALYTICS + CJA | &quot;Confrontare la suite di rapporti AA con la visualizzazione dati di CJA&quot; · &quot;Convalidare le visualizzazioni di pagina tra AA e CJA&quot; |
| Serie temporali operative e analisi causale | Eseguire query e analizzare dati storici di serie temporali per tipi di pubblico, set di dati e percorsi con attribuzione causale | `operational-stats-causal-analysis` | Tutte le candidature ammissibili | &quot;Mostra le tendenze delle dimensioni del pubblico negli ultimi 90 giorni&quot; · &quot;Perché la riga del set di dati ha conteggiato un picco il 3 marzo?&quot; |
| Creare abilità CJA personalizzate | Trasforma i modelli analitici in competenze riutilizzabili e ripetibili che persistono nelle sessioni | `cja-skill-creator` | Customer Journey Analytics (CJA) | &quot;Trasforma questa analisi settimanale dei ricavi in un’abilità riutilizzabile&quot; · &quot;Salva come abilità per il reporting mensile di funnel&quot; |

## Tipi di pubblico

| Caso d&#39;uso | Descrizione | Competenza | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| [Crea tipi di pubblico dal linguaggio naturale](audiences/create-audience-from-natural-language.md) | Orchestrare la creazione di tipi di pubblico dettagliati con l’approvazione dell’utente in ogni fase | `audience-creation-flow` | Real-Time CDP (RTCDP) | &quot;Crea un pubblico di utenti che hanno acquistato negli ultimi 30 giorni&quot; · &quot;Crea un segmento per i membri fedeltà di alto valore in California&quot; |
| Creare definizioni di PQL | Assembla le definizioni del pubblico da proprietà XDM, eventi comportamentali o tipi di pubblico esistenti; supporta l’aggregazione e le finestre temporali | `segment-definition-assembly` | Real-Time CDP (RTCDP) | &quot;Crea un PQL per le persone che hanno visualizzato più di 3 prodotti ma non hanno acquistato&quot; · &quot;Aggiungi una finestra temporale di 7 giorni alla condizione dell’evento&quot; |
| Cerca e trova tipi di pubblico | Trova i tipi di pubblico per ID, nome, ricerca semantica; rileva i duplicati e analizza le sovrapposizioni | `audience-search` | Real-Time CDP (RTCDP) | &quot;Trova tutti i tipi di pubblico fidelizzati&quot; · &quot;Esiste un duplicato del segmento &quot;Acquirenti festivi&quot;?&quot; |
| Stimare la dimensione del pubblico | Stimare la portata del profilo per un’espressione PQL utilizzando l’API di anteprima Adobe Experience Platform con polling | `audience-size-estimate` | Real-Time CDP (RTCDP) | &quot;Quanto è grande questo pubblico?&quot; · &quot;Stimare la portata di questa espressione PQL&quot; |
| Cascata dimensione pubblico | Scomporre un PQL in sottopredicati e mostrare in che modo ogni condizione contribuisce alla dimensione finale del pubblico | `audience-size-waterfall` | Real-Time CDP (RTCDP) | &quot;Mostrami la cascata per questo PQL&quot; · &quot;Suddividi in che modo ogni condizione riduce il pubblico&quot; |
| Scopri i campi XDM per il targeting | Cerca i campi per nome, descrizione o valore dei dati; scopri dove si trovano e dove sono già utilizzati | `field-discovery` | Real-Time CDP (RTCDP) | &quot;Quali campi posso utilizzare per eseguire il targeting dei clienti fidelizzati?&quot; · &quot;Trova campi relativi alla cronologia acquisti&quot; |
| Pubblicare/salvare tipi di pubblico | Mantenere le definizioni del pubblico in Experience Platform Segmentation Service con convenzioni di denominazione e controlli di conformità | `audience-publish` | Real-Time CDP (RTCDP) | &quot;Salva come bozza&quot; · &quot;Pubblica il pubblico con il nome &quot;Venditori primaverili&quot;&quot; |

## Percorsi

| Caso d&#39;uso | Descrizione | Competenza | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| [Crea percorsi dal linguaggio naturale](journeys/create-journey-from-natural-language.md) | Orchestrare la creazione di percorsi in AJO da un prompt di testo o da un’immagine o un diagramma di flusso caricati | `journey-create` | Adobe Journey Optimizer (AJO) | &quot;Crea un percorso di benvenuto che invia un’e-mail dopo l’iscrizione, attende 3 giorni, quindi invia un follow-up&quot; · &quot;Crea un percorso da questa immagine di diagramma di flusso caricata&quot; |
| Analizzare i conflitti di percorso | Rilevare sovrapposizioni di pubblico, conflitti di pianificazione e problemi di deduplicazione tra percorsi attivi | `journey-analyze-conflict` | Adobe Journey Optimizer (AJO) | &quot;Il mio percorso di abbandono del carrello è in conflitto con altri percorsi?&quot; · &quot;Verificare la sovrapposizione del pubblico tra i miei percorsi attivi&quot; |
| Analizzare l’abbandono del percorso | Identifica dove e perché i clienti abbandonano durante un percorso e rileva pattern di comportamento che portano al disimpegno | `journey-analyze-fallout` | Adobe Journey Optimizer (AJO) | &quot;Dove vanno le persone nel mio percorso di ricoinvolgimento?&quot; · &quot;Quali nodi nel percorso X hanno il fallout più elevato?&quot; |
| Analizzare gli errori delle azioni personalizzate | Identifica quando le azioni personalizzate hanno esito negativo o i tassi di errore si sono impennati all’interno di un percorso e diagnostica le cause principali prima che gli errori si trasformino in interruzioni più ampie | `journey-analyze-custom-action` | Adobe Journey Optimizer (AJO) | &quot;Perché le azioni personalizzate non riescono nel percorso di registrazione fedeltà?&quot; · &quot;Visualizza la frequenza di errori per l&#39;azione personalizzata ExternalPush nel percorso di benvenuto&quot; |
| [Creare, modificare e gestire le sfide relative alla fedeltà](journeys/create-loyalty-challenge.md) | Semplificare e accelerare la gestione dei programmi fedeltà | `loyalty` | Adobe Journey Optimizer (AJO) | &quot;Crea una sfida incoraggiando i membri a provare una nuova bevanda stagionale&quot; · &quot;Dimostrami le sfide di fedeltà con i tassi più elevati di abbandono dei membri&quot;. |

## Elementi fondamentali

| Caso d&#39;uso | Descrizione | Competenza | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| Conoscenza del prodotto e documentazione | Rispondi alle domande pratiche, concettuali, sulla risoluzione dei problemi e sulle best practice contenute nei documenti ufficiali di Adobe | `product-knowledge` | Tutte le candidature ammissibili | &quot;Come si imposta una destinazione di streaming?&quot; · &quot;Qual è la differenza tra segmentazione in batch e segmentazione in streaming?&quot; |
| Query di entità Experience Platform/Journey Optimizer | Funge da punto di ingresso principale per domande sulle entità della piattaforma; passa a KG, all’individuazione dei campi o alle API in base alle esigenze | `operational-insights` | Tutte le candidature ammissibili | &quot;Quanti set di dati ho?&quot; · &quot;Mostra tutti i percorsi attivi&quot; · &quot;Elenca le destinazioni&quot; |
| Query di Knowledge Graph | Conteggi aggregati, join tra entità, ricerche di relazioni ed esplorazione dei metadati tramite singole query SQL | `knowledge-graph` | Tutte le candidature ammissibili | &quot;Quali tipi di pubblico utilizzano questo set di dati?&quot; · &quot;Mostra relazioni tra schemi e set di dati&quot; |
| Operazioni API per Experience Platform/Journey Optimizer/Customer Journey Analytics | Fornisci un gateway API diretto per mutazioni, controlli dello stato in tempo reale e tipi di entità non inclusi nel Knowledge Graph | `cxo-api` | Tutte le candidature ammissibili | &quot;Elimina set di dati X&quot; · &quot;Controlla lo stato del processo di acquisizione batch&quot; |
| Risoluzione entità e collegamento | Utilizza la ricerca semantica e lessicale per risolvere le menzioni di entità nelle entità Experience Platform effettive e individuare i campi XDM | `entity-linking` | Adobe Experience Platform | &quot;Risolvi &#39;Acquirenti di vacanze&#39; a un pubblico effettivo&quot; · &quot;Trovami campi relativi alla cronologia degli acquisti&quot; |
| Gestire le abilità personalizzate | Salva, modifica o elimina le abilità riutilizzabili di proprietà dell&#39;utente che persistono nelle sessioni | `manage-skill` | Tutte le candidature ammissibili | &quot;Salva il flusso di lavoro come un’abilità&quot; · &quot;Elimina l’abilità di reporting settimanale&quot; · &quot;Trasforma questa in un’abilità riutilizzabile&quot; |
| Monitorare la capacità di streaming e le violazioni | Controlla l’utilizzo dello streaming, la capacità e lo stato di violazione correnti e storici nelle sandbox | `observability-streaming-capacity`, `observability-streaming-usage`, `observability-capacity-breaches` | Adobe Experience Platform | &quot;Qual è la capacità di streaming corrente nella sandbox corrente?&quot; · &quot;La mia sandbox attuale ha superato i limiti di capacità nell’ultima settimana?&quot; |
| [Visualizza i risultati della valutazione dello stato](https://experienceleague.adobe.com/en/docs/experience-platform/run-and-operate/health-checks/overview) | Visualizzare la valutazione più recente dello stato di integrità per la sandbox, eseguire il drill-in di un controllo non riuscito e visualizzare le entità interessate | `rao-view-latest-health-checks-assessment` | Adobe Experience Platform | &quot;Cosa c&#39;è che non va nella mia sandbox?&quot; · &quot;Informazioni sulla valutazione del controllo di integrità più recente&quot; · &quot;Quali sono i problemi relativi al controllo di descrizione dello spazio dei nomi personalizzato?&quot; |
| Correggi problemi di verifica stato | Correggi i problemi relativi a spazio dei nomi, criteri di unione e schema delle identità contrassegnate direttamente dalla chat, con la tua approvazione prima di apportare qualsiasi modifica | `rao-remediate-identity-namespace-description`, `rao-remediate-merge-policy-duplicate-name`, `rao-remediate-missing-audit-field-group`, `rao-remediate-default-merge-policy-naming` | Adobe Experience Platform | &quot;Correggi le descrizioni dello spazio dei nomi delle identità&quot; · &quot;Correggi i nomi dei criteri di unione duplicati&quot; · &quot;Correggi gli schemi senza il gruppo di campi di audit&quot; · &quot;Correggi la denominazione predefinita dei criteri di unione&quot; |

## Strumenti sandbox

| Caso d&#39;uso | Descrizione | Competenza | Applicazione | Prompt di esempio |
| --- | --- | --- | --- | --- |
| [Spostamento di oggetti tra sandbox](/help/agents/sandbox-tooling.md) | Migra facilmente schemi, tipi di pubblico e altre configurazioni di oggetti tra sandbox, con le dipendenze risolte automaticamente | `sandbox-tooling-workflow` | Adobe Experience Platform | &quot;Sposta lo schema Luma Loyalty Members Platinum dalla sandbox corrente alla sandbox di produzione&quot; · &quot;Promuovi il pubblico US Gold Loyalty Members allo stage&quot; |
