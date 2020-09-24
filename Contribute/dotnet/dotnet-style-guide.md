---
title: Шаблон и подсказки для статей о .NET
description: В этой статье приводится удобный шаблон написания статей для репозиториев с документацией по .NET
ms.topic: contributor-guide
ms.prod: non-product-specific
ms.custom: external-contributor-guide
ms.date: 11/07/2018
ms.openlocfilehash: 15288ccb1831e994fd078f47788ad4c2f502775c
ms.sourcegitcommit: 92d06515af1d9d0e5abf632fc3b6425c487174d5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/21/2020
ms.locfileid: "90837219"
---
# <a name="metadata-and-markdown-template-for-net-docs"></a><span data-ttu-id="2693a-103">Шаблон метаданных и Markdown для документации .NET</span><span class="sxs-lookup"><span data-stu-id="2693a-103">Metadata and Markdown template for .NET docs</span></span>

<span data-ttu-id="2693a-104">Этот шаблон dotnet/docs содержит примеры синтаксиса Markdown и инструкции по указанию метаданных.</span><span class="sxs-lookup"><span data-stu-id="2693a-104">This dotnet/docs template contains examples of Markdown syntax and guidance on setting the metadata.</span></span>

<span data-ttu-id="2693a-105">При создании файла Markdown скопируйте приведенный шаблон в новый файл, укажите метаданные, как описано ниже, и установите заголовок H1 над названием статьи.</span><span class="sxs-lookup"><span data-stu-id="2693a-105">When creating a Markdown file, copy the included template to a new file, fill out the metadata as specified below, and set the H1 heading above to the title of the article.</span></span>

## <a name="metadata"></a><span data-ttu-id="2693a-106">Метаданные</span><span class="sxs-lookup"><span data-stu-id="2693a-106">Metadata</span></span>

<span data-ttu-id="2693a-107">Необходимый блок метаданных приводится в следующем примере блока метаданных:</span><span class="sxs-lookup"><span data-stu-id="2693a-107">The required metadata block is in the following sample metadata block:</span></span>

```markdown
---
title: [ARTICLE TITLE]
description: [usually a summary of your first paragraph. It gets displayed in search results, and can help drive the correct traffic if well written.]
author: [GITHUB USERNAME]
ms.date: [CREATION/UPDATE DATE - mm/dd/yyyy]
---
# The H1 should not be the same as the title, but should describe the article contents
```

- <span data-ttu-id="2693a-108">Между двоеточием (:) и значением в элементе метаданных **должен** быть пробел.</span><span class="sxs-lookup"><span data-stu-id="2693a-108">You **must** have a space between the colon (:) and the value for a metadata element.</span></span>
- <span data-ttu-id="2693a-109">Двоеточия в значении (например, заголовке) прерывают анализ метаданных.</span><span class="sxs-lookup"><span data-stu-id="2693a-109">Colons in a value (for example, a title) break the metadata parser.</span></span> <span data-ttu-id="2693a-110">В этом случае заключите заголовок в двойные кавычки (например, `title: "Writing .NET Core console apps: An advanced step-by-step guide"`).</span><span class="sxs-lookup"><span data-stu-id="2693a-110">In this case, surround the title with double quotes (for example, `title: "Writing .NET Core console apps: An advanced step-by-step guide"`).</span></span>
- <span data-ttu-id="2693a-111">**title**: Отображается в результатах поиска.</span><span class="sxs-lookup"><span data-stu-id="2693a-111">**title**: Appears in search engine results.</span></span> <span data-ttu-id="2693a-112">Заголовок должен совпадать со значением в заголовке H1 и не превышать 60 символов.</span><span class="sxs-lookup"><span data-stu-id="2693a-112">The title shouldn't be identical to the title in your H1 heading, and it should contain 60 characters or less.</span></span>
- <span data-ttu-id="2693a-113">**description**: Описание содержимого статьи.</span><span class="sxs-lookup"><span data-stu-id="2693a-113">**description**: Summarizes the content of the article.</span></span> <span data-ttu-id="2693a-114">Обычно описание отображается на странице результатов поиска, но не используется для упорядочивания результатов.</span><span class="sxs-lookup"><span data-stu-id="2693a-114">It's usually shown in the search results page, but it isn't used for search ranking.</span></span> <span data-ttu-id="2693a-115">Длина: 115–145 символов с пробелами.</span><span class="sxs-lookup"><span data-stu-id="2693a-115">Its length should be 115-145 characters including spaces.</span></span>
- <span data-ttu-id="2693a-116">**author**: В этом поле необходимо указать **имя пользователя автора на GitHub**.</span><span class="sxs-lookup"><span data-stu-id="2693a-116">**author**: The author field should contain the **GitHub username** of the author.</span></span>
- <span data-ttu-id="2693a-117">**ms.date**: Дата последнего значительного изменения.</span><span class="sxs-lookup"><span data-stu-id="2693a-117">**ms.date**: The date of the last significant update.</span></span> <span data-ttu-id="2693a-118">Измените это значение в существующей статье, если вы пересмотрели и обновили всю статью.</span><span class="sxs-lookup"><span data-stu-id="2693a-118">Update this on existing articles if you reviewed and updated the entire article.</span></span> <span data-ttu-id="2693a-119">Небольшие исправления, вроде опечаток, не считаются обновлением.</span><span class="sxs-lookup"><span data-stu-id="2693a-119">Small fixes, such as typos or similar do not warrant an update.</span></span>

