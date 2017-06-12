---
title: "How to: Block Inventory Items for Sales or Purchases"
ms.custom: na
ms.date: "06-05-2016"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "blocking, inventory items"
  - "inventory management, blocking items"
ms.assetid: bfe853e2-7aba-4c60-bfc6-8ef283ed5c81
caps.latest.revision: 2
ms.author: "edupont"
translation.priority.ht: 
  - "de-ch"
  - "fr-ch"
---
# How to: Block Inventory Items for Sales or Purchases
In [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)], an item can be marked as blocked for sales, blocked for purchase, or blocked for all purposes.  
  
 The following table illustrates what occurs when items are blocked.  
  
|Item marked as|Result|  
|--------------------|------------|  
|**Sale blocked**|You cannot use the item in a sales document or in a sales item journal.|  
|**Purchase blocked**|You cannot use the item in a purchase document, in a purchase item journal, or in purchase planning processes.|  
|**Blocked**|You cannot use the item for any item transaction. For more information about blocking an item for all purposes, see [Item Card](../Topic/\($%20N_30%20Item%20Card%20$\).md).|  
  
### To block inventory items for sales  
  
1.  In the **Search** box, enter **Items**, and then choose the related link.  
  
2.  Select the item that you want to block. On the **Home** tab, in the **Manage** group, choose **Edit**.  
  
3.  To block the selected item for sales transactions, on the **Invoicing** FastTab, select the **Sale blocked** check box.  
  
4.  Choose the **OK** button.  
  
### To block inventory items for purchase  
  
1.  In the **Search** box, enter **Items**, and then choose the related link.  
  
2.  Select the item that you want to block. On the **Home** tab, in the **Manage** group, choose **Edit**.  
  
3.  To block an item for purchase transactions, on the **Replenishment** FastTab, select the **Purchase blocked** check box.  
  
4.  Choose the **OK** button.  
  
 You will receive an error message if you try to do the following:  
  
-   Enter sales lines and purchase lines in sales documents and purchase documents for blocked items. For more information, see the [Sales Line](../Topic/\($%20T_37%20Sales%20Line%20$\).md) table and the [Purchase Line](../Topic/\($%20T_39%20Purchase%20Line%20$\).md) table.  
  
-   Create new lines in an item journal for blocked items. For more information, see the [Item Journal](../../WarehouseActivities/-$-n_40-item-journal-$-.md) window.  
  
-   Post item transactions for blocked items.  
  
## See Also  
 [Item](../Topic/\($%20T_27%20Item%20$\).md)   
 [Sales Line](../Topic/\($%20T_37%20Sales%20Line%20$\).md)   
 [Purchase Line](../Topic/\($%20T_39%20Purchase%20Line%20$\).md)   
 [Item Journal](../../WarehouseActivities/-$-n_40-item-journal-$-.md)   
 [Item Journal Line](../Topic/\($%20T_83%20Item%20Journal%20Line%20$\).md)   
 [Swiss Inventory Management](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Switzerland/swiss-inventory-management.md)   
 [How to: Block Shipment for Negative Inventory](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Austria/how-to-block-shipment-for-negative-inventory.md)   
 [How to: Copy Existing Items to New Items](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Austria/how-to-copy-existing-items-to-new-items.md)   
 [How to: Deactivate Item Cost Tracking](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Switzerland/how-to-deactivate-item-cost-tracking.md)