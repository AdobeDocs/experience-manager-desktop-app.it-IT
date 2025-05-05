---
title: Usa la versione 1.10 dell'app desktop  [!DNL Experience Manager] .
description: Scopri come utilizzare l’app desktop Adobe Experience Manager versione 1.10 e ottimizzare il tuo lavoro con le risorse sul desktop.
feature: Desktop App,Asset Management
exl-id: 2fdc1c8d-b822-4cca-ad06-bd875a00aa6d
source-git-commit: 5676e7ece8bb43f051dae72d17e15ab1c34caefc
workflow-type: tm+mt
source-wordcount: '2329'
ht-degree: 0%

---

# Usa [!DNL Experience Manager] app desktop v1.10 {#use-aem-desktop-app-v1x}

Utilizzando l&#39;app, le risorse in [!DNL Experience Manager] sono facilmente accessibili sul desktop locale e possono essere utilizzate in qualsiasi applicazione desktop. Assets può essere facilmente rilevato in Mac Finder o Esplora risorse, aperto in applicazioni desktop e modificato localmente. Le modifiche vengono salvate in [!DNL Experience Manager] con una nuova versione creata nell&#39;archivio.

Questa integrazione consente la gestione centralizzata delle risorse e l&#39;accesso a tutte le applicazioni Creative Cloud e di altro tipo, garantendo la conformità con il branding e altri standard.

Le attività chiave eseguite con l&#39;app desktop [!DNL Experience Manager] v1 includono:

