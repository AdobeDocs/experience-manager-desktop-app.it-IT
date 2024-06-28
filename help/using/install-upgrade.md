---
title: Installare e configurare l’app desktop
description: Installare e configurare [!DNL Adobe Experience Manager] app desktop con cui lavorare [!DNL Adobe Experience Manager Assets] e scaricare le risorse sul file system locale.
feature: Desktop App,Release Information
exl-id: 422e51c1-c456-4151-bb43-4b3d29a58187
source-git-commit: 1c7437786a50eeafa884ce92b745f3438b2d2b88
workflow-type: tm+mt
source-wordcount: '1449'
ht-degree: 0%

---

# Installa [!DNL Adobe Experience Manager] app desktop {#install-app-v2}

Utilizzo di [!DNL Adobe Experience Manager] dell&#39;app desktop, le risorse in [!DNL Experience Manager] sono facilmente disponibili sul desktop locale e possono essere utilizzati in qualsiasi applicazione desktop nativa. Assets può essere visualizzato in anteprima e aperto nelle app desktop. Possono essere visualizzati nel Finder o in Explorer per l&#39;utilizzo nei documenti e modificati localmente. Le modifiche vengono salvate di nuovo in [!DNL Experience Manager], creando una nuova versione al momento del caricamento.

Tale integrazione consente a vari ruoli dell’organizzazione di:

* Gestione centralizzata delle risorse in [!DNL Experience Manager Assets].

* Accedi alle risorse in qualsiasi applicazione desktop nativa, incluse le applicazioni di terze parti e in Adobe Creative Cloud. In questo modo gli utenti possono aderire facilmente ai vari standard, compreso il branding.

Per utilizzare [!DNL Experience Manager] app desktop:

* Assicurati che il tuo [!DNL Experience Manager] è compatibile con [!DNL Experience Manager] app desktop.

