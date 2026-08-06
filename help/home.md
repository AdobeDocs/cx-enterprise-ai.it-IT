---
title: IA nelle applicazioni CX Enterprise
description: Scopri in che modo le applicazioni CX Enterprise utilizzano gli strumenti Generative AI (GenAI), AI Assistant, Agentic AI, CX Enterprise Collaborator e MCP.
TQID: https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 4da8c6f87f4227983b19c682fdceb0db9a352122
workflow-type: tm+mt
source-wordcount: 862
ht-degree: 3%

---

# IA in CX Enterprise

Questa guida descrive le funzionalità di intelligenza artificiale di Adobe CX Enterprise: IA generativa, AI Assistant, Agent Orchestrator, Experience Platform Agents, CX Enterprise Collaborator e MCP.

## Panoramica delle funzionalità di intelligenza artificiale

Inizia qui per un primer su dove e come viene utilizzata l&#39;intelligenza artificiale in CX Enterprise:

- [Informazioni sull&#39;intelligenza artificiale generativa](./overview/generative-ai.md) descrive quali applicazioni CX Enterprise supportano l&#39;intelligenza artificiale generativa e l&#39;Assistente all&#39;intelligenza artificiale e come si confrontano.
- [Informazioni sull&#39;intelligenza artificiale per gli agenti](./overview/agentic-ai.md) spiega come gli agenti Experience Platform funzionano sia nelle applicazioni aziendali CX esistenti che nelle applicazioni AI-first ed elenca gli agenti disponibili in ciascuna di esse.
- Il monitoraggio di [IA](./overview/monitoring.md) riguarda le dashboard che tengono traccia dell&#39;adozione, dell&#39;utilizzo, del feedback e del consumo di crediti AI da parte degli agenti.
- [Consumo crediti AI](./overview/ai-credit-consumption.md) spiega come i processi agente utilizzano i crediti AI, con tassi di consumo stimati per agente e tipo di processo.
- [Gli strumenti per agenti di CX Enterprise](https://experienceleague.adobe.com/it/docs/cx-enterprise-agentic-tools/using/overview) includono ulteriori competenze e strumenti per l&#39;agente che estendono gli agenti di CX Enterprise (esercitazioni video).

## Assistente IA

[L&#39;Assistente AI](./ai-assistant/ai-assistant-ui.md) è uno strumento di IA conversazionale e generativo disponibile nelle applicazioni basate su Adobe Experience Platform. Utilizzalo per acquisire conoscenze sul prodotto, risolvere problemi, trovare informazioni operative e accedere agli agenti Experience Platform, il tutto attraverso prompt del linguaggio naturale in un’interfaccia a schermo intero o con visualizzazione a barra.

Per informazioni su come spostarsi nell&#39;interfaccia, leggere la [Guida dell&#39;interfaccia utente dell&#39;Assistente AI](./ai-assistant/ai-assistant-ui.md). Per visualizzare i prompt di esempio dell&#39;agente, vedere la [libreria di prompt](./ai-assistant/prompt-library.md).

## Agenti Agent Orchestrator e Experience Platform

[Agent Orchestrator](./agents/agent-orchestrator.md) è il livello agente che attiva gli agenti Experience Platform. Quando fai una domanda all’Assistente AI, Agent Orchestrator pianifica il lavoro, chiama gli agenti specializzati necessari per rispondervi e restituisce una risposta unificata, il tutto con una supervisione umana.

I seguenti agenti Experience Platform sono documentati in questa guida:

- [Agente Audience](./agents/audience.md)
- [Data Insights Agent](./agents/cja-data-insights-agent.md)
- [Agente di sperimentazione](./agents/agent-experiment.md)
- [Agente di individuazione campi](./agents/field-discovery-agent.md)
- [Journey Agent](./agents/ajo-agent.md)
- [Agente notifiche](./agents/notifications.md)
- [Agente di supporto prodotto](./agents/product-support.md)
- [Adobe Marketing Agent for Microsoft 365 Copilot](./agents/ama-ms.md)
- [Convalidare i dati](./agents/data-validation.md)

Per l&#39;elenco completo degli agenti, delle applicazioni supportate da ciascuno e dei requisiti di idoneità, vedere [Agentic AI in CX Enterprise](./overview/agentic-ai.md).

## Collaboratore

Coworker è un’evoluzione dell’Assistente all’intelligenza artificiale che automatizza l’esperienza del cliente e i flussi di lavoro di marketing, consentendo al team di concentrarsi sugli obiettivi aziendali anziché sull’esecuzione di routine. Invece di fare una domanda alla volta, descrivi un obiettivo. Il collaboratore pianifica, esegue, convalida e restituisce il lavoro completato per l’approvazione. Il collega include:

- **[Chat collaboratore](https://experienceleague.adobe.com/it/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/overview)**: interfaccia di conversazione per l&#39;esplorazione dei dati, la convalida di tipi di pubblico e percorsi e il completamento di attività in più passaggi nelle applicazioni CX Enterprise.
- **[Campagne collaboratori](https://experienceleague.adobe.com/it/docs/cx-enterprise-ai/experience-cloud-ai/coworker/campaigns/overview)**: applicazione nativa per l&#39;intelligenza artificiale che consolida il briefing della campagna, la creazione di tipi di pubblico, la generazione di contenuti, la progettazione di percorsi e la verifica in un&#39;unica esperienza di conversazione. Utilizza modelli incorporati, best practice e indicazioni per aiutare i team di piccole dimensioni a lanciare campagne in modo rapido.
- **Progetti collaboratori** (presto disponibile): area di lavoro unificata per automatizzare i flussi di lavoro di orchestrazione dell&#39;esperienza del cliente end-to-end, che consente ai team di coordinare attività, approvazioni ed esecuzione per gestire i risultati dalla strategia fino alla consegna. La documentazione dei progetti sarà presto disponibile.

I clienti idonei vengono gradualmente trasferiti da Assistente AI e Agenti Experience Platform a Chat per collaboratori. Leggi [Prova collaboratore](./agents/trial.md) per scoprire l&#39;idoneità alla prova, l&#39;utilizzo del credito AI e come ottenere l&#39;accesso.

Per visualizzare la chat di Coworker in azione, segui [Chat di Coworker in Playground](./coworker/playground-coworker-chat.md) oppure leggi casi d&#39;uso reali come [Convalida dati di migrazione da AA a CJA](./coworker/data-validation-aa-cja.md) e [Analizza dati CJA](./coworker/chat/analytics-chat.md).

Per la documentazione completa del prodotto relativa a Chat con collaboratori, Campagne e Progetti, vedi [Collaboratore](./coworker/overview.md). Per la replica degli oggetti sandbox-to-sandbox, vedere [Sandbox Tooling Agent Skills](./agents/sandbox-tooling.md).

## MCP

[Adobe CX Coworker Gateway](./mcp/overview.md) è l&#39;endpoint MCP (Unified Model Context Protocol) per CX Enterprise. Offre ai client compatibili con MCP, come [!DNL Claude], [!DNL ChatGPT] e [!DNL Cursor], un&#39;unica connessione gestita agli strumenti di prodotto che la tua organizzazione è autorizzata a utilizzare. Questi strumenti includono [!DNL Real-Time CDP], [!DNL Experience Platform], [!DNL Journey Optimizer], [!DNL Customer Journey Analytics], [!DNL Adobe Analytics] e [!DNL Workfront].

Ti avvicini ora a CX Customer Gateway? Consultare [Accedere agli strumenti del gateway di lavoro CX](./mcp/access.md) e [Installare il gateway di lavoro CX](./mcp/install.md) per connettersi.

## Introduzione

### Requisiti di accesso

Prima di poter utilizzare l’Assistente IA e gli agenti Experience Platform, l’amministratore di Adobe deve concedere le autorizzazioni appropriate. I requisiti variano a seconda dell&#39;applicazione. Per ulteriori informazioni, vedere [Accesso](./agents/agent-orchestrator.md#access) nella guida di Agent Orchestrator.

### Privacy e sicurezza

L’Assistente AI e gli agenti Experience Platform danno priorità a privacy, sicurezza e governance, incluso l’isolamento dei dati specifico per sandbox e i criteri di controllo degli accessi esistenti. Per informazioni complete, leggere [Privacy, sicurezza e governance nell&#39;Assistente AI](./ai-assistant/privacy.md).

## Best practice

Per ottenere il massimo valore dall’esperienza di Assistente AI o Collaboratore, segui queste best practice:

- **Sii specifico** nelle tue richieste per ottenere informazioni mirate e rilevanti.
- **Verificare le risposte** esaminando le citazioni di origine e le spiegazioni di ragionamento fornite.
- **Utilizza l&#39;impostazione del contesto** per assicurarti di utilizzare le origini dati più rilevanti per le tue domande.
- **Fornisci un feedback** per migliorare le prestazioni e la precisione nel tempo.
- **Combina approfondimenti** da più agenti per un&#39;analisi più completa.

## Considerazioni giuridiche

L’Assistente per l’intelligenza artificiale attualmente supporta solo le risposte in inglese e i modelli di lingua a volte commettono errori. Verifica sempre le informazioni fornite e utilizza i passaggi di ragionamento inclusi in ogni risposta per capire come sono state generate. Per informazioni dettagliate, leggere la [liberatoria legale](./ai-assistant/legal-disclaimer.md).

