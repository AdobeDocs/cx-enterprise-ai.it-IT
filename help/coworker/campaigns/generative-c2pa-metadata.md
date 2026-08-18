---
description: Scopri in che modo Campagne Coworker allega e mantiene automaticamente i metadati C2PA (Content Credentials) sulle immagini generate e modificate dall’intelligenza artificiale, senza richiedere alcuna azione.
title: Metadati C2PA nelle campagne collaboratrici
hide: true
source-git-commit: 785b5d106cb029d68506c90385786cbdae164991
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 2%

---

# Metadati C2PA nelle campagne collaboratrici {#overview}

Nuove leggi stanno emergendo sulla trasparenza generativa dell’intelligenza artificiale e Adobe sta lavorando per soddisfare i requisiti applicabili in tutte le giurisdizioni. I metadati [C2PA](https://c2pa.org/) (noti anche come Content Credentials) sono lo strumento di provenienza utilizzato da Adobe per soddisfare i requisiti di queste normative.

I metadati C2PA sono metadati invisibili e duraturi che registrano il modo in cui un contenuto è stato creato o modificato. Quando generi o modifichi un’immagine con strumenti di intelligenza artificiale generativi in Campagne collaboratrici, i metadati C2PA vengono automaticamente allegati a tale immagine. Non è richiesta alcuna azione da parte tua.

## Azioni che associano metadati C2PA {#cc-workflows}

La tabella seguente riepiloga quando vengono allegati metadati C2PA, in base all’azione dell’immagine eseguita nella generazione di immagini nelle campagne di Coworker.

| Azione | Descrizione | Metadati C2PA allegati? | Esempio di caso d’uso |
| --- | --- | --- | --- |
| **Generare un&#39;immagine** | Create una nuova immagine da un prompt di testo o da un&#39;immagine di riferimento oppure generate un&#39;immagine simile da una già esistente. | Sempre. L’immagine viene generata dall’intelligenza artificiale generativa, in modo da trasportare sempre nuovi metadati C2PA. | Un’immagine del banner per una campagna e-mail viene generata da un prompt di testo che descrive l’elemento visivo desiderato. |
| **Ritagliare un&#39;immagine** (ritaglio centrato o avanzato) | Regolare un&#39;immagine alle dimensioni richieste | Solo se l’immagine di origine conteneva già metadati C2PA. Con il ritaglio vengono ricreati i pixel dell’immagine, che normalmente cancellano i metadati C2PA, pertanto la generazione di immagini in Campagne collaborative li legge dall’immagine sorgente prima del ritaglio, quindi li ricostruisce e li ricollega al risultato ritagliato. Il ritaglio stesso non aggiunge una nuova azione di IA generativa, ma mantiene quella esistente. | Un’immagine del banner generata viene ritagliata per adattarla a una pagina web: i metadati C2PA vengono conservati attraverso il ritaglio. <br> Una foto stock caricata, utilizzata come sfondo di notifica push, viene ritagliata per adattarsi allo schermo: poiché la foto stock non comporta alcuna azione AI generativa, non vengono creati metadati C2PA. |
| **Aggiungi una sovrapposizione di testo** | Rendering del testo generato sopra un&#39;immagine di sfondo | Solo se l’immagine di sfondo conteneva già metadati C2PA. Il rendering della sovrapposizione produce una nuova immagine dallo sfondo più il testo, che normalmente cancella i metadati C2PA, in modo che la generazione di immagini in Campagne Coworker li legga in anticipo dall’immagine di sfondo, quindi li ricostruisce e li ricollega al risultato. Il passaggio di sovrapposizione non aggiunge una nuova azione di IA generativa. | Un titolo promozionale viene riprodotto come sovrapposizione di testo su un’immagine di sfondo generata per una pagina di destinazione: i metadati C2PA dell’immagine di sfondo vengono mantenuti. |
| **Sovrapponi immagini** | Composito di due o più immagini | Se una qualsiasi delle immagini sorgente dispone di metadati C2PA, l&#39;immagine combinata ne trasporta tutti, uniti in un unico set di metadati C2PA. La composizione produce una nuova immagine dalle sorgenti, che normalmente cancella i metadati C2PA, così la generazione di immagini in Campagne di Coworker legge ciascuna prima della composizione, quindi crea un record combinato di metadati C2PA elencando ogni sorgente che ha contribuito a un’azione di intelligenza artificiale generativa. | Un’immagine del prodotto generata viene composta con uno sfondo generato per un’intestazione e-mail: il risultato contiene metadati C2PA che riflettono entrambe le sorgenti di intelligenza artificiale generative. <br> Due foto del brand caricate vengono composte in un unico collage: poiché nessuna delle due origini è associata a un’azione di intelligenza artificiale generativa, non vengono creati metadati C2PA. |

## Tipi di contenuto e ambito {#cc-content-types}

* **Immagini**: coperte. I metadati C2PA vengono allegati quando le immagini vengono generate con intelligenza artificiale generativa e vengono conservati mediante le operazioni di ritaglio, sovrapposizione di testo e sovrapposizione di immagini eseguite dalla generazione di immagini in Campagne Coworker.
* **Testo**: non applicabile. Gli output di solo testo per la generazione di immagini nelle campagne Coworker, come la generazione di copie, la traduzione e i suggerimenti di allineamento del brand, non richiedono metadati C2PA.

## Cosa succede quando il contenuto si sposta {#cc-content-moves}

Campagne collaboratore mantiene Content Credentials associato alle risorse immagine supportate. Se un’immagine contiene Content Credentials quando viene importata in Campagne collaboratrici, queste credenziali vengono mantenute quando la risorsa viene utilizzata nei contenuti della campagna generata e nelle esperienze e-mail in uscita. [Ulteriori informazioni sui metadati C2PA](https://helpx.adobe.com/it/firefly/using/content-credentials.html){target="_blank"}.

<!-- Some ways of bringing images into your content, such as extracting an image from a PDF or from an embedded (base64) source, may not preserve the original C2PA metadata. In these cases, no C2PA metadata can be read from the source, and none is created for the result. -->

>[!MORELIKETHIS]
>
>[Linee guida per l&#39;utente di Adobe Experience Cloud Generative AI](https://www.adobe.com/it/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"}
