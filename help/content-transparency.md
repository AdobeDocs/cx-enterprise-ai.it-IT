---
title: Trasparenza dei contenuti di IA generativa
description: Scopri come Adobe allega automaticamente i metadati C2PA ai contenuti generati e modificati da GenAI nelle applicazioni Adobe CX Enterprise.
feature_v2:
  - id: f84b2906-3ce9-4ef0-86f6-cda249273937
  - id: ec4263d9-bf7c-44c7-b3f1-3e664861c8f2
source-git-commit: 4a9ab38cc3aa650dbb90639558d25f6acf707da5
workflow-type: tm+mt
source-wordcount: 1714
ht-degree: 1%

---


# Trasparenza dei contenuti di IA generativa

Nel mese di agosto 2026, Adobe sta gradualmente implementando il supporto dei metadati C2PA nelle applicazioni Adobe Creative Cloud, Adobe Document Cloud, Adobe Firefly e Adobe CX Enterprise.

>[!NOTE]
>
>In seguito al rollout, i flussi di lavoro futuri che coinvolgono contenuti creati o modificati tramite IA avranno automaticamente il supporto per i metadati C2PA.

Questa pagina contiene informazioni dettagliate su come Adobe gestisce l&#39;associazione automatica dei metadati C2PA tra le applicazioni Adobe CX Enterprise.

Le nuove normative impongono ai fornitori di tecnologie di intelligenza artificiale generative di supportare divulgazioni durevoli e leggibili da dispositivo automatico associate ai flussi di lavoro di contenuti generati e modificati da GenAI per una maggiore trasparenza.

