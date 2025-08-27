---
title: Carica risorse tramite  [!DNL Experience Manager] app desktop
description: Carica le risorse tramite  [!DNL Adobe Experience Manager] app desktop.
feature: Desktop App,Asset Management
exl-id: f082c712-dc04-4bed-bac8-fa78f93de1c7
source-git-commit: db592420ded4d2f7288982a1ea17618484c82537
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 1%

---

# Caricare le risorse {#upload-assets}

Gli utenti di AEM Desktop App con diritti di aggiunta di risorse possono aggiungere risorse (come immagini, documenti, video o altri supporti).

## Modifica le risorse e carica le risorse aggiornate in [!DNL Experience Manager] {#edit-assets-upload-updated-assets}

Apri le risorse per la modifica quando desideri apportare modifiche e caricare le risorse aggiornate nel server [!DNL Experience Manager]. Per evitare conflitti con le modifiche apportate da altri utenti, utilizza l’app per avviare una sessione di modifica. Prima di iniziare la modifica, accertati che sulla risorsa non sia presente un’icona a forma di lucchetto che indica che un altro utente sta modificando la risorsa.

Per modificare una risorsa, cerca la risorsa o passa alla sua posizione. Fai clic sull&#39;icona ![Altro](assets/do-not-localize/more2_da2.png) e fai clic su **[!UICONTROL Edit]**.

Utilizza **[!UICONTROL Toggle Check-out]** per bloccare la risorsa per evitare conflitti con le modifiche apportate da altri utenti in entrambe le seguenti situazioni:

* Hai iniziato a modificare una risorsa senza prima estrarla (ad esempio semplicemente aprendola).
* Intendi iniziare presto a modificare una risorsa e non desideri che altri la modifichino.

Dopo aver apportato le modifiche, l&#39;app visualizza lo stato **[!UICONTROL Edited Locally]** per le risorse modificate. Tutte le modifiche salvate nelle risorse sono solo locali finché non carichi le modifiche in [!DNL Experience Manager]. Per caricare una o più risorse una alla volta, fai clic su **[!UICONTROL Upload Changes]** tra le opzioni per una risorsa. Crea una versione della risorsa in [!DNL Experience Manager]. Utilizzando l&#39;interfaccia Web di [!DNL Assets], è possibile visualizzare la cronologia delle risorse nella [visualizzazione Timeline](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/using/activity-stream).

