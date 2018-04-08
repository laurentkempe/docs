---
title: Azure Logic Apps | Serverless apps. Architecture, patterns, and Azure implementation.
description: Azure Logic Apps enable building automated scalable workflows that integrate apps and data across cloud services and on-premises systems.
author: JEREMYLIKNESS
ms.author: jeliknes
ms.date: 4/4/2018
ms.prod: .net
ms.technology: dotnet
ms.topic: article
---
# Azure Logic Apps

[Azure Logic Apps](/azure/logic-apps) provides a serverless engine to build automated workflows to integrate apps and data between cloud services and on-premises systems. s you build workflows using a visual designer. You can trigger workflows based on events or timers and leverage connectors to integration applications and facilitate business-to-business (B2B) communication. Logic Apps integrates seamlessly with Azure Functions.

![Azure Logic Apps logo](./media/logic-apps/logic-apps-logo.png)

Do more than connect your cloud services like functions with cloud resources using Logic Apps. You can also orchestrate on-premises workflows with the on-premises gateway. For example, you can trigger a SQL stored procedure in response to a cloud-based event or conditional logic in your workflow.

![Logic Apps architecture](./media/logic-apps/logic-apps-architecture.png)

Like Azure Functions, you kick off Logic App workflows with a trigger. There are many triggers for you to choose from. The following capture shows just a few of the more popular ones out of hundreds that are available.

![Logic Apps triggers](./media/logic-apps/logic-app-triggers.png)

Once the app is triggered, you can use the visual designer to build out steps, loops, conditions, and actions. Any data ingested in a previous step is available for you to use in subsequent steps. The following workflow loads URLs from a CosmosDB database. It finds the ones with a host of `t.co` then searches for them on Twitter. If it finds corresponding tweets, it updates the documents with the related tweets by calling a function.

![Logic App workflow](./media/logic-apps/logic-app-workflow.png)

The Logic Apps dashboard shows the history of running your workflows and whether or not each run completed successfully or not. You can navigate into any given run and inspect the data used by each step for troubleshooting. Logic Apps also provides existing templates you can edit and are suited for complex enterprise workflows.

To learn more, see: [Azure Logic Apps](/azure/logic-apps).

>[!div class="step-by-step"]
[Previous] (./application-insights.md)
[Next] (./event-grid.md)