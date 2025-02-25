---
title: Use a flow to add a row in Dataverse | Microsoft Docs
description: Learn how to add rows in Microsoft Dataverse with flows. 
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

# Use a flow to add a row in Dataverse

Use the **Add a new row** action to add a new row in Microsoft Dataverse.

Follow these steps to add a new **Account** in Dataverse when you receive an email to your signup address, as shown in the following image.

1. Create a flow with the **When a new email arrives (V3)** trigger to your flow.
1. Select **New step** to add an action to your flow.
1. Enter **new row** into the **Search connectors and actions** search box on the **Choose an operation** card.
1. Select **Microsoft Dataverse**.
1. Select **Add a new row** action.

   ![Add a new row image](../media/add-row/add-row-1.png)

1. Select the **Accounts** table n the **Add a new row** card.

   ![Select the Accounts table](../media/add-row/add-row-2.png)

   After you select a table, the card expands, displaying both optional and required items. All mandatory items display an asterisk (\*).

1. Optional: if you don't see a column that you need, select **Show advanced options** at the bottom of the card to view all columns.

   ![Card that shows all columns for the add a new row action](../media/add-row/show-all-advanced.png)

>[!TIP]
>You can use outputs from previous triggers and actions in the **Dynamic content** selector shown in the following image, or modify them by building an **Expression** as outlined in [Use expressions in flow actions](https://flow.microsoft.com/en-us/blog/use-expressions-in-actions/).

   ![Dynamic content](../media/add-row/dynamic-content.png)