![Opzione Carica modifiche nell&#39;app](assets/upload_changes_single1_da2.png "Opzione Carica modifiche nell&#39;app")

![Opzione Carica modifiche durante la visualizzazione di un&#39;anteprima grande di una risorsa](assets/upload_changes_single2_da2.png "Opzione Carica modifiche durante la visualizzazione di un&#39;anteprima grande di una risorsa")

Per le best practice sulla modifica collaborativa, vedere [Flusso di lavoro avanzato: collaborare agli stessi file ed evitare conflitti di modifica](#adv-workflow-collaborate-avoid-conflicts).

Nei casi seguenti, potrebbe essere utile ignorare le modifiche e le modifiche apportate alla risorsa locale. Fai clic su **[!UICONTROL Discard Changes]**.

* Se non si desidera salvare le modifiche localmente in [!DNL Experience Manager].
* Inizia ad apportare modifiche alla risorsa originale dopo aver salvato alcune modifiche.
* Interrompi la modifica della risorsa perché non è più necessaria.

Se necessario, attiva il check-out. La risorsa aggiornata viene rimossa dalla cartella della cache locale e scaricata nuovamente quando la modifichi o la apri.

## Carica e aggiungi nuove risorse in [!DNL Experience Manager] {#upload-and-add-new-assets-to-aem}

Gli utenti possono aggiungere nuove risorse all’archivio DAM. Ad esempio, è possibile essere un fotografo di agenzia o un collaboratore esterno che desidera aggiungere un numero elevato di foto da un servizio fotografico all&#39;archivio [!DNL Experience Manager]. Per aggiungere nuovi contenuti a [!DNL Experience Manager], seleziona l&#39;opzione ![carica nel cloud](assets/do-not-localize/upload_to_cloud_da2.png) nella barra superiore dell&#39;app. Individuare i file di risorse nel file system locale e fare clic su **[!UICONTROL Select]**. In alternativa, per caricare le risorse, trascina i file o le cartelle sull’interfaccia dell’applicazione. In Windows, se trascini le risorse su una cartella all’interno dell’app, le risorse vengono caricate nella cartella. Se il caricamento richiede più tempo, l’app visualizza una barra di avanzamento.

<!-- ![Download progress bar for large-sized assets](assets/upload_status_da2.png "Download progress bar for large-sized assets")
-->

È possibile caricare cartelle o singoli file dal file system locale. La gerarchia di una cartella viene mantenuta al momento del caricamento. Prima di caricare le risorse in blocco, vedi [Caricamenti in blocco](#bulk-upload-assets).

Per visualizzare l&#39;elenco delle risorse trasferite in una determinata sessione, fare clic su **[!UICONTROL View]** > **[!UICONTROL Assets transfers]**. L’elenco ti consente di visualizzare e verificare rapidamente i trasferimenti di file della sessione corrente.

![Elenco delle risorse trasferite in una sessione specifica](assets/assets_transfered_da2.png "Elenco delle risorse trasferite in una sessione specifica")

È possibile controllare la concorrenza di caricamento (accelerazione) nell&#39;impostazione **[!UICONTROL Preferences]** > **[!UICONTROL Upload acceleration]**. Una maggiore concorrenza in genere consente caricamenti più veloci, ma può richiedere molte risorse e consumare una maggiore potenza di elaborazione del computer locale. Se il sistema è lento, ritenta il caricamento utilizzando un valore di concorrenza inferiore.

>[!NOTE]
>
>L’elenco dei trasferimenti non è permanente e non è disponibile se esci dall’app e riapri.

## Caricare risorse in blocco {#bulk-upload-assets}

Utenti o organizzazioni, come fotografi o agenzie creative, possono creare numerose risorse locali durante attività come servizi fotografici, ritocchi o la selezione da un set più ampio. Queste attività vengono spesso eseguite al di fuori di [!DNL Experience Manager]. Possono caricare queste cartelle locali di grandi dimensioni in [!DNL Assets] direttamente dall&#39;app desktop. Le gerarchie di cartelle vengono mantenute e tutte le sottocartelle nidificate e le risorse incluse vengono caricate. Le risorse caricate sono immediatamente disponibili anche per altri utenti dello stesso server. Assets viene caricato in background, pertanto l’operazione non è associata a una sessione del browser web.

![Carica in blocco più cartelle locali dal desktop in [!DNL Experience Manager]](assets/upload_local_folders_da2.png "Carica in blocco più cartelle locali dal desktop in Experience Manager")

Dopo il caricamento, se le modifiche previste non vengono riportate nell&#39;app, fare clic sull&#39;icona di aggiornamento ![Icona di aggiornamento](assets/do-not-localize/refresh.png).

>[!NOTE]
>
>Non utilizzare la funzionalità di caricamento per eseguire la migrazione delle risorse tra due distribuzioni di [!DNL Experience Manager]. Vedi invece la [guida alla migrazione](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/administer/assets-migration-guide).

## Passaggi successivi {#next-steps}

* [Guarda un video per iniziare a utilizzare Adobe Experience Manager Desktop App](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/creative-workflows/aem-desktop-app)

* Fornisci feedback sulla documentazione utilizzando [!UICONTROL Edit this page] ![modifica la pagina](assets/do-not-localize/edit-page.png) o [!UICONTROL Log an issue] ![crea un problema GitHub](assets/do-not-localize/github-issue.png) disponibile nella barra laterale a destra

* Contatta il [Servizio clienti](https://experienceleague.adobe.com/it?support-solution=General#support)

>[!MORELIKETHIS]
>
>* [Scaricare le risorse](/help/using/download-assets.md)
>* [Interfaccia utente](/help/using/user-interface.md)
>* [Ricerca](/help/using/search.md)
