---
title: "Consolidate Companies"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "combining, companies"
  - "consolidating, companies"
  - "companies, consolidating"
ms.assetid: fdfc319b-ef2b-478a-ab14-59600a3567d6
caps.latest.revision: 4
ms.author: "sgroespe"
manager: "terryaus"
translation.priority.ht: 
  - "da-dk"
  - "de-at"
  - "de-ch"
  - "de-de"
  - "en-au"
  - "en-ca"
  - "en-gb"
  - "en-in"
  - "en-my"
  - "en-nz"
  - "en-ph"
  - "en-sg"
  - "en-zw"
  - "es-es"
  - "es-mx"
  - "fi-fi"
  - "fr-be"
  - "fr-ca"
  - "fr-ch"
  - "fr-fr"
  - "is-is"
  - "it-ch"
  - "it-it"
  - "nb-no"
  - "nl-be"
  - "nl-nl"
  - "ru-ru"
  - "sv-se"
---
# Consolidate Companies
You can consolidate the general ledger entries of two or more separate companies \(subsidiaries\) into a consolidated company. Each individual company involved in a consolidation is called a business unit. The combined company is called the consolidated company.  
  
 You can import data into the consolidated company from other companies in the same database, from other [!INCLUDE[navnow](../ApplicationDesign/includes/navnow_md.md)] databases, or from files.  
  
 If the financial statements of a business unit are in a different currency than those of the consolidated company, you must set up exchange rates for consolidation. There are three different exchange rates for consolidation: Average Rate \(Manual\), Closing Rate and Last Closing Rate. For each general ledger account that is consolidated from the business unit, the content of the **Consol. Translation Method** field determines which exchange rate is used.  
  
 On each business unit card, you specify in the Currency Exchange Rate field whether the consolidation should use exchange rates from the business unit company or the consolidated company. If you use exchange rates from the consolidated company, you can change the exchange rates for a business unit.  
  
 Before you import data into the consolidated company, you can test that the setup of the companies is compatible. Then you can import the data.  
  
 The following table describes a sequence of tasks, with links to the topics that describe them. These tasks are listed in the order in which they are generally performed.  
  
|**To**|**See**|  
|------------|-------------|  
|Learn what you can accomplish with the consolidation features in Product Name.|[About Consolidations](../Finance/about-consolidations.md)|  
|Get an overview of how to perform a consolidation, from setup through finalization of the consolidation process.|[How to: Process Consolidations](../Finance/how-to-process-consolidations.md)|  
|Update exchange rates for a business unit that has financial statements in a foreign currency.|[How to: Specify Exchange Rates for Consolidations](../Finance/how-to-specify-exchange-rates-for-consolidations.md)|  
|Export data from a company in a different Product Name database.|[How to: Export Business Unit Information](../Finance/how-to-export-business-unit-information.md)|  
|Check whether there are differences between the setup of the consolidated company and the setup of the business units in a different Product Name database.|[How to: Test Databases Before Consolidating](../Finance/how-to-test-databases-before-consolidating.md)|  
|Check whether there are differences between the setup of the consolidated company and the setup of the business units in a file.|[How to: Test Files Before Consolidating](../Finance/how-to-test-files-before-consolidating.md)|  
|Import consolidations data from business units in the same database.|[How to: Consolidate from Databases](../Finance/how-to-consolidate-from-databases.md)|  
|Import consolidations data from a file.|[How to: Consolidate from Files](../Finance/how-to-consolidate-from-files.md)|  
  
## See Also  
 [Consol. Translation Method](assetId:///743e3a71-e883-4163-9f45-1dc3a4cbe27b)   
 [Set Up Consolidations](../Finance/set-up-consolidations.md)