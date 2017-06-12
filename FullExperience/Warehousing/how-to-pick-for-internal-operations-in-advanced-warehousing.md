---
title: "How to: Pick for Internal Operations in Advanced Warehousing"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "assembly, picking"
  - "picking, assembly"
ms.assetid: 742fb367-3178-4bdb-abb0-a33331b4a0c3
caps.latest.revision: 13
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
# How to: Pick for Internal Operations in Advanced Warehousing
In advanced warehousing where the location is set up to use picking as well as shipping, you can pick components for production and assembly activities with the **Warehouse Pick** window.  
  
 Alternatively, you can use the **Movement Worksheet** window to move items between bins ad hoc, meaning without reference to a source document. For more information, see [How to: Move Items in Advanced Warehousing](../WarehouseActivities/how-to-move-items-in-advanced-warehousing.md).  
  
 For information about picking items for internal operations in basic warehouse locations that are set up for picking only, see [How to: Move Components to an Operation Area in Basic Warehousing](../WarehouseActivities/how-to-move-components-to-an-operation-area-in-basic-warehousing.md). For information about picking and posting consumption of production components in basic warehousing, see [How to: Pick for Production in Basic Warehousing](../WarehouseActivities/how-to-pick-for-production-in-basic-warehousing.md).  
  
 You cannot create a warehouse pick document from scratch because a pick activity is always part of a workflow, either in a pull or a push scenario.  
  
 You can create the warehouse pick document in a push fashion by selecting **Create Whse. Pick** on the source document, such as a released assembly order or warehouse shipment. For more information, see [Whse.\-Source \- Create Document](../Topic/\($%20R_7305%20Whse.-Source%20-%20Create%20Document%20$\).md) and [How to: Pick Items for Warehouse Shipment](../WarehouseActivities/how-to-pick-items-for-warehouse-shipment.md).  
  
 Alternatively, you can create the warehouse pick document in a pull fashion by using the **Pick Worksheet** window to detect pick requests, both for shipment and internal operations, and then create the required warehouse pick documents.  
  
 The following procedure explains a pull scenario where you pick components for a released production order through the **Pick Worksheet** window. The procedure also applies for an assembly order.  
  
 To create pick requests, both for pull and for push scenarios, the source documents in question must be released. Release source documents for internal operations in the following ways.  
  
|Source document|Release method|  
|---------------------|--------------------|  
|Production Order|Change order type to released production order. For more information, see [How to: Release Production Orders by Status Change](../OperationsPlanning/how-to-release-production-orders-by-status-change.md).|  
|Assembly Order|Change status to Released. For more information, see [Assembly Order](../WarehouseActivities/-$-n_900-assembly-order-$-.md).|  
|||  
  
### To pick components using the pick worksheet  
  
1.  In the **Search** box, enter **Pick Worksheet**, and then choose the related link.  
  
2.  On the **Home** tab, in the **Process** group, choose **Get Warehouse Documents**, and then select the component lines from the released production order.  
  
3.  Inspect the lines, sort them to ensure an efficient picking round, and combine them with other worksheet lines if necessary to make best use of employee time.  
  
4.  On the **Actions** tab, in the **Functions** group, choose **Create Pick**.  
  
5.  Define how to create the warehouse pick documents and how to sort pick lines by filling fields in the **Create Pick** window.  
  
6.  Choose the **OK** button. Warehouse pick documents are created with pick lines for each component that is required in the internal operation. For more information, see [Warehouse Pick](../Topic/\($%20N_5779%20Warehouse%20Pick%20$\).md).  
  
 If the internal operation area, such as a production shop floor, is set up with a default bin for placement of components to be used in the operation, then that bin code is inserted in the Place lines on the warehouse pick document to instruct warehouse workers where to place the items. For more information, see the [To\-Production Bin Code](../Topic/\($%20T_14_7314%20To-Production%20Bin%20Code%20$\).md) or the [To\-Assembly Bin Code](../Topic/\($%20T_14_7330%20To-Assembly%20Bin%20Code%20$\).md) field.  
  
## See Also  
 [Pick Worksheet](../Topic/\($%20N_7345%20Pick%20Worksheet%20$\).md)   
 [Warehouse Pick](../Topic/\($%20N_5779%20Warehouse%20Pick%20$\).md)   
 [How to: Plan Picks in Worksheets](../WarehouseActivities/how-to-plan-picks-in-worksheets.md)   
 [How to: Pick Items for Warehouse Shipment](../WarehouseActivities/how-to-pick-items-for-warehouse-shipment.md)   
 [Movement Worksheet](../Topic/\($%20N_7351%20Movement%20Worksheet%20$\).md)   
 [Create Pick](../Topic/\($%20B_5754%20Create%20Pick%20$\).md)   
 [To\-Production Bin Code](../Topic/\($%20T_14_7314%20To-Production%20Bin%20Code%20$\).md)   
 [How to: Pick for Production in Basic Warehousing](../WarehouseActivities/how-to-pick-for-production-in-basic-warehousing.md)   
 [How to: Move Components to an Operation Area in Basic Warehousing](../WarehouseActivities/how-to-move-components-to-an-operation-area-in-basic-warehousing.md)   
 [How to: Move Items in Advanced Warehousing](../WarehouseActivities/how-to-move-items-in-advanced-warehousing.md)