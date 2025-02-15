---
title: Project.ProjectFinish property (Project)
ms.prod: project-server
api_name:
- Project.Project.ProjectFinish
ms.assetid: ff56a629-5a83-0a13-6312-b91803b30d53
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# Project.ProjectFinish property (Project)

Gets or sets the finish date for a project. Read/write **Variant**.


## Syntax

_expression_. `ProjectFinish`

_expression_ A variable that represents a **[Project](project.project.md)** object.


## Remarks

Setting **ProjectFinish** also causes the project to be scheduled from its finish date. This has the same effect as setting the **ScheduleFromStart** property to **False**.

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]