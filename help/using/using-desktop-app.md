---
title: 'Utilizzo dell''app desktop  [!DNL Experience Manager] '
description: Utilizzo dell'app desktop  [!DNL Adobe Experience Manager] .
feature: Desktop App,Asset Management
source-git-commit: 2947fbd3bfeb15b37a8f1b0118e969b5d70499d0
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 1%

---


# Aprire le risorse sul desktop {#openondesktop-v2}

Puoi aprire le risorse remote da visualizzare nell’applicazione nativa. Le risorse vengono scaricate in una cartella locale. Vengono quindi avviati nell’applicazione nativa associata al formato di file. È possibile modificare l&#39;applicazione nativa per aprire tipi di file (estensioni) specifici in Mac o Windows.

Fare clic su **[!UICONTROL Open]** dal menu delle risorse. La risorsa viene scaricata localmente e aperta nell’applicazione nativa. Nella barra di stato, controlla l’avanzamento del download e la velocità di trasferimento delle risorse di grandi dimensioni.

<!-- ![Download progress bar for large-sized assets](assets/download_status_bar_da2.png "Download progress bar for large-sized assets")
-->

>[!NOTE]
>
>Se le modifiche previste non vengono riportate nell&#39;app, fare clic sull&#39;icona di aggiornamento ![Icona di aggiornamento](assets/do-not-localize/refresh.png) oppure fare clic con il pulsante destro del mouse nell&#39;interfaccia dell&#39;app e quindi scegliere **[!UICONTROL Refresh]**. Le azioni non sono disponibili mentre sono in corso download o caricamenti di dimensioni maggiori.

Per aprire la cartella di download locale di una risorsa, fai clic sull&#39;icona ![Altre azioni](assets/do-not-localize/more2_da2.png), quindi sull&#39;azione ![Mostra icona](assets/do-not-localize/reveal_action2_da2.png) **[!UICONTROL Reveal File]**.

## Utilizzare o inserire risorse in documenti nativi {#place-assets-in-native-documents}

In alcuni casi, ad esempio quando si inserisce una risorsa in un documento nativo, si accede a un file in Esplora risorse o in Mac Finder. Per accedere al percorso del file system del file scaricato localmente, utilizzare l&#39;opzione ![Mostra icona](assets/do-not-localize/reveal_action2_da2.png) **[!UICONTROL Reveal File]**.

![Azione Mostra file per una risorsa](assets/revealfile_action_da2.png "Azione Mostra file per una risorsa")

Fare clic su **[!UICONTROL Reveal File]** o su **[!UICONTROL Reveal Folder]** in una cartella per aprire Esplora risorse o Mac Finder con il file o la cartella preselezionati nel computer locale. Ad esempio, l&#39;opzione è utile per inserire i file [!DNL Experience Manager] nelle applicazioni native che supportano il posizionamento o il collegamento di file locali. Per informazioni su come inserire file in Adobe InDesign, vedere [Inserimento di elementi grafici](https://helpx.adobe.com/it/indesign/using/placing-graphics.html).

L&#39;azione **[!UICONTROL Reveal File]** apre una condivisione di rete locale. Vengono visualizzate solo le risorse disponibili localmente. In altre parole, visualizza le risorse che sono state rivelate, scaricate o aperte/modificate utilizzando l’app. La condivisione di rete locale non carica le modifiche in [!DNL Experience Manager]. Per caricare le modifiche, utilizza esplicitamente le azioni **[!UICONTROL Upload Changes]** o **[!UICONTROL Upload]** nell&#39;app.

>[!NOTE]
>
>Per garantire la compatibilità con le versioni precedenti dell&#39;app desktop [!DNL Experience Manager] v1.x, i file visualizzati vengono gestiti da una condivisione di rete locale, esponendo solo i file disponibili in locale. I percorsi desktop dei file rivelati sono gli stessi dei percorsi creati dall’app v1.x.

>[!CAUTION]
>
>Non utilizzare l&#39;opzione **[!UICONTROL Reveal File]** per modificare le risorse nelle applicazioni native. Utilizzare invece le azioni **[!UICONTROL Edit]**. Per ulteriori informazioni, consulta [Flusso di lavoro avanzato: collabora agli stessi file ed evita di modificare i conflitti](#adv-workflow-collaborate-avoid-conflicts).

## Passaggi successivi {#next-steps}

* [Guarda un video per iniziare a utilizzare Adobe Experience Manager Desktop App](https://experienceleague.adobe.com/it/docs/experience-manager-learn/assets/creative-workflows/aem-desktop-app)

* Fornisci feedback sulla documentazione utilizzando [!UICONTROL Edit this page] ![modifica la pagina](assets/do-not-localize/edit-page.png) o [!UICONTROL Log an issue] ![crea un problema GitHub](assets/do-not-localize/github-issue.png) disponibile nella barra laterale a destra

* Contatta il [Servizio clienti](https://experienceleague.adobe.com/it?support-solution=General#support)

>[!MORELIKETHIS]
>
>* [Interfaccia utente](/help/using/user-interface.md)
>* [Gestione di Assets nell&#39;app desktop](/help/using/assets-management-tasks.md)
>* [Ricerca](/help/using/search.md)