<span data-ttu-id="2693a-120">К каждой статье прикрепляются другие метаданные, но обычно мы применяем значения большинства метаданных на уровне папки в файле **docfx.json**.</span><span class="sxs-lookup"><span data-stu-id="2693a-120">Other metadata is attached to each article, but we typically apply most metadata values at the folder level, specified in **docfx.json**.</span></span>

## <a name="basic-markdown-gfm-and-special-characters"></a><span data-ttu-id="2693a-121">Базовый Markdown, GFM и специальные символы</span><span class="sxs-lookup"><span data-stu-id="2693a-121">Basic Markdown, GFM, and special characters</span></span>

<span data-ttu-id="2693a-122">О базовых принципах Markdown, GitHub Flavored Markdown (GFM) и конкретных расширениях OPS можно прочитать в статье [Справочник по Markdown](../markdown-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2693a-122">You can learn the basics of Markdown, GitHub Flavored Markdown (GFM), and OPS-specific extensions in the [Markdown reference](../markdown-reference.md) article.</span></span>

<span data-ttu-id="2693a-123">Markdown использует для форматирования специальные символы, например \*, \` и \#.</span><span class="sxs-lookup"><span data-stu-id="2693a-123">Markdown uses special characters such as \*, \`, and \# for formatting.</span></span> <span data-ttu-id="2693a-124">Если вы хотите включить такой символ в свою статью, сделайте одно из двух:</span><span class="sxs-lookup"><span data-stu-id="2693a-124">If you wish to include one of these characters in your content, you must do one of two things:</span></span>

- <span data-ttu-id="2693a-125">Поставьте обратную косую черту перед символом, чтобы экранировать его (например, `\*` для \*).</span><span class="sxs-lookup"><span data-stu-id="2693a-125">Put a backslash before the special character to "escape" it (for example, `\*` for a \*).</span></span>
- <span data-ttu-id="2693a-126">Используйте [код сущности HTML](http://www.ascii.cl/htmlcodes.htm) для символа (например, `&#42;` для &#42;).</span><span class="sxs-lookup"><span data-stu-id="2693a-126">Use the [HTML entity code](http://www.ascii.cl/htmlcodes.htm) for the character (for example, `&#42;` for a &#42;).</span></span>

## <a name="file-names"></a><span data-ttu-id="2693a-127">Имена файлов</span><span class="sxs-lookup"><span data-stu-id="2693a-127">File names</span></span>

<span data-ttu-id="2693a-128">В именах файлов используются следующие правила:</span><span class="sxs-lookup"><span data-stu-id="2693a-128">File names use the following rules:</span></span>

* <span data-ttu-id="2693a-129">Имя может содержать только строчные буквы, цифры и дефисы.</span><span class="sxs-lookup"><span data-stu-id="2693a-129">Contain only lowercase letters, numbers, and hyphens.</span></span>
* <span data-ttu-id="2693a-130">Должны отсутствовать пробелы и знаки препинания.</span><span class="sxs-lookup"><span data-stu-id="2693a-130">No spaces or punctuation characters.</span></span> <span data-ttu-id="2693a-131">Для разделения слов и чисел в имени файла следует использовать дефисы.</span><span class="sxs-lookup"><span data-stu-id="2693a-131">Use the hyphens to separate words and numbers in the file name.</span></span>
* <span data-ttu-id="2693a-132">Следует использовать конкретные команды действий, такие как develop, buy, build, troubleshoot.</span><span class="sxs-lookup"><span data-stu-id="2693a-132">Use action verbs that are specific, such as develop, buy, build, troubleshoot.</span></span> <span data-ttu-id="2693a-133">Использование слов, оканчивающихся на -ing, не допускается.</span><span class="sxs-lookup"><span data-stu-id="2693a-133">No -ing words.</span></span>
* <span data-ttu-id="2693a-134">Нельзя использовать служебные (короткие) слова, такие как a, and, the, in, or и т. д.</span><span class="sxs-lookup"><span data-stu-id="2693a-134">No small words - don't include a, and, the, in, or, etc.</span></span>
* <span data-ttu-id="2693a-135">Имя должно быть основано на разметке Markdown и иметь расширение файла .md.</span><span class="sxs-lookup"><span data-stu-id="2693a-135">Must be in Markdown and use the .md file extension.</span></span>
* <span data-ttu-id="2693a-136">Имя файла должно быть коротким в разумных пределах.</span><span class="sxs-lookup"><span data-stu-id="2693a-136">Keep file names reasonably short.</span></span> <span data-ttu-id="2693a-137">Оно будет частью URL-адреса статьи.</span><span class="sxs-lookup"><span data-stu-id="2693a-137">They are part of the URL for your articles.</span></span>

## <a name="headings"></a><span data-ttu-id="2693a-138">Заголовки</span><span class="sxs-lookup"><span data-stu-id="2693a-138">Headings</span></span>

<span data-ttu-id="2693a-139">Используйте выделение прописных букв, как в предложении.</span><span class="sxs-lookup"><span data-stu-id="2693a-139">Use sentence-style capitalization.</span></span> <span data-ttu-id="2693a-140">Первое слово заголовка всегда должно начинаться с прописной буквы.</span><span class="sxs-lookup"><span data-stu-id="2693a-140">Always capitalize the first word of a heading.</span></span>

## <a name="text-styling"></a><span data-ttu-id="2693a-141">Стиль текста</span><span class="sxs-lookup"><span data-stu-id="2693a-141">Text styling</span></span>

<span data-ttu-id="2693a-142">*Курсив*</span><span class="sxs-lookup"><span data-stu-id="2693a-142">*Italics*</span></span>\
<span data-ttu-id="2693a-143">Используйте для обозначения файлов, папок, путей (длинные элементы вынесите в отдельную строку), новых терминов.</span><span class="sxs-lookup"><span data-stu-id="2693a-143">Use for files, folders, paths (for long items, split onto their own line), new terms.</span></span>

<span data-ttu-id="2693a-144">**Полужирный шрифт**</span><span class="sxs-lookup"><span data-stu-id="2693a-144">**Bold**</span></span>\
<span data-ttu-id="2693a-145">Используйте для элементов пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="2693a-145">Use for UI elements.</span></span>

`Code`\
<span data-ttu-id="2693a-146">Используйте для встроенного кода, ключевых слов языка, имен пакетов NuGet, команд в командной строке, имен таблиц баз данных и столбцов и URL-адресов, которые не должны быть активными.</span><span class="sxs-lookup"><span data-stu-id="2693a-146">Use for inline code, language keywords, NuGet package names, command-line commands, database table and column names, and URLs that you don't want to be clickable.</span></span>

## <a name="links"></a><span data-ttu-id="2693a-147">Создание ссылок</span><span class="sxs-lookup"><span data-stu-id="2693a-147">Links</span></span>

<span data-ttu-id="2693a-148">См. общую статью о [Ссылках](../how-to-write-links.md), чтобы узнать больше о привязках, внутренних ссылках, ссылках на другие документы, включениях кода и внешних ссылках.</span><span class="sxs-lookup"><span data-stu-id="2693a-148">See the general article on [Links](../how-to-write-links.md) for information about anchors, internal links, links to other documents, code includes, and external links.</span></span>

<span data-ttu-id="2693a-149">Команда по документации .NET использует следующие соглашения:</span><span class="sxs-lookup"><span data-stu-id="2693a-149">The .NET docs team uses the following conventions:</span></span>

- <span data-ttu-id="2693a-150">В большинстве случаев мы используем относительные ссылки и не рекомендуем использовать `~/` в ссылках, поскольку относительные ссылки разрешаются в источнике на GitHub.</span><span class="sxs-lookup"><span data-stu-id="2693a-150">In most cases, we use the relative links and discourage the use of `~/` in links because relative links resolve in the source on GitHub.</span></span> <span data-ttu-id="2693a-151">Но если мы размещаем ссылку на файл в зависимом репозитории, мы используем символ `~/`, чтобы указать путь.</span><span class="sxs-lookup"><span data-stu-id="2693a-151">However, whenever we link to a file in a dependent repo, we use the `~/` character to provide the path.</span></span> <span data-ttu-id="2693a-152">Поскольку файлы в зависимом репозитории располагаются в другом месте на GitHub, ссылки не будут корректно разрешаться при использовании относительных ссылок, как бы они ни были записаны.</span><span class="sxs-lookup"><span data-stu-id="2693a-152">Because the files in the dependent repo are in a different location in GitHub the links won't resolve correctly with relative links regardless of how they were written.</span></span>
- <span data-ttu-id="2693a-153">Спецификации языка C# и Visual Basic включены в документацию .NET путем включения источника из репозиториев этих языков.</span><span class="sxs-lookup"><span data-stu-id="2693a-153">The C# language specification and the Visual Basic language specification are included in the .NET docs by including the source from the language repositories.</span></span> <span data-ttu-id="2693a-154">Источники Markdown управляются в репозиториях [csharplang](https://github.com/dotnet/csharplang) и [vblang](https://github.com/dotnet/vblang).</span><span class="sxs-lookup"><span data-stu-id="2693a-154">The markdown sources are managed in the [csharplang](https://github.com/dotnet/csharplang) and [vblang](https://github.com/dotnet/vblang) repositories.</span></span>

<span data-ttu-id="2693a-155">Ссылки на спецификации должны указывать на исходные каталоги, содержащие эти спецификации.</span><span class="sxs-lookup"><span data-stu-id="2693a-155">Links to the spec must point to the source directories where those specs are included.</span></span> <span data-ttu-id="2693a-156">Для C# это **~/_csharplang/spec**, а для VB — **~/_vblang/spec**, как в следующем примере:</span><span class="sxs-lookup"><span data-stu-id="2693a-156">For C#, it's **~/_csharplang/spec** and for VB, it's **~/_vblang/spec**, as in the following example:</span></span>

```markdown
[C# Query Expressions](~/_csharplang/spec/expressions.md#query-expressions)
```

### <a name="links-to-apis"></a><span data-ttu-id="2693a-157">Ссылки на API</span><span class="sxs-lookup"><span data-stu-id="2693a-157">Links to APIs</span></span>

<span data-ttu-id="2693a-158">Система сборки имеет некоторые расширения, которые позволяют нам ссылаться на API .NET без использования внешних ссылок.</span><span class="sxs-lookup"><span data-stu-id="2693a-158">The build system has some extensions that allow us to link to .NET APIs without having to use external links.</span></span> <span data-ttu-id="2693a-159">Можно выбрать один из следующих вариантов синтаксиса:</span><span class="sxs-lookup"><span data-stu-id="2693a-159">You use one of the following syntax:</span></span>

1. <span data-ttu-id="2693a-160">Автоматическая ссылка: `<xref:UID>` или `<xref:UID?displayProperty=nameWithType>`.</span><span class="sxs-lookup"><span data-stu-id="2693a-160">Auto-link: `<xref:UID>` or `<xref:UID?displayProperty=nameWithType>`</span></span>

   <span data-ttu-id="2693a-161">Параметр запроса `displayProperty` создает полный текст ссылки.</span><span class="sxs-lookup"><span data-stu-id="2693a-161">The `displayProperty` query parameter produces a fully qualified link text.</span></span> <span data-ttu-id="2693a-162">По умолчанию в тексте ссылки отображается только имя члена или типа.</span><span class="sxs-lookup"><span data-stu-id="2693a-162">By default, link text shows only the member or type name.</span></span>

2. <span data-ttu-id="2693a-163">Ссылка с разметкой Markdown: `[link text](xref:UID)`</span><span class="sxs-lookup"><span data-stu-id="2693a-163">Markdown link: `[link text](xref:UID)`</span></span>

   <span data-ttu-id="2693a-164">Используется, когда требуется настроить текст ссылки.</span><span class="sxs-lookup"><span data-stu-id="2693a-164">Use when you want to customize the link text displayed.</span></span>

<span data-ttu-id="2693a-165">Примеры:</span><span class="sxs-lookup"><span data-stu-id="2693a-165">Examples:</span></span>

- <span data-ttu-id="2693a-166">`<xref:System.String>` отображается как [String](https://docs.microsoft.com/dotnet/api/system.string);</span><span class="sxs-lookup"><span data-stu-id="2693a-166">`<xref:System.String>` renders as [String](https://docs.microsoft.com/dotnet/api/system.string)</span></span>
- <span data-ttu-id="2693a-167">`<xref:System.String?displayProperty=nameWithType>` отображается как [System.String](https://docs.microsoft.com/dotnet/api/system.string);</span><span class="sxs-lookup"><span data-stu-id="2693a-167">`<xref:System.String?displayProperty=nameWithType>` renders as [System.String](https://docs.microsoft.com/dotnet/api/system.string)</span></span>
- <span data-ttu-id="2693a-168">`[String class](xref:System.String)` отображается как [String class](https://docs.microsoft.com/dotnet/api/system.string).</span><span class="sxs-lookup"><span data-stu-id="2693a-168">`[String class](xref:System.String)` renders as [String class](https://docs.microsoft.com/dotnet/api/system.string)</span></span>

<span data-ttu-id="2693a-169">Дополнительные сведения об использовании этой нотации см. в разделе об [использовании перекрестных ссылок](https://dotnet.github.io/docfx/tutorial/links_and_cross_references.html#using-cross-reference).</span><span class="sxs-lookup"><span data-stu-id="2693a-169">For more information about using this notation, see [Using cross reference](https://dotnet.github.io/docfx/tutorial/links_and_cross_references.html#using-cross-reference).</span></span>

<span data-ttu-id="2693a-170">Если идентификатор содержит специальные символы \`, \# или \*, значение UID должно быть закодировано в HTML как `%60`, `%23` и `%2A` соответственно.</span><span class="sxs-lookup"><span data-stu-id="2693a-170">Some UIDs contain the special characters \`, \# or \*, the UID value needs to be HTML encoded as `%60`, `%23` and `%2A` respectively.</span></span> <span data-ttu-id="2693a-171">Иногда круглые скобки тоже кодируются, но это не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2693a-171">You'll sometimes see parentheses encoded but it's not a requirement.</span></span>

<span data-ttu-id="2693a-172">Примеры:</span><span class="sxs-lookup"><span data-stu-id="2693a-172">Examples:</span></span>

- <span data-ttu-id="2693a-173">System.Threading.Tasks.Task\`1 заменяется на `System.Threading.Tasks.Task%601`;</span><span class="sxs-lookup"><span data-stu-id="2693a-173">System.Threading.Tasks.Task\`1 becomes `System.Threading.Tasks.Task%601`</span></span>
- <span data-ttu-id="2693a-174">System.Exception.\#ctor заменяется на `System.Exception.%23ctor`;</span><span class="sxs-lookup"><span data-stu-id="2693a-174">System.Exception.\#ctor becomes `System.Exception.%23ctor`</span></span>
- <span data-ttu-id="2693a-175">System.Lazy\`1.\#ctor(System.Threading.LazyThreadSafetyMode) заменяется на `System.Lazy%601.%23ctor%28System.Threading.LazyThreadSafetyMode%29`.</span><span class="sxs-lookup"><span data-stu-id="2693a-175">System.Lazy\`1.\#ctor(System.Threading.LazyThreadSafetyMode) becomes  `System.Lazy%601.%23ctor%28System.Threading.LazyThreadSafetyMode%29`</span></span>

<span data-ttu-id="2693a-176">UID для типов, список перегрузки членов или конкретный перегруженный член можно найти в `https://xref.docs.microsoft.com/autocomplete`.</span><span class="sxs-lookup"><span data-stu-id="2693a-176">You can find the UIDs of types, a member overload list, or a particular overloaded member from `https://xref.docs.microsoft.com/autocomplete`.</span></span> <span data-ttu-id="2693a-177">Строка запроса `?text=*\<type-member-name>*` определяет тип или элемент, UID которых вы хотите увидеть.</span><span class="sxs-lookup"><span data-stu-id="2693a-177">The query string `?text=*\<type-member-name>*` identifies the type or member whose UIDs you'd like to see.</span></span> <span data-ttu-id="2693a-178">Например, `https://xref.docs.microsoft.com/autocomplete?text=string.format` извлекает перегрузки [String.Format](https://docs.microsoft.com/dotnet/api/system.string.format).</span><span class="sxs-lookup"><span data-stu-id="2693a-178">For example, `https://xref.docs.microsoft.com/autocomplete?text=string.format` retrieves the [String.Format](https://docs.microsoft.com/dotnet/api/system.string.format) overloads.</span></span> <span data-ttu-id="2693a-179">Инструмент ищет предоставленный параметр запроса `text` в любой части UID.</span><span class="sxs-lookup"><span data-stu-id="2693a-179">The tool searches for the provided `text` query parameter in any part of the UID.</span></span> <span data-ttu-id="2693a-180">Например, вы можете искать имя члена (ToString), частичное имя члена (ToStri), тип и имя члена (Double.ToString) и т. д.</span><span class="sxs-lookup"><span data-stu-id="2693a-180">For example, you can search for member name (ToString), partial member name (ToStri), type and member name (Double.ToString), etc.</span></span>

<span data-ttu-id="2693a-181">Если добавить символ \* (или `%2A`) после UID, ссылка будет представлять страницу перегрузки, а не конкретный API.</span><span class="sxs-lookup"><span data-stu-id="2693a-181">If you add a \* (or `%2A`) after the UID, the link then represents the overload page and not a specific API.</span></span> <span data-ttu-id="2693a-182">Например, этот символ можно использовать, если требуется создать ссылку на страницу [List\<T>.BinarySearch Method](https://docs.microsoft.com/dotnet/api/system.collections.generic.list-1.binarysearch) обычным способом, а не на конкретную перегрузку, например [List\<T>.BinarySearch(T, IComparer\<T>)](https://docs.microsoft.com/dotnet/api/system.collections.generic.list-1.binarysearch#System_Collections_Generic_List_1_BinarySearch__0_).</span><span class="sxs-lookup"><span data-stu-id="2693a-182">For example, you can use that when you want to link to the [List\<T>.BinarySearch Method](https://docs.microsoft.com/dotnet/api/system.collections.generic.list-1.binarysearch) page in a generic way instead of a specific overload such as [List\<T>.BinarySearch(T, IComparer\<T>)](https://docs.microsoft.com/dotnet/api/system.collections.generic.list-1.binarysearch#System_Collections_Generic_List_1_BinarySearch__0_).</span></span> <span data-ttu-id="2693a-183">Также можно использовать \* для ссылки на страницу члена, если этот член не перегружен. Это позволит не включать список параметров в UID.</span><span class="sxs-lookup"><span data-stu-id="2693a-183">You can also use \* to link to a member page when the member is not overloaded; this saves you from having to include the parameter list in the UID.</span></span>

<span data-ttu-id="2693a-184">Чтобы сослаться на конкретную перегрузку метода, включите полное имя типа каждого параметра метода.</span><span class="sxs-lookup"><span data-stu-id="2693a-184">To link to a specific method overload, you must include the fully qualified type name of each of the method's parameters.</span></span> <span data-ttu-id="2693a-185">Например, \<xref:System.DateTime.ToString> ссылается на метод [DateTime.ToString](https://docs.microsoft.com/dotnet/api/system.datetime.tostring#System_DateTime_ToString) без параметров, а \<xref:System.DateTime.ToString(System.String,System.IFormatProvider)> ссылается на метод [DateTime.ToString(String,IFormatProvider)](https://docs.microsoft.com/dotnet/api/system.datetime.tostring#System_DateTime_ToString_System_String_System_IFormatProvider_).</span><span class="sxs-lookup"><span data-stu-id="2693a-185">For example, \<xref:System.DateTime.ToString> links to the parameterless [DateTime.ToString](https://docs.microsoft.com/dotnet/api/system.datetime.tostring#System_DateTime_ToString) method, while \<xref:System.DateTime.ToString(System.String,System.IFormatProvider)> links to the  [DateTime.ToString(String,IFormatProvider)](https://docs.microsoft.com/dotnet/api/system.datetime.tostring#System_DateTime_ToString_System_String_System_IFormatProvider_) method.</span></span>

<span data-ttu-id="2693a-186">Чтобы сослаться на универсальный тип, например [System.Collections.Generic.List\<T>](https://docs.microsoft.com/dotnet/api/system.collections.generic.list-1), используйте символ \` (`%60`) с указанием числа параметров универсального типа.</span><span class="sxs-lookup"><span data-stu-id="2693a-186">To link to a generic type, such as [System.Collections.Generic.List\<T>](https://docs.microsoft.com/dotnet/api/system.collections.generic.list-1), you use the \` (`%60`) character followed by the number of generic type parameters.</span></span> <span data-ttu-id="2693a-187">Например, `<xref:System.Nullable%601>` ссылается на тип [System.Nullable\<T>](https://docs.microsoft.com/dotnet/api/system.nullable-1), а `<xref:System.Func%602>` — на делегат [System.Func\<T,TResult>](https://docs.microsoft.com/dotnet/api/system.func-2).</span><span class="sxs-lookup"><span data-stu-id="2693a-187">For example, `<xref:System.Nullable%601>` links to the [System.Nullable\<T>](https://docs.microsoft.com/dotnet/api/system.nullable-1) type, while `<xref:System.Func%602>` links to the [System.Func\<T,TResult>](https://docs.microsoft.com/dotnet/api/system.func-2) delegate.</span></span>

## <a name="code"></a><span data-ttu-id="2693a-188">Код</span><span class="sxs-lookup"><span data-stu-id="2693a-188">Code</span></span>

<span data-ttu-id="2693a-189">Лучший способ включить код — включить фрагменты кода из рабочего примера.</span><span class="sxs-lookup"><span data-stu-id="2693a-189">The best way to include code is to include snippets from a working sample.</span></span> <span data-ttu-id="2693a-190">Создайте свой пример кода в соответствии с инструкциями из статьи [об участии в составлении документации по .NET](dotnet-contribute.md#contribute-to-samples).</span><span class="sxs-lookup"><span data-stu-id="2693a-190">Create your sample following the instructions in the [contributing to .NET](dotnet-contribute.md#contribute-to-samples) article.</span></span> <span data-ttu-id="2693a-191">Если включать фрагменты кода из полных программ, весь код будет проходить через систему непрерывной интеграции.</span><span class="sxs-lookup"><span data-stu-id="2693a-191">Including snippets from full programs ensures that all code runs through our Continuous Integration (CI) system.</span></span> <span data-ttu-id="2693a-192">Но если вам нужно показать что-то, что вызывает ошибки во время компиляции или выполнения, используйте встроенные блоки кода.</span><span class="sxs-lookup"><span data-stu-id="2693a-192">However, if you need to show something that causes compile time or runtime errors, you can use inline code blocks.</span></span>

<span data-ttu-id="2693a-193">Сведения о синтаксисе Markdown для отображения кода в документах см. в статье [Включение кода в документы](../code-in-docs.md).</span><span class="sxs-lookup"><span data-stu-id="2693a-193">For information about the Markdown syntax for showing code in docs, see [How to include code in docs](../code-in-docs.md).</span></span>

## <a name="images"></a><span data-ttu-id="2693a-194">Изображения</span><span class="sxs-lookup"><span data-stu-id="2693a-194">Images</span></span>

### <a name="static-image-or-animated-gif"></a><span data-ttu-id="2693a-195">Статическое изображение или анимационный GIF</span><span class="sxs-lookup"><span data-stu-id="2693a-195">Static image or animated GIF</span></span>

```markdown
![this is the alt text](../images/Logo_DotNet.png)
```

### <a name="linked-image"></a><span data-ttu-id="2693a-196">Изображения по ссылкам</span><span class="sxs-lookup"><span data-stu-id="2693a-196">Linked image</span></span>

```markdown
[![alt text for linked image](../images/Logo_DotNet.png)](https://dot.net)
```

## <a name="videos"></a><span data-ttu-id="2693a-197">Видеоролики</span><span class="sxs-lookup"><span data-stu-id="2693a-197">Videos</span></span>

<span data-ttu-id="2693a-198">Сейчас можно встраивать видео Channel 9 и YouTube со следующим синтаксисом:</span><span class="sxs-lookup"><span data-stu-id="2693a-198">Currently, you can embed both Channel 9 and YouTube videos with the following syntax:</span></span>

### <a name="channel-9"></a><span data-ttu-id="2693a-199">Channel 9</span><span class="sxs-lookup"><span data-stu-id="2693a-199">Channel 9</span></span>

```markdown
> [!VIDEO <channel9_video_link>]
```

<span data-ttu-id="2693a-200">Чтобы получить корректный URL-адрес видео, откройте вкладку **Встроить** под видео и скопируйте URL-адрес из элемента `<iframe>`.</span><span class="sxs-lookup"><span data-stu-id="2693a-200">To get the video's correct URL, select the **Embed** tab below the video frame, and copy the URL from the `<iframe>` element.</span></span> <span data-ttu-id="2693a-201">Например:</span><span class="sxs-lookup"><span data-stu-id="2693a-201">For example:</span></span>

```markdown
> [!VIDEO https://channel9.msdn.com/Blogs/dotnet/NET-Core-20-Released/player]
```

### <a name="youtube"></a><span data-ttu-id="2693a-202">YouTube</span><span class="sxs-lookup"><span data-stu-id="2693a-202">YouTube</span></span>

<span data-ttu-id="2693a-203">Чтобы получить корректный URL-адрес видео, щелкните правой кнопкой мыши на видео, выберите **Копировать код внедрения** и скопируйте URL-адрес из элемента `<iframe>`.</span><span class="sxs-lookup"><span data-stu-id="2693a-203">To get the video's correct URL, right-click on the video, select **Copy Embed Code**, and copy the URL from the `<iframe>` element.</span></span>

```markdown
> [!VIDEO <youtube_video_link>]
```

<span data-ttu-id="2693a-204">Например:</span><span class="sxs-lookup"><span data-stu-id="2693a-204">For example:</span></span>

```markdown
> [!VIDEO https://www.youtube.com/embed/Q2mMbjw6cLA]
```

## <a name="docsmicrosoft-extensions"></a><span data-ttu-id="2693a-205">Расширения docs.microsoft</span><span class="sxs-lookup"><span data-stu-id="2693a-205">docs.microsoft extensions</span></span>

<span data-ttu-id="2693a-206">docs.microsoft предоставляет несколько дополнительных расширений для GitHub Flavored Markdown.</span><span class="sxs-lookup"><span data-stu-id="2693a-206">docs.microsoft provides a few additional extensions to GitHub Flavored Markdown.</span></span>

### <a name="checked-lists"></a><span data-ttu-id="2693a-207">Списки с установленными флажками</span><span class="sxs-lookup"><span data-stu-id="2693a-207">Checked lists</span></span>

<span data-ttu-id="2693a-208">К спискам можно применять настраиваемые стили.</span><span class="sxs-lookup"><span data-stu-id="2693a-208">A custom style is available for lists.</span></span> <span data-ttu-id="2693a-209">Можно отображать списки с зелеными флажками.</span><span class="sxs-lookup"><span data-stu-id="2693a-209">You can render lists with green check marks.</span></span>

```markdown
> [!div class="checklist"]
> * How to create a .NET Core app
> * How to add a reference to the Microsoft.XmlSerializer.Generator package
> * How to edit your MyApp.csproj to add dependencies
> * How to add a class and an XmlSerializer
> * How to build and run the application
```

<span data-ttu-id="2693a-210">Это выглядит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="2693a-210">This renders as:</span></span>

> [!div class="checklist"]
> * <span data-ttu-id="2693a-211">Создание приложения .NET Core</span><span class="sxs-lookup"><span data-stu-id="2693a-211">How to create a .NET Core app</span></span>
> * <span data-ttu-id="2693a-212">Добавление ссылки на пакет Microsoft.XmlSerializer.Generator</span><span class="sxs-lookup"><span data-stu-id="2693a-212">How to add a reference to the Microsoft.XmlSerializer.Generator package</span></span>
> * <span data-ttu-id="2693a-213">Редактирование MyApp.csproj для добавления зависимостей</span><span class="sxs-lookup"><span data-stu-id="2693a-213">How to edit your MyApp.csproj to add dependencies</span></span>
> * <span data-ttu-id="2693a-214">Добавление класса как XmlSerializer</span><span class="sxs-lookup"><span data-stu-id="2693a-214">How to add a class and an XmlSerializer</span></span>
> * <span data-ttu-id="2693a-215">Создание и запуск приложения</span><span class="sxs-lookup"><span data-stu-id="2693a-215">How to build and run the application</span></span>

<span data-ttu-id="2693a-216">Пример списков с флажками в действии можно посмотреть в [документации по .NET Core](https://docs.microsoft.com/dotnet/core/additional-tools/xml-serializer-generator).</span><span class="sxs-lookup"><span data-stu-id="2693a-216">You can see an example of checked lists in action in the [.NET Core docs](https://docs.microsoft.com/dotnet/core/additional-tools/xml-serializer-generator).</span></span>

### <a name="buttons"></a><span data-ttu-id="2693a-217">Кнопки</span><span class="sxs-lookup"><span data-stu-id="2693a-217">Buttons</span></span>

<span data-ttu-id="2693a-218">Ссылки на кнопки:</span><span class="sxs-lookup"><span data-stu-id="2693a-218">Button links:</span></span>

```markdown
> [!div class="button"]
> [button links](dotnet-contribute.md)
```

<span data-ttu-id="2693a-219">Это выглядит следующим образом:</span><span class="sxs-lookup"><span data-stu-id="2693a-219">This renders as:</span></span>

> [!div class="button"]
> [<span data-ttu-id="2693a-220">ссылки на кнопки</span><span class="sxs-lookup"><span data-stu-id="2693a-220">button links</span></span>](dotnet-contribute.md)

<span data-ttu-id="2693a-221">Пример кнопок в действии можно посмотреть в [документации по Visual Studio](https://docs.microsoft.com/visualstudio/install/install-visual-studio#step-2---download-visual-studio).</span><span class="sxs-lookup"><span data-stu-id="2693a-221">You can see an example of buttons in action in the [Visual Studio docs](https://docs.microsoft.com/visualstudio/install/install-visual-studio#step-2---download-visual-studio).</span></span>

### <a name="step-by-steps"></a><span data-ttu-id="2693a-222">Пошаговые инструкции</span><span class="sxs-lookup"><span data-stu-id="2693a-222">Step-by-steps</span></span>

```markdown
>[!div class="step-by-step"]
> [Pre](../docs/csharp/expression-trees-interpreting.md)
> [Next](../docs/csharp/expression-trees-translating.md)
```

<span data-ttu-id="2693a-223">Пример пошаговых инструкций в действии можно посмотреть в [руководстве по C#](https://docs.microsoft.com/dotnet/csharp/tour-of-csharp/program-structure).</span><span class="sxs-lookup"><span data-stu-id="2693a-223">You can see an example of step-by-steps in action at the [C# Guide](https://docs.microsoft.com/dotnet/csharp/tour-of-csharp/program-structure).</span></span>
