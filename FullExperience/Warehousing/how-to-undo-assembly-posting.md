---
title: "How to: Undo Assembly Posting"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "assembly, undoing"
  - "undoing, assembly"
ms.assetid: 73d1ea4c-d4e9-499c-99cb-52a004c5ed3e
caps.latest.revision: 11
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
  - "en-nz"
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
# How to: Undo Assembly Posting
Sometimes you may need to undo a posted assembly order, for example when the order was posted with mistakes that must be corrected, or because it should not have been posted in the first place and must be rolled back. To reverse an order posting, open the posted assembly order, and on the **Actions** tab, in the **General** group, choose **Undo Assembly**.  
  
 When you undo a posted assembly order, a set of corrective item ledger entries is created to reverse the original entries. Each positive output entry for the assembly item is reversed by a negative output entry. Each negative consumption entry for an assembly component is reversed by a positive consumption entry. Fixed cost application is automatically created between the corrective and original entries to ensure exact cost reversal.  
  
 When you undo a fully posted assembly order, then you can choose to recreate the assembly order to its original state, for example to make corrections before reposting it. Alternatively, you can choose to not recreate the assembly order.  
  
 When you undo a partially posted assembly order, then all affected quantity fields, such as the **Assembled Quantity**, **Consumed Quantity**, and **Remaining Quantity** fields are restored to the values they had before the posting in question.  
  
 To recreate or restore assembly orders, the following conditions must apply to the assembly item that was output in the original posting:  
  
-   It must still be in inventory, that is, it is not sold or otherwise consumed by outbound transactions.  
  
-   It must not be reserved.  
  
-   It must exist in the bin that it was output to.  
  
 In addition, existing assembly orders can only be restored if the number of lines and the sequence of lines on the original assembly order are not changed.  
  
> [!TIP]  
>  To solve conflicts due to line changes, you can manually revert the changes on the lines in question before undoing the related posted assembly order. Alternatively, you can post the assembly order fully and then select to recreate it when undoing the posting.  
  
 The following procedure describes how to undo posted assembly orders where the items were assembled to stock. If you want to undo posted assembly orders where the items were assembled to a sales order, then you must use the **Undo Shipment** function on the posted shipment that relates to the posted assembly order. For more information, see [How to: Undo Quantity Postings on Posted Shipments](../Sales/how-to-undo-quantity-postings-on-posted-shipments.md). The undoing of the posted assembly order then happens automatically in the same way as described in this topic.  
  
### To undo posting of an assembly order  
  
1.  To undo a fully or partially posted assembly order, in the **Search** box, enter **Posted Assembly Orders**, and choose the related link.  
  
     The **Posted Assembly Orders** window opens showing one or more posted assembly orders that are posted from the assembly order in question. Each partial posting creates a separate posted assembly order.  
  
2.  Open the posted assembly order that you want to undo, and then on the **Actions** tab, in the **General** group, choose **Undo Assembly**.  
  
     If the posted assembly order that you want to undo relates to a fully posted assembly order that is now deleted, then you have the option to recreate it, typically because you want to reprocess it.  
  
3.  If you want to recreate the assembly order, choose the **Yes** button. To undo the posting without recreating the related assembly order, choose the **No** button.  
  
 The **Reversed** field on the assembly order header changes to **Yes**. The assembly order posting is now reversed, and you can proceed to process the entire assembly order if you chose to recreate it or the open assembly order that you have restored to its original state.  
  
> [!NOTE]  
>  To restore quantities from multiple partial postings in an assembly order, you must undo all the posted assembly orders in question by following steps 1 through 3 above for each posted assembly order.  
  
## See Also  
 [Posted Assembly Order](../Topic/\($%20N_920%20Posted%20Assembly%20Order%20$\).md)   
 [Assembly Order](../WarehouseActivities/-$-n_900-assembly-order-$-.md)   
 [Reversed](../Topic/\($%20T_910_100%20Reversed%20$\).md)   
 [Item Rcpt. Entry No.](../Topic/\($%20T_910_39%20Item%20Rcpt.%20Entry%20No.%20$\).md)   
 [Item Shpt. Entry No.](../Topic/\($%20T_911_39%20Item%20Shpt.%20Entry%20No.%20$\).md)   
 [How to: Assign Exact Cost Reversing in Sales](../Finance/how-to-assign-exact-cost-reversing-in-sales.md)   
 [Assembled Quantity](../Topic/\($%20T_900_44%20Assembled%20Quantity%20$\).md)   
 [Consumed Quantity](../Topic/\($%20T_901_44%20Consumed%20Quantity%20$\).md)   
 [Remaining Quantity](../Topic/\($%20T_900_42%20Remaining%20Quantity%20$\).md)   
 [How to: Undo Quantity Postings on Posted Shipments](../Sales/how-to-undo-quantity-postings-on-posted-shipments.md)   
 [Assemble to Order or Assemble to Stock](../DesignAndEngineering/assemble-to-order-or-assemble-to-stock.md)   
 [How to: Assemble Items](../WarehouseActivities/how-to-assemble-items.md)   
 [How to: Sell Items Assembled to Order](../Sales/how-to-sell-items-assembled-to-order.md)