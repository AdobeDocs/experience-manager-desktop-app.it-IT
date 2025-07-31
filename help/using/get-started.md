---
title: Inizia [!DNL Experience Manager] app desktop
description: Scopri in che modo l'app desktop  [!DNL Experience Manager]  migliora la creazione e la pubblicazione di contenuti con flussi di lavoro e funzionalità di produttività semplificati.
feature: Desktop App,Asset Management
source-git-commit: 2947fbd3bfeb15b37a8f1b0118e969b5d70499d0
workflow-type: tm+mt
source-wordcount: '1213'
ht-degree: 0%

---


# Inizia a usare l&#39;app desktop [!DNL Adobe Experience Manager] {#getting-started-desktop-app}

Utilizzare l&#39;app desktop [!DNL Adobe Experience Manager] per accedere alle risorse digitali archiviate in un archivio DAM [!DNL Adobe Experience Manager] sul desktop locale. Puoi quindi utilizzare queste risorse in qualsiasi applicazione desktop. Puoi aprire e modificare le risorse localmente nelle applicazioni desktop. Dopo aver apportato le modifiche, caricarle di nuovo in [!DNL Experience Manager] con il controllo della versione per condividere gli aggiornamenti con altri utenti. È inoltre possibile caricare nuovi file e gerarchie di cartelle in [!DNL Experience Manager], creare cartelle ed eliminare risorse o cartelle da [!DNL Experience Manager] DAM.

L&#39;integrazione consente a vari ruoli dell&#39;organizzazione di gestire centralmente le risorse in [!DNL Experience Manager Assets] e di accedere alle risorse sul desktop locale nelle applicazioni native su Windows o macOS.

Quando apri l&#39;applicazione dopo la disconnessione o per la prima volta, fornisci l&#39;URL del server [!DNL Experience Manager] nel formato `https://[aem-server-url]:[port]/`. Selezionare quindi l&#39;opzione [!UICONTROL Connect]. Immetti le credenziali per connettere l&#39;app al server.

Le attività chiave eseguite con l&#39;app desktop [!DNL Adobe Experience Manager] sono:

![Flussi di lavoro e attività eseguibili con [!DNL Experience Manager] app desktop](assets/aem_desktop_app_usecases_v2.png)

## Funzionamento dell’app desktop {#how-app-works2}

Prima di iniziare a utilizzare l&#39;applicazione, scopri [come funziona l&#39;app](release-notes.md#how-app-works). Inoltre, acquisisci familiarità con i seguenti termini:

* **[!UICONTROL Desktop Actions]**: dall&#39;interfaccia Web di Assets, dall&#39;interno di un browser, è possibile esplorare i percorsi delle risorse o estrarle e aprire la risorsa per la modifica nell&#39;applicazione desktop nativa. Queste azioni sono disponibili dall’interfaccia web e utilizzano le funzionalità dell’app desktop.

* Lo stato del file è **[!UICONTROL Cloud Only]**: tali risorse non vengono scaricate nel computer locale e sono disponibili solo nel server [!DNL Experience Manager].

* Lo stato del file è **[!UICONTROL Available locally]**: le risorse vengono scaricate e sono disponibili nel computer locale nello stato corrente. Le risorse non vengono modificate.

