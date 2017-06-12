---
title: "Walkthrough: Setting Up and Invoicing Sales Prepayments"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "finance, invoicing prepayments"
  - "prepayments, applying to an order"
  - "finance, setting up prepayments"
  - "prepayments, setting up"
  - "prepayments, correcting orders"
  - "invoicing prepayments"
  - "prepayments, creating an invoice"
  - "business process walkthroughs, setting up and invoicing prepayments"
  - "prepayments, invoicing"
  - "correcting, prepayments"
ms.assetid: 29cdb024-6a59-4225-a0b1-c8c2fab0900a
caps.latest.revision: 21
ms.author: "sgroespe"
manager: "terryaus"
translation.priority.ht: 
  - "da-dk"
  - "de-de"
  - "es-es"
  - "fi-fi"
  - "fr-fr"
  - "it-it"
  - "nb-no"
  - "nl-nl"
  - "sv-se"
---
# Walkthrough: Setting Up and Invoicing Sales Prepayments
Prepayments are payments that are invoiced and posted to a sales or purchase prepayment order before final invoicing. You may require a deposit before you manufacture items to order, or you may require payment before you ship items to a customer. You use the prepayments functionality in [!INCLUDE[navnow](../ApplicationDesign/includes/navnow_md.md)] to invoice and collect deposits that are required from customers or remit deposits to vendors. Thus, you can make sure that all payments are posted against an invoice.  
  
 Prepayment requirements can be defined for a customer or vendor for all items or selected items. After you complete the required setup, you can generate prepayment invoices from sales and purchase orders for the calculated prepayment amount. You can change the default amounts on the invoice as needed. For example, you can send additional prepayment invoices if additional items are added to the order.  
  
## About This Walkthrough  
 This walkthrough will take you through the following scenarios:  
  
-   Setting up prepayments.  
  
-   Creating an order that requires a prepayment.  
  
-   Creating a prepayment invoice.  
  
-   Correcting the prepayment requirements on an order.  
  
-   Applying prepayments to an order.  
  
-   Invoicing the final amount on an order with prepayment.  
  
### Roles  
 This walkthrough includes tasks for the following roles:  
  
-   Accounting Manager \(Phyllis\)  
  
-   Order Processor \(Susan\)  
  
-   Accounts Receivable Administrator \(Arnie\)  
  
## Story  
 Phyllis is an accounting manager. She makes decisions about which customers are required to pay a deposit before items are manufactured or shipped. Phyllis sets up [!INCLUDE[navnow](../ApplicationDesign/includes/navnow_md.md)] to calculate prepayments automatically.  
  
 Susan is a sales order processor. When a customer calls to place an order, she enters the order into the system while the customer is on the telephone. This way, she can verify prices and payment terms with the customer immediately, and she can make adjustments to the order while she negotiates with the customer.  
  
 Arnie works in the Accounts Receivable department, where he posts invoices and payments.  
  
 In this scenario, Phyllis sets up prepayment requirements for the customer Selangorian, based on their credit history, and gives Susan instructions for how to handle their orders.  
  
 When the customer calls, Susan negotiates with the customer until they reach an agreement. She can then choose to calculate the prepayment in several different ways.  
  
 After Susan sends the prepayment invoice, the customer orders an extra item. Susan updates the order and creates a second prepayment invoice.  
  
 Arnie registers the customer's payment and applies it to the invoices, and then sends the final invoice.  
  
## Setting Up Prepayments  
 Phyllis sets up the system to handle prepayments for customers.  
  
-   Phyllis decides to have the same number series for prepayments as the one used for sales invoicing.  
  
-   Phyllis sets the program to check if prepayments are required before final invoicing on an order.  
  
-   Phyllis sets up default values for a required prepayment percentage for particular items and customers.  
  
 The following procedures describe how to complete Phyllis' tasks:  
  
#### To set up number series for prepayments  
  
1.  In the **Search** box, enter **Sales & Receivables Setup**, and then choose the related link.  
  
2.  In the **Sales & Receivables Setup** window, expand the **Numbering** FastTab.  
  
3.  Verify that the number series for posted prepayment invoices in the **Posted Prepmt. Inv. Nos.** field is the same as for posted sales invoices \(**Posted Invoice Nos.**\) and the number series for posted prepayment credit memos \(**Posted Prepmt. Cr. Memo Nos.**\) is the same as for posted credit memos \(**Posted Credit Memo Nos.**\).  
  
#### To block shipments for unpaid prepayment  
  
1.  In the **Sales & Receivables Setup** window, on the **General** FastTab, select the **Check Prepayment when Posting** field.  
  
     When the **Check Prepayment when Posting** field is selected, you cannot ship or invoice an order that has an unpaid prepayment amount.  
  
