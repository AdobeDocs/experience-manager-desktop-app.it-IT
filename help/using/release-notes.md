---
title: Note sulla versione dell'app desktop [!DNL Adobe Experience Manager]
description: Dettagli sulla versione, miglioramenti, nuove funzioni, compatibilità e collegamenti per il download dell'app desktop  [!DNL Adobe Experience Manager] .
mini-toc-levels: 1
feature: Desktop App,Release Information
exl-id: e058e7a2-fcc8-4ad1-899e-20695db6bc72
source-git-commit: b5dace65444ca15d09ec8648deb4c262415f40cf
workflow-type: tm+mt
source-wordcount: '2195'
ht-degree: 10%

---

# Note sulla versione dell&#39;app desktop [!DNL Adobe Experience Manager] {#release-notes-v2}

Di seguito sono riportate le informazioni sulla versione dell’app desktop più recente versione 2.3.3. La data di rilascio è il 16 maggio 2025.

La versione più recente dell’app desktop include le correzioni e i miglioramenti seguenti:

* Puoi caricare le nuove risorse create dal computer locale in AEM, dove è memorizzato l’archivio centrale, e visualizzarle nell’app desktop.
* La funzione di aggiornamento automatico aggiorna automaticamente i contenuti in tempo reale, assicurandoti di visualizzare sempre le informazioni più recenti senza ricaricare manualmente la pagina e ottenere l’elenco delle risorse aggiornate.
* La funzione di fissaggio o sblocco delle cartelle consente di mantenere facilmente accessibili importanti cartelle fissandole o di annullare la visualizzazione sbloccandole quando non sono più necessarie.
* La funzione Rinomina titolo consente di aggiornare o modificare facilmente il titolo di una risorsa, consentendoti di mantenere i nomi precisi e organizzati in base all’evoluzione del contenuto.
* È possibile mantenere il file originale e apportare modifiche a uno simile duplicando i file in percorsi locali e cloud utilizzando l&#39;operazione di duplicazione dei file.
* La funzione di archiviazione ed estrazione consente di gestire l&#39;accesso ai file bloccando un file per la modifica (estrazione) e il salvataggio delle modifiche e rendendolo disponibile ad altri utenti (archiviazione).
* Puoi visualizzare, scaricare e sfogliare le raccolte.
* Puoi assegnare i metadati durante la creazione di una nuova cartella.

Le **versioni supportate di [!DNL Experience Manager]** sono:

