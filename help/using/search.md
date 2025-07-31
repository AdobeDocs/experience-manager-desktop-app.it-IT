---
title: Sfoglia, cerca e visualizza in anteprima le risorse nell'app desktop [!DNL Experience Manager]
description: Sfoglia, cerca e visualizza in anteprima le risorse nell'app desktop  [!DNL Adobe Experience Manager] .
feature: Desktop App
source-git-commit: 2947fbd3bfeb15b37a8f1b0118e969b5d70499d0
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 0%

---


# Sfogliare, cercare e visualizzare in anteprima le risorse {#browse-search-preview-assets}

È possibile cercare, cercare e visualizzare in anteprima le risorse disponibili nell&#39;archivio [!DNL Experience Manager], il tutto dall&#39;applicazione desktop. Prova quanto segue nell’app:

1. Individua una cartella e visualizza alcune informazioni di base delle risorse disponibili nella cartella, insieme a miniature di piccole dimensioni di tutte le risorse.

   ![Sfogliare i file e le cartelle DAM](assets/browse_folder_da2.png "Sfogliare i file e le cartelle DAM")

1. Per visualizzare ulteriori informazioni e una miniatura più grande di una singola risorsa, fai clic sul nome del file.

   ![Visualizza un&#39;anteprima più grande di una risorsa e delle azioni](assets/large_preview_actions_da2.png "Visualizza un&#39;anteprima più grande di una risorsa e delle azioni")

1. Fare clic su **[!UICONTROL Open]** o **[!UICONTROL Edit]** per scaricare il file localmente e visualizzarlo o modificarlo rispettivamente nell&#39;applicazione nativa.
1. Eseguire ricerche utilizzando parole chiave per trovare una risorsa correlata nell&#39;archivio [!DNL Experience Manager]. Utilizzare `?` e `*` come caratteri jolly. Questi caratteri jolly sostituiscono rispettivamente un singolo carattere o più caratteri. Filtra e ordina i risultati in base alle esigenze.

   ![Ricerca di esempio con carattere jolly asterisco](assets/search_wildcard_da2.png "Ricerca di esempio con carattere jolly asterisco")

   ![Altra ricerca di esempio con carattere jolly asterisco](assets/search_wildcard2_da2.png "Un&#39;altra ricerca di esempio con posizionamento diverso del carattere jolly asterisco")

>[!NOTE]
>
>L’app visualizza le risorse confrontando i criteri di ricerca in più campi di metadati e non solo il titolo della risorsa o il nome del file.

## Aprire le risorse sul desktop {#openondesktop-v2}

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

### Gestire i caratteri speciali nei nomi delle risorse {#special-characters-in-filename}

Nell’app legacy, i nomi dei nodi creati nell’archivio mantenevano gli spazi e le maiuscole/minuscole dei nomi delle cartelle forniti dall’utente. Affinché l&#39;applicazione corrente emuli le regole di denominazione dei nodi dell&#39;app v1.10, abilita [!UICONTROL Use legacy conventions when creating nodes for assets and folders] in [!UICONTROL Preferences]. Consulta [preferenze app](/help/using/install-upgrade.md#set-preferences). Questa preferenza legacy è disabilitata per impostazione predefinita.

>[!NOTE]
>
>L’app modifica solo i nomi dei nodi nell’archivio utilizzando le seguenti convenzioni di denominazione. L&#39;app mantiene invariato il `Title` della risorsa.

| Caratteri ‡ | Preferenze legacy nell’app | Quando si verifica nei nomi dei file | Nei nomi delle cartelle | Esempio |
|---|---|---|---|---|
| `. / : [ ] \| *` | Abilitato o disabilitato | Sostituito con `-` (trattino). Un `.` (punto) nell&#39;estensione del nome file viene mantenuto invariato. | Sostituito con `-` (trattino). | `myimage.jpg` rimane invariato e `my.image.jpg` diventa `my-image.jpg`. |
| `% ; # , + ? ^ { } "` e spazi vuoti | ![icona di deselezione](assets/do-not-localize/deselect-icon.png) disabilitata | Gli spazi vuoti vengono mantenuti | Sostituito con `-` (trattino). | `My Folder.` modifiche apportate a `my-folder-`. |
| `# % { } ? & .` | ![icona di deselezione](assets/do-not-localize/deselect-icon.png) disabilitata | Sostituito con `-` (trattino). | NA. | `#My New File.` modifiche apportate a `-My New File-`. |
| Caratteri maiuscoli | ![icona di deselezione](assets/do-not-localize/deselect-icon.png) disabilitata | Il rivestimento viene mantenuto inalterato. | È stato modificato in caratteri minuscoli. | `My New Folder` modifiche apportate a `my-new-folder`. |
| Caratteri maiuscoli | ![icona selezionata per la selezione](assets/do-not-localize/selection-checked-icon.png) abilitata | Il rivestimento viene mantenuto inalterato. | Il rivestimento viene mantenuto inalterato. | NA. |

‡ L’elenco dei caratteri è un elenco separato da spazi.

## Trova tutte le immagini modificate {#find-all-edited-images}

L&#39;applicazione fornisce una visualizzazione, denominata **[!UICONTROL Edited locally]**, che consente di accedere rapidamente a tutti i file scaricati localmente (tramite [!UICONTROL Open] o [!UICONTROL Edit] azioni) e modificati. L’app ti consente di selezionare tutte le risorse modificate localmente e di caricare le modifiche in pochi clic. In questa vista vengono visualizzate anche le risorse modificate localmente che presentano un conflitto di modifica.

![Filtra per visualizzare tutte le risorse modificate localmente](assets/edited_locally_filter_da2.png "Ad esempio, filtra per visualizzare tutte le risorse modificate localmente per un caricamento di massa di modifiche")

## Passaggi successivi {#next-steps}

* [Guarda un video per iniziare a utilizzare Adobe Experience Manager Desktop App](https://experienceleague.adobe.com/it/docs/experience-manager-learn/assets/creative-workflows/aem-desktop-app)

* Fornisci feedback sulla documentazione utilizzando [!UICONTROL Edit this page] ![modifica la pagina](assets/do-not-localize/edit-page.png) o [!UICONTROL Log an issue] ![crea un problema GitHub](assets/do-not-localize/github-issue.png) disponibile nella barra laterale a destra

* Contatta il [Servizio clienti](https://experienceleague.adobe.com/it?support-solution=General#support)

>[!MORELIKETHIS]
>
>* [Interfaccia utente](/help/using/user-interface.md)
>* [Utilizzo dell&#39;app desktop](/help/using/using-desktop-app.md)
>* [Gestione di Assets nell&#39;app desktop](/help/using/assets-management-tasks.md)
