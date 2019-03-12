---
title: h1-empty
description: Объяснение проблемы со сборкой документов h1-empty и способа ее устранения
author: meganbradley
ms.author: mbradley
ms.topic: error-reference
ms.date: 12/12/2018
ms.prod: non-product-specific
ms.openlocfilehash: bb07235f7cd1ba6d45418c48a4190255bdd9a428
ms.sourcegitcommit: 4053577bd0478d711257a283ee661d618b49c2df
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2019
ms.locfileid: "57427683"
---
# <a name="h1-empty"></a><span data-ttu-id="5b596-103">h1-empty</span><span class="sxs-lookup"><span data-stu-id="5b596-103">h1-empty</span></span>

## <a name="warning"></a><span data-ttu-id="5b596-104">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="5b596-104">Warning</span></span>

`H1 is required. Add content to your top-level heading.`

<span data-ttu-id="5b596-105">H1 — это первый заголовок в файле Markdown.</span><span class="sxs-lookup"><span data-stu-id="5b596-105">H1 refers to the first heading in a Markdown file.</span></span> <span data-ttu-id="5b596-106">При публикации на веб-сайте docs.microsoft.com заголовок H1 отображается крупным шрифтом в верхней части страницы.</span><span class="sxs-lookup"><span data-stu-id="5b596-106">When published to docs.microsoft.com, the H1 shows at the top of the page in a large font.</span></span> <span data-ttu-id="5b596-107">Для создания заголовка H1 необходимо указать в начале строки один символ решетки (#), после которого следует пробел и текст заголовка.</span><span class="sxs-lookup"><span data-stu-id="5b596-107">An H1 is created by beginning a line with a single hash (#) followed by a space, then the heading text.</span></span>

## <a name="resolution"></a><span data-ttu-id="5b596-108">Способы устранения</span><span class="sxs-lookup"><span data-stu-id="5b596-108">Resolution</span></span>

<span data-ttu-id="5b596-109">Чтобы устранить эту проблему, убедитесь в том, что, помимо символа решетки, заголовок H1 также включает в себя содержимое.</span><span class="sxs-lookup"><span data-stu-id="5b596-109">To fix this issue, make sure your H1 includes content, not just a hash.</span></span>

<span data-ttu-id="5b596-110">Неверно:</span><span class="sxs-lookup"><span data-stu-id="5b596-110">Bad:</span></span>

```markdown
---
author: meganbradley
ms.author: mbradley
---
#
This is not an H1
```

<span data-ttu-id="5b596-111">Верно:</span><span class="sxs-lookup"><span data-stu-id="5b596-111">Good:</span></span>

```markdown
---
author: meganbradley
ms.author: mbradley
---
# This is an H1
```

<!--make sure to add this file to your includes folder and verify the path-->
[!INCLUDE [validation-reference-help](includes/validation-reference-help.md)]