* [!DNL Experience Manager] come [!DNL Cloud Service]. Consulta le [note sulla versione](https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/release-notes/home).
* [!DNL Experience Manager] 6.5.0 o versione successiva, su Adobe Managed Services (AMS) o On-Premise. Consulta le [note sulla versione del service pack](https://experienceleague.adobe.com/it/docs/experience-manager-65/content/release-notes/release-notes).

L&#39;app desktop [!DNL Adobe Experience Manager] è disponibile per i seguenti **sistemi operativi**:

* macOS X 10.14 o versione successiva, con le ultime correzioni di bug.
* Windows 10 con Service Pack e correzioni di bug più recenti.

Sono disponibili due versioni del programma di installazione di Windows per AEM Desktop App versione 2.3.1 e successive. Il programma di installazione di base installa l&#39;app desktop AEM nella directory App Data locale dell&#39;utente. Adobe consiglia questo processo di installazione per la maggior parte degli utenti. È disponibile anche un programma di installazione di Windows Enterprise, che installa l&#39;app desktop AEM nella directory dei file di programma condivisi. Questi due programmi di installazione installano la stessa versione di AEM Desktop App, senza differenze di funzionalità.

I **URL di download** per il sistema operativo supportato sono:

| Sistema operativo | [!DNL Experience Manager] as a [!DNL Cloud Service] | [!DNL Experience Manager] 6.x |
|---|---|---|
| macOS (v2.3.3) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-x64-2.3.3.dmg) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-x64-2.3.3.dmg) |
| Silicio macOS Apple (M1) (v2.3.3) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-arm64-2.3.3.dmg) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-arm64-2.3.3.dmg) |
| Windows a 64 bit (v2.3.3) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win-x64-2.3.3.exe) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win-x64-2.3.3.exe) |
| Windows Enterprise a 64 bit (v2.3.3) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win-x64-2.3.3.msi) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win-x64-2.3.3.msi) |
| macOS (v2.3.1) | [Collegamento di download](https://nam04.safelinks.protection.outlook.com/?url=https%3A%2F%2Fexperience.adobe.com%2F%23%2Fdownloads%2Fcontent%2Fsoftware-distribution%2Fen%2Faemcloud.html%3Fpackage%3D%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faemcloud%2Fpublic%2Faem-desktop-app%2Faem-desktop-osx-x64-2.3.1.dmg&amp;data=05%7C02%7Canujm%40adobe.com%7Cfcf599743bd649c5cd7308dcab9ea5cd%7Cfa7b1b5a7b34438794aed2c178decee1%7C0%7C0%7C638573945081954149%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&amp;sdata=mwSX5ilZL0he2raIx8t5ecQ%2FWuizky4MpcCXX3mEN38%3D&amp;reserved=0) | [Collegamento di download](https://nam04.safelinks.protection.outlook.com/?url=https%3A%2F%2Fexperience.adobe.com%2F%23%2Fdownloads%2Fcontent%2Fsoftware-distribution%2Fen%2Faem.html%3Fpackage%3D%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Fadobe%2Fpackages%2Fadobe%2Faem-desktop-app%2Faem-desktop-osx-x64-2.3.1.dmg&amp;data=05%7C02%7Canujm%40adobe.com%7Cfcf599743bd649c5cd7308dcab9ea5cd%7Cfa7b1b5a7b34438794aed2c178decee1%7C0%7C0%7C638573945081981239%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&amp;sdata=LJH3OCFq7yRykN4wU8HN9%2FBXC%2BjfXLJH4QizeFZfRHE%3D&amp;reserved=0) |
| Silicio macOS Apple (M1) (v2.3.1) | [Collegamento di download](https://nam04.safelinks.protection.outlook.com/?url=https%3A%2F%2Fexperience.adobe.com%2F%23%2Fdownloads%2Fcontent%2Fsoftware-distribution%2Fen%2Faemcloud.html%3Fpackage%3D%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faemcloud%2Fpublic%2Faem-desktop-app%2Faem-desktop-osx-arm64-2.3.1.dmg&amp;data=05%7C02%7Canujm%40adobe.com%7Cfcf599743bd649c5cd7308dcab9ea5cd%7Cfa7b1b5a7b34438794aed2c178decee1%7C0%7C0%7C638573945081965822%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&amp;sdata=2YENn0tDduiucogClt6aBZHDOE6dbzBdigq8VQawIO0%3D&amp;reserved=0) | [Collegamento di download](https://nam04.safelinks.protection.outlook.com/?url=https%3A%2F%2Fexperience.adobe.com%2F%23%2Fdownloads%2Fcontent%2Fsoftware-distribution%2Fen%2Faem.html%3Fpackage%3D%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Fadobe%2Fpackages%2Fadobe%2Faem-desktop-app%2Faem-desktop-osx-arm64-2.3.1.dmg&amp;data=05%7C02%7Canujm%40adobe.com%7Cfcf599743bd649c5cd7308dcab9ea5cd%7Cfa7b1b5a7b34438794aed2c178decee1%7C0%7C0%7C638573945081986151%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&amp;sdata=jCepldg4dMej0%2BrK2mUonXwqsWL8ksE8%2BLMSgsH9qTA%3D&amp;reserved=0) |
| Windows a 64 bit (v2.3.1) | [Collegamento di download](https://nam04.safelinks.protection.outlook.com/?url=https%3A%2F%2Fexperience.adobe.com%2F%23%2Fdownloads%2Fcontent%2Fsoftware-distribution%2Fen%2Faemcloud.html%3Fpackage%3D%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faemcloud%2Fpublic%2Faem-desktop-app%2Faem-desktop-win-x64-2.3.1.exe&amp;data=05%7C02%7Canujm%40adobe.com%7Cfcf599743bd649c5cd7308dcab9ea5cd%7Cfa7b1b5a7b34438794aed2c178decee1%7C0%7C0%7C638573945081970892%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&amp;sdata=sRn2UWW%2Bi7SMEvSO74ZGGvJ40vHh1KhLc7zAfKc37Es%3D&amp;reserved=0) | [Collegamento di download](https://nam04.safelinks.protection.outlook.com/?url=https%3A%2F%2Fexperience.adobe.com%2F%23%2Fdownloads%2Fcontent%2Fsoftware-distribution%2Fen%2Faem.html%3Fpackage%3D%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Fadobe%2Fpackages%2Fadobe%2Faem-desktop-app%2Faem-desktop-win-x64-2.3.1.exe&amp;data=05%7C02%7Canujm%40adobe.com%7Cfcf599743bd649c5cd7308dcab9ea5cd%7Cfa7b1b5a7b34438794aed2c178decee1%7C0%7C0%7C638573945081991004%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&amp;sdata=aQWZtEK%2F3cWX8n8Au%2FwZ5Zd9xPVo5phvk%2FuF%2Be0HRrE%3D&amp;reserved=0) |
| Windows Enterprise a 64 bit (v2.3.1) | [Collegamento di download](https://nam04.safelinks.protection.outlook.com/?url=https%3A%2F%2Fexperience.adobe.com%2F%23%2Fdownloads%2Fcontent%2Fsoftware-distribution%2Fen%2Faemcloud.html%3Fpackage%3D%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faemcloud%2Fpublic%2Faem-desktop-app%2Faem-desktop-win-x64-2.3.1.msi&amp;data=05%7C02%7Canujm%40adobe.com%7Cfcf599743bd649c5cd7308dcab9ea5cd%7Cfa7b1b5a7b34438794aed2c178decee1%7C0%7C0%7C638573945081976350%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&amp;sdata=v9C0sLDSkuL%2FMIyae2WkbitJPVgSlAw2BqcaH5Im0uw%3D&amp;reserved=0) | [Collegamento di download](https://nam04.safelinks.protection.outlook.com/?url=https%3A%2F%2Fexperience.adobe.com%2F%23%2Fdownloads%2Fcontent%2Fsoftware-distribution%2Fen%2Faem.html%3Fpackage%3D%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Fadobe%2Fpackages%2Fadobe%2Faem-desktop-app%2Faem-desktop-win-x64-2.3.1.msi&amp;data=05%7C02%7Canujm%40adobe.com%7Cfcf599743bd649c5cd7308dcab9ea5cd%7Cfa7b1b5a7b34438794aed2c178decee1%7C0%7C0%7C638573945081995827%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&amp;sdata=2btCh0aIrUBiyeG37K9YorvzTeIJOggbq%2FRauUMn4LY%3D&amp;reserved=0) |
| macOS (v2.3.0) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-x64-2.3.0.dmg) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-x64-2.3.0.dmg) |
| Silicio macOS Apple (M1) (v2.3.0) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-arm64-2.3.0.dmg) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-arm64-2.3.0.dmg) |
| Windows a 64 bit (v2.3.0) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win-x64-2.3.0.exe) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win-x64-2.3.0.exe) |
| macOS (v2.2.2) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-x64-2.2.2.dmg) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-x64-2.2.2.dmg) |
| Silicio macOS Apple (M1) (v2.2.2) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-arm64-2.2.2.dmg) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-arm64-2.2.2.dmg) |
| Windows a 64 bit (v2.2.2) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win-x64-2.2.2.exe) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win-x64-2.2.2.exe) |
| macOS (v2.2.1) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-x64-2.2.1.dmg) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-x64-2.2.1.dmg) |
| Silicio macOS Apple (M1) (v2.2.1) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-arm64-2.2.1.dmg) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-arm64-2.2.1.dmg) |
| Windows a 64 bit (v2.2.1) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win-x64-2.2.1.exe) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win-x64-2.2.1.exe) |
| macOS (v2.2.0) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-x64-2.2.0.dmg) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-x64-2.2.0.dmg) |
| Silicio macOS Apple (M1) (v2.2.0) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-arm64-2.2.0.dmg) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-arm64-2.2.0.dmg) |
| Windows a 64 bit (v2.2.0) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win-x64-2.2.0.exe) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win-x64-2.2.0.exe) |
| macOS (v2.1.5.0) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-2.1.5.0.dmg) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-2.1.5.0.dmg) |
| Windows a 64 bit (v2.1.5.0) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win64-2.1.5.0.exe) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win64-2.1.5.0.exe) |
| Windows a 32 bit (v2.1.5.0) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win32-2.1.5.0.exe) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win32-2.1.5.0.exe) |
| macOS (v2.1.4.0) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-2.1.4.0.dmg) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-2.1.4.0.dmg) |
| Windows a 64 bit (v2.1.4.0) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win64-2.1.4.0.exe) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win64-2.1.4.0.exe) |
| Windows a 32 bit (v2.1.4.0) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win32-2.1.4.0.exe) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win32-2.1.4.0.exe) |
| macOS (v2.1.3.4) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-2.1.3.4.dmg) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-2.1.3.4.dmg) |
| Windows a 64 bit (v2.1.3.4) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win64-2.1.3.4.exe) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win64-2.1.3.4.exe) |
| Windows a 32 bit (v2.1.3.1) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win32-2.1.3.1.exe) | [Collegamento di download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win32-2.1.3.1.exe) |

