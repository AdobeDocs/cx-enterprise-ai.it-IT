---
description: qui la descrizione.
title: Interrompere una campagna
feature_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 1c4f9585c04eae8693e38541084cead08412d192
workflow-type: tm+mt
source-wordcount: 410
ht-degree: 0%

---

# Interrompere una campagna {#stop-campaign}

Gli utenti possono ora interrompere una campagna che invia attivamente (una campagna &quot;live&quot;) direttamente dalla pagina dei dettagli della campagna. L’interruzione di una campagna è permanente: i destinatari cessano immediatamente di avanzare nella campagna e quest’ultima non può essere ripresa o riavviata in un secondo momento.

## Prerequisiti

- La campagna deve essere in uno stato live (invio attivo). L’azione Interrompi non è disponibile per le campagne bozza, pianificate o già interrotte.
- [INPUT NECESSARIO — per confermare con l&#39;ingegnere: l&#39;arresto di una campagna richiede un ruolo o un&#39;autorizzazione specifica oppure è possibile eseguire questa operazione da qualsiasi utente con accesso alla campagna?]

## Funzionamento di questa funzione

Un’azione &quot;Interrompi campagna&quot; viene visualizzata nell’intestazione dei dettagli della campagna ogni volta che questa viene pubblicata. Selezionandola si apre una finestra di dialogo di conferma che avvisa che l’azione è permanente. La conferma richiama il backend per interrompere la campagna; al completamento, lo stato della campagna cambia in &quot;Interrotto&quot; e viene visualizzato un messaggio di conferma.

### Comportamenti chiave

- L’azione Interrompi campagna viene visualizzata solo mentre una campagna è in esecuzione (invio attivo).
- L’arresto è permanente: i destinatari non progrediscono più nella campagna e non possono riprenderla.
- Una finestra di dialogo di conferma richiede all’utente di confermare esplicitamente prima che la campagna venga interrotta.
- Dopo l’interruzione, il badge di stato della campagna diventa &quot;Arrestato&quot;.
- Se la richiesta di interruzione non riesce, viene visualizzato un messaggio di errore e la campagna rimane attiva.

## Come usarlo

1. Apri una campagna attualmente live (invio attivo).
2. Nell&#39;intestazione dei dettagli della campagna fare clic su **Interrompi campagna**.
3. Nella finestra di dialogo di conferma, controlla l’avviso: &quot;L’arresto della campagna è permanente. Tutti i destinatari cesseranno di progredire e la campagna non può essere ripresa.&quot;
4. Fai clic su **Interrompi** per confermare.
5. &quot;Campagna interrotta&quot;. viene visualizzato un messaggio di conferma e lo stato della campagna si aggiorna su &quot;Arrestato&quot;.

### Campi/parametri di input

Non applicabile — questa funzione è una singola azione di conferma senza campi di input.

## Callout dell’interfaccia utente

> **Nota autore tecnico**: schermate necessarie per:

- [ ] Il pulsante &quot;Interrompi campagna&quot; nell&#39;intestazione dei dettagli della campagna, visualizzato in una campagna live
- [ ] La finestra di dialogo di conferma con l&#39;avviso di permanenza
- [ ] Il badge di stato &quot;Interrotto&quot; dopo un&#39;interruzione riuscita
- [ ] Messaggio di errore visualizzato se l&#39;arresto non riesce

## Funzionalità non disponibili in questa funzionalità

- Non mette temporaneamente in pausa una campagna. Non è possibile riprendere una campagna interrotta; l’interruzione è un’azione unidirezionale.
- Non supporta il riavvio o il riavvio di una campagna interrotta dallo stesso record della campagna.
- [INPUT NECESSARIO — per confermare con l&#39;ingegnere: è pianificata una funzionalità &quot;pausa e ripresa&quot; separata o è prevista l&#39;interruzione della spedizione dell&#39;unica azione di controllo dello stato in questa versione?]