In qualità di fornitore di strumenti, Adobe allega automaticamente metadati C2PA leggibili da dispositivo automatico a contenuti generati e modificati tramite GenAI utilizzando le tecnologie Adobe (inclusi i modelli di IA generativa di terze parti supportati nei flussi di lavoro di Adobe). [Ulteriori informazioni su C2PA](https://c2pa.org/).

## Cosa cambia

Con il lancio nell’agosto 2026, Adobe introdurrà il supporto per i metadati C2PA nelle applicazioni Adobe Creative Cloud, Adobe Document Cloud, Adobe Firefly e Adobe CX Enterprise.

Questa versione include:

* Aggiunta automatica di metadati C2PA a contenuti generati e modificati da GenAI supportati.
* Supporto per tipi di contenuto, tra cui immagini, video, audio e testo.
* Conservazione dei metadati C2PA in tutti i flussi di lavoro Adobe supportati.

Non è necessaria alcuna azione aggiuntiva per allegare metadati C2PA a contenuti IA generativi qualificati.

>[!NOTE]
>
>I metadati C2PA non influiscono sull’aspetto del contenuto. I metadati C2PA e le filigrane visibili hanno scopi diversi. I metadati C2PA forniscono informazioni sulla provenienza leggibili da un dispositivo automatico, mentre le filigrane visibili forniscono informazioni visive. Puoi scegliere di aggiungere filigrane visibili al contenuto in base alle esigenze aziendali e ai requisiti legali di ciascuna giurisdizione applicabile.

## Quali dettagli vengono aggiunti come parte dei metadati C2PA

I metadati C2PA allegati automaticamente possono includere informazioni quali:

* Informazioni su nome e versione del sistema di IA utilizzato (ad esempio, Adobe GenStudio, Adobe Firefly)
* Modello di IA utilizzato (ad esempio, Adobe Firefly)
* Utilizzo: se è stato generato o modificato utilizzando GenAI
* Ora e data di creazione e/o modifica dei contenuti con strumenti di intelligenza artificiale generativi
* Identificatore univoco (che può essere utilizzato per distinguere ogni utilizzo di IA generativa)

## Metadati C2PA nel supply chain dei contenuti

I metadati C2PA sono progettati per rimanere associati ai contenuti supportati mentre si spostano tra le applicazioni Adobe e le piattaforme compatibili di terze parti.

Quando il contenuto viene pubblicato, distribuito o condiviso, le piattaforme che supportano i metadati C2PA o le tecnologie di provenienza correlate possono leggere i metadati allegati e visualizzare informazioni sulla trasparenza agli utenti.

Adobe non controlla il modo in cui i servizi esterni interpretano, visualizzano o utilizzano i metadati C2PA dopo che il contenuto ha lasciato le applicazioni Adobe. I clienti devono consultare la documentazione per le singole piattaforme di pubblicazione per comprendere come vengono gestiti i metadati C2PA.

## Filigrana visibile

In alcune circostanze e in alcune aree geografiche, le organizzazioni possono scegliere o essere tenute a identificare in modo visibile i contenuti generati o modificati da GenAI.

Adobe fornisce [indicazioni](https://helpx.adobe.com/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html) sull&#39;utilizzo delle funzionalità di filigrana esistenti supportate tramite le applicazioni Adobe. La necessità di applicare una filigrana visibile dipende dai requisiti aziendali di un’organizzazione e dalle leggi e dalle normative applicabili nelle giurisdizioni in cui il contenuto viene pubblicato.

>[!NOTE]
>
>I metadati C2PA e le filigrane visibili hanno scopi diversi. I metadati C2PA forniscono informazioni sulla provenienza leggibili da un dispositivo automatico, mentre le filigrane visibili forniscono una divulgazione visiva che le organizzazioni possono scegliere di applicare.

## Disponibilità e versioni

Queste funzioni verranno implementate durante **agosto 2026** nei flussi di lavoro aziendali supportati di Adobe CX.

>[!NOTE]
>
>In seguito al rollout, i flussi di lavoro futuri che coinvolgono contenuti creati o modificati tramite IA avranno automaticamente il supporto per i metadati C2PA.

La versione include:

### Metadati C2PA automatici

I metadati C2PA vengono collegati automaticamente ai contenuti supportati generati e modificati da GenAI. Questa funzionalità è attivata per impostazione predefinita e non può essere disattivata.

### Linee guida per la filigrana

Adobe fornisce la [documentazione](https://helpx.adobe.com/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html) che descrive come utilizzare le funzioni di filigrana esistenti disponibili nelle applicazioni Adobe supportate per le organizzazioni che scelgono o devono applicare etichette visibili.

## Applicazioni supportate in Adobe CX Enterprise {#supported-applications}

Le applicazioni e i servizi Adobe riportati di seguito forniscono informazioni aggiuntive su come e quando i metadati C2PA vengono allegati ai contenuti qualificati all&#39;interno di determinate app CX Enterprise.

Tuttavia, laddove applicabile, tutte le applicazioni Adobe CX Enterprise continuano a conservare i metadati C2PA esistenti man mano che le risorse supportate passano attraverso i flussi di lavoro Adobe. Questo aiuta a mantenere l’integrità delle informazioni sulla provenienza in tutto il supply chain dei contenuti.

>[!NOTE]
>
>Le note sulla versione o le linee guida per ciascuna delle applicazioni elencate di seguito saranno rese disponibili su Experience League nelle rispettive sezioni della pagina del prodotto dell’applicazione. La tabella verrà aggiornata con i collegamenti non appena saranno disponibili. Consulta le sezioni più recenti dei prodotti su Experience League.

| Applicazione/soluzione | Note sulla versione/Guida |
|---|---|
| Adobe Advertising Cloud | [Documentazione](https://experienceleague.adobe.com/en/docs/advertising/creative/creative-studio/creative-studio-content-credentials) |
| Adobe Experience Manager (AEM) | [Documentazione](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/c2pa-metadata-dynamic-media-openapi) |
| Assistente AI per la generazione di contenuti (funzione in Adobe Journey Optimizer/Adobe Campaign) | [Documentazione](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/generate-content/generative-c2pa-metadata) |
| Ultimate B2B Adobe Journey Optimizer | [Documentazione](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/content-management/assets/c2pa-metadata) |
| Prime B2B di Adobe Journey Optimizer (alias Adobe Marketo Optimizer) | [Documentazione](https://experienceleague.adobe.com/en/docs/marketo-optimizer/user/content/assets/c2pa-metadata) |
| Adobe Journey Optimizer B2C | |
| Adobe Campaign | |
| Adobe Commerce | [Documentazione](https://experienceleague.adobe.com/en/docs/commerce/optimizer/manage-results/success-metrics#c2pa-metadata-on-exported-reports) |
| GenStudio for Performance Marketing | [Documentazione](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/content-credentials) |
| Adobe Marketo Engage | [Documentazione](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/images-and-files/c2pa-metadata) |
| Adobe Workfront | [Documentazione](https://experienceleague.adobe.com/en/docs/workfront/using/documents/c2pa-metadata-overview) |
| Campagne CX Enterprise Collaborator (precedentemente HALO) | [Documentazione](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/campaigns/c2pa-metadata) |

## Collegamenti correlati

* [Guida alla filigrana visibile](https://helpx.adobe.com/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html)
* [Adobe Inspect](https://contentauthenticity.adobe.com/inspect)
* [Panoramica dell&#39;iniziativa Adobe GenAI Labeling Compliance](https://helpx.adobe.com/creative-cloud/apps/generative-ai/ai-content-labeling-faq.html)

## Domande frequenti

**Quali app Adobe applicano i metadati C2PA ai contenuti modificati o creati dall&#39;intelligenza artificiale generativa?**

Le applicazioni Adobe CX Enterprise supportate allegano automaticamente i metadati C2PA ai contenuti qualificati generati da GenAI e modificati da GenAI. Per ulteriori informazioni sulle applicazioni Adobe CX Enterprise, consultare la sezione [Applicazioni supportate](#supported-applications).

**A quali tipi di contenuto Adobe aggiungono metadati C2PA?**

In generale, immagini, audio, video, documenti e testo rientrano nell’ambito di applicazione. Tuttavia, consulta la documentazione nella sezione [Applicazioni supportate](#supported-applications) per scoprire in che modo ogni applicazione supporta i metadati C2PA per diversi prodotti e tipi di contenuto.

**Quali applicazioni in Adobe CX conservano i metadati C2PA durante la modifica e la pubblicazione?**

Tutte le applicazioni Adobe CX Enterprise sono progettate per conservare i metadati C2PA man mano che i contenuti passano attraverso flussi di lavoro Adobe compatibili. La conservazione al di fuori delle applicazioni Adobe dipende dal fatto che le piattaforme esterne supportino i metadati C2PA.

**Cosa succede quando più immagini generate da GenAI vengono combinate in un&#39;unica immagine?**

I metadati C2PA risultanti dipendono dall’applicazione e dal flusso di lavoro utilizzati. Se supportato, Adobe conserva le informazioni sulla provenienza durante l’intero processo di modifica. Consulta la sezione [Applicazioni supportate](#supported-applications-across-adobe-cx-enterprise) per la documentazione relativa al comportamento specifico del flusso di lavoro in ogni app.

**Cosa succede quando le immagini generate da GenAI da applicazioni Adobe e non Adobe vengono combinate?**

Adobe conserva i metadati C2PA disponibili e supportati all’interno del flusso di lavoro. Laddove applicabile, Adobe aggiornerà i metadati sottostanti con le informazioni più recenti ogni volta che il contenuto applicabile (immagine, audio, video, testo) viene modificato o creato utilizzando GenAI nei flussi di lavoro di Adobe. Quando combini più origini in una nuova risorsa, i metadati sottostanti non vengono sostituiti né persi. Al contrario, la nuova risorsa ottiene i propri metadati C2PA e i dettagli da ogni origine sono conservati al suo interno. Se un’origine disponeva già di propri metadati C2PA, provenienti da uno strumento Adobe o non Adobe, tale cronologia rimane associata a esso. Questo significa che la risorsa finale ha un quadro completo: il proprio record di essere stata creata o modificata con GenAI, più la storia individuale di ogni pezzo che vi è entrato.

**I flussi di lavoro modificati e creati da GenAI nelle applicazioni Adobe CX allegano automaticamente i metadati C2PA?**

Sì. Per i flussi di lavoro di intelligenza artificiale generativi supportati, Adobe allega automaticamente i metadati C2PA che identificano se il contenuto è stato generato o modificato da GenAI insieme ad altre informazioni sulla provenienza, come marche temporali, informazioni sul sistema di intelligenza artificiale e identificatori univoci.

**Come vengono mantenuti i metadati C2PA in tutto il contenuto supply chain?**

I metadati C2PA sono metadati duraturi progettati per rimanere associati ai contenuti supportati durante il trasferimento tra applicazioni Adobe compatibili e piattaforme di supporto di terze parti. I servizi esterni determinano la modalità di visualizzazione delle informazioni sulla provenienza allegate dopo la pubblicazione.

**In che modo le organizzazioni possono aggiungere le proprie informazioni autenticate senza interrompere la catena di provenienza?**

Alcune applicazioni Adobe consentono ai creatori e alle organizzazioni di aggiungere ulteriori informazioni autenticate ai metadati C2PA esistenti, preservandone la provenienza. La disponibilità varia a seconda dell&#39;applicazione.

**È possibile disattivare l&#39;associazione automatica dei metadati C2PA?**

No. Le nuove leggi generative sulla trasparenza dell’intelligenza artificiale richiedono alle aziende che forniscono strumenti di intelligenza artificiale generativi, tra cui Adobe, di allegare metadati durevoli a contenuti qualificati generati o modificati con intelligenza artificiale generativa. Impossibile disattivare l&#39;associazione automatica dei metadati C2PA.

**Cosa succederà ai contenuti creati/modificati con IA generativa prima della versione di agosto?**

Ai contenuti creati o modificati con strumenti di intelligenza artificiale generativi prima della versione di agosto 2026 non sono allegati metadati C2PA automatici. Tuttavia, i contenuti creati nel web Firefly e in altre app in cui erano stati precedentemente applicati metadati C2PA continuano a farli allegare.

**In che modo un cliente può verificare se al contenuto sono allegati metadati C2PA?**

I clienti possono verificare se al contenuto sono allegati metadati C2PA caricandolo nella pagina [Adobe Inspect](https://contentauthenticity.adobe.com/inspect).

**In che modo le piattaforme esterne visualizzano i metadati C2PA una volta pubblicato o condiviso il contenuto?**

Man mano che i contenuti si spostano tra piattaforme editoriali, canali di social media, servizi di posta elettronica e altri ecosistemi digitali, i servizi a valle che supportano i metadati C2PA, o le relative tecnologie di provenienza, possono essere in grado di leggere i metadati allegati e scegliere di visualizzare informazioni o indicatori basati su tali informazioni. Adobe non controlla il modo in cui le piattaforme esterne visualizzano, interpretano o applicano le divulgazioni associate ai metadati C2PA allegati. Per informazioni aggiornate su come una piattaforma specifica gestisce le informazioni sulla provenienza, i clienti devono controllare direttamente le linee guida di tale piattaforma.

**Queste modifiche aumentano il costo dei prodotti o degli abbonamenti Adobe?**

No. I metadati C2PA non influiscono sul costo dei prodotti Adobe.
