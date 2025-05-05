---
title: Installare e configurare l’app desktop v1.10
description: Installa e configura  [!DNL Experience Manager] l'app desktop versione 1.10 per l'utilizzo con  [!DNL Assets] server e mappa le risorse da installare come unità sul desktop.
exl-id: 7f3bdfb1-d345-4e48-b020-6e06531f46f2
source-git-commit: 1c7437786a50eeafa884ce92b745f3438b2d2b88
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 0%

---

# Installa e configura l&#39;app desktop [!DNL Experience Manager] v1.10 {#install-and-configure-aem-desktop-app}

Utilizzando l&#39;app desktop [!DNL Experience Manager], le risorse di [!DNL Experience Manager] sono facilmente accessibili sul desktop locale e possono essere utilizzate in qualsiasi applicazione desktop. Assets può essere rilevato in Mac Finder o Esplora risorse, modificato nelle app desktop e le modifiche vengono salvate nuovamente in [!DNL Experience Manager], creando una nuova versione al momento del caricamento.

Questa integrazione consente a diversi ruoli di gestire centralmente le risorse all’interno dell’organizzazione in Assets, di accedervi in Creative Cloud e altre applicazioni e di conformarsi facilmente a vari standard, tra cui il branding.

Per utilizzare l&#39;app desktop [!DNL Experience Manager]:

* Verificare che la versione del server [!DNL Experience Manager] sia compatibile con l&#39;app desktop [!DNL Experience Manager]. Vedere la [matrice di compatibilità](release-notes-of-v1.md#compatibilitymatrix).

* Scarica e installa l’applicazione.