1. [Connetti con un server  [!DNL Experience Manager] ](#installandconnect)
1. [Aprire le risorse direttamente nell’app desktop](#openondesktop)
1. [Modificare ed estrarre le risorse dall’app desktop](#workonassets)
1. [Caricare risorse e cartelle in blocco](#bulkupload)

Per le varie azioni consigliate e non consigliate, consulta le [best practice per l&#39;utilizzo dell&#39;app desktop](best-practices-for-v1.md). Se riscontri problemi durante l&#39;utilizzo dell&#39;app, vedi come [risolvere i problemi [!DNL Experience Manager] dell&#39;app desktop](troubleshoot-app-v1.md).

>[!NOTE]
>
>L&#39;app desktop è stata introdotta in [!DNL Experience Manager] versione 6.1 ed è stata denominata [!DNL Experience Manager Assets Companion App].

## [!DNL Experience Manager] punti di contatto dell&#39;app desktop nel flusso di lavoro creativo {#aem-desktop-app-touch-points-in-the-creative-workflow}

L&#39;app desktop [!DNL Experience Manager], insieme a [!DNL Assets], si integra nel flusso di lavoro creativo e offre i seguenti punti di contatto.

![[!DNL Experience Manager] punti di contatto dell&#39;app desktop per il flusso di lavoro creativo](assets/aem_desktopapp_workflow.png)

[!DNL Experience Manager] punti di contatto dell&#39;app desktop per il flusso di lavoro creativo

## Installa e connetti l&#39;app al server [!DNL Experience Manager] {#installandconnect}

Prima di iniziare a creare o modificare le risorse creative, connetti l&#39;applicazione desktop al server [!DNL Assets] per scaricare e caricare le risorse nell&#39;archivio. Esegui le seguenti attività:

1. [Installa l&#39;app](#installapp).
1. [Imposta le tue preferenze](#inapppref) e i dettagli di connessione.
1. [Connettersi a un [!DNL Experience Manager] server](#connect) e montare l&#39;archivio delle risorse come unità locale.
1. [Attiva azioni desktop](#desktopactions) nel server [!DNL Experience Manager].

L&#39;app desktop [!DNL Experience Manager] utilizza una connessione HTTPS per connettersi al server [!DNL Experience Manager] e trasferire le risorse in modo sicuro e affidabile.

>[!NOTE]
>
>Per tutti o parte dei passaggi di installazione e configurazione, potrebbe essere necessario l&#39;intervento dell&#39;amministratore di [!DNL Experience Manager] o dell&#39;amministratore di sistema.

### Installare l’applicazione {#installapp}

Assicurati che l’app supporti la tua versione del server Experience Manager per l’utilizzo dell’app desktop Experience Manager. Scarica il file di installazione appropriato (binario) per il sistema operativo in uso (Mac o Windows) e installa l’app.

A seconda delle preferenze di rete e di sistema, può essere necessaria una configurazione dettagliata. Per ulteriori dettagli, consulta [Installare e configurare [!DNL Experience Manager] l&#39;app desktop](install-configure-app-v1.md).

1. Vai alla [[!DNL Experience Manager] pagina di download dell&#39;app desktop v1.10](/help/using/release-notes-of-v1.md) e scarica il file binario appropriato per il tuo sistema operativo.
1. Avvia il file di installazione scaricato e segui le istruzioni visualizzate per installare l’app.

   >[!NOTE]
   >
   >È possibile installare e attivare una sola istanza dell&#39;app desktop [!DNL Experience Manager] alla volta.

### Comprendere le opzioni e le preferenze in-app {#inapppref}

L&#39;applicazione consente alle impostazioni di connettersi e disconnettersi dai server [!DNL Experience Manager], visualizzare lo stato dei caricamenti, gestire la cache locale e così via. Le impostazioni predefinite funzionano per un utente tipico dell’applicazione. Puoi modificare le impostazioni per sfruttare al meglio l’applicazione. Inoltre, è possibile sfruttare al meglio l&#39;integrazione con il server [!DNL Experience Manager]. Di seguito sono riportate le varie impostazioni:

**Esplora Assets** Aprire l&#39;unità locale in cui è montato l&#39;archivio [!DNL Assets]. In altre parole, esplora le risorse ora rese disponibili sul computer locale.

**Visualizza stato risorse** Quando vengono caricate risorse modificate o vengono aggiunte nuove risorse all&#39;archivio [!DNL Assets], l&#39;applicazione carica le risorse in background. Il caricamento in background consente operazioni senza problemi, senza dover attendere il completamento del caricamento, in particolare per le risorse di grandi dimensioni. Puoi salvare le modifiche localmente e dimenticarle. L’invio di queste risorse al server da parte dell’applicazione richiede un po’ di tempo, a seconda della larghezza di banda disponibile. Puoi controllare lo stato del caricamento, insieme ad alcune informazioni di base.

**Opzioni** Fare clic sulle opzioni nella barra delle applicazioni del desktop per impostare l&#39;avvio dell&#39;app all&#39;avvio, connettersi al server [!DNL Experience Manager] all&#39;avvio e modificare la lettera di unità locale per [!DNL Assets] dopo il montaggio.

**Avanzate > Gestisci cache** È possibile controllare la quantità di spazio su disco disponibile per la memorizzazione nella cache locale. Gli artefatti del server [!DNL Assets] sono memorizzati nella cache locale per un&#39;esperienza più fluida. È possibile modificare le impostazioni predefinite in base alle proprie esigenze. Inoltre, puoi cancellare la cache per recuperare nuovamente tutte le risorse. Quando si cancella la cache, vengono mantenute le modifiche non salvate. Tutte le risorse non archiviate nel server [!DNL Experience Manager] vengono mantenute e non eliminate.

### Connetti a un server [!DNL Experience Manager] {#connect}

L’app supporta la configurazione proxy su Mac e Windows. La configurazione viene letta all&#39;avvio dell&#39;app. Se modifichi le impostazioni proxy, riavvia l’app per rendere effettive le modifiche.

>[!NOTE]
>
>Se modifichi le impostazioni proxy, riavvia l’app per rendere effettive le modifiche. In caso contrario, l’app continua a utilizzare il server proxy configurato in precedenza.

1. Avvia l&#39;app desktop [!DNL Experience Manager]. Per mappare l&#39;istanza [!DNL Experience Manager] con l&#39;app, specificare il server [!DNL Experience Manager] nel formato `https://[aem-server-url]:[port]`.

   ![Esegui l&#39;autenticazione in Mac e fornisci l&#39;URL del server [!DNL Experience Manager]](assets/aem_desktop_app_server_url.png)

1. Nella schermata di accesso, specifica il nome utente e la password per l’istanza. Per specificare un&#39;istanza [!DNL Experience Manager] alternativa, selezionare l&#39;opzione **[!UICONTROL Alternate Login URL]**.

   ![Fornire le credenziali del server [!DNL Experience Manager] nella schermata di accesso nell&#39;app desktop [!DNL Experience Manager]](assets/login_screen_v1.png)

### Abilita azioni desktop nell&#39;interfaccia Web [!DNL Experience Manager] {#desktopactions}

Dall’interfaccia utente di Assets, puoi esplorare i percorsi delle risorse o estrarle e aprire la risorsa per la modifica nell’applicazione desktop. Queste opzioni sono denominate azioni desktop e non sono abilitate per impostazione predefinita. Per abilitarlo, segui la procedura riportata di seguito.

1. Nell’interfaccia di Assets, tocca o fai clic sull’icona Utente nell’angolo superiore destro della barra degli strumenti.
1. Fare clic su **[!UICONTROL My Preferences]** per visualizzare la finestra di dialogo **[!UICONTROL Preferences]**.

   Interfaccia ![[!DNL Experience Manager] con preferenze utente](assets/aem_ui_user_preferences.png)

1. Nella finestra di dialogo [!UICONTROL User Preferences], seleziona **[!UICONTROL Show Desktop Actions For Assets]**, quindi fai clic su **[!UICONTROL Accept]**.

   ![Seleziona [!UICONTROL Show Desktop Actions For Assets] per abilitare le azioni desktop](assets/enable_desktop_actions.png)

   *Figura: selezionare [!UICONTROL Show Desktop Actions For Assets] per abilitare le azioni desktop.*

## Accedere e aprire le risorse sul desktop {#openondesktop}

Quando fai clic su **Apri** per aprire una risorsa nel computer locale, l&#39;app scarica la risorsa nella cache interna. L’app avvia l’applicazione desktop nativa associata al tipo di file della risorsa scaricata.

In Mac, seleziona **Apri** dal menu di scelta rapida per aprire una risorsa tramite l&#39;app desktop [!DNL Experience Manager]. In Windows, seleziona Apri sul web dal menu di scelta rapida per aprire la risorsa. Nella finestra Stato risorsa, tocca o fai clic sull&#39;icona ![Apri sul desktop](assets/do-not-localize/aemassets_icon_openondesktop.png) per aprire la risorsa.

Per i file Adobe InDesign (INDD), selezionare **[!UICONTROL Open]** dal menu di scelta rapida. Quando fai clic su questa opzione, l’app scarica le risorse collegate nel file system locale e quindi apre il file INDD in Adobe InDesign. Questo metodo garantisce che le risorse necessarie siano disponibili localmente quando si modifica il file INDD.

![Opzioni del menu di scelta rapida per accedere e aprire le risorse tramite l&#39;app desktop [!DNL Experience Manager]](assets/aem_desktopapp_mac_context_menu.png)

*Figura: Opzioni del menu di scelta rapida per accedere e aprire le risorse tramite l&#39;app desktop [!DNL Experience Manager].*

>[!NOTE]
>
>L&#39;Adobe consiglia di passare a Opzioni visualizzazione Finder su Mac e disattivare le opzioni **Mostra informazioni elemento**, **Mostra anteprima elemento** e **Mostra colonna anteprima** per la cartella [!DNL Assets] montata. Migliora le prestazioni.

### Opzioni aggiuntive nell&#39;interfaccia [!DNL Experience Manager] {#additional-options-in-aem-assets}

Dopo aver mappato l&#39;archivio [!DNL Assets] sull&#39;unità locale, è possibile abilitare icone aggiuntive e la funzione Caricamento cartella per le risorse e le cartelle mappate.

1. Apri l&#39;interfaccia [!DNL Assets] e passa il puntatore su una cartella o una risorsa per visualizzare le azioni sul desktop come azioni rapide nella vista a schede.

   ![Nell&#39;interfaccia utente di Assets, apri il menu Azioni rapide per visualizzare le azioni sul desktop](assets/desktop_actions_in_card_view.png)

   *Figura: nell&#39;interfaccia utente di Assets, apri il menu Azioni rapide per visualizzare le azioni sul desktop.*

   Queste azioni sul desktop sono disponibili anche quando fai clic sull&#39;opzione **Azioni desktop** nella barra degli strumenti dopo aver selezionato la risorsa o dalla barra degli strumenti nella pagina della risorsa.

1. Per aprire la risorsa nell&#39;applicazione desktop associata all&#39;estensione di file specifica, fare clic sull&#39;azione rapida **Apri sul desktop** ![Apri sul desktop](assets/do-not-localize/aemassets_icon_openondesktop.png).

   In alternativa, scegliere **Apri** dal menu **Azioni desktop** nella barra degli strumenti.

Per individuare la risorsa specifica nel file system locale, fai clic su **Mostra** azione rapida ![Mostra icona](assets/do-not-localize/aemassets_reveal_icon.png). In alternativa, scegliere **Mostra** dal menu **Azioni desktop** nella barra degli strumenti.

## Comprendere gli stati delle risorse {#understand-the-asset-statuses}

| ![Icona app predefinita di Windows](assets/do-not-localize/win_default.png) | L’app è connessa al server e tutte le risorse sono sincronizzate. |
--- |--- |
| ![Icona Windows disabilitato](assets/do-not-localize/win_disabled.png) | L&#39;app viene avviata ma non è connessa al server. Alcune risorse potrebbero essere in attesa di sincronizzazione. |
| ![Icona sincronizzazione file di Windows](assets/do-not-localize/win_sync.png) | Sincronizzazione in corso di Assets. I file vengono caricati o scaricati. È possibile visualizzare gli stati esatti e sospendere i trasferimenti dalla finestra Stato cespite. |
| ![Icona riconnessione Windows](assets/do-not-localize/win_refresh.png) | L&#39;app sta tentando di riconnettersi. È possibile che i problemi di rete causino la disconnessione. |

## Lavorare sulle risorse {#workonassets}

### Estrarre risorse dall&#39;interfaccia Web [!DNL Experience Manager] {#check-out-assets-from-the-aem-web-interface}

[!DNL Experience Manager Assets] consente di estrarre le risorse per la modifica e archiviarle nuovamente dopo aver completato le modifiche. Dopo aver estratto una risorsa, solo tu puoi modificarla, annotarla, pubblicarla, spostarla o eliminarla. L’estrazione di una risorsa blocca la risorsa e impedisce ad altri utenti di eseguire una di queste operazioni. Per poter estrarre/archiviare le risorse, è necessario disporre dell&#39;accesso in scrittura.

Esistono due modi per estrarre le risorse dall&#39;interfaccia Web [!DNL Experience Manager]. Per informazioni dettagliate sul primo metodo, vedere [file di archiviazione ed estrazione dall&#39;interfaccia utente di Assets](https://experienceleague.adobe.com/it/docs/experience-manager-65/content/assets/managing/check-out-and-submit-assets). Segui questi passaggi per i secondi metodi per estrarre e aprire la risorsa quando l&#39;app desktop [!DNL Experience Manager] è installata.

1. Apri l&#39;interfaccia [!DNL Assets] e passa il puntatore su una cartella o una risorsa per visualizzare le azioni sul desktop come azioni rapide nella vista a schede.

   Opzione ![Proprietà nella vista a schede](assets/desktop_actions_in_card_view.png)

   Queste azioni sul desktop sono disponibili anche quando tocchi o fai clic sull’icona Azioni desktop nella barra degli strumenti dopo aver selezionato la risorsa o nella barra degli strumenti nella pagina della risorsa.

1. Per aprire la risorsa, tocca o fai clic sull&#39;icona Apri sul desktop ![Apri sul desktop](assets/do-not-localize/aemassets_icon_openondesktop.png).

   In alternativa, scegliere Apri dal menu Azioni desktop nella barra degli strumenti.

   >[!NOTE]
   >
   >Quando modifichi un file aperto ma non estratto, gli altri utenti non sanno che stai aggiornando la risorsa.

1. Per aprire una risorsa per la modifica in un&#39;applicazione Adobe Creative Cloud, fare clic sull&#39;icona ![Modifica desktop](assets/do-not-localize/aemassets_icon_editdesktop.png). Questa opzione estrae anche la risorsa per la modifica. Dopo aver completato la modifica, archivia la risorsa per aggiornare le modifiche in [!DNL Assets].

   In alternativa, scegliere Modifica dal menu Azioni desktop nella barra degli strumenti.

1. Selezionare l&#39;opzione Apri. Le risorse selezionate vengono aperte in modalità anteprima.
1. Per modificare le risorse, seleziona l’opzione Modifica. Le risorse vengono aperte in modalità di modifica.

### Estrarre risorse da Finder su macOS {#check-out-assets-on-mac}

L’app consente di estrarre i file di risorse per impedire ad altri utenti di modificare i file su cui stai lavorando.

1. Dal menu di scelta rapida di Mac, seleziona l’opzione Apri cartella AEM Assets per aprire il Finder.

   ![Opzioni del menu di scelta rapida per accedere e aprire le risorse tramite l&#39;app desktop [!DNL Experience Manager]](assets/aem_desktopapp_mac_context_menu.png)

   *Figura: Opzioni del menu di scelta rapida per accedere e aprire le risorse tramite l&#39;app desktop [!DNL Experience Manager].*

1. Passare alla risorsa da estrarre.
1. Fai clic con il pulsante destro del mouse sulla risorsa e seleziona Altre informazioni di Assets dal menu di scelta rapida.
1. Nella finestra di dialogo Informazioni risorsa, tocca o fai clic sull’icona Estrai per estrarre la risorsa. L’icona Check-Out attiva l’icona Check-In dopo averla toccata o fatta clic su di essa.

   ![Individua la risorsa da estrarre](assets/browse_assets_to_checkout.png)

1. Per archiviare la risorsa in modo che sia disponibile per altri utenti, tocca o fai clic sull’icona di archiviazione nella finestra di dialogo Informazioni risorsa.

### Estrarre risorse in Windows {#check-out-assets-on-windows}

L’app consente di estrarre i file di risorse per impedire ad altri utenti di modificare i file su cui stai lavorando.

1. Dal menu di scelta rapida, selezionare Esplora Assets per aprire Esplora risorse.
1. In Esplora risorse passare alla posizione della risorsa da estrarre.
1. Fai clic con il pulsante destro del mouse sulla risorsa e seleziona Apri sul web dal menu di scelta rapida.
1. Nella finestra di dialogo Informazioni risorsa, fai clic sull’icona Estrai. L&#39;icona Check-out consente di passare all&#39;icona Check-In.

   ![Icona Estrai attiva](assets/checkout_icon_toggles.png)

1. Esamina la risorsa in Explorer. L&#39;icona di blocco sulla risorsa ![icona di blocco risorsa](assets/do-not-localize/aemassets_icon_lockcheckout.png) indica che la risorsa è stata estratta.

   >[!NOTE]
   >
   >L’icona del lucchetto potrebbe apparire dopo un certo ritardo. L&#39;app desktop [!DNL Experience Manager] memorizza nella cache le risorse per l&#39;accesso rapido. L&#39;aggiornamento dello stato bloccato potrebbe richiedere alcuni minuti.

1. Per archiviare la risorsa in modo che sia disponibile per altri utenti, tocca o fai clic sull&#39;icona di archiviazione nella finestra di dialogo **Informazioni risorsa**.

### Archiviare una risorsa tramite il Finder o Esplora risorse e tramite l’interfaccia web {#check-in-an-asset-using-finder-or-explorer-and-using-web-interface}

Dopo aver modificato le risorse, salvale nell’applicazione desktop. Dal menu di scelta rapida, selezionare **Ulteriori informazioni su Assets** e fare clic su Archivia.

Le risorse sono state caricate nel server [!DNL Experience Manager]. In alternativa, è possibile controllare lo stato del caricamento selezionando **Visualizza stato risorsa** dall&#39;icona sulla barra delle applicazioni. In alternativa, è possibile archiviare una risorsa dall&#39;interfaccia Web [!DNL Experience Manager]. Fai clic sulle risorse estratte o selezionale. Dalla barra degli strumenti, fare clic sull&#39;icona di archiviazione ![icona di archiviazione](assets/do-not-localize/aemassets_icon_checkin.png).

Una risorsa viene caricata automaticamente in [!DNL Experience Manager] dopo il salvataggio locale di eventuali modifiche. L&#39;archiviazione rende la risorsa disponibile ad altri [!DNL Experience Manager] utenti per la modifica.

### Carica risorse e cartelle in blocco sul server [!DNL Experience Manager] {#bulkupload}

Utilizzando l&#39;app desktop [!DNL Experience Manager], puoi caricare un&#39;intera cartella contenente risorse dalla directory dei file locale in [!DNL Assets]. In questo modo, tutte le risorse all’interno della cartella vengono caricate in blocco invece di doverle caricare una alla volta.

1. Dall&#39;interfaccia utente di Assets, tocca o fai clic su **Crea** nella barra degli strumenti, quindi seleziona **Carica cartella** dal menu.
1. Individua la cartella da caricare e selezionala.
1. Tocca o fai clic su OK. La finestra di dialogo Stato di Assets mostra lo stato del caricamento.

   ![Visualizzare lo stato del caricamento nella finestra Stato risorsa](assets/aem_desktopapp_bulkupload_status.png)

   Visualizzare lo stato del caricamento nella finestra Stato risorsa

   >[!NOTE]
   >
   >Puoi mettere in pausa o annullare manualmente il caricamento toccando o facendo clic sull’icona appropriata.

1. Dopo il caricamento della cartella, chiudi la finestra di dialogo e passa all’interfaccia utente di Assets. La cartella caricata viene visualizzata nell’interfaccia web.

L&#39;Adobe non consiglia di copiare o trascinare un numero maggiore di file o cartelle nidificate dal file system locale nell&#39;area di condivisione di rete. L’app non è in grado di controllare il processo di caricamento a causa di limitazioni tecniche e prestazioni insoddisfacenti.

In alternativa, selezionare i file o le cartelle nel Finder o in Esplora risorse, copiarli, passare alla cartella di destinazione nell&#39;area di condivisione di rete e scegliere **Incolla Assets** dal menu di scelta rapida dell&#39;app desktop [!DNL Experience Manager]. In questo modo, l&#39;app desktop [!DNL Experience Manager] inizia a caricare le risorse incollate in modo simile all&#39;opzione **Carica cartella** disponibile nell&#39;interfaccia Web [!DNL Experience Manager].

>[!MORELIKETHIS]
>
>* [Risolvere i problemi [!DNL Experience Manager] relativi all&#39;applicazione desktop](troubleshoot-app-v1.md)
