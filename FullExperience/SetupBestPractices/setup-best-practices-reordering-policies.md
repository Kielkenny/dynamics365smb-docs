---
title: "Setup Best Practices: Reordering Policies"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "best practices, reordering policy setup"
  - "setup (best practices), reordering policies"
ms.assetid: eeced56e-5845-48bc-be55-5bbdc2aef59c
caps.latest.revision: 16
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
# Setup Best Practices: Reordering Policies
The **Reordering Policy** field on item cards offers four different planning methods that determine how the individual planning parameters interact.  
  
 One best\-practice foundation for selecting a reordering policy is the item’s ABC classification. For more information, see [ABC Classification](../Topic/ABC%20Classification.md).  
  
 The following table provides best practices for selecting between the four policies.  
  
|Setup option|Best practice|Comment|  
|------------------|-------------------|-------------|  
|**Order**|Use for A items.<br /><br /> Use for make\-to\-order items.<br /><br /> In manufacturing, use for top\-level items and for expensive components and subassemblies.<br /><br /> Use for items that are purchased as drop shipments and special orders.<br /><br /> Do not use if you do not accept automatic reservation.|A items, such as leather couches in a furniture store, are high\-value items with low and irregular order velocity where inventory is unacceptable, or the required attributes vary. The best reordering policy is therefore one that plans specifically for each demand.|  
|**Lot\-for\-Lot**|Use for B items.<br /><br /> In manufacturing, use for components that occur in multiple BOMs. This ensures that purchase orders are combined for the same vendor, so better prices can be negotiated.<br /><br /> Use if you are not sure about which reordering policy to select.|B items, such as dining chairs, have a regular and fairly high order velocity, but also high carrying costs. The best reordering policy for B items is therefore one that is economical by bundling demand in the reorder cycle.<br /><br /> 80 percent of items can use this policy.<br /><br /> Can be used successfully without planning parameters.|  
|**Fixed Reorder Qty.**|Use for C items.<br /><br /> Combine with reorder\-point parameters.<br /><br /> In manufacturing, use for lowest\-level components.<br /><br /> Do not use if the item is often reserved.|C items, such as tea cups, are low\-value items with high and regular order velocity. The best reordering policy for C items is therefore one that guarantees constant availability by always staying above a reorder point.<br /><br /> If the user reserves a quantity for some distant demand, then the planning foundation will be disturbed. Even if the projected inventory level is acceptable with regard to the reorder point, the quantities may not be available because of the reservation.|  
|**Maximum Qty.**|Use for C items with high carrying costs or storing limitations.<br /><br /> Combine with one or more order modifiers \(Minimum\/Maximum Order Quantity or Order Multiple\).|C items, such as tea cups, are low\-value items with high and regular order velocity. The best reordering policy for C items is therefore one that guarantees constant availability by always staying above a reorder point, but below a maximum inventory quantity.<br /><br /> To modify the suggested order, you may want the order quantity to be decreased to a specified maximum order quantity, increased to a specified minimum order quantity, or rounded up to meet a specified order multiple. **Note:**  If used with a reorder point, then inventory stays between the reorder point and the maximum quantity.|  
  
## See Also  
 [Setup Best Practices: Supply Planning](../SetupAndAdministration/setup-best-practices-supply-planning.md)   
 [Reordering Policy](../DesignAndEngineering/-$-t_27_5440-reordering-policy-$-.md)   
 [Design Details: Reordering Policies](../ApplicationDesign/design-details-reordering-policies.md)   
 [Design Details: Order](../ApplicationDesign/design-details-order.md)   
 [Design Details: Lot\-for\-Lot](../ApplicationDesign/design-details-lot-for-lot.md)   
 [Design Details: Fixed Reorder Qty.](../ApplicationDesign/design-details-fixed-reorder-qty..md)   
 [Design Details: Maximum Qty.](../ApplicationDesign/design-details-maximum-qty..md)   
 [Set Up a Company With RapidStart Services for Microsoft Dynamics NAV](../SetupAndAdministration/set-up-a-company-with-rapidstart-services-for-microsoft-dynamics-nav.md)