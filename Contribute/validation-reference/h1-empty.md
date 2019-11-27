---
title: h1-empty
description: Объяснение проблемы со сборкой документов h1-empty и способа ее устранения
author: meganbradley
ms.author: mbradley
ms.topic: error-reference
ms.date: 11/25/2019
ms.prod: non-product-specific
ms.openlocfilehash: d0b3ab2206d66ff68a967d7868353b5b399da80a
ms.sourcegitcommit: 423d9b8145a11426c91f45510b2d77319838eb27
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/26/2019
ms.locfileid: "74528791"
---
# <a name="h1-empty"></a><span data-ttu-id="edf1e-103">h1-empty</span><span class="sxs-lookup"><span data-stu-id="edf1e-103">h1-empty</span></span>

## <a name="warning"></a><span data-ttu-id="edf1e-104">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="edf1e-104">Warning</span></span>

`H1 is required. Add content to your top-level heading.`

<span data-ttu-id="edf1e-105">H1 — это первый заголовок в файле Markdown.</span><span class="sxs-lookup"><span data-stu-id="edf1e-105">H1 refers to the first heading in a Markdown file.</span></span> <span data-ttu-id="edf1e-106">При публикации на веб-сайте docs.microsoft.com заголовок H1 отображается крупным шрифтом в верхней части страницы.</span><span class="sxs-lookup"><span data-stu-id="edf1e-106">When published to docs.microsoft.com, the H1 shows at the top of the page in a large font.</span></span> <span data-ttu-id="edf1e-107">Для создания заголовка H1 необходимо указать в начале строки один символ решетки (#), после которого следует пробел и текст заголовка.</span><span class="sxs-lookup"><span data-stu-id="edf1e-107">An H1 is created by beginning a line with a single hash (#) followed by a space, then the heading text.</span></span>

## <a name="resolution"></a><span data-ttu-id="edf1e-108">Способы устранения</span><span class="sxs-lookup"><span data-stu-id="edf1e-108">Resolution</span></span>

<span data-ttu-id="edf1e-109">Чтобы устранить эту проблему, убедитесь в том, что, помимо символа решетки, заголовок H1 также включает в себя содержимое.</span><span class="sxs-lookup"><span data-stu-id="edf1e-109">To fix this issue, make sure your H1 includes content, not just a hash.</span></span>

<span data-ttu-id="edf1e-110">Неверно:</span><span class="sxs-lookup"><span data-stu-id="edf1e-110">Bad:</span></span>

```markdown
---
author: meganbradley
ms.author: mbradley
---
#
This is not an H1
```

<span data-ttu-id="edf1e-111">Верно:</span><span class="sxs-lookup"><span data-stu-id="edf1e-111">Good:</span></span>

```markdown
---
author: meganbradley
ms.author: mbradley
---
# This is an H1
```

<!--make sure to add this file to your includes folder and verify the path-->
[!INCLUDE [validation-reference-help](includes/validation-reference-help.md)]