* Lo stato del file è **[!UICONTROL Edited locally]**: tali risorse vengono modificate localmente e le modifiche rimangono sul server caricato su [!DNL Experience Manager]. Dopo il caricamento, lo stato cambia in [!UICONTROL Available locally]. Consulta [modificare le risorse](upload-assets.md#edit-assets-upload-updated-assets).

* Lo stato del file è **[!UICONTROL Editing conflict]**: se modifichi una risorsa contemporaneamente, l&#39;app indica che si è verificato un conflitto di modifica. L’app fornisce anche opzioni per mantenere o eliminare le modifiche. Consulta [come evitare di modificare i conflitti](assets-management-tasks.md#adv-workflow-collaborate-avoid-conflicts).

* Lo stato del file è **[!UICONTROL Modified remotely]**: l&#39;app indica se una risorsa scaricata è stata modificata nel server [!DNL Experience Manager]. L’app offre anche l’opzione di scaricare la versione più recente e aggiornare la copia locale. Consulta [come evitare di modificare i conflitti](assets-management-tasks.md#adv-workflow-collaborate-avoid-conflicts).

* **[!UICONTROL Check-out]**: se si sta modificando un file o si intende modificarlo, cambiare lo stato per estrarlo. Aggiunge un&#39;icona di blocco alla risorsa nell&#39;app e nell&#39;interfaccia Web [!DNL Experience Manager]. L’icona Blocca indica ad altri utenti di evitare di modificare contemporaneamente la stessa risorsa poiché si verifica un conflitto di modifica.

* **[!UICONTROL Check-in]**: contrassegna la risorsa come sicura per la modifica da parte di altri utenti senza causare un conflitto di modifica. Quando carichi le modifiche, l’icona del lucchetto viene rimossa automaticamente. L’attivazione dello stato di archiviazione comporta anche la rimozione dell’icona del lucchetto, ma Adobe consiglia di evitare di eseguire manualmente il check-in senza caricare le modifiche. Se si eliminano le modifiche, attivare manualmente il check-in.

* Azione **[!UICONTROL Open]**: è sufficiente aprire la risorsa per visualizzarne l&#39;anteprima nell&#39;applicazione nativa. Adobe consiglia di evitare di modificare la risorsa utilizzando questa azione. Il motivo è che non estrae la risorsa. Nel frattempo, altri utenti possono apportare modifiche che causano conflitti di modifica.

* Azione **[!UICONTROL Edit]**: utilizzare l&#39;azione per modificare l&#39;immagine. Facendo clic su [!UICONTROL Edit], la risorsa viene estratta e viene aggiunta un&#39;icona di blocco sulla risorsa. Dopo aver fatto clic su Modifica, se non desideri modificare la risorsa fai clic su [!UICONTROL Toggle check-in]. Per eliminare, rinominare o spostare le risorse nella gerarchia di cartelle DAM [!DNL Experience Manager], utilizzare le azioni dell&#39;interfaccia Web [!DNL Experience Manager] e non l&#39;azione di modifica.

* Azione **[!UICONTROL Download]**: scarica la risorsa nel computer locale. Puoi scaricare le risorse ora e modificarle in un secondo momento; lavorare offline e caricare le modifiche in un secondo momento. Assets viene scaricato in una cartella cache del file system.

* Azione **[!UICONTROL Reveal File]** o **[!UICONTROL Reveal Folder]**: quando le risorse vengono scaricate in una cartella della cache locale, l&#39;app simula un&#39;unità di rete locale. Fornisce un percorso locale per ogni risorsa. Per conoscere questo percorso, utilizza l’opzione di visualizzazione appropriata nell’app. Per inserire risorse nell’applicazione Creative Cloud è necessaria un’azione di visualizzazione. Vedi [posiziona risorse](search.md#place-assets-in-native-documents).

* Azione **[!UICONTROL Open In Web]**: per visualizzare la risorsa nell&#39;interfaccia Web [!DNL Experience Manager], aprirla nel Web. È possibile avviare altri flussi di lavoro dall&#39;interfaccia [!DNL Experience Manager], ad esempio aggiornando i metadati o individuando le risorse.

* Azione **[!UICONTROL Delete]**: eliminare la risorsa dall&#39;archivio DAM [!DNL Experience Manager]. L’azione elimina la copia originale della risorsa sul server Experience Manager. Se desideri ignorare solo le modifiche apportate alla risorsa locale, vedi [ignorare le modifiche](upload-assets.md#edit-assets-upload-updated-assets).

* **[!UICONTROL Upload Changes]**: l&#39;app desktop carica la risorsa aggiornata solo quando l&#39;utente carica esplicitamente nel server [!DNL Experience Manager]. Quando si salvano le modifiche, queste vengono salvate solo nel computer locale. Quando carichi, la risorsa viene automaticamente archiviata e l’icona del lucchetto rimossa. Consulta [modificare le risorse](upload-assets.md#edit-assets-upload-updated-assets).

## Abilita azioni desktop nell&#39;interfaccia Web [!DNL Experience Manager] {#desktopactions-v2}

Dall&#39;interfaccia utente di [!DNL Assets] in un browser, puoi esplorare i percorsi delle risorse o estrarle e aprire la risorsa per la modifica nell&#39;applicazione desktop. Queste opzioni sono denominate [!UICONTROL Desktop Actions] e non sono abilitate per impostazione predefinita. Per abilitarlo, segui la procedura riportata di seguito.

1. Nella console [!DNL Assets] fare clic sull&#39;icona **[!UICONTROL User]** nella barra degli strumenti.
1. Fare clic su **[!UICONTROL My Preferences]** per visualizzare la finestra di dialogo **[!UICONTROL Preferences]**.

1. Nella finestra di dialogo [!UICONTROL User Preferences], seleziona **[!UICONTROL Show Desktop Actions For Assets]**, quindi fai clic su **[!UICONTROL Accept]**.

   ![Seleziona Mostra azioni desktop per Assets per abilitare le azioni desktop](assets/enable_desktop_actions1.png)

## Inizia dall&#39;interfaccia Web [!DNL Assets] {#adv-workflow-start-from-aem-ui}

Se necessario, avvia il flusso di lavoro dall’interfaccia web di Assets. L&#39;app desktop si integra con [!DNL Experience Manager] per assumere il controllo quando richiesto utilizzando le azioni desktop.

Un caso speciale di avvio di un flusso di lavoro dall’interfaccia web è l’individuazione delle risorse. La barra di Omnisearch nell’interfaccia utente di Assets offre un’esperienza di ricerca ricca e avanzata. È possibile individuare prima una risorsa desiderata sul Web e quindi avviare il flusso di lavoro nell&#39;app, utilizzando [!UICONTROL Desktop Actions]. Alcuni casi di esempio includono il filtraggio dei risultati di ricerca tramite facet, l’individuazione di una risorsa specifica concessa in licenza da Adobe Stock o una personalizzazione implementata dall’organizzazione che consente di individuare meglio dall’interfaccia web.

La funzionalità dell’app desktop viene utilizzata quando si tentano le seguenti azioni sull’interfaccia web di Assets:

* I [!UICONTROL Desktop Actions] che consentono [!UICONTROL Open], [!UICONTROL Edit] e [!UICONTROL Reveal]
* [!UICONTROL Upload folder]
* [!UICONTROL Check-out] oppure [!UICONTROL check-in]

Ad esempio, le azioni disponibili nell&#39;interfaccia Web per una risorsa estratta nell&#39;app sono [!UICONTROL Open], [!UICONTROL Reveal] e [!UICONTROL Check in].

![Azioni desktop nell&#39;interfaccia Web [!DNL Experience Manager]](assets/assets_web_actions_da2.png "Azioni desktop nell&#39;interfaccia Web di Experience Manager")

>[!NOTE]
>
>Il browser potrebbe richiedere di consentire l&#39;avvio di [!DNL Adobe Experience Manager] Desktop. Per effettuare il trasferimento ininterrotto dal browser all’app ogni volta, seleziona la casella di controllo appropriata per consentire all’app di funzionare.

Non è possibile trovare le informazioni o il flusso di lavoro seguenti tramite l&#39;interfaccia Web. Utilizza l’app desktop poiché l’interfaccia web non tiene traccia delle modifiche locali e non è a conoscenza di quanto segue:

* I file vengono modificati localmente.
* File con un conflitto di modifica e un modo per risolverlo.
* Carica modifiche locali in [!DNL Experience Manager].
* Vari stati dei file disponibili localmente.

Al contrario, è possibile aprire la risorsa nell&#39;interfaccia Web a partire dall&#39;app desktop utilizzando l&#39;azione **[!UICONTROL Open In Web]**.

## Passaggi successivi {#next-steps}

* [Guarda un video per iniziare a utilizzare Adobe Experience Manager Desktop App](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/creative-workflows/aem-desktop-app)

* Fornisci feedback sulla documentazione utilizzando [!UICONTROL Edit this page] ![modifica la pagina](assets/do-not-localize/edit-page.png) o [!UICONTROL Log an issue] ![crea un problema GitHub](assets/do-not-localize/github-issue.png) disponibile nella barra laterale a destra

* Contatta il [Servizio clienti](https://experienceleague.adobe.com/it?support-solution=General#support)

>[!MORELIKETHIS]
>
>* [Interfaccia utente](/help/using/user-interface.md)
>* [Note sulla versione e problemi noti](/help/using/release-notes.md)
>* [Installa o aggiorna l&#39;app desktop](/help/using/install-upgrade.md)
