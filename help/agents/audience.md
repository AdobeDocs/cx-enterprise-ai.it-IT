---
title: Agente Audience
description: Scopri come utilizzare Audience Agent per creare tipi di pubblico, visualizzarne le modifiche, rilevare tipi di pubblico duplicati e visualizzarne le informazioni.
TQID: https://experienceleague.adobe.com/574QhqKI0YDoPHD9BFmB6jl-HET3zVom3eD4cJQABSE
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eb30f47f-d87a-400f-8f78-63ce7979ff56
source-git-commit: 130f2df3026a4ad948b314026ca5f1b71970d0b1
workflow-type: tm+mt
source-wordcount: 1242
ht-degree: 2%

---

# Agente Audience

>[!AVAILABILITY]
>
>Audience Agent è disponibile per tutti i clienti che hanno accesso all’Assistente per l’intelligenza artificiale. Tuttavia, per utilizzare completamente le funzioni di Audience Agent, sono necessarie le seguenti autorizzazioni.
>
>**Visualizza segmenti**: questa autorizzazione ti consente di utilizzare Audience Agent per visualizzare approfondimenti sui tipi di pubblico direttamente nell&#39;Assistente AI.
>
>**Gestisci segmenti**: con autorizzazione consente di utilizzare Audience Agent per creare nuovi tipi di pubblico direttamente nell&#39;Assistente IA.

Audience Agent consente di visualizzare informazioni sui tipi di pubblico, tra cui il rilevamento di modifiche significative nelle dimensioni del pubblico, il rilevamento di tipi di pubblico duplicati, l’esplorazione dell’inventario dei tipi di pubblico e il recupero delle dimensioni dei tipi di pubblico.

>[!SLIDE](audience-agent-overview)

## Casi d’uso supportati

Audience Agent nell’Assistente IA supporta i seguenti casi d’uso:

- Esplorare il pubblico in modo conversazionale
  - Trovare le dimensioni dei tipi di pubblico esistenti
  - Cerca tipi di pubblico basati su attributi completi o parziali denominati
  - Rilevare tipi di pubblico duplicati
  - Scopri i campi XDM da utilizzare per definire un pubblico
- Rilevare cambiamenti significativi nelle dimensioni del pubblico
  - Questo consente di trovare tipi di pubblico che sono improvvisamente cresciuti o si sono ridotti, per analizzare meglio i potenziali cambiamenti di mercato
- Creazione di un pubblico
  - Questa abilità ti consente di creare un pubblico in base agli attributi e agli eventi forniti
  - Inoltre, questa abilità ti consente di stimare le dimensioni potenziali di un pubblico prima di crearlo, consentendoti di eseguire rapidamente l’iterazione del pubblico più efficace prima che sia pronto per essere attivato

<!--
  - Find your audience size and detect significant changes in audience size
  - This lets you find audiences that have suddenly grown or shrunk, letting you better analyze potential market changes
- Detect duplicate audiences
  - This lets you reduce redundancies with your created audiences
- Find audiences based on full or partial attributes named
  - This lets you more easily navigate through your audience inventory
- Discover XDM fields you can use to define an audience
  - This skill lets you more easily identify the right fields to use in your audience based on context and relevance 
-->

Audience Agent non supporta **attualmente** la seguente funzionalità:

- Esplorazione del pubblico basata sugli obiettivi
  - L’esplorazione del pubblico basata sugli obiettivi consente di scoprire set di dati e profili rilevanti allineati a un obiettivo di business applicando modelli di apprendimento automatico come la propensione all’acquisto o alla conversione.

Inoltre, quando utilizzi Audience Agent, tieni presente i seguenti vincoli:

- Audience Agent richiede almeno 24 ore per elaborare i tuoi dati
  - **impossibile** ad esempio disporre di una query per la ricerca di dati nelle ultime 24 ore. Dovrai controllare almeno nelle ultime 48 ore.
- Audience Agent supporta solo i seguenti tipi di pubblico:
  - **Tipi di pubblico basati sulle persone** valutati mediante segmentazione batch
  - **Tipi di pubblico basati sull&#39;account** per i seguenti casi d&#39;uso:
    - Esplorazione del pubblico conversazionale
    - Rilevamento di pubblico duplicato

