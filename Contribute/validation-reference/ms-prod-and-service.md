---
title: ms-prod-and-service
description: Объяснение и устранение проблем сборки документов ms-prod-and-service
author: meganbradley
ms.author: mbradley
ms.topic: error-reference
ms.date: 1/15/2019
ms.prod: non-product-specific
ms.openlocfilehash: 77c0dd71cf526ee837799bcd01e21290ce7d6058
ms.sourcegitcommit: 8e897e90268a8a87dc4b97d7c28d22ed5950c8d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "58636754"
---
# <a name="ms-prod-and-service"></a><span data-ttu-id="234e1-103">ms-prod-and-service</span><span class="sxs-lookup"><span data-stu-id="234e1-103">ms-prod-and-service</span></span>

[!INCLUDE [suggestion-note](includes/suggestion-note.md)]

## <a name="suggestion"></a><span data-ttu-id="234e1-104">Предложение</span><span class="sxs-lookup"><span data-stu-id="234e1-104">Suggestion</span></span>

`Both ms.prod and ms.service can't be specified. Use ms.prod for on-premise products, or ms.service for cloud services.`

## <a name="resolution"></a><span data-ttu-id="234e1-105">Способы устранения</span><span class="sxs-lookup"><span data-stu-id="234e1-105">Resolution</span></span>

<span data-ttu-id="234e1-106">Требуется указать значение `ms.prod` или `ms.service`, которые нельзя указывать одновременно: `ms.prod` используется для локальных продуктов, а `ms.service` — для облачных служб.</span><span class="sxs-lookup"><span data-stu-id="234e1-106">Either `ms.prod` or `ms.service` is required, and they can't both be present: `ms.prod` is used for on-premises products; `ms.service` is used for cloud services.</span></span> <span data-ttu-id="234e1-107">Определите подходящее значение для своей статьи, убедитесь в его правильности и удалите другое поле.</span><span class="sxs-lookup"><span data-stu-id="234e1-107">Determine which is appropriate for your article, verify that the value is correct, and remove the other field.</span></span>

<span data-ttu-id="234e1-108">Допустимые значения можно найти на [этом внутреннем сайте корпорации Майкрософт](https://docsmetadatatool.azurewebsites.net/allowlists).</span><span class="sxs-lookup"><span data-stu-id="234e1-108">Valid values can be found on [this Microsoft-internal site](https://docsmetadatatool.azurewebsites.net/allowlists).</span></span>

<!--make sure to add this file to your includes folder and verify the path-->
[!INCLUDE [validation-reference-help](includes/validation-reference-help.md)]
