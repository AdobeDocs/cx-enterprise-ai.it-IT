---
title: Agente di gestione dati per Adobe Experience Platform
description: Scopri come utilizzare l’agente di gestione dati in CX Coworker per trovare e analizzare i set di dati di Adobe Experience Platform e gestire i criteri di conservazione dei data lake.
source-git-commit: 40f144c7a06592c78dccc6c17f19554b62f667c9
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 3%
---
# Agente di gestione dati

>[!AVAILABILITY]
>
>L’agente di gestione dati è disponibile per tutti i clienti con accesso ad Adobe CX Enterprise Coworker.

Per comprendere e gestire la conservazione del data lake per i set di dati Experience Event, utilizza Data Management Agent in CX Coworker. Con la crescita dei set di dati Experience Event nel data lake di Adobe Experience Platform, il completamento delle query e dei processi a valle può richiedere più tempo, mentre i requisiti di conservazione diventano più difficili da gestire. Descrivi cosa desideri realizzare in linguaggio naturale. L’agente di gestione dati trova i set di dati Experience Event rilevanti, analizza il modo in cui vengono utilizzati attivamente e modella la quantità di dati che un periodo di conservazione proposto influirebbe. Quando sei pronto ad agire, ti consente di impostare, modificare o rimuovere un criterio di conservazione e richiede la tua conferma prima di qualsiasi modifica.

## Funzionamento dell&#39;agente di gestione dati {#what-the-data-management-agent-can-do}

L’agente di gestione dati fornisce quattro competenze.

>[!NOTE]
>
>Le competenze Elenco set di dati, Analisi dell’utilizzo set di dati e Analisi della conservazione dei set di dati sono di sola lettura. Solo l’abilità Gestisci conservazione dei set di dati può modificare i criteri di conservazione di un data lake e richiede una conferma esplicita prima di applicare qualsiasi modifica.

| Competenza | Descrizione |
|---|---|
| **Elenca set di dati** | Utilizzare quando si decide dove avviare una revisione della conservazione. Elenca i set di dati Experience Event con le dimensioni di archiviazione, il conteggio delle righe, le impostazioni di conservazione esistenti e l’abilitazione del profilo, per identificare rapidamente i set di dati potenzialmente idonei per un criterio di conservazione del data lake |
| **Analisi dell&#39;utilizzo del set di dati** | Da utilizzare prima di decidere se un set di dati è adatto per i criteri di conservazione di un data lake. Classifica il modo in cui viene utilizzato attivamente un set di dati specifico in base a segnali quali acquisizione recente, attività di query e utilizzo di applicazioni a valle. |
| **Analizzare la conservazione dei set di dati** | Utilizzare prima di eseguire il commit a un periodo di conservazione. Mostra le metriche di archiviazione di un set di dati e l’età dei relativi dati, quindi utilizza tale distribuzione di età per approssimare la quantità di dati che un potenziale periodo di conservazione manterrebbe o rimuoverebbe. |
| **Gestione conservazione set di dati** | Usa quando sei pronto ad agire. Imposta, modifica o rimuove un criterio di conservazione del data lake su un set di dati, con un’anteprima di impatto e una conferma prima di qualsiasi modifica. |

## Ambito: conservazione dei data lake rispetto ad altri strumenti di gestione dati {#scope}

Utilizza Data Management Agent quando devi trovare e analizzare i set di dati di Experience Event e impostare, modificare o rimuovere un criterio di conservazione del data lake.

Se non si è sicuri che i criteri di conservazione del data lake siano l&#39;opzione giusta per l&#39;obiettivo, vedere [Scegliere la funzionalità di gestione del ciclo di vita dei dati appropriata](https://experienceleague.adobe.com/it/docs/experience-platform/data-lifecycle/choose-a-capability) per confrontare le opzioni di conservazione ed eliminazione disponibili.

Queste abilità non gestiscono le seguenti funzionalità correlate:

