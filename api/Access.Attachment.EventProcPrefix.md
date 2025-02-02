---
title: Attachment.EventProcPrefix property (Access)
keywords: vbaac10.chm13912
f1_keywords:
- vbaac10.chm13912
ms.prod: access
api_name:
- Access.Attachment.EventProcPrefix
ms.assetid: f58670ff-b42c-69eb-0561-90ce5cc40d19
ms.date: 02/07/2019
ms.localizationpriority: medium
---


# Attachment.EventProcPrefix property (Access)

Gets or sets the prefix portion of an event procedure name. Read/write **String**.


## Syntax

_expression_.**EventProcPrefix**

_expression_ A variable that represents an **[Attachment](Access.Attachment.md)** object.


## Remarks

For example, if you have a command button with an event procedure named **Details_Click**, the **EventProcPrefix** property returns the string **Details**.

Microsoft Access adds the prefix portion of an event procedure name to the event name with an underscore character ( _ ).




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]