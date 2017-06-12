---
title: "How to: Set Up and Close Income Statement Balances"
ms.custom: na
ms.date: "06-05-2016"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "income statements, setting up balances"
  - "balances, income statements"
  - "income statements, closing balances"
  - "closing, income statement balances"
ms.assetid: 8f85fba6-8afa-4bec-81b3-a4828f5434e6
caps.latest.revision: 22
ms.author: "edupont"
manager: "terryaus"
translation.priority.ht: 
  - "es-es"
---
# How to: Set Up and Close Income Statement Balances
You can use income statement balancing accounts to balance and track several accounts at the same time. The **Close Income Statement** batch job transfers income statement accounts to an account in the balance sheet, and closes the income statement accounts. When the **Close Income Statement** batch job is run, the entries are automatically posted.  
  
> [!NOTE]  
>  The fiscal year must be closed before the batch job can run.  
  
### To set up the income statement balance account  
  
1.  In the **Search** box, enter **Chart of Accounts**, and then choose the related link.  
  
2.  Select an existing general ledger account. On the **Home** tab, choose **Edit** to open the **G\/L Account Card** window.  
  
3.  Expand the **General** FastTab.  
  
4.  In the **Income Stmt. Bal. Acc.** field, select the adjustment account for the auxiliary commercial account.  
  
    > [!NOTE]  
    >  During adjustment, balances will be expensed or credited to this account.  
  
5.  Enter information into the required fields, and then choose the **OK** button.  
  
### To close income statement balances  
  
1.  In the **Search** box, enter **Close Income Statement**, and then choose the related link.  
  
2.  In the **Options** FastTab, fill in the fields as described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**Fiscal Year Ending Date**|Select the date of the closed fiscal year.|  
    |**Gen. Journal Template**|Select the required general journal template.|  
    |**Gen. Journal Batch**|Select the required general journal batch.|  
    |**Document No.**|Enter the document number.|  
    |**Retained Earnings Acc.**|Select the account for the retained earnings entries.|  
    |**Posting Description**|Enter the required description.|  
  
3.  In the **Close by** section, fill in the fields as described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**Business Unit Code**|Select to create an entry for each business code.|  
    |**Dimensions**|Select to create an entry for each general ledger dimension.|  
    |**Inventory Period Closed**|Select to indicate that the inventory period with ending dates equal to or greater than the last date of the accounting period is closed.|  
  
4.  Choose the **OK** button.  
  
## See Also  
 [Spain Local Functionality](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Spain/spain-local-functionality.md)