2.  Close the **Sales & Receivables Setup** window.  
  
 By default, Phyllis requires customer 20000 to be invoiced for a 30% down payment on all orders. Therefore, she will enter a default prepayment percentage on the customer card.  
  
 Phyllis requires all customers to be invoiced a 20% deposit for item 1100. Customer 20000 has a poor payment history. Therefore, she requires a 40% prepayment from customer 20000 for item 1100. The following procedure illustrates how to set up default prepayment percentages.  
  
#### To assign default prepayment percentages to customers and items  
  
1.  In the **Search** box, enter **Customers**, and then choose the related link.  
  
2.  Select the line with customer 20000 \(Selangorian\), and then, on the **Home** tab, in the **Manage** group, choose **Edit**.  
  
3.  On the customer card for customer 20000, expand the **Invoicing** FastTab.  
  
4.  In the **Prepayment %** field, type **30**.  
  
5.  Choose the **OK** button to close the customer card.  
  
6.  In the **Search** box, enter **Items**, and then choose the related link.  
  
7.  Select the line with item 1100, and then, on the **Home** tab, in the **Manage** group, choose **Edit**.  
  
8.  On the item card, on the **Navigate** tab, in the **Sales** group, choose **Prepayment Percentages**.  
  
9. Fill in two lines in the **Sales Prepayment Percentages** window as follows.  
  
    |**Sales Type**|**Sales Code**|**Item No.**|**Prepayment %**|  
    |--------------------|--------------------|------------------|----------------------|  
    |**Customer**|**20000**|**1100**|**40**|  
    |**All Customers**||**1100**|**20**|  
  
    > [!IMPORTANT]  
    >  Depending on your country\/region, you must also specify a tax group code on the **Invoicing** FastTab for items 1000 and 1100.  
  
10. Close all windows.  
  
#### To specify an account for sales prepayments in general posting setup  
  
1.  In the **Search** box, enter **General Posting Setup**, and then choose the related link.  
  
2.  Select the line where the **Gen. Bus. Posting Group** field is set to **EXPORT**, and the **Gen. Prod. Posting Group** field is set to **RETAIL**, and then, on the **Home** tab, in the **Manage** group, choose **Edit**.  
  
3.  In the **General Posting Setup Card** window, on the **Sales** FastTab, in the **Sales Prepayments Account** field, specify the relevant account.  
  
4.  Choose the **OK** button.  
  
## Creating an Order that Requires a Prepayment  
 In the following scenario, Susan, the order processor, creates an order when talking to a customer. The items that the customer orders require a prepayment, and the customer has made some late payments in the past. Therefore, Susan has been instructed to require a fixed amount of 2,000 as a prepayment on the order.  
  
 The customer requests to be able to pay 35%, to which Susan can agree. Therefore, she changes the order.  
  
 Susan creates the prepayment invoice and sends it to the customer.  
  
#### To create a sales order with a prepayment  
  
1.  In the **Search** box, enter **Sales Orders**, and then choose the related link.  
  
2.  On the **Home** tab, choose **New**.  
  
3.  On the new sales order, press Enter and an order number is automatically assigned to the order.  
  
4.  In the **Sell\-to Customer No.** field, select **20000**.  
  
5.  Accept the overdue balance warning that is displayed.  
  
     When you press Enter in the **Sell\-to Customer No.** field, most fields on the sales order are filled in automatically.  
  
6.  Fill in two sales lines with the following information.  
  
    |**Type**|**No.**|**Quantity**|  
    |--------------|-------------|------------------|  
    |**Item**|**1000**|**1**|  
    |**Item**|**1100**|**1**|  
  
     By default, the prepayment fields on the sales line are hidden, so you must display them.  
  
7.  On **Lines** FastTab, on the toolbar, choose **Actions**![Actions](../GettingStarted/media/actionsicon.png "ActionsIcon"), and then choose **Choose Columns**.  
  
8.  Add the following fields: **Prepayment %**, **Prepayment Line Amount Excl. VAT**, and **Prepmt. Amt. Inv. Excl. VAT**.  
  
9. Choose the **OK** button.  
  
     The **Sales Order** window updates.  
  
10. Verify that the **Prepayment %** field on the line with item **1000** contains **30**. The default value was taken from the sales header, which was populated from the customer card.  
  
     The **Prepayment %** field on the line with item **1100** contains **40**. This is the percentage you entered in the **Sales Prepayment Percentages** window for item **1100** and customer **20000**.  
  
     For more information, see [How to: Define Prepayment Percentages](../Purchasing/how-to-define-prepayment-percentages.md).  
  
11. On the **Navigate** tab, in the **Order** group, choose **Statistics**.  
  
12. On the **Prepayment** FastTab, the **Prepmt. Line Amount Excl. VAT** field contains **1,560**. If you create a prepayment invoice for the order now, then this is the amount that is displayed on the invoice.  
  
     In this scenario, Susan has been instructed to suggest a total prepayment of 2000 for the order.  
  
    > [!IMPORTANT]  
    >  Depending on your country\/region, the following step might not apply.  
  
