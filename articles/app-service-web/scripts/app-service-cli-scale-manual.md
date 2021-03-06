---
title: Azure CLI Script Sample - Scale a Web App manually using Azure CLI 2.0 | Microsoft Docs
description: Azure CLI Script Sample - Scale a Web App manually using Azure CLI 2.0
services: appservice
documentationcenter: appservice
author: syntaxc4
manager: erikre
editor: 
tags: azure-service-management

ms.assetid: 251d9074-8fff-4121-ad16-9eca9556ac96
ms.service: app-service
ms.devlang: azurecli
ms.topic: sample
ms.tgt_pltfrm: na
ms.workload: web
ms.date: 03/20/2017
ms.author: cfowler
---

# Scale a web app manually

In this scenario you will learn to create a resource group, app service plan and web app. You will then scale the App Service Plan from a single instance to multiple instances.

[!INCLUDE [sample-cli-install](../../../includes/sample-cli-install.md)]

## Sample script

[!code-azurecli-interactive[main](../../../cli_scripts/app-service/scale-manual/scale-manual.sh "Manual Scale")]

[!INCLUDE [cli-script-clean-up](../../../includes/cli-script-clean-up.md)]

## Script explanation

This script uses the following commands to create a resource group, web app, and all related resources. Each command in the table links to command specific documentation.

| Command | Notes |
|---|---|
| [az group create](https://docs.microsoft.com/cli/azure/group#create) | Creates a resource group in which all resources are stored. |
| [az appservice plan create](https://docs.microsoft.com/cli/azure/appservice/plan#create) | Creates an App Service plan. This is like a server farm for your Azure web app. |
| [az appservice web create](https://docs.microsoft.com/cli/azure/appservice/web#create) | Creates an Azure web app within the App Service plan. |
| [az appservice plan update](https://docs.microsoft.com/cli/azure/appservice/plan#update) | Updates properties of the App Service plan. |

## Next steps

For more information on the Azure CLI, see [Azure CLI documentation](https://docs.microsoft.com/cli/azure/overview).

Additional App Service CLI script samples can be found in the [Azure App Service documentation](../app-service-cli-samples.md).
