---
title: TextBox.FormatConditions property (Access)
keywords: vbaac10.chm11038
f1_keywords:
- vbaac10.chm11038
ms.prod: access
api_name:
- Access.TextBox.FormatConditions
ms.assetid: 6c643d8b-9b90-2b50-2ba0-c46bb821d38d
ms.date: 03/01/2019
ms.localizationpriority: medium
---


# TextBox.FormatConditions property (Access)

Use the **FormatConditions** property to return a read-only reference to the **[FormatConditions](Access.FormatConditions.md)** collection and its related properties.


## Syntax

_expression_.**FormatConditions**

_expression_ A variable that represents a **[TextBox](Access.TextBox.md)** object.


## Example

The following example sets format properties for an existing conditional format for the **Textbox1** control.

```vb
With Forms("forms1").Controls("Textbox1").FormatConditions(1) 
 .BackColor = RGB(255,255,255) 
 .FontBold = True 
 .ForeColor = RGB(255,0,0) 
End With
```



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]