13. Change the amount in the **Prepmt. Line Amount Excl. VAT** field to **2000** and then close the window.  
  
14. Verify the **Prepayment %** field on the sales lines, and you will see that it has been recalculated to **40.81625**.  
  
     The recalculation includes all lines that have a prepayment percentage that is greater than 0.  
  
     Now the customer asks if the prepayment percent can be set to 35%. Susan's supervisor approves the change.  
  
15. In the **Sales Order** window, expand the **Prepayment** FastTab.  
  
16. In the **Prepayment %** field, enter **35**.  
  
17. In the warning that appears, choose the **Yes** button. A rate of 35% will be applied as the payment percentage for the whole order.  
  
18. Verify that the lines have been updated accordingly.  
  
## Creating a Prepayment Invoice  
 After entering the correct prepayment values on the order, Susan creates the prepayment invoice and sends it to the customer.  
  
#### To create a prepayment invoice  
  
1.  In the sales order, on the **Actions** tab, in the **Posting** group, choose **Prepayment**, and then choose **Post Prepayment Invoice**.  
  
> [!NOTE]  
>  Susan would select **Post and Print Prepmt. Invoice** and mail the invoice to the customer.  
  
## Creating an Additional Prepayment Invoice  
 The following day, the customer calls Susan and makes changes to the order. The customer wants two of item 1100. Susan reopens and updates the order, and then she creates a second prepayment invoice on the order and sends it to the customer.  
  
#### To create an additional prepayment invoice  
  
1.  On the sales order, on the **Actions** tab, in the **Release** group, choose **Reopen**.  
  
2.  On the line for item **1100**, in the **Quantity** field, enter **2**.  
  
     Scroll to see the prepayment fields. The **Prepayment Line Amount Excl. VAT** field now contains **630**, and the **Prepmt. Amt. Inv. Excl. VAT** field contains **315**. This shows that there is an additional prepayment amount that has not been invoiced yet.  
  
3.  To post an invoice for the additional prepayment amount, on the **Actions** tab, in the **Posting** group, choose **Prepayment**, and then choose **Post Prepayment Invoice**.  
  
## Applying the Prepayments  
 The customer pays the prepayments amount and Arnie, who works in the accounts department, registers the payment and applies it to the prepayment invoices.  
  
#### To apply a payment to the prepayment invoices  
  
1.  In the **Search** box, enter **Cash Receipt Journals**, and then choose the related link.  
  
2.  Fill in a journal line with the following information.  
  
    |Field name|Enter|  
    |----------------|-----------|  
    |**Document Type**|**Payment**|  
    |**Account Type**|**Customer**|  
    |**Account No.**|**20000**|  
  
3.  On the **Home** tab, in the **Process** group, choose **Apply Entries**.  
  
4.  In the **Apply Customer Entries** window, select the first prepayment invoice, and then, on the **Home** tab, in the **Process** group, choose **Set Applies\-to ID**.  
  
5.  Repeat the previous step for the second prepayment.  
  
6.  Choose the **OK** button.  
  
     The amount field has now been filled in with the sum of the two prepayment invoices.  
  
7.  Post the journal.  
  
## Invoicing the Remaining Amount  
 Now Arnie has been informed that the items on the order have been shipped and that the order is ready for invoicing. Arnie creates the invoice for the order.  
  
#### To invoice the remaining amount  
  
1.  Open the sales order.  
  
2.  On the **Home** tab, in the **Process** group, choose **Post**. In the window that opens, choose **Ship and Invoice**, and then choose the **OK** button.  
  
> [!NOTE]  
>  Normally, the shipping department would have already posted the shipment.  
  
 Arnie can view the history to verify that the sales invoice was created as intended.  
  
-   In the **Search** box, enter **Posted Sales Invoices**, and then choose the related link.  
  
## Next Steps  
 This walkthrough has taken you through steps to set up [!INCLUDE[navnow](../ApplicationDesign/includes/navnow_md.md)] to handle prepayments. You have set up default prepayment percentages on customers and items, and you have also used different methods to calculate the prepayments on an order. You have tried to assign one total prepayment amount to the order, and you have had the prepayment amount calculated as a percentage of the whole order.  
  
 You have also posted a prepayment invoice, created a second prepayment invoice when the order has changed, and posted the final invoice for the remaining amount.  
  
 The prepayments functionality in [!INCLUDE[navnow](../ApplicationDesign/includes/navnow_md.md)] makes it easy to set up and enforce prepayment rules for customers and items, and it enables you to post every payment against an invoice.  
  
## See Also  
 [Business Process Walkthroughs](../GettingStarted/business-process-walkthroughs.md)