- **Criteri di conservazione archivio profili.** Per gestire la durata della permanenza degli eventi esperienza nell’archivio Profili, configura i criteri di scadenza degli eventi esperienza nei set di dati degli eventi esperienza abilitati per il profilo. Vedi [Scadenza evento esperienza](https://experienceleague.adobe.com/it/docs/experience-platform/profile/event-expirations).
- **Scadenza dati profilo pseudonimo a livello di sandbox.** Per eliminare automaticamente i dati di profilo pseudonimi in una sandbox quando soddisfano le condizioni configurate, vedere [Profili pseudonimi](https://experienceleague.adobe.com/it/docs/experience-platform/profile/pseudonymous-profiles).
- **Scadenza set di dati.** Per pianificare l&#39;eliminazione di un intero set di dati in una data futura, vedere [Scadenza set di dati](https://experienceleague.adobe.com/it/docs/experience-platform/data-lifecycle/ui/dataset-expiration).
- **Eliminazione record.** Per rimuovere singoli record di profilo per motivi di privacy o igiene, vedere [Eliminazione record](https://experienceleague.adobe.com/it/docs/experience-platform/data-lifecycle/ui/record-delete).

## Prerequisiti {#prerequisites}

Prima di iniziare, assicurati di avere:

- Accedi a Adobe Experience Platform e alla sandbox che contiene i set di dati da rivedere.
- Le autorizzazioni Adobe Experience Platform necessarie per i set di dati e le azioni di conservazione che desideri utilizzare. L’agente di gestione dati utilizza le autorizzazioni Experience Platform esistenti e non concede l’accesso aggiuntivo. Per informazioni sul funzionamento delle autorizzazioni e dei ruoli di Adobe Experience Platform, vedere [Panoramica sul controllo degli accessi](https://experienceleague.adobe.com/it/docs/experience-platform/access-control/home).
- Il plug-in Adobe CXO installato in CX Collaborator.

Per istruzioni sull&#39;installazione dei plug-in, consulta la [Guida dell&#39;interfaccia utente di Coworker](https://experienceleague.adobe.com/it/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide).

## Utilizzare Data Management Agent {#use-the-data-management-agent}

Interagisci con Data Management Agent tramite CX Coworker utilizzando il linguaggio naturale. Descrivi il tuo obiettivo, quindi perfeziona i risultati con domande di follow-up.

>[!NOTE]
>
>Prima di iniziare, assicurati di lavorare nella sandbox che contiene i set di dati da rivedere.

Per utilizzare Data Management Agent:

1. Passare a **[!UICONTROL CX Collaboratore]**. Per informazioni dettagliate sull&#39;accesso, vedere la [Guida all&#39;interfaccia utente di Collaborator](https://experienceleague.adobe.com/it/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide).
1. Immettere una richiesta che descriva ciò che si desidera eseguire.
1. Rivedi i risultati e utilizza le domande di follow-up per continuare la tua indagine.

Se una richiesta modifica un criterio di conservazione di un data lake, Data Management Agent mostra l’impatto proposto e richiede la tua conferma prima di applicare la modifica.

Per un flusso di lavoro end-to-end per l&#39;identificazione dei set di dati, l&#39;analisi dell&#39;impatto di utilizzo e conservazione e la gestione dei criteri di conservazione dei data lake, vedere [Gestione della conservazione dei data lake](../coworker/chat/use-cases/data-management/manage-data-lake-retention.md).

## Funzionamento di Data Management Agent {#how-the-data-management-agent-works}

Data Management Agent utilizza calcoli deterministici per analizzare l’utilizzo dei set di dati, in modo che gli stessi input producano lo stesso livello di utilizzo. Inoltre, calcola l’impatto sulla conservazione a livello di programmazione anziché affidarsi a stime generate dall’intelligenza artificiale. L’impatto sulla conservazione rimane un’approssimazione perché si basa sulla distribuzione per età dei dati. L’agente recupera i dati direttamente dai servizi Adobe Experience Platform per fornire informazioni aggiornate sui set di dati.

## Limitazioni {#limitations}

Data Management Agent è in grado di identificare i set di dati potenzialmente idonei per un criterio di conservazione del data lake, ma non decide se un set di dati ne richiede uno. Non applica, modifica o rimuove un criterio di conservazione senza la tua esplicita conferma.

## Passaggi successivi {#next-steps}

Per informazioni sull&#39;utilizzo di ogni abilità per trovare, analizzare e gestire la conservazione del data lake nei set di dati Experience Event, consulta [Gestire la conservazione del data lake](../coworker/chat/use-cases/data-management/manage-data-lake-retention.md).

Per ulteriori informazioni sul funzionamento dei criteri di conservazione del data lake in Adobe Experience Platform, inclusi il comportamento e la configurazione della conservazione, vedere [Guida alla conservazione dei dataset di Experience Event (TTL)](https://experienceleague.adobe.com/it/docs/experience-platform/catalog/datasets/experience-event-dataset-retention-ttl-guide).