## Supporto per risorse e tipi di file diversi {#support-for-file-types}

L&#39;applicazione supporta le risorse archiviate in [!DNL Experience Manager] che rappresentano il file binario per le operazioni di base. L’apertura di file nell’applicazione desktop nativa si basa sull’associazione del sistema operativo dei tipi di file specifici, come PNG o JPG, ad applicazioni specifiche, come Mac Preview o Adobe Photoshop.

Alcuni tipi di file supportano il posizionamento di risorse collegate nel file binario. L&#39;applicazione prescarica le risorse collegate se la risorsa è presente nell&#39;archivio [!DNL Experience Manager] quando tali file binari vengono aperti tramite l&#39;app desktop. I tipi di file attualmente supportati sono:

* [!DNL Adobe InDesign] file (formato INDD)
* [!DNL Adobe Illustrator] file (formato AI)
* [!DNL Adobe Photoshop] file (formato PS)

La funzionalità è supportata con le versioni [!DNL Adobe Creative Cloud] 2018 e [!DNL Adobe Creative Cloud] 2019 dell&#39;applicazione precedente. L&#39;app utilizza un approccio euristico e di corrispondenza ottimale per mappare i percorsi desktop locali delle risorse collegate agli URL nel server [!DNL Experience Manager]. Si basa su alcuni presupposti descritti di seguito:

