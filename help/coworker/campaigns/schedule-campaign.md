---
description: qui la descrizione.
title: Pianificare una campagna
product_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
feature_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: a3df1a0f8e1014d95483f977aaa64435c18e6578
workflow-type: tm+mt
source-wordcount: 676
ht-degree: 1%

---

# Pianificare una campagna {#schedule-campaign}

Quando si avvia una campagna, gli utenti possono ora scegliere esattamente quando questa viene interrotta: immediatamente, in una data e un’ora future specifiche o in una pianificazione ripetuta (ricorrente). Gli utenti possono anche tornare in un secondo momento e modificare la pianificazione di una campagna già avviata o pianificata.

> **Modifiche**: in precedenza era possibile avviare le campagne solo immediatamente. Questa versione aggiunge la programmazione futura una tantum, le pianificazioni ricorrenti e la possibilità di modificare una pianificazione dopo il lancio.

## Prerequisiti

- La campagna deve essere pronta per il lancio (configurazione completa).
- Non sono necessari prerequisiti oltre a disporre di una campagna in uno stato avviabile.

## Funzionamento di questa funzione

Quando un utente avvia una campagna, scegli una delle tre modalità di pianificazione, quindi conferma. La pianificazione scelta determina quando inizia l’invio della campagna e, per le campagne ricorrenti, quanto spesso si ripete e quando (o se) termina. Una volta pianificata o live una campagna, la sua pianificazione può essere modificata dalle impostazioni della campagna.

### Comportamenti chiave

- All&#39;avvio sono disponibili tre modalità di pianificazione: **Ora**, **Pianifica una volta** e **Ricorrente**.
- Una campagna pianificata per il futuro mostra uno stato &quot;Pianificato&quot; fino all’arrivo dell’ora di inizio, quindi passa automaticamente a &quot;Live&quot;.
- Una campagna ricorrente che è iniziata mostra &quot;Live&quot; insieme a un riepilogo della sua ricorrenza (ad esempio, &quot;Weekly on mar, Thu at 9:00 AM&quot;).
- È possibile impostare l’esecuzione di campagne ricorrenti a tempo indeterminato (&quot;Mai&quot; fine) o fino a una data di fine specifica. Le campagne una tantum e immediate non dispongono di un’opzione di data di fine, in quanto vengono eseguite una volta.
- Gli utenti possono modificare la pianificazione di una campagna già avviata o pianificata, utilizzando le stesse opzioni di pianificazione, dalle impostazioni della campagna.

## Come usarlo

**Per pianificare una campagna al lancio:**

1. Dalla campagna, fai clic su **Pronto per il lancio**.
2. Nella finestra di dialogo di avvio, scegli un’opzione di pianificazione:
   - **Ora** — la campagna inizia l&#39;invio subito dopo il lancio.
   - **Pianifica una volta** — scegli una **data di inizio** futura (data e ora insieme).
   - **Ricorrente** — scegli una **Frequenza** (Giornaliera, Settimanale o Mensile) e un&#39;ora di inizio, quindi imposta il criterio di ricorrenza (vedi campi di seguito).
3. Se è selezionata l&#39;opzione Ricorrente, scegliere se la campagna termina **Mai** o **In una data** e scegliere una data di fine, se applicabile.
4. Conferma di avviare la campagna con la pianificazione selezionata.

**Per modificare una pianificazione esistente:**

1. Apri la campagna e vai alle relative impostazioni.
2. Individuare la sezione relativa alla programmazione e selezionare il sintetico della programmazione corrente.
3. Aggiorna la pianificazione utilizzando le stesse opzioni descritte in precedenza.
4. Salva la modifica.

### Campi/parametri di input

| Campo | Descrizione | Obbligatorio |
| --- | --- | --- |
| Modalità Schedule | Scelta tra Now (Ora), Schedule (Pianifica) una volta o Recurring (Ricorrente) | Sì |
| Data di inizio | Data e ora di inizio della campagna (modalità Pianifica una volta) | Sì, per programmare una volta |
| Frequenza | Giornaliero, Settimanale o Mensile (modalità Ricorrente) | Sì, per ricorrente |
| Ora di inizio | Ora del giorno inviata dalla campagna ricorrente | Sì, per ricorrente |
| Giorni della settimana | Giorni in cui si ripete la campagna | Sì, per frequenza settimanale |
| Giorno del mese | Giorno del mese in cui si ripete la campagna | Sì, per frequenza mensile |
| Fine campagna | Mai, o in una data di fine specifica | Sì, per ricorrente |

## Callout dell’interfaccia utente

> **Nota autore tecnico**: schermate necessarie per:

- [ ] La finestra di dialogo di avvio mostra le opzioni Now (Ora) / Schedule Once (Pianifica una volta) / Recurring (Ricorrente)
- [ ] Il selettore di data e ora Schedule Once
- [ ] Le opzioni ricorrenti: selettore di frequenza, interruttori di giorno settimanali, griglia mensile del giorno del mese
- [ ] La &quot;Fine campagna&quot; mai / In una scelta di data
- [ ] Il badge di stato &quot;Pianificato&quot; su una campagna in attesa del suo orario di inizio
- [ ] Il badge di stato &quot;Live&quot; con un riepilogo delle ricorrenze (ad esempio &quot;Ogni settimana il martedì, alle 9:00&quot;)
- [ ] La sezione pianificazione nelle impostazioni della campagna, che mostra il punto di ingresso per la modifica

## Funzionalità non disponibili in questa funzionalità

- Non supporta intervalli di ripetizione personalizzati, ad esempio &quot;ogni 2 settimane&quot; o &quot;ogni 3 giorni&quot;; sono disponibili solo le frequenze giornaliere, settimanali o mensili standard.
- Non supporta la ricorrenza relativa mensile, ad esempio &quot;il secondo lunedì del mese&quot;; per la selezione mensile è disponibile solo una selezione specifica per giorno del mese.
- Non offre una data di fine per le campagne **Ora** o **Pianifica una volta**. Una data di fine è disponibile solo quando è selezionata l&#39;opzione Ricorrente, poiché le campagne una tantum vengono eseguite una sola volta per definizione.
