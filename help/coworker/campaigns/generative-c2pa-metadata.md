---
description: Scopri in che modo Campagne coorker allega e mantiene automaticamente i metadati C2PA (Content Credentials) sulle immagini, dalla generazione alla consegna e-mail.
title: Metadati C2PA nelle campagne collaboratrici
hide: true
source-git-commit: 9796ac7d3d55e7a278414d44a214bfdf5311d727
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 6%

---

# Metadati C2PA nelle campagne collaboratrici {#overview}

Nuove leggi stanno emergendo sulla trasparenza generativa dell’intelligenza artificiale e Adobe sta lavorando per soddisfare i requisiti applicabili in tutte le giurisdizioni. I metadati [C2PA](https://c2pa.org/) (noti anche come Content Credentials) sono lo strumento di provenienza utilizzato da Adobe per soddisfare i requisiti di queste normative.

I metadati C2PA sono metadati invisibili e duraturi che registrano il modo in cui un contenuto è stato creato o modificato. Quando generi o modifichi un’immagine con strumenti di intelligenza artificiale generativi in Campagne collaboratrici, i metadati C2PA vengono automaticamente allegati a tale immagine. Non è richiesta alcuna azione da parte tua.

>[!BEGINSHADEBOX]

## Content Credentials nelle campagne e-mail {#content-credentials-email}

Le immagini inviate nelle campagne e-mail mantengono intatto il Content Credentials, in modo che i destinatari possano verificare l’origine e l’autenticità di qualsiasi immagine direttamente dall’e-mail consegnata.

>[!ENDSHADEBOX]

## Azioni che associano metadati C2PA {#cc-workflows}

La tabella seguente riepiloga quando vengono allegati metadati C2PA, in base all’azione dell’immagine eseguita nella generazione di immagini nelle campagne di Coworker.

| Azione | Descrizione | Metadati C2PA allegati? | Esempio di caso d’uso |
| --- | --- | --- | --- |
| **Generare un&#39;immagine** | Create una nuova immagine da un prompt di testo o da un&#39;immagine di riferimento oppure generate un&#39;immagine simile da una già esistente. | Sempre. L’immagine viene generata dall’intelligenza artificiale generativa, in modo da trasportare sempre nuovi metadati C2PA. | Un’immagine del banner per una campagna e-mail viene generata da un prompt di testo che descrive l’elemento visivo desiderato. |

## Tipi di contenuto e ambito {#cc-content-types}

* **Immagini**: coperte. I metadati C2PA vengono allegati quando le immagini vengono generate con intelligenza artificiale generativa e vengono conservati mediante le operazioni di ritaglio, sovrapposizione di testo e sovrapposizione di immagini eseguite dalla generazione di immagini in Campagne Coworker.
* **Testo**: non applicabile. Gli output di solo testo per la generazione di immagini nelle campagne Coworker, come la generazione di copie, la traduzione e i suggerimenti di allineamento del brand, non richiedono metadati C2PA.

## Cosa succede quando il contenuto si sposta {#cc-content-moves}

Campagne collaboratore mantiene Content Credentials associato alle risorse immagine supportate. Se un’immagine contiene Content Credentials quando viene importata in Campagne collaboratrici, queste credenziali vengono mantenute quando la risorsa viene utilizzata nei contenuti della campagna generata e nelle esperienze e-mail in uscita.

<!-- Some ways of bringing images into your content, such as extracting an image from a PDF or from an embedded (base64) source, may not preserve the original C2PA metadata. In these cases, no C2PA metadata can be read from the source, and none is created for the result. -->

## Risorse aggiuntive

* [Ulteriori informazioni sui metadati C2PA](https://helpx.adobe.com/it/firefly/using/content-credentials.html){target="_blank"}

* [Linee guida utente per l’intelligenza artificiale generativa di Adobe Experience Cloud](https://www.adobe.com/it/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"}

* [Guardrail e limitazioni](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/generate-content/gs-generative#generative-guardrails){target="_blank"}