* I percorsi dei file inseriti nell&#39;applicazione nativa utilizzano un percorso desktop globale (inserito dalla condivisione di rete locale visualizzata con l&#39;opzione [!UICONTROL Reveal]).

* I percorsi vengono memorizzati dall’app nativa nel record XMP del file.

* [!DNL Experience Manager] ha estratto il record XMP con i percorsi del record di metadati della risorsa.

* I percorsi possono corrispondere alle risorse in [!DNL Experience Manager], ovvero i file inseriti si trovano anche in [!DNL Experience Manager] in un percorso corrispondente.

## Nuove funzioni, miglioramenti e correzioni di bug {#what-is-new}

Per ulteriori informazioni, vedere [Novità della versione v2.0](introduction.md#whats-new-v2).

**Aggiornamenti nell&#39;app v2.3.1**

* Il nuovo programma di installazione di Enterprise Windows installa l&#39;applicazione in Programmi.
* Supporto per l&#39;**autenticazione di base** durante gli accessi AEM e SSO.
* Numero configurabile di risorse consentito durante l’operazione di caricamento

**Aggiornamenti nell&#39;app v2.3.0**

* È stato aggiunto il supporto per l’accesso IMS. L’integrazione IMS consente all’app desktop di eseguire automaticamente l’aggiornamento del token di accesso, consentendo all’utente di rimanere connesso per un massimo di 14 giorni.

* Supporto migliorato per proxy aziendali e filtro web.

**Aggiornamenti nell&#39;app v2.2.2**

* (Solo Windows) L’app desktop visualizza una schermata vuota dopo l’installazione delle versioni 2.2.0 e 2.2.1.

**Aggiornamenti nell&#39;app v2.2.1**

* L&#39;app desktop visualizza un messaggio di errore di timeout della sessione quando si fa clic su **[!UICONTROL Sign In]**.

* Problemi durante l’accesso all’app desktop v2.2.0 su macOS.

* L&#39;app desktop visualizza un messaggio di errore quando si ordinano le risorse facendo clic su **[!UICONTROL Edited Locally]**.

**Aggiornamenti nell&#39;app v2.2.0**

* Supporto per Apple Silicon (M1).

* Possibilità di ricordare la stringa di connessione durante l&#39;accesso all&#39;app desktop.

**Aggiornamenti nell&#39;app v2.1.5.0**

* L’app desktop non risponde quando carichi i file in una cartella contenente caratteri cinesi (ASSETS-9237).

* l&#39;app desktop sostituisce i punti con trattini nei nomi dei file (ASSETS-10955).

**Aggiornamenti nell&#39;app v2.1.4.0**

La nuova versione dell’applicazione offre correzioni di bug.

**Aggiornamenti nell&#39;app v2.1.3.4**

La nuova versione dell&#39;applicazione offre una correzione di bug.

**Aggiornamenti nell&#39;app v2.1.3.3**

La nuova versione dell&#39;applicazione offre una correzione di bug.

**Aggiornamenti nell&#39;app v2.1.3.2**

Questa versione dell&#39;applicazione offre una correzione di bug.

**Aggiornamenti nell&#39;app v2.1.3.1**

Il bug corretto in questa versione è:

* Le velocità di caricamento e download delle risorse sono migliorate, anche con risorse di grandi dimensioni. Questa versione ha risolto un problema che causava l&#39;errore di caricamento di risorse con [!DNL desktop app] in alcuni casi in cui venivano caricati file di dimensioni molto grandi.

**Aggiornamento nell&#39;app v2.1.2.0**

* Una nuova opzione per [!UICONTROL Clear Cookies] è stata aggiunta al menu principale dell&#39;applicazione. Consente di risolvere i potenziali problemi di accesso, ad esempio quando si modifica una connessione da un server a un altro. Vedi [cancellare i cookie prima di connettersi](/help/using/troubleshoot.md#cannot-login-cookies-issue).

* È stata aggiunta una nuova opzione che, se selezionata, consente all&#39;app di caricare cartelle e file con nomi di nodo in [!DNL Adobe Experience Manager] corrispondenti ai nomi di file e cartelle locali. Questo processo garantisce la coerenza tra i nomi locali e quelli caricati.

  Questo comportamento è simile a quello predefinito nella versione 1 dell’app desktop. Nella versione corrente, invece, se l&#39;opzione non è abilitata, gli spazi vuoti e i caratteri `% ; # , + ? ^ { } "` nei nomi delle cartelle vengono sostituiti con trattini nei percorsi delle cartelle. Inoltre, nei percorsi delle cartelle i caratteri maiuscoli vengono convertiti in minuscolo. Nei nomi dei file, tuttavia, i caratteri `# % { } ? &` vengono sostituiti con un trattino, ma gli spazi vuoti e le maiuscole vengono mantenuti. Per ulteriori informazioni, consulta [Preferenze app](/help/using/install-upgrade.md#set-preferences) e [Caricare e aggiungere nuove risorse](/help/using/using.md#upload-and-add-new-assets-to-aem).

**Aggiornamento nell&#39;app v2.1.1.0**

* Un’impostazione avanzata consente all’app di emulare il comportamento dell’app v1.10 durante il caricamento delle cartelle. Nella versione 1.10, i nomi dei nodi creati nell’archivio rispettano gli spazi e le maiuscole/minuscole dei nomi delle cartelle forniti dall’utente. Nella versione 2.1, il comportamento predefinito è invariato: più spazi nei nomi delle cartelle vengono sostituiti da trattini nel nome del nodo dell’archivio e i nomi dei nodi vengono convertiti in minuscolo. Consulta [le preferenze dell&#39;app](/help/using/install-upgrade.md#set-preferences).

**Aggiornamento nell&#39;app v2.1.0.0**

* Per caricare le risorse, gli utenti possono ora trascinare i file o le cartelle sull’interfaccia dell’applicazione, direttamente da Esplora risorse o da Mac Finder. Questo processo funziona in aggiunta all’opzione di caricamento disponibile nell’applicazione. Vedi [caricare le risorse](/help/using/using.md#upload-and-add-new-assets-to-aem) <!-- CQ-4309527 -->

**Aggiornamento nell&#39;app v2.0.3**

Il bug corretto in questa versione è:

* È stato risolto il problema di accesso per gli utenti dell&#39;app su Windows che tentavano di accedere all&#39;archivio DAM in [!DNL Adobe Experience Manager] 6.5.5.0.

**Aggiornamenti nell&#39;app v2.0.2**

Le correzioni e gli aggiornamenti di bug sono:

* L’impostazione di accelerazione del caricamento è ora disponibile per migliorarne le prestazioni. Quando questa impostazione è attivata, l’app viene caricata più rapidamente utilizzando più thread di CPU locali e richiede più risorse.

* La risorsa viene caricata quando i nomi di file o i percorsi contenenti determinati caratteri GB18030 sono fissi. <!-- CQ-4283494 -->

* L’opzione Ordina per rilevanza è disponibile dopo il passaggio a un altro tipo di ordinamento nei risultati della ricerca. <!-- CQ-4286874 -->

* L’app desktop ora elenca le sottocartelle senza la necessità di un aggiornamento esplicito. <!-- CQ-4285711 -->

* (Windows) È stato risolto un raro problema di interfaccia app inutilizzabile su alcuni computer Windows. Gli utenti non possono fare clic sull’interfaccia dell’app perché appare distorta con l’area di clic degli elementi dell’interfaccia &quot;spostati&quot; lateralmente. <!-- CQ-4280785 -->

**Aggiornamenti nell&#39;app v2.0.1**

Le correzioni e gli aggiornamenti di bug sono:

* Consenti all&#39;opzione di configurare la directory `%Temp%` affinché corrisponda al percorso `%APPDATA%`. <!-- CQ-4282665 -->

* Consenti agli utenti di accedere a [!DNL Experience Manager] Author tramite autenticazione Okta SAML. <!-- CQ-4278134 -->

## Istruzioni di installazione {#installation-instructions-v2}

Per informazioni su come installare e configurare l&#39;app, vedere [Installa [!DNL Experience Manager] app desktop](install-upgrade.md).

Se aggiorni un&#39;app desktop [!DNL Experience Manager] precedente, segui le best practice per la transizione elencate in [aggiorna dalla versione precedente](install-upgrade.md#upgrade-from-previous-version).

## Note importanti sul funzionamento dell’app {#how-app-works}

È importante essere a conoscenza delle informazioni seguenti relative all’applicazione e al relativo funzionamento.

* L&#39;applicazione fornisce il controllo completo sulle operazioni che richiedono il trasferimento completo dei file binari delle risorse da e verso [!DNL Experience Manager] (**Apri**, **Modifica**, **Carica modifiche** e **Carica Assets**).

   * Se desideri utilizzare la risorsa sul desktop, devi selezionare in modo esplicito le opzioni Apri, Modifica o Scarica sul desktop singolarmente, in una cartella o tramite selezione multipla.

   * Se desideri apportare modifiche locali alle risorse caricate in [!DNL Experience Manager], devi selezionare [!UICONTROL Upload Changes], singolarmente o tramite selezione multipla.

   * L&#39;applicazione non è un &#39;client di sincronizzazione&#39; che sincronizza le risorse tra il desktop e [!DNL Experience Manager].

   * L&#39;applicazione non fornisce una condivisione di rete che mappa l&#39;archivio [!DNL Experience Manager] come struttura di cartelle virtuali.

* L’elenco delle risorse visualizzato dall’applicazione si basa sullo stato dell’archivio Assets. I file scaricati in locale e successivamente rinominati nei file locali o nella cartella della cache non vengono visualizzati o gestiti con l&#39;applicazione.

* Se l’app non mostra i risultati previsti, fai clic sull’icona di aggiornamento nella barra superiore.

* La condivisione di rete locale, visualizzata quando utilizzi un’azione [!UICONTROL Reveal File], mostra solo i file (e le cartelle) disponibili in locale. Con [!UICONTROL Reveal File] e [!UICONTROL Reveal Folder] le risorse vengono prescaricate in modo da visualizzare le risorse corrette nella condivisione di rete locale.

* Quando un’app Adobe Creative Cloud legge i file di risorse collegati o inseriti in un file nativo dell’app Creative Cloud, viene utilizzata la condivisione di rete locale SMB (Mac)/WebDAV (Windows).

Il diagramma seguente illustra il flusso di risorse e file dal cloud al file system locale e viceversa, in base alle azioni dell’utente.

![Flusso delle risorse dal server [!DNL Experience Manager] alle app desktop native tramite l&#39;app desktop](assets/da20_flow_diagram.png)

## Problemi noti {#known-issues-v2}

**Problemi relativi all’interfaccia utente:**

* A volte, l’interfaccia dell’app desktop potrebbe diventare vuota. Fare clic con il pulsante destro del mouse e scegliere [!UICONTROL Refresh] per ricaricare l&#39;applicazione. Dopo tale aggiornamento, inizi dalla directory principale dell’archivio DAM. Gli aggiornamenti o gli stati delle risorse vengono mantenuti. <!-- CQ-4270267 -->

* È difficile spostarsi tra le cartelle e i risultati della ricerca senza il riquadro di rilevamento o il puntatore del mouse. La barra di scorrimento non viene visualizzata con mouse senza rotellina. <!-- CQ-4269947 -->

* Di rado, la barra di avanzamento non viene visualizzata correttamente quando cambia la risorsa in fase di caricamento.

* Dopo che l’utente applica e rimuove il filtro per trovare tutte le risorse modificate in locale, l’app non ritorna ai risultati della ricerca originale o alla vista cartelle in cui si trovava inizialmente l’utente. L’app visualizza la cartella principale dell’archivio DAM.

* Talvolta, quando ci si connette a un URL in cui non è in esecuzione un server [!DNL Experience Manager], la schermata di connessione non risponde. Esci dall’applicazione e riavviala.

**Problemi relativi a operazioni di creazione, lettura, aggiornamento ed eliminazione:**

* Durante il caricamento di modifiche apportate a una risorsa con commenti, questi vengono memorizzati insieme alla risorsa in [!DNL Experience Manager] ma non sono visibili come commenti per il controllo delle versioni. Questo problema è stato risolto in [!DNL Experience Manager] 6.4.5 e [!DNL Experience Manager] 6.5.1. Adobe consiglia di installare i service pack più recenti. <!-- CQ-4268990 -->

* Un utente non può annullare i trasferimenti di risorse. Se hai attivato per errore un trasferimento di grandi dimensioni, esci dall’applicazione e riavviala. <!-- CQ-4278940 -->

**Problemi relativi alla piattaforma:**

* In alcuni casi, in Windows, lo stato di una risorsa può cambiare immediatamente in [!UICONTROL Edited Locally] dopo l’apertura, anche se non sono state apportate modifiche. Fai clic su [!UICONTROL Refresh] per aggiornare.

>[!MORELIKETHIS]
>
>* [[!DNL Experience Manager] as a [!DNL Cloud Service] documentazione](https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service)
>* [[!DNL Experience Manager] as a [!DNL Cloud Service] [!DNL Assets] documentazione](https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/assets/overview)
>* [Come usare [!DNL Experience Manager] l&#39;app desktop](using.md)
>* [Installare e aggiornare l’app desktop](install-upgrade.md)
>* [Best practice e suggerimenti per la risoluzione dei problemi](troubleshoot.md)
