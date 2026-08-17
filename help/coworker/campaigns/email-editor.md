---
description: descrizione.
title: Comprendere l’editor e-mail
feature_v2: id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 1c4f9585c04eae8693e38541084cead08412d192
workflow-type: tm+mt
source-wordcount: 707
ht-degree: 0%

---

# Comprendere l’editor e-mail {#email-editor}

L’editor e-mail consente di perfezionare un’e-mail generata dall’intelligenza artificiale direttamente sulla bacheca della campagna. Modifica l’oggetto e il preheader, formatta il testo e le immagini in linea o sostituiscili in un altro modello. <!-- It's an inline editor over the email's actual HTML, not a drag-and-drop block builder. -->

>[!PREREQUISITES]
>
>Crea una campagna con un messaggio e-mail generato.

## Funzionamento di questa funzione

Facendo clic su una scheda e-mail nella bacheca della campagna, l’editor e-mail viene aperto come pannello laterale. Da lì, l’utente può modificare l’oggetto e il preheader (con alternative suggerite dall’intelligenza artificiale), fare clic nel corpo dell’e-mail per selezionare e formattare testo o immagini, passare da una variante generata dall’intelligenza artificiale a un’altra, scambiare il modello HTML, verificare la compatibilità e-mail con il client e inviare un messaggio e-mail di test alla propria casella in entrata. Le modifiche vengono salvate automaticamente e le versioni precedenti possono essere riviste e ripristinate.

### Comportamenti chiave

- Facendo clic su un testo o un’immagine nel corpo dell’e-mail, questo viene selezionato e viene visualizzata una barra degli strumenti di formattazione mobile.
- Opzioni di formattazione del testo: Grassetto, Corsivo, Sottolineato, font e dimensione font.
- Opzioni immagine: Sostituisci, Elimina, Collega, Modifica con Express, Genera immagine (AI), Carica dal computer.
- I caricamenti di immagini sono limitati a 10 MB; le immagini superiori a circa 3 MB vengono compresse automaticamente, con una nota sulla qualità che consiglia immagini inferiori a 3 MB.
- I campi Oggetto e Preheader dispongono ciascuno di un’opzione &quot;Smart suggestions&quot; per le alternative generate da IA.
- Cambia il salvataggio automatico (in caso di sfocatura e poco dopo le azioni di formattazione) — un indicatore di stato mostra le modifiche non salvate, Salvataggio in corso..., Salvato, Salvato automaticamente o Impossibile salvare (con un&#39;opzione Riprova).
- Annulla/Ripristina è disponibile per la sessione di modifica corrente.
- Le versioni salvate in precedenza possono essere visualizzate in anteprima e ripristinate da un pannello di cronologia delle versioni.
- Se esistono più varianti generate dall’intelligenza artificiale, l’utente può passare da una all’altra da un pannello di miniature all’altra.
- Il modello HTML dell’e-mail può essere scambiato utilizzando &quot;Cambia modello HTML&quot;.
- &quot;Send test email&quot; (Invia e-mail di test) invia un’anteprima reale alla casella in entrata dell’utente utilizzando dati di esempio, senza influire sul reporting delle campagne.
- In alcuni ambienti è disponibile un controllo di compatibilità del client e-mail che riguarda Gmail, Outlook, Apple Mail, Yahoo Mail, Samsung Email e Thunderbird. [INPUT NECESSARIO: è dietro un flag di funzione; verificare che sia abilitato per il pubblico di destinazione prima di documentarlo come generalmente disponibile]

## Come accedere

1. Apri la campagna desiderata e fai clic su Apri editor nella scheda e-mail.

SCHERMATA

1. Modifica direttamente i campi **Oggetto** e **Preintestazione** oppure fai clic su **Suggerimenti avanzati** accanto a per le alternative generate da IA.
1. Fai clic sul corpo dell’e-mail per selezionare un blocco di testo o un’immagine, quindi utilizza la barra degli strumenti mobile che viene visualizzata per formattare il testo o gestire l’immagine.
1. Utilizza **Cambia modello HTML** per sostituire il corpo dell&#39;e-mail con un altro modello.
1. Utilizza **Invia e-mail di test**, immetti un indirizzo del destinatario e fai clic su **Invia** per inviare un&#39;anteprima live a tale indirizzo tramite e-mail.
1. Utilizza l’icona della cronologia delle versioni per visualizzare in anteprima e ripristinare una versione salvata in precedenza.
1. Le modifiche vengono salvate automaticamente: non è richiesto alcun passaggio di salvataggio manuale.

### Campi/parametri di input

| Campo | Descrizione | Obbligatorio |
| --- | --- | --- |
| Argomento | Oggetto dell’e-mail | No (può essere lasciato vuoto; non attualmente applicato) |
| Preheader | Testo di anteprima visualizzato accanto all&#39;oggetto in una casella in entrata | No |
| Indirizzo e-mail del destinatario | Dove inviare un’e-mail di test | Sì, per inviare l’e-mail di test |

## Callout dell’interfaccia utente

> **Nota autore tecnico**: schermate necessarie per:

- [ ] Pannello laterale dell&#39;editor e-mail (campi oggetto/preintestazione più corpo dell&#39;e-mail)
- [ ] Barra degli strumenti mobile per la selezione del testo
- [ ] Barra degli strumenti mobile per la selezione dell&#39;immagine
- [ ] Il pannello delle miniature della variante AI
- [ ] Il pannello della cronologia delle versioni
- [ ] Finestra di dialogo &quot;Cambia modello HTML&quot;
- [ ] La finestra di dialogo Invia e-mail di test
- [ ] Verifica compatibilità client e-mail (se attivato nell&#39;ambiente di destinazione)

## Funzionalità non disponibili in questa funzionalità

- Non si tratta di un generatore di blocchi drag-and-drop, non esiste una libreria di blocchi e i blocchi di contenuto non possono essere aggiunti, rimossi o riordinati; la modifica avviene direttamente sul HTML e-mail esistente.
- Attualmente non supporta l’inserimento di tag di personalizzazione/unione.
- Non fornisce un campo di testo alternativo per le immagini.
- Non applica un oggetto, un preheader o altri controlli a livello di contenuto prima che un’e-mail venga considerata &quot;pronta&quot;; gli unici controlli pre-lancio sono a livello di campagna (configurazione dell’invio, e-mail di test inviata, un pubblico reale), non i controlli sul contenuto dell’e-mail stesso.
- L’attivazione dell’anteprima desktop/mobile non è disponibile nella visualizzazione standard di modifica delle e-mail per campagne. [È NECESSARIO INPUT per confermare l&#39;ambito]
- [INPUT NECESSARIO — per confermare con il tecnico: se l&#39;editor diventa di sola lettura (non solo il campo del mittente) dopo l&#39;attivazione/l&#39;avvio di una campagna.]
