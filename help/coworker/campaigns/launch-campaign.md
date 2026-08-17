---
description: qui la descrizione.
title: Avviare una campagna
feature_v2: id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 1c4f9585c04eae8693e38541084cead08412d192
workflow-type: tm+mt
source-wordcount: 757
ht-degree: 0%

---

# Avviare una campagna {#launch-campaign}

Il lancio di una campagna è l’azione che la sposta dalla bozza all’invio attivo. Prima di aprire la finestra di dialogo di lancio, Halo controlla che la campagna sia pronta e blocca il lancio fino al completamento della configurazione richiesta. La finestra di dialogo di lancio mostra un’anteprima dell’e-mail e del pubblico, consente all’utente di rivedere o modificare la pianificazione di invio in linea e segnala se il lancio è stato completato correttamente. Questa sezione descrive l&#39;esperienza di lancio end-to-end; per le opzioni di pianificazione offerte durante il lancio, consulta [Pianificare una campagna](/help/coworker/campaigns/schedule-campaign.md).

## Prerequisiti

- Lo stato della campagna deve essere Bozza. <!-- The Launch action isn't available once a campaign is already live. -->
<!-- - The campaign must pass a readiness check: sending settings configured, at least one test email sent, and a real (non-sample) audience uploaded. -->
- [HA BISOGNO DI INPUT — per confermare con il tecnico: alcuni utenti potrebbero vedere un&#39;esperienza &quot;in arrivo&quot; invece di un pulsante Launch vero e proprio, che offre solo il download della campagna o l&#39;invio di un&#39;e-mail di bozza anziché il lancio in-app. Conferma cosa determina l&#39;esperienza ottenuta da un determinato utente o campagna.]

## Funzionamento di questa funzione

Quando un utente lancia una campagna, Halo verifica innanzitutto che la campagna sia pronta. Se manca qualcosa, una finestra di dialogo elenca ciò che deve essere risolto prima che il lancio possa procedere. Al termine della convalida, la finestra di dialogo di avvio mostra un’anteprima dell’e-mail e del pubblico/flusso di lavoro, consente all’utente di rivedere o modificare la pianificazione di invio senza uscire dal flusso e, per gli invii di grandi dimensioni, mostra una stima dell’avviso relativo al volume di invio. La conferma attiva il lancio e Halo riporta uno dei tre risultati: lanciato, già avviato o non riuscito.

### Comportamenti chiave

- Launch è disponibile solo per le campagne in stato Bozza; non è possibile avviare nuovamente una campagna già live.
- Un controllo di preparazione viene eseguito automaticamente prima dell’apertura della finestra di dialogo di avvio. I problemi non risolti bloccano l’avvio e vengono elencati in modo da risolverli tutti.
- La finestra di dialogo per il lancio mostra un’anteprima e-mail (oggetto, preintestazione, mittente) e un’anteprima del pubblico/flusso di lavoro.
- La pianificazione dell’invio può essere rivista o modificata dall’interno della finestra di dialogo di avvio.
- Per gli invii di grandi dimensioni, la finestra di dialogo mostra un impatto stimato sul volume di invio. [INPUT NECESSARIO. La formulazione esatta dell&#39;avviso non è disponibile dal codice]
- Una volta completata l’operazione, lo stato della campagna diventa &quot;Pianificato&quot; o &quot;Live&quot; (a seconda della pianificazione scelta); un messaggio di conferma informa che gli approfondimenti della campagna saranno disponibili entro 2 ore.
- Se la campagna è già stata avviata (ad esempio, da un clic duplicato), Halo mostra un messaggio &quot;già avviato&quot; anziché un errore.
- Se il lancio non riesce, viene visualizzato un messaggio di errore e la campagna rimane in stato Bozza; l’utente può riprovare.
- Una volta interrotta <!--(see [Stop a live campaign](./stop-live-campaign.md))-->, la campagna non può essere riavviata dallo stesso record della campagna. L&#39;interruzione è uno stato separato e permanente.

## Come accedere

**Per avviare una campagna:**

1. Dalla campagna, fai clic su **Lancio** (visualizzato come &quot;Pronto per il lancio&quot; mentre è ancora in bozza).
2. Se manca qualcosa, in una finestra di dialogo dal titolo &quot;A some Things still need care&quot; (Alcune cose richiedono ancora attenzione) viene indicato cosa completare:
   - **Configura impostazioni e-mail** — i parametri di invio (mittente/dominio) non sono ancora stati impostati.
   - **E-mail non testate**: invia almeno un&#39;e-mail di test per verificare l&#39;e-mail prima del lancio.
   - **Pubblico reale richiesto per il lancio**: la campagna utilizza ancora un pubblico di esempio; carica un CSV di pubblico reale.
     Risolvi ogni elemento, quindi riprova Launch.
3. Una volta che la campagna supera il controllo di preparazione, si apre la finestra di dialogo di lancio con un’anteprima dell’e-mail e del pubblico.
4. Rivedi la pianificazione mostrata nella finestra di dialogo. Per modificarla, utilizzare le opzioni di pianificazione descritte in [Pianifica all&#39;avvio di una campagna](/help/coworker/campaigns/schedule-campaign.md), quindi salvare.
5. Conferma l&#39;avvio. Al completamento, viene visualizzato un messaggio di conferma e lo stato della campagna viene aggiornato (a &quot;Pianificato&quot; o &quot;Live&quot;).

<!-- 
## Input fields / parameters

Not applicable beyond the schedule fields already documented in [Schedule when a campaign launches](/help/coworker/campaigns/schedule-campaign.md) — launching itself doesn't require any additional input. 
-->

## Callout dell’interfaccia utente

> **Nota autore tecnico**: schermate necessarie per:

- [ ] Il punto/pulsante di ingresso Launch nell&#39;intestazione dei dettagli della campagna
- [ ] La finestra di dialogo di preparazione/convalida elenca gli elementi incompleti
- [ ] La finestra di dialogo di avvio che mostra l&#39;anteprima e-mail + pubblico e la sezione pianificazione
- [ ] Avviso di impatto del volume di invio stimato (per pubblici di grandi dimensioni)
- [ ] Il messaggio di conferma del successo dopo il lancio
- [ ] Il messaggio &quot;già avviato&quot;
- [ ] Messaggio di errore generico di errore di avvio-errore

## Funzionalità non disponibili in questa funzionalità

- Non consente il lancio di una campagna con un pubblico di esempio (non reale), e-mail non testate o impostazioni di invio non configurate; tutte e tre devono essere risolte per prime.
- Il lancio non accetta una pianificazione come parte della stessa azione; la pianificazione viene salvata separatamente (all&#39;interno della stessa finestra di dialogo) prima o come parte della conferma del lancio.
- Non supporta il rilancio di una campagna che è stata interrotta — l&#39;arresto è permanente <!--(see [Stop a live campaign](./stop-live-campaign.md))-->.
- [INPUT NECESSARIO — per confermare con il tecnico/PM: per alcuni utenti, Launch potrebbe essere sostituito da un’esperienza &quot;in arrivo&quot; che offre solo il download di una campagna (PDF/DOCX) o l’invio di un’e-mail di bozza, senza avvio in-app self-service. Prima della pubblicazione, confermare il pubblico a cui si applica, in quanto modifica i passaggi della procedura per tale coorte.]
