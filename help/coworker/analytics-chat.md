---
title: Analizzare i dati di Customer Journey Analytics con Chat con i collaboratori
description: Scopri come utilizzare Adobe CX Enterprise Collaborator Chat per analizzare i dati di Customer Journey Analytics, creare funnel e individuare i punti di contatto dei clienti nel percorso.
source-git-commit: 6e3ab12f1d9ec706e745749b7ca47b91a09ff8b3
workflow-type: tm+mt
source-wordcount: '2104'
ht-degree: 4%

---

# Analizzare i dati di Customer Journey Analytics con Chat con i collaboratori

>[!AVAILABILITY]
>
>La funzionalità descritta in questo articolo è nella fase di test limitato del rilascio e potrebbe non essere ancora disponibile nell’ambiente. Questa nota verrà rimossa quando la funzionalità sarà generalmente disponibile. Per informazioni sulla procedura di rilascio di Customer Journey Analytics, vedere [Versioni delle funzionalità di Customer Journey Analytics](https://experienceleague.adobe.com/it/docs/analytics-platform/using/releases/latest).

Adobe CX Enterprise Collaborator Chat può eseguire analisi avanzate dei dati che in precedenza erano possibili solo in Analysis Workspace. Chat con collaboratori accede ai dati dalle visualizzazioni dati di Customer Journey Analytics, consentendoti di esplorarli e ottenere risposte a prompt in linguaggio naturale.

Prima di iniziare l’analisi, scopri l’interfaccia e le opzioni di configurazione di Chat per collaboratori, quindi assicurati che Customer Workfront sia connesso a Customer Journey Analytics e alla visualizzazione dati che contiene i dati che desideri utilizzare.

## Introduzione alla chat con i collaboratori

### Opzioni di interfaccia e configurazione

Prima di utilizzare Chat con collaboratori con i dati di Customer Journey Analytics, scopri come accedere e gestire le opzioni di configurazione per le seguenti funzioni:

* Input chat

* Conversazioni

* Marketplace

* Server MCP

* Memoria

* Plug-in

* Abilità

* E altro ancora

Per ulteriori informazioni, consulta la [Guida dell&#39;interfaccia utente di Chat per collaboratori](https://experienceleague.adobe.com/it/docs/cx-enterprise-coworker/content/chat/ui-guide).

### Casi d’uso per Customer Journey Analytics

È possibile visualizzare casi di utilizzo di Customer Journey Analytics e prompt di esempio utilizzati dai professionisti in Adobe CX Enterprise Chat per collaboratori. Ogni prompt viene creato per essere copiato, adattato con i propri dati e contesto e perfezionato attraverso la conversazione.

Per ulteriori informazioni, vedi [Casi d&#39;uso](https://experienceleague.adobe.com/it/docs/cx-enterprise-coworker/content/chat/use-cases).

## Verifica che Chat con i collaboratori sia connessa a Customer Journey Analytics

1. In Chat con collaboratori, verifica che Coworker sia connesso a Customer Journey Analytics:

1. Seleziona l&#39;icona MCP nella barra a sinistra, quindi accertati che [!UICONTROL **cja-mcp**] sia disponibile nell&#39;elenco dei server MCP connessi.

   ![L&#39;icona MCP è evidenziata nella barra a sinistra di Collaboratore](assets/data-validation-aa-cja/coworker-mcp-cja.png)

1. (Condizionale) Se [!UICONTROL **cja-mcp**] non è ancora connesso, selezionare [!UICONTROL **Aggiungi server MCP**], specificare cja nel campo [!UICONTROL **Nome server**] e selezionarlo quando viene visualizzato, quindi selezionare [!UICONTROL **Aggiungi server**].

## Connettersi alla visualizzazione dati corretta

Una visualizzazione dati è un contenitore in Customer Journey Analytics che determina il modo in cui i dati vengono interpretati.

Potresti avere accesso a varie visualizzazioni dati in Customer Journey Analytics, ciascuna contenente dimensioni e metriche diverse che puoi utilizzare durante l’analisi dei dati.

### Decidere quali visualizzazioni dati utilizzare

Comunica al collega i tipi di domande a cui desideri rispondere e chiedi a quali visualizzazioni dati hai accesso e cosa è meglio fornire tali informazioni. Puoi anche [impostare la visualizzazione dati come preferenza in memoria](#add-a-data-view-preference-in-memory).

**Utente:**

>[!BEGINSHADEBOX]

Sono interessato a capire dove i clienti abbandonano nel percorso dei clienti. A quali visualizzazioni dati in Customer Journey Analytics posso accedere per rispondere a questa domanda?

>[!ENDSHADEBOX]

**Risposta chat collaboratore:**

>[!BEGINSHADEBOX]

Puoi accedere a tre visualizzazioni dati. La visualizzazione dati `Customer lifecycle` contiene le dimensioni e le metriche seguenti, che sono le migliori per rispondere alla domanda.

>[!ENDSHADEBOX]

**Utente:**

>[!BEGINSHADEBOX]

Bene, usiamo quella visualizzazione dati.

>[!ENDSHADEBOX]

**Risposta chat collaboratore:**

>[!BEGINSHADEBOX]

Ok, utilizzerò la visualizzazione dati `Customer lifecycle` per rispondere a domande future in questa sessione di chat.

>[!ENDSHADEBOX]

### Aggiungere una preferenza per la visualizzazione dati in memoria

La chat di Coworker contiene una funzione di memoria che ti consente di fornire accesso a informazioni che si estendono su tutte le chat. È buona prassi aggiungere le visualizzazioni dati preferite come preferenze nella memoria di Coworker.

1. In Chat con collaboratori, nella barra di navigazione a sinistra, seleziona l’icona Memoria.

1. Nella sezione Preferenze memorizzate della pagina Memoria, specifica una o più visualizzazioni dati da utilizzare nelle chat di Collaborator Chat.

   ![Sezione memoria nella barra a sinistra](assets/data-validation-aa-cja/coworker-memory.png)

## Analizzare in Customer Journey Analytics

Dopo aver creato una visualizzazione, puoi aprirla in Analysis Workspace in Customer Journey Analytics per un’analisi più approfondita con un controllo più granulare. La visualizzazione si apre in un nuovo progetto Analysis Workspace in Customer Journey Analytics.

Per aprire una visualizzazione in un nuovo progetto Analysis Workspace:

1. Seleziona [!UICONTROL **Analizza in CJA**] accanto a qualsiasi visualizzazione creata in Coworker.

1. Con la visualizzazione aperta in Customer Journey Analytics, puoi utilizzare l’interfaccia del browser drag-and-drop di Analysis Workspace per apportare modifiche, definire ulteriormente l’analisi, creare un pubblico e molto altro. Puoi anche condividere il tuo progetto Workspace con chi desideri.

   Per ulteriori informazioni su Analysis Workspace, consulta [Panoramica di Analysis Workspace](https://experienceleague.adobe.com/it/docs/analytics-platform/using/cja-workspace/home).

## Esempio: individuare il punto di partenza dei clienti

Puoi chiedere a Chat con i colleghi di utilizzare i tuoi dati per analizzare qualsiasi domanda di business.

Ad esempio, in qualità di responsabile marketing, merchandiser o lead di crescita, potresti voler capire dove i clienti abbandonano il percorso di acquisto, perché lo hanno fatto e cosa si può fare per aumentare i tassi di conversione.

>[!NOTE]
>
>Le figure seguenti sono dati di esempio illustrativi per un retailer fittizio, [!DNL TechPulse Electronics], utilizzato per mostrare la forma della conversazione.

### I tipi di domande che è possibile porre

Non è necessario sapere cos’è una &quot;visualizzazione di abbandono&quot; o quale metrica entra in quale slot. Descrivi invece il risultato a cui tieni in considerazione in un linguaggio semplice:

* &quot;Dove stiamo perdendo la gente sulla via dell&#39;acquisto?&quot;
* &quot;Qual è il mio funnel di conversione completo, dalla visualizzazione del prodotto al pagamento?&quot;
* &quot;Quali canali di marketing perdono di più tra il carrello e l’acquisto?&quot;
* &quot;L’abbandono del carrello è peggiore su dispositivi mobili o desktop?&quot;
* &quot;Le persone dei social network a pagamento si convertono in modo diverso rispetto alle persone delle e-mail?&quot;

### La conversazione

#### &#x200B;1. Inizia con la domanda di business

**Utente:**

>[!BEGINSHADEBOX]

Dove stiamo perdendo la gente sulla strada per l&#39;acquisto?

>[!ENDSHADEBOX]

**Risposta chat collaboratore:**

Tieni presente che Chat con i collaboratori sceglie la visualizzazione corretta, sequenzia i punti di contatto e aggiunge anche i passaggi successivi consigliati.

>[!BEGINSHADEBOX]

![Risposta di Collaboratore funnel](assets/data-validation-aa-cja/coworker-funnel-response.png)

Questa è una domanda di funnel — lasciate che esegua il funnel di conversione per vedere dove avviene il drop-off sul percorso di acquisto.

Ecco dove stai perdendo delle persone:

| Passaggio funnel | Count | Conversione al successivo | Dispersione |
| --- | --- | --- | --- |
| Sessions | 137,476 | 45,0% visualizza un prodotto | 55% di abbandono senza navigazione dei prodotti |
| Visualizzazioni di prodotti | 61,845 | 55,0% aggiungi al carrello | 45% navigazione ma non aggiunta |
| Aggiunte al carrello | 34,045 | Acquisto del 16,4% | 83,6% carrello di abbandono |
| Acquisti | 5,582 | — | — |

**Il grande risultato: il carrello da acquistare è la tua perdita più grande**

28.463 persone aggiungono articoli al carrello ma non completano mai l’acquisto. Si tratta di un tasso di abbandono dell&#39;83,6% tra carrello e acquisto, di gran lunga il più grande singolo punto di errore.

In termini di dollari, la conversione di appena il 10% in più di quei caricatori aggiungerebbe circa 2.846 acquisti. Con la scala dati corrente, si tratta di ricavi potenzialmente significativi rimasti sul tavolo.

**Informazioni sulle priorità:**

| Priorità | Problema | Scala delle opportunità |
| --- | --- | --- |
| #1 | Abbandono carrello all’acquisto (calo dell’83,6%) | 28.463 acquirenti persi |
| #2 | Sessione alla visualizzazione prodotto (il 55% non naviga mai) | 75.631 sessioni senza coinvolgimento con il prodotto |
| #3 | Visualizzazione prodotto al carrello (il 45% non viene aggiunto) | 27.800 interessati ma non impegnati |

**Passaggi successivi consigliati:**

1. Suddividere l’abbandono del carrello per canale di marketing: alcuni canali generano traffico a basso intento che si aggiunge al carrello ma non acquista mai?
1. Osservare l&#39;abbandono del carrello per tipo di dispositivo — l&#39;attrito del checkout mobile uccide le conversioni?
1. Individuare i prodotti più abbandonati: problemi di prezzo? Sorpresa sulla spedizione?

**In quali casi vuoi che mi occupi io?** La suddivisione del canale ti direbbe direttamente quali azioni di marketing ti stanno portando &quot;quasi-acquirenti&quot; rispetto agli acquirenti effettivi.

>[!ENDSHADEBOX]

#### &#x200B;2. Eseguire un drill-through nella perdita

**Utente:**

>[!BEGINSHADEBOX]

Ok, suddividiamo per canale di marketing

>[!ENDSHADEBOX]

**Risposta chat collaboratore:**

>[!BEGINSHADEBOX]

![Risposta di Collaboratore funnel](assets/data-validation-aa-cja/coworker-funnel-response2.png)

È presente una dimensione **Canale di marketing** personalizzata. Lasciate che prenda il funnel in questo modo, poi calcoli i tassi di conversione per canale e identifichi dove ogni canale perde.

**Il verdetto: la perdita non è specifica del canale**

Questo è un risultato davvero rivelatore. Ecco il raggruppamento per canale di funnel:

| Canale | Sessions | Alla vista prodotto | Da aggiungere al carrello | Per acquistare | Conversione globale | Ricavi/sessione |
| --- | --- | --- | --- | --- | --- | --- |
| Ricerca a pagamento | 43,958 | 45.1% | 54.6% | 16.6% | 4.09% | $499.58 |
| Ricerca organica | 31,492 | 44.9% | 54.9% | 16.9% | 4.17% | $494.76 |
| Diretto | 25,661 | 43.6% | 55.4% | 15.8% | 3.82% | $497.29 |
| E-mail | 17,586 | 45.3% | 55.4% | 16.2% | 4.07% | $501.13 |
| Social network a pagamento | 12,684 | 45.4% | 55.7% | 16.0% | 4.03% | $512.17 |
| Visualizzazione | 6,511 | 45.3% | 55.7% | 16.2% | 4.09% | $501.45 |

**Attività principali:**

1. Il tasso di caduta da carrello ad acquisto è uniformemente negativo su tutti i canali (83-84%). Questo significa che il problema non riguarda la qualità del traffico — ogni canale offre visitatori coinvolti in modo simile. La perdita si trova nell’esperienza di pagamento stessa, non nel marketing.
1. Nessun canale è significativamente migliore o peggiore nella conversione. I tassi di conversione complessivi si concentrano strettamente tra il 3,8% e il 4,2% e i ricavi per sessione sono quasi identici (495-512 dollari).
1. Dove l’impatto del volume conta di più: la ricerca a pagamento perde il maggior numero di persone in termini assoluti (9,015 abbandoni del carrello), seguita dalla ricerca organica (6,449 persi). Queste sono le maggiori opportunità di valore in dollari perché guidano più traffico.

**Informazioni strategiche**

I canali di marketing stanno facendo il loro lavoro — tutti fanno sì che la gente si interessi e aggiunga al carrello a ritmi simili. Il problema è a valle del marketing: il vostro pagamento e pagamento è dove il denaro sta perdendo.

**Ricerche successive consigliate:**

1. Suddividere l’abbandono del carrello per tipo di dispositivo: il checkout mobile è interrotto o frustrante?
1. Guarda quali prodotti vengono abbandonati di più — c&#39;è una sorpresa di prezzo o di spedizione al pagamento?
1. Controlla se la campagna &quot;Holiday_flash_sale&quot; ha avuto una migliore conversione del pagamento — le campagne basate sull’urgenza potrebbero superare l’attrito del pagamento

**Scegliere l&#39;angolo da esplorare.**

>[!ENDSHADEBOX]

#### &#x200B;3. Continua a indagare

**Utente:**

>[!BEGINSHADEBOX]

Interessante. Proviamo a suddividerci per tipo di dispositivo.

>[!ENDSHADEBOX]

**Risposta chat collaboratore:**

>[!BEGINSHADEBOX]

![Risposta di Collaboratore funnel](assets/data-validation-aa-cja/coworker-funnel-response3.png)

**Trovato: il checkout mobile è interrotto**

Il funnel è identico tra i dispositivi fino al momento del check-out, quindi il dispositivo mobile cade da un precipizio:

| Dispositivo | Sessions | Alla vista prodotto | Da aggiungere al carrello | Per acquistare | Conversione globale |
| --- | --- | --- | --- | --- | --- |
| Desktop | 70,172 | 44.9% | 54.8% | 23.2% | 5.70% |
| Tablet | 14,149 | 44.7% | 55.6% | 14.3% | 3.56% |
| Mobile | 53,449 | 44.9% | 55.3% | 8.1% | 2.02% |

**La pistola fumante**

| Metrica | Desktop | Mobile | Intervallo |
| --- | --- | --- | --- |
| Percentuale da carrello ad acquisto | 23.2% | 8.1% | 15 punti percentuali |
| Mobile è | — | 2,8x peggiore | — |
| Carrelli abbandonati | 13,274 | 12,178 | Quasi lo stesso volume assoluto |

L’esperienza di navigazione e di aggiunta al carrello è ottimale per i dispositivi mobili (tasso di navigazione identico al 45%, tasso di aggiunta al carrello pari al 55%). Le persone sono interessate e coinvolte allo stesso modo. Ma qualcosa nel flusso delle casse mobili uccide le conversioni.

**L&#39;opportunità di ricavo**

Se il checkout mobile viene convertito alla stessa velocità del desktop, si otterrebbero circa 1.991 acquisti aggiuntivi, con un aumento del 35% del volume totale degli acquisti dalla correzione di un&#39;esperienza.

**Cosa potrebbe succedere**

Il pattern dei dati (coinvolgimento uguale, calo catastrofico del checkout) è un segnale classico per:

* Limitazione del modulo di pagamento su schermi di piccole dimensioni (problemi di riempimento automatico, layout del modulo)
* Costi imprevisti rilevati al momento del pagamento (spedizione, imposte) che causano shock da adesivo
* Il checkout dell’ospite non è disponibile o una bacheca di accesso su dispositivi mobili
* Problemi di caricamento pagina o timeout durante l’elaborazione del pagamento su dispositivi mobili

**Passaggi successivi consigliati:**

1. Suddividere l’abbandono del carrello mobile per categoria di prodotto: è peggio per gli articoli a prezzo elevato (suggerendo problemi di attendibilità per i pagamenti mobili)?
1. Osserva quali canali di marketing sono più determinanti per il traffico mobile: stai spendendo dollari dei media pagati per inviare persone verso un funnel mobile non funzionante?
1. Controlla se c&#39;è un segnale nella pagina o nella sezione del sito: possiamo vedere quali pagine di pagamento sono state visitate per ultime dagli utenti di dispositivi mobili prima di abbandonarle?

**Quali elementi vuoi esplorare o queste prove sono sufficienti per indirizzare l&#39;utente e il team di checkout?**

>[!ENDSHADEBOX]

#### &#x200B;4. Trasformalo in una decisione

**Utente:**

>[!BEGINSHADEBOX]

Quindi cosa dovrei fare?

>[!ENDSHADEBOX]

**Risposta chat collaboratore:**

>[!BEGINSHADEBOX]

In base a ciò che mostrano i dati, ecco dove vorrei concentrarmi:

* **Correggi l&#39;estrazione mobile. Non si tratta di un problema di canale.** Ogni canale converte le persone nel carrello a un ritmo sano e simile, in modo che la spesa pubblicitaria funzioni in modo trasversale. I ricavi vengono persi in modo specifico nel flusso di pagamento mobile, che è il luogo in cui appartiene la correzione.
* **Inizia con il pagamento e con l&#39;attrito del modulo.** Questi sono i motivi più comuni per cui gli acquirenti di dispositivi mobili ad alto intento abbandonano il carrello. L&#39;offerta di opzioni per il portafoglio mobile e la riduzione della forma sono di solito le vincite più veloci.
* **Controlla di nuovo dopo la correzione.** Una volta che il pagamento cambia spedizione, osserva se il tasso di acquisto del carrello mobile si sposta verso il tasso desktop del 23,2%.

Vuoi che salvi questo come progetto in modo da poterlo tenere traccia, o che imposti un avviso se il carrello mobile da acquistare scende al di sotto di una soglia?

>[!ENDSHADEBOX]

### Cos’è appena successo

In quattro semplici domande, Coworker ci ha aiutato:

* Costruisci un funnel di conversione in più passaggi e contrassegna il carrello da acquistare come la perdita più grande
* Escludi canale di marketing come causa: ogni canale ha registrato perdite quasi equivalenti
* Individua il problema reale al pagamento mobile e quantifica la correzione con un incremento del 35% negli acquisti
* Approfitta di una correzione specifica per definire le priorità: pagamenti mobili e attrito tra moduli. Questo è confrontato con il tasso di conversione del 23,2% del desktop

<!--

## Example #2: Find which marketing efforts drive revenue

You can ask Coworker Chat to use your data to analyze any business question.

For example, as a marketing manager, demand generation lead, or CMO, you might want to know which marketing efforts actually deserve credit for revenue so you can confidently decide where to put your marketing spend, rather than rewarding whichever channel happened to get the last click.

>[!NOTE]
>
>The figures below are illustrative sample data for a fictional retailer, [!DNL TechPulse Electronics], used to show the shape of the conversation.

### The types of questions you can ask

You don't need to know what an "attribution model" is, or how to configure an Attribution panel. Instead, describe the outcome you care about in plain language:

* "Which channels actually drive our revenue, not just the last click?"
* "If I change how I give credit for a sale, does my best channel change?"
* "Which campaigns start customer journeys versus close them?"
* "Am I over-investing in paid search because it always gets the last click?"
* "What role does email play in conversions it never gets credit for?"

### The conversation

#### 1. Start with the business question

**You:**

>[!BEGINSHADEBOX]

Which marketing channels actually drive our revenue?

>[!ENDSHADEBOX]

**Coworker Chat response:**

Notice that Coworker Chat picks the right analysis, starts with the model most reports default to, and immediately flags what that model can't tell you.

>[!BEGINSHADEBOX]

![Coworker Chat showing attributed revenue by marketing channel under a last-touch model](assets/data-validation-aa-cja/coworker-attribution-response.png)

This is an attribution question — let me attribute revenue to your marketing channels so you can see who's earning it.

I'll start with **last-touch attribution**, since that's what most out-of-the-box reports show. It gives all the credit for a sale to the last channel a person used before purchasing.

| Marketing channel | Attributed revenue (last touch) | Share |
| --- | --- | --- |
| Paid search | $948,000 | 34% |
| Organic search | $614,000 | 22% |
| Direct | $474,000 | 17% |
| Email | $307,000 | 11% |
| Paid social | $251,000 | 9% |
| Display | $195,000 | 7% |

**The headline: paid search looks like your hero**

Under last touch, paid search earns a third of all revenue — more than any other channel. If this were the only view you had, you'd likely pour more budget into paid search.

**One important caveat before you do that**

Last touch only tells you who *closed* the sale. It says nothing about who *started* the journey or *assisted* along the way. A channel that introduces people to your brand weeks before they buy gets zero credit here, even if the purchase never would've happened without it.

To know whether paid search is really driving revenue — or just harvesting demand other channels created — you need to compare attribution models.

**Recommended next step:**

Compare the same channels across first-touch, last-touch, and linear models. If paid search stays on top across all of them, it's a genuine driver. If it shrinks under first touch, it's a closer, not a creator.

**Want me to run that comparison?**

>[!ENDSHADEBOX]

#### 2. Compare attribution models

**You:**

>[!BEGINSHADEBOX]

Yes, compare it across models.

>[!ENDSHADEBOX]

**Coworker Chat response:**

>[!BEGINSHADEBOX]

![Coworker Chat comparing channel revenue share across first-touch, last-touch, and linear attribution models](assets/data-validation-aa-cja/coworker-attribution-response2.png)

Here's each channel's share of revenue under three models. First touch credits the channel that started the journey, last touch credits the one that closed it, and linear splits credit evenly across every touch.

| Marketing channel | First touch | Last touch | Linear |
| --- | --- | --- | --- |
| Paid search | 19% | 34% | 26% |
| Organic search | 20% | 22% | 21% |
| Direct | 9% | 17% | 13% |
| Email | 18% | 11% | 15% |
| Paid social | 21% | 9% | 15% |
| Display | 13% | 7% | 10% |

**The verdict: your "best" channel depends entirely on how you count**

This is the finding that changes budget decisions.

1. **Paid search closes far more than it starts.** It jumps from 19% of first touches to 34% of last touches. That's the signature of a *harvester* — it captures people who are already ready to buy, often after another channel introduced them. Valuable, but it's finishing journeys, not creating them.
1. **Paid social and email are badly undercredited by last touch.** Paid social starts 21% of journeys but gets credit for only 9% of sales. Email starts 18% but closes 11%. These channels are doing the expensive work at the top of the funnel and handing warm prospects to paid search.
1. **Organic search is your steady workhorse.** It sits around 20% across every model — it both starts and closes journeys reliably.

**Why this matters for budget**

If you cut paid social or email based on their weak last-touch numbers, you'd starve the top of your funnel — and paid search would have far fewer ready-to-buy people to close. You'd likely see paid search revenue fall too, even though you didn't touch its budget.

**Recommended next step:**

Look at the campaign level to see exactly which efforts start journeys versus close them. That's where you can act — trimming or protecting specific campaigns rather than whole channels.

**Want me to break this down by campaign?**

>[!ENDSHADEBOX]

#### 3. Keep investigating

**You:**

>[!BEGINSHADEBOX]

Let's break it down by campaign.

>[!ENDSHADEBOX]

**Coworker Chat response:**

>[!BEGINSHADEBOX]

![Coworker Chat showing top campaigns ranked by their role as initiators or closers of customer journeys](assets/data-validation-aa-cja/coworker-attribution-response3.png)

There's a **Campaign Name** dimension. Here are your highest-involvement campaigns, comparing the revenue they start (first touch) against the revenue they close (last touch).

| Campaign | Starts (first touch) | Closes (last touch) | Role |
| --- | --- | --- | --- |
| brand_awareness_q3 | $412,000 | $103,000 | Initiator |
| email_winback | $214,000 | $88,000 | Initiator |
| holiday_flash_sale | $268,000 | $249,000 | All-rounder |
| retargeting_dynamic | $71,000 | $339,000 | Closer |
| branded_search_always_on | $84,000 | $498,000 | Closer / harvester |

**The pattern: some of your "worst" campaigns are actually your best starters**

* **brand_awareness_q3** and **email_winback** start far more revenue than they close. On a last-touch ROI report, these look like underperformers you might cut. In reality, they're filling the top of your funnel — the journeys other campaigns finish.
* **retargeting_dynamic** and **branded_search_always_on** are the opposite. They close a lot but start almost nothing. They're efficient closers, but they can only close demand that already exists. Branded search, in particular, is largely capturing people who were going to search for you by name anyway.
* **holiday_flash_sale** does both — it introduces new shoppers and closes them, which is why urgency-driven promotions often look strong under any model.

**What this tells you strategically**

The campaigns you'd cut first on a last-touch report — the awareness and win-back efforts — are the ones creating the demand your closers depend on. Judge initiators on the journeys they start, and closers on the journeys they finish.

**Recommended next steps:**

1. Protect the initiator campaigns even though their last-touch ROI looks weak — they're feeding the funnel.
1. Right-size the branded search spend — test whether trimming it changes total revenue, since much of that demand may convert anyway.
1. Adopt a balanced model — like linear or a position-based model — as your default reporting view, so no channel gets systematically over- or under-rewarded.

**Want me to save this as a project, or is this enough to take into your budget planning?**

>[!ENDSHADEBOX]

#### 4. Turn it into a decision

**You:**

>[!BEGINSHADEBOX]

So how should I allocate budget?

>[!ENDSHADEBOX]

**Coworker Chat response:**

>[!BEGINSHADEBOX]

Based on what the data shows, here's where I'd focus:

* **Stop judging upper-funnel channels on last touch alone.** Paid social and email start about 20% of your revenue each, but last touch credits them for less than half of that. Protect their budgets — they're creating the demand paid search closes.
* **Treat branded search as a harvester, not a driver.** It closes a lot but starts almost nothing. Test trimming it, since much of that demand may convert through other paths anyway.
* **Make a balanced model your default.** Reporting on linear or a position-based model instead of last touch will stop you from over-rewarding closers and under-funding the channels that start journeys.
* **Re-check after you rebalance.** Watch whether total revenue holds steady as you shift spend toward initiators — that's the signal your funnel is healthier, not just your last-touch report.

Want me to save this as a project so you can track it, or build a calculated metric that reports revenue on a balanced attribution model going forward?

>[!ENDSHADEBOX]

### What just happened

In four plain-language questions, Coworker helped us:

* Attribute revenue to marketing channels and flag that the default last-touch view tells only part of the story
* Compare attribution models and reveal that the "best" channel changes completely depending on how credit is counted
* Discover that paid social and email start far more revenue than they ever get credit for closing
* Identify which campaigns initiate journeys versus close them, and walk away with a budget direction: protect the initiators, right-size the harvesters, and report on a balanced model

-->
