---
title: Strumenti Adobe Journey Optimizer in CX Customer Gateway
description: Scopri quali strumenti Adobe Journey Optimizer sono disponibili tramite il gateway di lavoro CX.
source-git-commit: 30f4d593bdec8cb45d10c4c49fac3dce16e8ca03
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 3%

---

# Strumenti Adobe Journey Optimizer in CX Customer Gateway {#ajo-mcp}

Utilizza gli strumenti del prodotto Adobe Journey Optimizer per verificare le campagne e le configurazioni del canale da un client compatibile con MCP. Questi strumenti sono disponibili tramite [CX Coworker Gateway](overview.md) quando l&#39;organizzazione è abilitata e l&#39;account utente dispone delle autorizzazioni Journey Optimizer necessarie.

>[!AVAILABILITY]
>
>Gli strumenti del prodotto Journey Optimizer sono disponibili in Beta. L’accesso avviene solo su invito e richiede l’abilitazione dell’organizzazione Adobe. Vedere [Accedere agli strumenti di Gateway aziendale CX](access.md).

## Funzionalità principali {#mcp-capabilities}

Gli strumenti di Journey Optimizer forniscono una superficie di sola lettura per la revisione della configurazione di campagne e canali. Puoi eseguire le seguenti azioni:

- Elencare le campagne Journey Optimizer e filtrare per stato.
- Recupera i dettagli della campagna, tra cui il targeting, la pianificazione, il canale e i metadati di configurazione del contenuto.
- Elenca le configurazioni del canale per i canali e-mail, SMS, push e WhatsApp.
- Controlla la configurazione della campagna e del canale in linguaggio naturale senza navigare tra le schermate dei prodotti.

>[!IMPORTANT]
>
>Tutti gli strumenti di Journey Optimizer nel Beta corrente sono di sola lettura. La creazione, l’aggiornamento, l’eliminazione, l’avvio, l’arresto o la pubblicazione di campagne non è supportata.

## Strumenti disponibili {#mcp-tools}

| Strumento | Descrizione |
| --- | --- |
| `ajo_campaign_list` | Sfoglia le campagne di marketing Journey Optimizer. Supporta il filtraggio per stato, ad esempio `DRAFT`, `LIVE`, `STOPPED` e `COMPLETED`. |
| `ajo_campaign_get` | Recupera i dettagli e la configurazione per una campagna specifica per ID, inclusi i metadati di targeting del pubblico, pianificazione, canale e impostazioni di contenuto. |
| `ajo_channel_configuration_list`, `ajo_channel_configuration_get` | Visualizza i predefiniti di superficie e le impostazioni di branding per e-mail, SMS, push o [!DNL WhatsApp] canali. |

## Esempi di prompt {#mcp-use-cases}

| Obiettivo | Esempio di prompt |
| --- | --- |
| Panoramica della campagna | &quot;Mostra tutte le campagne Journey Optimizer&quot; |
| Controllo dello stato | &quot;Quali campagne sono attualmente live?&quot; |
| Dettagli della campagna | &quot;Ottenere i dettagli completi della campagna `[campaign ID]`.&quot; |
| Pubblico e targeting | &quot;Quale pubblico è destinatario nella campagna `[campaign ID]`?&quot; |
| Pianificazione e tempistica | &quot;Quando è pianificata l&#39;esecuzione della campagna `[campaign ID]`?&quot; |
| Risoluzione dei problemi | &quot;Rivedi la configurazione della campagna `[campaign ID]` e segnala i possibili problemi.&quot; |
| Configurazione dei canali | &quot;Quali configurazioni del canale e-mail sono disponibili?&quot; |
| Audit del canale | &quot;Quali configurazioni di canale sono mancanti o incomplete?&quot; |

## Contesto del prodotto e autorizzazioni {#mcp-context}

L’account utente deve disporre dell’autorizzazione per visualizzare le campagne Journey Optimizer e le configurazioni dei canali di cui hai bisogno. MCP non ignora le autorizzazioni del prodotto.

Se la tua organizzazione utilizza più sandbox, specifica il contesto della sandbox o dell’ambiente nel prompt quando sono necessari i risultati di una sandbox specifica.

## Limitazioni note {#mcp-limitations}

| Limitazione | Descrizione | Soluzione alternativa |
| --- | --- | --- |
| Superficie di sola lettura | Gli strumenti di Journey Optimizer espongono solo le operazioni di recupero. Non puoi creare, aggiornare, eliminare, avviare, interrompere o pubblicare campagne. | Utilizza l’interfaccia utente o le API di Journey Optimizer per le operazioni di scrittura. |
| Nessun coinvolgimento o metrica delle prestazioni | Gli strumenti non restituiscono dati di reporting come impression, tassi di click-through, conversioni o stati di consegna. | Utilizza gli strumenti di reporting di Journey Optimizer, Customer Journey Analytics o Adobe Analytics per le metriche delle prestazioni. |
| La paginazione dell’elenco delle campagne è limitata | L’elenco delle campagne restituisce la prima pagina dei risultati, fino a 50 campagne ordinate alfabeticamente. I valori di offset e limite non vengono applicati. | Utilizza `Get Campaign` direttamente se l&#39;ID della campagna è noto. Utilizza l’interfaccia utente di Journey Optimizer per la navigazione e il filtraggio completi. |
| Nessun filtro lato server per data, canale o pianificazione | L’elenco delle campagne supporta il filtro dello stato, ma non la data di pubblicazione, la data di pianificazione, il canale o il tipo di campagna. | Utilizza l’elenco delle campagne dell’interfaccia utente di Journey Optimizer per il filtro nativo di data e canale. |
| Recupero contenuto messaggio non disponibile | Il HTML dei messaggi, le righe dell’oggetto, i token di personalizzazione e il contenuto dell’offerta non sono disponibili tramite gli strumenti correnti. | Visualizza il contenuto dei messaggi e la personalizzazione direttamente nell’interfaccia utente di Journey Optimizer. |