---
title: 'Scarica risorse tramite l''app desktop  [!DNL Experience Manager] '
description: Scarica le risorse tramite l'app desktop  [!DNL Adobe Experience Manager] .
feature: Desktop App,Asset Management
source-git-commit: 2947fbd3bfeb15b37a8f1b0118e969b5d70499d0
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 1%

---


# Scaricare le risorse localmente {#download-assets-locally}

L&#39;app scarica frequentemente le risorse dal server [!DNL Experience Manager] al file system locale. I download occupano spazio su disco e larghezza di banda. Conoscere gli scenari può aiutarti a ottimizzare il tempo di attesa per il completamento dei download. Puoi scaricare le risorse sul file system locale. L&#39;app recupera le risorse dal server [!DNL Experience Manager] e salva la stessa copia nel file system locale.

Fai clic su **[!UICONTROL More actions]** ![Icona altre opzioni](assets/do-not-localize/more2_da2.png) per le opzioni e fai clic su ![Icona download](assets/do-not-localize/download_cloud_da2.png) per scaricarle.

![Opzione Scarica per una risorsa](assets/download_option_da2.png "Opzione Scarica per una risorsa")

>[!NOTE]
>
>Quando si scaricano o si caricano uno o più file di grandi dimensioni, l’applicazione disattiva le azioni su risorse e cartelle. Le azioni sono disponibili al termine del download o del caricamento.

Quando si utilizza l&#39;azione [!UICONTROL Open] per aprire una risorsa in un&#39;applicazione desktop nativa, la risorsa viene scaricata localmente se non è già disponibile localmente. Vedi [Apri risorse](#openondesktop-v2).

Quando riveli il percorso di una risorsa o cartella dall’interno dell’app, la risorsa o cartella viene prima scaricata localmente e quindi aperta sul computer nella condivisione di rete locale. Vedi [Apri risorse](#openondesktop-v2).

Quando si utilizza l&#39;azione [!UICONTROL Edit] per modificare una risorsa in un&#39;applicazione desktop nativa, la risorsa viene scaricata localmente se non è già disponibile localmente. Consulta [Modifica risorse e carica risorse aggiornate in [!DNL Experience Manager]](#edit-assets-upload-updated-assets).

Se l&#39;app è installata e autorizzata a, completa le azioni quando utilizzi [!UICONTROL Desktop Actions] dall&#39;interfaccia Web [!DNL Experience Manager]. L’app scarica prima la risorsa e quindi completa l’azione.

## Scaricare più risorse {#download-multiple-assets}

Il download di più risorse può causare prestazioni insoddisfacenti se la coda è di grandi dimensioni o si verificano problemi di rete. Inoltre, quando si scarica una cartella è possibile mettere in coda inconsapevolmente molte risorse da scaricare. Per evitare lunghi tempi di attesa, l’app limita il numero di risorse scaricate contemporaneamente. Per informazioni su come configurarlo, vedere [Impostare le preferenze](install-upgrade.md#set-preferences). Anche al di sotto di questo limite, a volte l’app può cercare una conferma prima di scaricare una cartella apparentemente grande.

![L&#39;app conferma il download di un numero relativamente elevato di risorse](assets/download_confirmation_da2.png "L&#39;app conferma il download di un numero relativamente elevato di risorse")

Se le cartelle sono selezionate e scaricate, l&#39;applicazione scarica solo le risorse memorizzate direttamente nelle cartelle in [!DNL Experience Manager]. Non scarica automaticamente le risorse dalle sottocartelle.

## Passaggi successivi {#next-steps}

* [Guarda un video per iniziare a utilizzare Adobe Experience Manager Desktop App](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/creative-workflows/aem-desktop-app)

* Fornisci feedback sulla documentazione utilizzando [!UICONTROL Edit this page] ![modifica la pagina](assets/do-not-localize/edit-page.png) o [!UICONTROL Log an issue] ![crea un problema GitHub](assets/do-not-localize/github-issue.png) disponibile nella barra laterale a destra

* Contatta il [Servizio clienti](https://experienceleague.adobe.com/it?support-solution=General#support)

>[!MORELIKETHIS]
>
>* [Carica risorse](/help/using/upload-assets.md)
>* [Interfaccia utente](/help/using/user-interface.md)
>* [Ricerca](/help/using/search.md)

