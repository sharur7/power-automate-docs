---
title: Relate or unrelate rows in Dataverse | Microsoft Docs
description: Learn how to add relationships and remove relationships among rows in Microsoft Dataverse with flows.  
services: ''
suite: flow
documentationcenter: na
author: MSFTMAN
manager: KVIVEK
ms.author: Deonhe
editor: ''
tags: ''
ms.service: power-automate
ms.devlang: na
ms.topic: article
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 03/06/2021
search.app: 
  - Flow
  - Powerplatform
search.audienceType: 
  - maker
---

# Relate or unrelate rows in Dataverse

>[!IMPORTANT]
>You can associate two Dataverse rows only if they have a one-to-many or many-to-many relationship.

## Relate rows

Follow these steps to associate two rows while editing your flow.

1. Select **New step** to add an action to your flow.
1. Enter **relate rows** into the **Search connectors and actions** search box on the **Choose an operation** card.
1. Select **Microsoft Dataverse**.
1. Select **Relate rows** action.

   ![Relate rows image](../media/relate-rows/relate-rows-action.png)

   Like other actions in this connector, a list of supported tables is available.
   
1. Select the table to which you want to relate, or enter a custom value for the table name.  

   ![Table name](../media/relate-rows/table-name.png)

1. You will need to enter the identifier of the row you want to relate.  

   ![Identifier image for the row to relate](../media/relate-rows/identifier.png)

   The list of supported one-to-many and many-to-many relationships based on the table type selected is populated in the format \<Related Table Type\> – \<Relationship Schema Name\>. You can select the relationship to which you want to relate your row.  

   ![Relationship image](../media/relate-rows/relationship.png)

1. Enter the full resource URL of the row to which you want to add the relationship. 

   This URL is the full OData identifier of the resource, as shown in the following image.  

   ![Full odata URL](../media/relate-rows/relate-with-url.png)

   >[!TIP]
   >You can get the row identifier URL from a previous step from the available dynamic content.  


## Unrelate rows

1. Select **New step** to add an action to your flow.
1. Enter **unrelate rows** into the **Search connectors and actions** search box on the **Choose an operation** card.
1. Select **Microsoft Dataverse**.
1. Select **unrelate rows** action.

   Your flow uses this action to disassociate two Dataverse rows if they are linked via a one-to-many or many-to-many relationship.

   ![Unrelate rows image](../media/relate-rows/unrelate-action.png)

1. Select the type of table you want to unrelate from or enter a custom value for the table name.

1. Enter the identifier of the row you want to unrelate from.  

   ![Table name and identifier](../media/relate-rows/unrelate-table-name-identifier.png)

   The list of supported one-to-many and many-to-many relationships based on the table type you selected will be populated in the format \<Related Table Type\> – \<Relationship Schema Name\>. Select the relationship you want to unrelate the related table from or enter your custom value for the relationship schema name.  

   ![The unrelate rows card](../media/dataverse-how-tos/32bf6c8258bd3cf157fc90e63853fac0.png)

1. Enter the full resource URL of the related table you want to unrelate. This
will be the full OData identifier of the resource.  

   ![Resource URL](../media/dataverse-how-tos/13117f752dc1c3ab791b59457712f4c9.png)

   >[!TIP]
   >You can usually grab the row identifier from a previous step by using dynamic content.  

   ![Dynamic content from previous steps](../media/dataverse-how-tos/33403937ade7afee4e2583be75d81bc4.png)
