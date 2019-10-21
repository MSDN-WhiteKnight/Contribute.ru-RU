---
title: h1-in-moniker
description: Объяснение проблемы со сборкой документов h1-in-moniker и способа ее устранения
author: meganbradley
ms.author: mbradley
ms.topic: error-reference
ms.date: 10/09/2019
ms.prod: non-product-specific
ms.openlocfilehash: 3730385cfaf86c3a2a6165f1958d644e71ad7b56
ms.sourcegitcommit: 57eb071bdc55ef71fa3f8ac979326c3f8fbe9c45
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2019
ms.locfileid: "72246367"
---
# <a name="h1-in-moniker"></a><span data-ttu-id="ee0b8-103">h1-in-moniker</span><span class="sxs-lookup"><span data-stu-id="ee0b8-103">h1-in-moniker</span></span>

[!INCLUDE [suggestion-note](includes/suggestion-note.md)]

## <a name="suggestion"></a><span data-ttu-id="ee0b8-104">Предложение</span><span class="sxs-lookup"><span data-stu-id="ee0b8-104">Suggestion</span></span>

`H1s are not allowed in moniker sections. Each article should have one and only one H1.`

<span data-ttu-id="ee0b8-105">H1 — это первый заголовок в файле Markdown.</span><span class="sxs-lookup"><span data-stu-id="ee0b8-105">H1 refers to the first heading in a Markdown file.</span></span> <span data-ttu-id="ee0b8-106">При публикации на веб-сайте docs.microsoft.com заголовок H1 отображается крупным шрифтом в верхней части страницы.</span><span class="sxs-lookup"><span data-stu-id="ee0b8-106">When published to docs.microsoft.com, the H1 shows at the top of the page in a large font.</span></span> <span data-ttu-id="ee0b8-107">Для создания заголовка H1 необходимо указать в начале строки один символ решетки (#), после которого следует пробел и текст заголовка.</span><span class="sxs-lookup"><span data-stu-id="ee0b8-107">An H1 is created by beginning a line with a single hash (#) followed by a space, then the heading text.</span></span> <span data-ttu-id="ee0b8-108">В каждом файле может быть только один заголовок H1.</span><span class="sxs-lookup"><span data-stu-id="ee0b8-108">You can only have one H1 in each file.</span></span> <span data-ttu-id="ee0b8-109">Заголовки H1 не допускаются в разделах моникеров, так как их наличие может легко привести к дублированию или отсутствию заголовков H1 в зависимости от настройки системы управления версиями.</span><span class="sxs-lookup"><span data-stu-id="ee0b8-109">H1s aren't allowed in moniker sections, because H1s in monikers can easily cause duplicate or missing H1s depending on how versioning is configured.</span></span>

<span data-ttu-id="ee0b8-110">Кроме того, это сообщение можно получить, если раздел моникера содержит строку, состоящую из знаков равенства, которые образуют двойное подчеркивание, например: `=======`.</span><span class="sxs-lookup"><span data-stu-id="ee0b8-110">You might also get this message if a moniker section contains a line of equals signs making a double underline, like this: `=======`.</span></span> <span data-ttu-id="ee0b8-111">Это альтернативный синтаксис Markdown для заголовков H1.</span><span class="sxs-lookup"><span data-stu-id="ee0b8-111">This is an alternative Markdown syntax for an H1.</span></span> <span data-ttu-id="ee0b8-112">Он также часто встречается в конфликтах слияния:</span><span class="sxs-lookup"><span data-stu-id="ee0b8-112">It's also commonly seen in merge conflicts:</span></span>

```markdown
<<<<<<< HEAD
...
=======
...
>>>>>>> 1d82c7efe18f86136247fb366df5030843199c19
```

## <a name="resolution"></a><span data-ttu-id="ee0b8-113">Способы устранения</span><span class="sxs-lookup"><span data-stu-id="ee0b8-113">Resolution</span></span>

<span data-ttu-id="ee0b8-114">Чтобы устранить эту проблему, удалите заголовки H1 из всех разделов моникеров и убедитесь в том, что заголовок H1 в начале статьи подходит для всех разделов моникеров.</span><span class="sxs-lookup"><span data-stu-id="ee0b8-114">To fix this issue, remove H1s from all moniker sections, and make sure the H1 at the top of the article is appropriate for all moniker sections.</span></span> <span data-ttu-id="ee0b8-115">Обратите внимание на то, что пропускать уровни заголовков, например указывать H3 сразу после H1, запрещено.</span><span class="sxs-lookup"><span data-stu-id="ee0b8-115">Note that skipping heading levels, such as following H1 with H3, isn't allowed.</span></span>

<span data-ttu-id="ee0b8-116">Если заголовок H1 в разделе моникера фактически является двойным подчеркиванием (`=======`), удалите его или замените на заголовок из хэштегов, например `##`, в зависимости от ситуации.</span><span class="sxs-lookup"><span data-stu-id="ee0b8-116">If an H1 in a moniker section is actually a double underline (`=======`), remove it or replace it with a hashtag heading, such as `##`, as appropriate.</span></span> <span data-ttu-id="ee0b8-117">Если двойное подчеркивание является частью конфликта слияния, необходимо также удалить начальный и конечный маркеры конфликта слияния и устаревший текст.</span><span class="sxs-lookup"><span data-stu-id="ee0b8-117">If the double underline is part of a merge conflict, make sure to also remove the merge conflict beginning and ending markers and the obsolete text.</span></span>

<!--make sure to add this file to your includes folder and verify the path-->
[!INCLUDE [validation-reference-help](includes/validation-reference-help.md)]