## Prompt di esempio

Negli esempi seguenti vengono illustrati i prompt di esempio e le risposte per Audience Agent.

### Esplorazione del pubblico conversazionale

Mostrami i campi per gli acquirenti benestanti.

+++ Risposta

![L&#39;Assistente AI mostra una tabella che mostra i campi rilevanti per gli acquirenti benestanti.](./assets/audience/affluent-buyers.png)

+++

Quali tipi di pubblico non sono stati attivati o utilizzati in alcuna campagna negli ultimi 30 giorni?

+++ Risposta

![L&#39;Assistente AI mostra una tabella che mostra i tipi di pubblico che non sono stati attivati o utilizzati nelle campagne negli ultimi 30 giorni.](./assets/audience/not-activated.png)

+++

Elenca tutti i tipi di pubblico che sono stati mappati sulle nuove destinazioni negli ultimi 3 mesi.

+++ Risposta

![L&#39;Assistente AI elenca il pubblico mappato a una nuova destinazione negli ultimi 3 mesi.](./assets/audience/new-destination.png)

+++

Quale pubblico dell’account ha la dimensione di pubblico più grande e qual è tale dimensione?

+++ Risposta

![L&#39;Assistente AI mostra una tabella che visualizza i tipi di pubblico dell&#39;account più grandi.](./assets/audience/largest-account-audience.png)

+++

### Rilevare tipi di pubblico duplicati

Ho tipi di pubblico con descrizioni identiche o simili?

+++ Risposta

![L&#39;Assistente AI visualizza una tabella contenente la definizione del segmento e i nomi dei tipi di pubblico con le stesse definizioni del segmento.](./assets/audience/similar-descriptions.png)

+++

Identifica i tipi di pubblico che hanno le stesse regole ma nomi diversi.

+++ Risposta

![L&#39;Assistente di IA visualizza una tabella contenente i nomi dei tipi di pubblico che condividono le stesse regole di pubblico.](./assets/audience/same-rules-different-names.png)

+++

Mostra tutti i tipi di pubblico che hanno le stesse regole ma destinazioni di attivazione diverse.

+++ Risposta

![L&#39;Assistente AI mostra che non sono presenti definizioni di segmenti duplicate in destinazioni diverse.](./assets/audience/same-rules-different-destinations.png)

+++

Identifica i tipi di pubblico dell’account che hanno le stesse regole ma nomi diversi.

+++ Risposta

![L&#39;Assistente IA visualizza una tabella contenente i nomi e gli ID dei tipi di pubblico dell&#39;account che condividono le stesse regole di pubblico.](./assets/audience/duplicate-account-audience.png)

+++

### Recupera dimensione pubblico

Qual è la dimensione attuale del mio pubblico &quot;Membri Gold-star in California_f153e1&quot;?

+++ Risposta

![L&#39;Assistente di IA indica le dimensioni correnti del pubblico a cui è stato chiesto di fornire informazioni.](./assets/audience/current-size.png)

+++

Qual è il mio pubblico più grande?

+++ Risposta

![L&#39;Assistente AI fornisce informazioni sul pubblico con il maggior numero di profili, inclusi nome e ID pubblico.](./assets/audience/largest-audience.png)

+++

### Rilevare cambiamenti significativi nelle dimensioni del pubblico

Quali tipi di pubblico sono aumentati di oltre il 20% nell’ultima settimana?

+++ Risposta

![L&#39;Assistente IA visualizza una tabella che elenca i nomi di tutti i tipi di pubblico che corrispondono alla query. Mostra inoltre l&#39;aumento percentuale, la dimensione corrente del pubblico e la dimensione precedente del pubblico.](./assets/audience/increase-past-week.png)

+++

Quali tipi di pubblico sono diminuiti di oltre il 10% nell’ultimo mese?

+++ Risposta

![L&#39;Assistente IA visualizza una tabella che elenca i nomi di tutti i tipi di pubblico che corrispondono alla query. Vengono inoltre visualizzate la dimensione del pubblico corrente, la dimensione del pubblico precedente e la data della dimensione del pubblico precedente.](./assets/audience/decrease-month.png)

+++

Qual è il mio pubblico in più rapida crescita?

+++ Risposta

![L&#39;Assistente AI indica il nome del pubblico in più rapida crescita, nonché le dimensioni correnti e la percentuale di crescita.](./assets/audience/fastest-growing.png)

+++

### Creazione di un pubblico

>[!AVAILABILITY]
>
>Puoi utilizzare l’abilità Crea pubblico solo se fai parte del programma Agent Orchestrator Explorer. Per ulteriori informazioni, contatta l’Assistenza clienti di Adobe.

Quando crei un pubblico con Audience Agent, l’Assistente AI ti guiderà attraverso un piano. Ad esempio, puoi chiedere di &quot;Creare un pubblico composto da persone che vivono in California&quot;. Assistente IA elenca quindi il piano che verrà intrapreso per creare il pubblico.

+++ Risposta

![L&#39;Assistente AI mostra il piano per la creazione di un pubblico.](./assets/audience/audience-create-plan.png)

+++

Il piano si articola in tre fasi:

1. [Identificare le caratteristiche del pubblico](#identify)
2. [Stimare la dimensione del pubblico](#estimate)
3. [Creare e mantenere un nuovo pubblico](#create)

#### Identificare le caratteristiche del pubblico {#identify}

![Passaggio 1 del piano, che consiste nell&#39;identificare le caratteristiche del pubblico.](./assets/audience/plan-step-1.png){align="center" width="80%"}

Dopo aver accettato il piano, l’Assistente AI acquisirà le caratteristiche del pubblico in base alla query iniziale.

+++ Risposta

![La definizione del pubblico basata sulla query utente.](./assets/audience/audience-create-definition.png)

Per questa query, l’Assistente AI genera il Profile Query Language (PQL) rilevante che cercherà le persone che vivono in California. In questo caso d’uso, la query PQL sarà simile alla seguente:

```sql
homeAddress.state.equals("California", false)
```

Per ulteriori informazioni su PQL, leggere la [panoramica di PQL](https://experienceleague.adobe.com/it/docs/experience-platform/segmentation/pql/overview).

+++

Se la definizione del pubblico dell’Assistente AI è corretta, puoi approvare e passare al passaggio successivo.

#### Stimare la dimensione del pubblico {#estimate}

![Passaggio 2 del piano, che consiste nel stimare la dimensione del pubblico potenziale.](./assets/audience/plan-step-2.png){align="center" width="80%"}

Dopo aver approvato le caratteristiche del pubblico identificato, AI Assistant stimerà le dimensioni del pubblico potenziale e i dettagli di definizione del pubblico.

+++ Risposta

![Viene visualizzata la stima di esempio per il pubblico potenziale. Vengono visualizzate la dimensione stimata e la definizione del segmento.](./assets/audience/audience-create-estimate.png)

+++

Se la dimensione stimata è corretta, puoi approvare e passare al passaggio successivo.

#### Creare e mantenere un nuovo pubblico {#create}

![Passaggio 3 del piano, che consiste nel completare la creazione del pubblico.](./assets/audience/plan-step-3.png){align="center" width="80%"}

Infine, se le caratteristiche e le dimensioni del pubblico sono corrette, puoi approvare o rifiutare la creazione del pubblico.

+++ Risposta

Innanzitutto, puoi esaminare il pubblico proposto tramite la griglia dati fornita.

![Viene visualizzata la schermata di revisione.](./assets/audience/audience-create-review.png)

Se il pubblico è corretto, puoi accettare la proposta selezionando **[!UICONTROL Crea]** per completare la creazione del pubblico.

![Viene visualizzata la proposta completa per il pubblico.](./assets/audience/audience-create-proposal.png)

+++

Il pubblico viene ora creato.

![La proposta di pubblico è stata accettata e il pubblico è stato creato.](./assets/audience/audience-finish-create.png){align="center" width="80%"}

## Passaggi successivi

Dopo aver letto questa guida, avrai una migliore comprensione di Audience Agent e delle funzioni che supporta. Per ulteriori informazioni sugli agenti in Adobe Experience Platform, leggere la [panoramica di Agent Orchestrator](./agent-orchestrator.md).

