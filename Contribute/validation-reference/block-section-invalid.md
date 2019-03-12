---
title: block-section-invalid
description: Объяснение проблемы со сборкой документов block-section-invalid и способа ее устранения
author: meganbradley
ms.author: mbradley
ms.topic: error-reference
ms.date: 2/28/2019
ms.prod: non-product-specific
ms.openlocfilehash: 257b963ae37f5a8f0edc2fbca6186ab0f258cfc0
ms.sourcegitcommit: 4053577bd0478d711257a283ee661d618b49c2df
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2019
ms.locfileid: "57427887"
---
# <a name="block-section-invalid"></a>block-section-invalid

## <a name="warning"></a>Предупреждение

`Invalid syntax for alert, div, or video. The text will be rendered as a block quote.`

Несколько расширений Markdown для документов начинаются со строки `> [!`. Между символами `>` и `[` требуется пробел. Кроме того, необходима закрывающая скобка `]`. Если синтаксис неверен, текст будет отображаться в виде цитаты.

## <a name="resolution"></a>Способы устранения

[!INCLUDE [docs-authoring-pack](includes/docs-authoring-pack.md)]

Убедитесь в том, что расширение имеет правильный синтаксис:

```markdown

Alerts:

> [!NOTE]
> Information the user should notice even if skimming.

> [!TIP]
> Optional information to help a user be more successful.

> [!IMPORTANT]
> Essential information required for user success.

> [!CAUTION]
> Negative potential consequences of an action.

> [!WARNING]
> Dangerous certain consequences of an action.

Videos:

> [!VIDEO https://channel9.msdn.com/Series/Youve-Got-Key-Values-A-Redis-Jump-Start/03/player]

> [!VIDEO https://www.youtube.com/embed/iAtwVM-Z7rY]

> [!VIDEO https://www.microsoft.com/en-us/videoplayer/embed/RE1XVQS]

Sections (div):

> [!div class="class"]

```


<!--make sure to add this file to your includes folder and verify the path-->
[!INCLUDE [validation-reference-help](includes/validation-reference-help.md)]