* Scarica e installa l’applicazione. Consulta [installare l’app desktop](#install-v2) di seguito.

* Verifica la connessione utilizzando alcune risorse. Consulta [come sfogliare e cercare le risorse](using.md#browse-search-preview-assets).

## Requisiti di sistema, prerequisiti e collegamenti per il download {#tech-specs-v2}

Per informazioni dettagliate, vedere [[!DNL Experience Manager] Note sulla versione dell’app desktop](release-notes.md).

## Aggiornamento da una versione precedente {#upgrade-from-previous-version}

Se utilizzi la versione 1.x dell’app desktop, comprendi le differenze e le analogie tra la versione precedente e quella più recente dell’app. Consulta [novità dell’app desktop](introduction.md#whats-new-v2) e [come funziona l’app](release-notes.md#how-app-works).

>[!NOTE]
>
>Due versioni di un&#39;app desktop non possono coesistere in un computer. Prima di installare una versione, disinstalla l’altra versione.

Per effettuare l’aggiornamento da una versione precedente dell’app, segui queste istruzioni:

1. Prima di eseguire l&#39;aggiornamento, sincronizza tutte le risorse e carica le modifiche in [!DNL Experience Manager]. In questo modo si evita di perdere eventuali modifiche durante la disinstallazione dell’app.

1. Disinstalla la versione precedente dell’app. Durante la disinstallazione, selezionare l&#39;opzione per cancellare la cache.

1. Riavvia il computer.

1. [Scarica](release-notes.md) e [installare](#install-v2) l’app più recente. Seguire le istruzioni riportate di seguito.

## Installa {#install-v2}

Per installare l’app desktop, segui la procedura riportata di seguito. Disinstalla qualsiasi Adobe esistente [!DNL Experience Manager] app desktop v1.x prima di installare l’app più recente. Per ulteriori informazioni, vedi sopra.

1. Scarica il programma di installazione più recente da [note sulla versione](release-notes.md) pagina.

1. Mantieni l’URL e le credenziali del [!DNL Experience Manager] di installazione.

1. Se aggiorni un’app da un’altra versione, consulta [aggiornare l’app desktop](#upgrade-from-previous-version).

1. Ignora questo passaggio se utilizzi [!DNL Experience Manager] as a [!DNL Cloud Service], [!DNL Experience Manager] 6.4.4 o successiva, oppure [!DNL Experience Manager] 6.5.0 o successiva. Assicurati che il tuo [!DNL Experience Manager] la configurazione soddisfa i requisiti di compatibilità indicati nella [note sulla versione](release-notes.md). Se necessario, scaricare le [pacchetto di compatibilità](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq640/featurepack/adobe-asset-link-support) e installarlo utilizzando [!DNL Experience Manager] Gestione pacchetti come [!DNL Experience Manager] amministratore. Per installare un pacchetto, vedi [Come utilizzare i pacchetti](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/sites/administering/contentmanagement/package-manager).

1. Eseguire il file binario del programma di installazione e seguire le istruzioni visualizzate per l&#39;installazione.

1. In Windows, è possibile che venga richiesto di installare `Visual Studio C++ Redistributable 2015`. Seguire le istruzioni visualizzate sullo schermo per installarlo. Se l&#39;installazione non riesce, installarla manualmente. Scarica il programma di installazione da [qui](https://www.microsoft.com/en-us/download/details.aspx?id=52685) e installare entrambi `vc_redist.x64.exe` e `vc_redist.x86.exe` file. Esegui di nuovo [!DNL Experience Manager] programma di installazione dell&#39;app desktop.

1. Riavviare il computer come richiesto. Avvia e configura l’app desktop.

1. Per collegare l’app a un [!DNL Experience Manager] archivio, fai clic sull’icona dell’app nell’area di notifica e avvia l’app. Fornisci l’indirizzo del [!DNL Experience Manager] server nel formato `https://[aem_server]:[port]/`.

   Clic **[!UICONTROL Connect]** e fornisci le credenziali.

   ![Schermata di connessione dell’app desktop all’indirizzo del server di input](assets/connect_da2.png)

   *Figura: Schermata di connessione all’indirizzo del server di input.*

   Seleziona **[!UICONTROL Remember Connection]** per evitare di immettere i dettagli di connessione ogni volta che si accede all&#39;app desktop.

   >[!CAUTION]
   >
   >Verificare che non siano presenti spazi iniziali o finali prima o dopo l&#39;indirizzo del [!DNL Experience Manager] server. In caso contrario, l’app non può connettersi al [!DNL Experience Manager] server.

1. [Facoltativo] Clic **[!UICONTROL I want to connect a different way]** e fai clic su **[!UICONTROL Adobe login]** per accedere al server Experience Manager Assets utilizzando Adobe Identity Management Service (IMS). L’accesso IMS consente all’app desktop di eseguire automaticamente l’aggiornamento del token di accesso, consentendo all’utente di rimanere connesso per un massimo di 14 giorni. Clic **[!UICONTROL Direct login]** per eseguire l&#39;accesso standard al [!DNL Experience Manager] utilizzando le credenziali dell&#39;utente.

   ![Accesso Adobe](assets/adobe-login.png)

1. Una volta stabilita la connessione, puoi visualizzare l’elenco delle cartelle e delle risorse disponibili nella cartella principale del [!DNL Experience Manager] DAM Puoi sfogliare le cartelle dall’interno dell’app.

   ![All’accesso, l’app visualizza il contenuto DAM](assets/firstview_da2.png)

   *Figura: L’applicazione visualizza il contenuto DAM dopo l’accesso*

1. ([!DNL Experience Manager] 6.5.1 o versione successiva) Se utilizzi l’app desktop con [!DNL Experience Manager] 6.5.1 o versione successiva, aggiorna il connettore S3 o Azure alla versione 1.10.4 o successiva. Consulta [Connettore Azure](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/implementing/deploying/deploying/data-store-config#azure-data-store) o [Connettore S3](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/implementing/deploying/deploying/data-store-config#amazon-s-data-store).

   Se sei un cliente Adobe di Managed Services (AMS), contatta l’Assistenza clienti Adobe.

## Impostare le preferenze {#set-preferences}

Per modificare le preferenze, fare clic su ![Icona Altre opzioni](assets/do-not-localize/more_options_da2.png) e **[!UICONTROL Preference]** ![Icona Preferenze](assets/do-not-localize/preferences_icon_da2.png). In **[!UICONTROL Preferences]** regolare i valori dei seguenti elementi:

* [!UICONTROL Launch the application on logon].

* [!UICONTROL Show a window when the application starts].

* **[!UICONTROL Cache Directory]**: posizione della cache locale dell’app (contiene le risorse scaricate localmente).

* **[!UICONTROL Network Drive Letter]**: lettera di unità utilizzata per la mappatura a [!DNL Experience Manager] DAM Non modificare la lettera dell&#39;unità di rete se non si è sicuri. L&#39;app può essere mappata su qualsiasi lettera di unità in Windows. Se due utenti inseriscono risorse da lettere di unità diverse, non possono vedere le risorse posizionate l’uno dall’altro. Il percorso delle risorse cambia. Le risorse rimangono nel file binario (ad esempio, INDD) e non vengono rimosse. L’app elenca tutte le lettere di unità disponibili e per impostazione predefinita utilizza l’ultima lettera disponibile, che è in genere `Z`.

* **[!UICONTROL Maximum Cache Size]**: cache consentita sul disco rigido in GB utilizzata per l’archiviazione delle risorse scaricate localmente.

* **[!UICONTROL Current cache size]**: dimensione di archiviazione delle risorse scaricate localmente. Le informazioni vengono visualizzate solo dopo il download delle risorse tramite l’app.

* **[!UICONTROL Automatically download linked assets]**: quando scarichi il file originale, le risorse posizionate nelle app di Creative Cloud native supportate vengono recuperate automaticamente.

* **[!UICONTROL Maximum number of downloads]**: ![icona di avviso](assets/do-not-localize/caution-icon.png) Cambiate con cautela. Quando si scaricano le risorse per la prima volta (tramite l’opzione Mostra, Apri, Modifica, Scarica o simile), le risorse vengono scaricate solo se il batch contiene meno di questo numero. Il valore predefinito è 50. Non cambiare se non si è sicuri. L’aumento del valore può causare tempi di attesa più lunghi, mentre una riduzione di questo valore potrebbe impedire di scaricare tutte le risorse o cartelle necessarie in un unico tentativo.

* **[!UICONTROL Use legacy conventions when creating nodes for assets and folders]**: ![icona di avviso](assets/do-not-localize/caution-icon.png) Cambiate con cautela. Questa impostazione consente all’app di emulare il comportamento dell’app v1.10 durante il caricamento delle cartelle. Nella versione 1.10, i nomi dei nodi creati nell’archivio rispettano gli spazi e le maiuscole/minuscole dei nomi delle cartelle forniti dall’utente. Tuttavia, nella versione 2.1 dell’app, gli spazi in più nei nomi delle cartelle vengono convertiti in trattini. Ad esempio, il caricamento `New Folder` o `new   folder` crea lo stesso nodo nell’archivio se l’opzione non è selezionata e viene mantenuto il comportamento predefinito nella versione v2.1. Se questa opzione è selezionata, nell’archivio vengono creati nodi diversi per le due cartelle precedenti e il comportamento corrisponde a quello dell’app v1.10.

  Il comportamento predefinito della versione 2.1 rimane invariato: sostituisce più spazi nei nomi delle cartelle con trattini nel nome del nodo dell’archivio e converte i nomi dei nodi in minuscolo.

* **[!UICONTROL Upload Acceleration]**: ![icona di avviso](assets/do-not-localize/caution-icon.png) Cambiate con cautela. Quando si caricano le risorse, l’applicazione può utilizzare i caricamenti simultanei per migliorare la velocità di caricamento. Per aumentare la concorrenza del caricamento, sposta il cursore verso destra. Il dispositivo di scorrimento all’estrema sinistra significa assenza di concorrenza (caricamento a thread singolo), la posizione centrale corrisponde a dieci thread simultanei e il limite massimo all’estrema destra corrisponde a 20 thread simultanei. Un limite di concorrenza più elevato richiede più risorse.

Per aggiornare le preferenze non disponibili, esci da [!DNL Experience Manager] e quindi aggiornare. Dopo aver aggiornato le preferenze, fai clic su ![Salva preferenze](assets/do-not-localize/save_preferences_da2.png).

![Preferenze e impostazioni dell’app desktop](assets/preferences_da2.png)

*Figura: Preferenze dell’app desktop.*

### Supporto proxy {#proxy-support}

Il [!DNL Experience Manager] L’app desktop utilizza il proxy predefinito del sistema per la connessione a Internet tramite HTTPS. L&#39;app può connettersi solo utilizzando un proxy di rete che non richiede autenticazione aggiuntiva.

Se si configurano o si modificano le impostazioni del server proxy per Windows (Opzioni Internet > Impostazioni LAN), riavviare [!DNL Experience Manager] dell&#39;app desktop per rendere effettive le modifiche. La configurazione proxy viene applicata all&#39;avvio dell&#39;app desktop. Per rendere effettive le modifiche, chiudi e riavvia l’app.

Se il proxy richiede l&#39;autenticazione, il team IT può consentire [!DNL Experience Manager Assets] URL nelle impostazioni del server proxy per consentire il passaggio del traffico dell&#39;applicazione.

## Disinstallare l’app {#uninstall-the-app}

Per disinstallare l&#39;applicazione in Windows, eseguire la procedura seguente:

1. Carica tutte le modifiche in [!DNL Experience Manager] per evitare la perdita di eventuali modifiche. Consulta [Modificare le risorse e caricare le risorse aggiornate in [!DNL Experience Manager]](using.md#edit-assets-upload-updated-assets). Disconnettersi e [!UICONTROL Exit] l’app.

1. Rimuovi l’app come rimuoveresti qualsiasi altra applicazione del sistema operativo. Disinstallarlo da Aggiungi e rimuovi programmi in Windows.

1. Per rimuovere la cache e i registri, seleziona la casella di controllo necessaria.

   ![Finestra di dialogo di disinstallazione per rimuovere registri e cache](assets/uninstall_da2.png)

1. Seguire le istruzioni visualizzate. Al termine, riavviare il computer.

Per disinstallare l&#39;applicazione su Mac, eseguire la procedura seguente:

1. Carica tutte le modifiche in [!DNL Experience Manager] per evitare la perdita di eventuali modifiche. Consulta [Modificare le risorse e caricare le risorse aggiornate in [!DNL Experience Manager]](using.md#edit-assets-upload-updated-assets). Disconnettersi e [!UICONTROL Exit] l’app.

1. Rimuovi il `Adobe Experience Manager Desktop.app` da `/Applications`.

In alternativa, per pulire le cache interne dell’applicazione sul Mac e disinstallare l’app, puoi eseguire il seguente comando nel terminale:

```shell
/Applications/Adobe Experience Manager Desktop/Contents/Resources/uninstall-osx/uninstall.sh
```
