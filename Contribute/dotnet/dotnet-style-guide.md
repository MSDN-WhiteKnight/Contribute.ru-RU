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
# <a name="metadata-and-markdown-template-for-net-docs"></a>Шаблон метаданных и Markdown для документации .NET

Этот шаблон dotnet/docs содержит примеры синтаксиса Markdown и инструкции по указанию метаданных.

При создании файла Markdown скопируйте приведенный шаблон в новый файл, укажите метаданные, как описано ниже, и установите заголовок H1 над названием статьи.

## <a name="metadata"></a>Метаданные

Необходимый блок метаданных приводится в следующем примере блока метаданных:

```markdown
---
title: [ARTICLE TITLE]
description: [usually a summary of your first paragraph. It gets displayed in search results, and can help drive the correct traffic if well written.]
author: [GITHUB USERNAME]
ms.date: [CREATION/UPDATE DATE - mm/dd/yyyy]
---
# The H1 should not be the same as the title, but should describe the article contents
```

- Между двоеточием (:) и значением в элементе метаданных **должен** быть пробел.
- Двоеточия в значении (например, заголовке) прерывают анализ метаданных. В этом случае заключите заголовок в двойные кавычки (например, `title: "Writing .NET Core console apps: An advanced step-by-step guide"`).
- **title**: Отображается в результатах поиска. Заголовок должен совпадать со значением в заголовке H1 и не превышать 60 символов.
- **description**: Описание содержимого статьи. Обычно описание отображается на странице результатов поиска, но не используется для упорядочивания результатов. Длина: 115–145 символов с пробелами.
- **author**: В этом поле необходимо указать **имя пользователя автора на GitHub**.
- **ms.date**: Дата последнего значительного изменения. Измените это значение в существующей статье, если вы пересмотрели и обновили всю статью. Небольшие исправления, вроде опечаток, не считаются обновлением.

К каждой статье прикрепляются другие метаданные, но обычно мы применяем значения большинства метаданных на уровне папки в файле **docfx.json**.

## <a name="basic-markdown-gfm-and-special-characters"></a>Базовый Markdown, GFM и специальные символы

О базовых принципах Markdown, GitHub Flavored Markdown (GFM) и конкретных расширениях OPS можно прочитать в статье [Справочник по Markdown](../markdown-reference.md).

Markdown использует для форматирования специальные символы, например \*, \` и \#. Если вы хотите включить такой символ в свою статью, сделайте одно из двух:

- Поставьте обратную косую черту перед символом, чтобы экранировать его (например, `\*` для \*).
- Используйте [код сущности HTML](http://www.ascii.cl/htmlcodes.htm) для символа (например, `&#42;` для &#42;).

## <a name="file-names"></a>Имена файлов

В именах файлов используются следующие правила:

* Имя может содержать только строчные буквы, цифры и дефисы.
* Должны отсутствовать пробелы и знаки препинания. Для разделения слов и чисел в имени файла следует использовать дефисы.
* Следует использовать конкретные команды действий, такие как develop, buy, build, troubleshoot. Использование слов, оканчивающихся на -ing, не допускается.
* Нельзя использовать служебные (короткие) слова, такие как a, and, the, in, or и т. д.
* Имя должно быть основано на разметке Markdown и иметь расширение файла .md.
* Имя файла должно быть коротким в разумных пределах. Оно будет частью URL-адреса статьи.

## <a name="headings"></a>Заголовки

Используйте выделение прописных букв, как в предложении. Первое слово заголовка всегда должно начинаться с прописной буквы.

## <a name="text-styling"></a>Стиль текста

*Курсив*\
Используйте для обозначения файлов, папок, путей (длинные элементы вынесите в отдельную строку), новых терминов.

**Полужирный шрифт**\
Используйте для элементов пользовательского интерфейса.

`Code`\
Используйте для встроенного кода, ключевых слов языка, имен пакетов NuGet, команд в командной строке, имен таблиц баз данных и столбцов и URL-адресов, которые не должны быть активными.

## <a name="links"></a>Создание ссылок

См. общую статью о [Ссылках](../how-to-write-links.md), чтобы узнать больше о привязках, внутренних ссылках, ссылках на другие документы, включениях кода и внешних ссылках.

Команда по документации .NET использует следующие соглашения:

- В большинстве случаев мы используем относительные ссылки и не рекомендуем использовать `~/` в ссылках, поскольку относительные ссылки разрешаются в источнике на GitHub. Но если мы размещаем ссылку на файл в зависимом репозитории, мы используем символ `~/`, чтобы указать путь. Поскольку файлы в зависимом репозитории располагаются в другом месте на GitHub, ссылки не будут корректно разрешаться при использовании относительных ссылок, как бы они ни были записаны.
- Спецификации языка C# и Visual Basic включены в документацию .NET путем включения источника из репозиториев этих языков. Источники Markdown управляются в репозиториях [csharplang](https://github.com/dotnet/csharplang) и [vblang](https://github.com/dotnet/vblang).

Ссылки на спецификации должны указывать на исходные каталоги, содержащие эти спецификации. Для C# это **~/_csharplang/spec**, а для VB — **~/_vblang/spec**, как в следующем примере:

```markdown
[C# Query Expressions](~/_csharplang/spec/expressions.md#query-expressions)
```

### <a name="links-to-apis"></a>Ссылки на API

Система сборки имеет некоторые расширения, которые позволяют нам ссылаться на API .NET без использования внешних ссылок. Можно выбрать один из следующих вариантов синтаксиса:

1. Автоматическая ссылка: `<xref:UID>` или `<xref:UID?displayProperty=nameWithType>`.

   Параметр запроса `displayProperty` создает полный текст ссылки. По умолчанию в тексте ссылки отображается только имя члена или типа.

2. Ссылка с разметкой Markdown: `[link text](xref:UID)`

   Используется, когда требуется настроить текст ссылки.

Примеры:

- `<xref:System.String>` отображается как [String](https://docs.microsoft.com/dotnet/api/system.string);
- `<xref:System.String?displayProperty=nameWithType>` отображается как [System.String](https://docs.microsoft.com/dotnet/api/system.string);
- `[String class](xref:System.String)` отображается как [String class](https://docs.microsoft.com/dotnet/api/system.string).

Дополнительные сведения об использовании этой нотации см. в разделе об [использовании перекрестных ссылок](https://dotnet.github.io/docfx/tutorial/links_and_cross_references.html#using-cross-reference).

Если идентификатор содержит специальные символы \`, \# или \*, значение UID должно быть закодировано в HTML как `%60`, `%23` и `%2A` соответственно. Иногда круглые скобки тоже кодируются, но это не обязательно.

Примеры:

- System.Threading.Tasks.Task\`1 заменяется на `System.Threading.Tasks.Task%601`;
- System.Exception.\#ctor заменяется на `System.Exception.%23ctor`;
- System.Lazy\`1.\#ctor(System.Threading.LazyThreadSafetyMode) заменяется на `System.Lazy%601.%23ctor%28System.Threading.LazyThreadSafetyMode%29`.

UID для типов, список перегрузки членов или конкретный перегруженный член можно найти в `https://xref.docs.microsoft.com/autocomplete`. Строка запроса `?text=*\<type-member-name>*` определяет тип или элемент, UID которых вы хотите увидеть. Например, `https://xref.docs.microsoft.com/autocomplete?text=string.format` извлекает перегрузки [String.Format](https://docs.microsoft.com/dotnet/api/system.string.format). Инструмент ищет предоставленный параметр запроса `text` в любой части UID. Например, вы можете искать имя члена (ToString), частичное имя члена (ToStri), тип и имя члена (Double.ToString) и т. д.

Если добавить символ \* (или `%2A`) после UID, ссылка будет представлять страницу перегрузки, а не конкретный API. Например, этот символ можно использовать, если требуется создать ссылку на страницу [List\<T>.BinarySearch Method](https://docs.microsoft.com/dotnet/api/system.collections.generic.list-1.binarysearch) обычным способом, а не на конкретную перегрузку, например [List\<T>.BinarySearch(T, IComparer\<T>)](https://docs.microsoft.com/dotnet/api/system.collections.generic.list-1.binarysearch#System_Collections_Generic_List_1_BinarySearch__0_). Также можно использовать \* для ссылки на страницу члена, если этот член не перегружен. Это позволит не включать список параметров в UID.

Чтобы сослаться на конкретную перегрузку метода, включите полное имя типа каждого параметра метода. Например, \<xref:System.DateTime.ToString> ссылается на метод [DateTime.ToString](https://docs.microsoft.com/dotnet/api/system.datetime.tostring#System_DateTime_ToString) без параметров, а \<xref:System.DateTime.ToString(System.String,System.IFormatProvider)> ссылается на метод [DateTime.ToString(String,IFormatProvider)](https://docs.microsoft.com/dotnet/api/system.datetime.tostring#System_DateTime_ToString_System_String_System_IFormatProvider_).

Чтобы сослаться на универсальный тип, например [System.Collections.Generic.List\<T>](https://docs.microsoft.com/dotnet/api/system.collections.generic.list-1), используйте символ \` (`%60`) с указанием числа параметров универсального типа. Например, `<xref:System.Nullable%601>` ссылается на тип [System.Nullable\<T>](https://docs.microsoft.com/dotnet/api/system.nullable-1), а `<xref:System.Func%602>` — на делегат [System.Func\<T,TResult>](https://docs.microsoft.com/dotnet/api/system.func-2).

## <a name="code"></a>Код

Лучший способ включить код — включить фрагменты кода из рабочего примера. Создайте свой пример кода в соответствии с инструкциями из статьи [об участии в составлении документации по .NET](dotnet-contribute.md#contribute-to-samples). Если включать фрагменты кода из полных программ, весь код будет проходить через систему непрерывной интеграции. Но если вам нужно показать что-то, что вызывает ошибки во время компиляции или выполнения, используйте встроенные блоки кода.

Сведения о синтаксисе Markdown для отображения кода в документах см. в статье [Включение кода в документы](../code-in-docs.md).

## <a name="images"></a>Изображения

### <a name="static-image-or-animated-gif"></a>Статическое изображение или анимационный GIF

```markdown
![this is the alt text](../images/Logo_DotNet.png)
```

### <a name="linked-image"></a>Изображения по ссылкам

```markdown
[![alt text for linked image](../images/Logo_DotNet.png)](https://dot.net)
```

## <a name="videos"></a>Видеоролики

Сейчас можно встраивать видео Channel 9 и YouTube со следующим синтаксисом:

### <a name="channel-9"></a>Channel 9

```markdown
> [!VIDEO <channel9_video_link>]
```

Чтобы получить корректный URL-адрес видео, откройте вкладку **Встроить** под видео и скопируйте URL-адрес из элемента `<iframe>`. Например:

```markdown
> [!VIDEO https://channel9.msdn.com/Blogs/dotnet/NET-Core-20-Released/player]
```

### <a name="youtube"></a>YouTube

Чтобы получить корректный URL-адрес видео, щелкните правой кнопкой мыши на видео, выберите **Копировать код внедрения** и скопируйте URL-адрес из элемента `<iframe>`.

```markdown
> [!VIDEO <youtube_video_link>]
```

Например:

```markdown
> [!VIDEO https://www.youtube.com/embed/Q2mMbjw6cLA]
```

## <a name="docsmicrosoft-extensions"></a>Расширения docs.microsoft

docs.microsoft предоставляет несколько дополнительных расширений для GitHub Flavored Markdown.

### <a name="checked-lists"></a>Списки с установленными флажками

К спискам можно применять настраиваемые стили. Можно отображать списки с зелеными флажками.

```markdown
> [!div class="checklist"]
> * How to create a .NET Core app
> * How to add a reference to the Microsoft.XmlSerializer.Generator package
> * How to edit your MyApp.csproj to add dependencies
> * How to add a class and an XmlSerializer
> * How to build and run the application
```

Это выглядит следующим образом:

> [!div class="checklist"]
> * Создание приложения .NET Core
> * Добавление ссылки на пакет Microsoft.XmlSerializer.Generator
> * Редактирование MyApp.csproj для добавления зависимостей
> * Добавление класса как XmlSerializer
> * Создание и запуск приложения

Пример списков с флажками в действии можно посмотреть в [документации по .NET Core](https://docs.microsoft.com/dotnet/core/additional-tools/xml-serializer-generator).

### <a name="buttons"></a>Кнопки

Ссылки на кнопки:

```markdown
> [!div class="button"]
> [button links](dotnet-contribute.md)
```

Это выглядит следующим образом:

> [!div class="button"]
> [ссылки на кнопки](dotnet-contribute.md)

Пример кнопок в действии можно посмотреть в [документации по Visual Studio](https://docs.microsoft.com/visualstudio/install/install-visual-studio#step-2---download-visual-studio).

### <a name="step-by-steps"></a>Пошаговые инструкции

```markdown
>[!div class="step-by-step"]
> [Pre](../docs/csharp/expression-trees-interpreting.md)
> [Next](../docs/csharp/expression-trees-translating.md)
```

Пример пошаговых инструкций в действии можно посмотреть в [руководстве по C#](https://docs.microsoft.com/dotnet/csharp/tour-of-csharp/program-structure).