* Verifica la connessione utilizzando alcune risorse. Consulta [Accedere e aprire le risorse sul desktop](use-app-v1.md#openondesktop).

## Requisiti di sistema, prerequisiti e collegamenti per il download {#system-requirements-prerequisites-and-download-links}

Per informazioni dettagliate, consulta le [[!DNL Experience Manager] note sulla versione dell&#39;app desktop](release-notes-of-v1.md).

## Installa e connetti l&#39;app al server [!DNL Experience Manager] {#install-and-connect-aem-desktop-app-to-aem-server}

Per ulteriori dettagli, vedere [Installare e connettere [!DNL Experience Manager] l&#39;app desktop al [!DNL Experience Manager] server](use-app-v1.md#installandconnect).

>[!NOTE]
>
>È possibile installare e attivare una sola istanza dell&#39;app desktop [!DNL Experience Manager] alla volta.

## Gestione dei file {#file-handling}

Quando si modifica un file da un percorso di condivisione di rete montato dall&#39;app desktop, i file vengono salvati in tale percorso in due fasi. Nella prima fase, un file viene salvato localmente. L’utente può salvare il file e continuare a utilizzarlo senza attendere il completamento del trasferimento.

Nella seconda fase, l&#39;app desktop carica il file aggiornato sul server [!DNL Experience Manager] dopo un ritardo predefinito (ad esempio, 30 secondi). Questa operazione viene eseguita in background. Per visualizzare lo stato dell’operazione di caricamento, utilizza l’opzione Visualizza stato risorsa.

1. Carica una risorsa in Assets.

1. Fare clic sull&#39;icona dell&#39;app desktop [!DNL Experience Manager] nella barra degli strumenti.

1. Dal menu, seleziona l’opzione Visualizza stato risorsa.

1. Nella finestra di dialogo, controlla lo stato dell’operazione di caricamento.

>[!NOTE]
>
>L&#39;app desktop [!DNL Experience Manager] può gestire risorse fino a 40 GB di dimensioni.

## Connettersi a un&#39;istanza [!DNL Experience Manager] dietro un Dispatcher {#connect-to-an-aem-instance-behind-a-dispatcher}

I metodi di copia e spostamento nell&#39;API di Assets richiedono il passaggio delle seguenti intestazioni aggiuntive a [!DNL Experience Manager]:

* Destinazione X
* Profondità X
* X-Overwrite

Il desktop [!DNL Experience Manager] si connette a [!DNL Experience Manager] utilizzando un URL che include la porta predefinita. Pertanto, l&#39;impostazione `virtualhosts` nella configurazione Dispatcher deve includere il numero di porta predefinito. Per ulteriori informazioni sulla configurazione di `virtualhosts`, vedere [identificare gli host virtuali](https://experienceleague.adobe.com/en/docs/experience-manager-dispatcher/using/configuring/dispatcher-configuration#identifying-virtual-hosts-virtualhosts).

Per ulteriori informazioni sulla configurazione di Dispatcher per passare attraverso queste intestazioni aggiuntive, vedere [Specifica delle intestazioni HTTP](https://experienceleague.adobe.com/en/docs/experience-manager-dispatcher/using/configuring/dispatcher-configuration#specifying-the-http-headers-to-pass-through-clientheaders).

### Supporto proxy {#proxy-support}

L&#39;app desktop [!DNL Experience Manager] utilizza il proxy predefinito del sistema per connettersi a Internet tramite HTTPS. L&#39;app può connettersi solo utilizzando un proxy di rete che non richiede autenticazione aggiuntiva.

Se si configurano o si modificano le impostazioni del server proxy per Windows (Opzioni Internet > Impostazioni LAN), riavviare l&#39;app desktop [!DNL Experience Manager] per rendere effettive le modifiche.

>[!NOTE]
>
>La configurazione proxy viene applicata solo all&#39;avvio dell&#39;app desktop. Per rendere effettive le modifiche, chiudi e riavvia l’app.

Se il proxy richiede l&#39;autenticazione, il team IT può consentire il passaggio del traffico dell&#39;applicazione mediante l&#39;URL Experience Manager Assets nelle impostazioni del server proxy.

## Personalizzare la finestra di dialogo Informazioni risorsa {#customize-the-asset-info-dialog}

Potete personalizzare la finestra di dialogo Info risorsa sovrapponendo uno o entrambi i componenti:

* Pagina dell&#39;interfaccia utente Granite in `/libs/dam/gui/content/assets/moreinfo`.

* Il componente HTL `/css/javascript` in `/libs/dam/gui/components/admin/moreinfo`.

Quale componente viene sovrapposto dipende dalla natura della personalizzazione. Per modificare i componenti da visualizzare nella finestra di dialogo Informazioni risorsa, sovrapponi la pagina dell’interfaccia utente Granite. Per modificare il contenuto HTML, CSS o JavaScript della finestra di dialogo, sovrapponi il componente HTL.

## Gestisci cache {#manage-cache}

In Windows, la cache si trova in `%LOCALAPPDATA%\Adobe\AssetsCompanion\Cache\`, dove è una versione codificata dell&#39;host [!DNL Experience Manager] configurato nell&#39;app desktop. `http://localhost:4502`, ad esempio, verrà visualizzato come `http%3A%2F%2Flocalhost%3A4502%2F`.

In macOS X, una directory simile si trova in `~/Library/Group Containers/group.com.adobe.aem.desktop/cache`.

### Opzione in-app per gestire la cache {#in-app-option-to-manage-cache}

È possibile controllare la quantità di spazio su disco disponibile per la memorizzazione nella cache locale. Gli artefatti del server Assets vengono memorizzati nella cache locale per un’esperienza più fluida. È possibile modificare le impostazioni predefinite in base alle proprie esigenze. Inoltre, puoi cancellare la cache per recuperare nuovamente tutte le risorse. Per impostare le opzioni desiderate, fare clic sull&#39;icona dell&#39;applicazione e fare clic su **[!UICONTROL Advanced]** > **[!UICONTROL Manage Cache]**. **&#x200B;**

>[!NOTE]
>
>Quando si cancella la cache, vengono mantenute le modifiche non salvate. Tutte le risorse non archiviate nel server [!DNL Experience Manager] vengono mantenute e non eliminate.

### Cambia la posizione della cache in Windows {#change-location-of-cache-on-windows}

La posizione predefinita della cache per l&#39;app desktop [!DNL Experience Manager] è la seguente:

* In Windows, `%LocalAppData%\Adobe\AssetsCompanion\Cache\EncodedAEMEndpoint`.

* In Mac, `~/Library/Group/Containers/group.com.adobe.aem.desktop/cache/EncodedAEMEndpoint`.

`EncodedAEMEndpoint` è l&#39;URL dell&#39;endpoint [!DNL Experience Manager] configurato dall&#39;app. Il valore è una versione codificata dell&#39;URL di destinazione del server [!DNL Experience Manager]. Ad esempio, se l&#39;applicazione è destinata a `http://localhost:4502`, il nome della directory è `http%3A%2F%2Flocalhost%3A4502`. Il percorso Windows della directory cache in questo esempio è `%LocalAppData%\Adobe\AssetsCompanion\Cache\http%3A%2F%2Flocalhost%3A4502`.

Per puntare l&#39;applicazione a una cartella diversa o a un&#39;unità diversa, modificare il file di configurazione dell&#39;applicazione.

1. Passa alla directory di installazione dell’app. Il percorso predefinito in Windows è `C:\Program Files (x86)\Adobe\Adobe Experience Manager Desktop`.

1. Modificare il file `Adobe Experience Manager Desktop.exe.config` con un editor di testo.

   Per salvare le modifiche apportate al file sono necessari privilegi di amministratore.

1. Cercare la stringa &quot;ProxyCacheRoot&quot;. Il valore è impostato sulla posizione della cache `%LocalAppData%\Adobe\AssetsCompanion\Cache`. È sufficiente modificare questo valore in qualsiasi percorso valido.

   >[!NOTE]
   >
   >L&#39;app crea automaticamente una sottodirectory *&lt;endpoint AEM codificato>*. Questo comportamento non è configurabile.

>[!MORELIKETHIS]
>
>* Guarda un [introduzione all&#39;app desktop](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/creative-workflows/aem-desktop-app) (5 minuti, 43 secondi). [!DNL Experience Manager] 
>* [Utilizza [!DNL Experience Manager] app desktop](use-app-v1.md).
>* [Risoluzione dei problemi [!DNL Experience Manager] app desktop](troubleshoot-app-v1.md).
