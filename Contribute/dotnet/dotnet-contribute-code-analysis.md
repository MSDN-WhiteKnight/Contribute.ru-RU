---
title: Отправка документации по правилам анализа кода .NET в репозиторий документации .NET
description: В этой статье показано, как писать статьи и создавать примеры кода для правил анализа кода .NET в репозиториях документации по .NET.
author: mavasani
ms.author: mavasani
ms.topic: contributor-guide
ms.prod: non-product-specific
ms.custom: external-contributor-guide
ms.date: 10/09/2020
ms.openlocfilehash: 27ae1a31c55c41aa1c97bf1f88dbf28bec35a80a
ms.sourcegitcommit: f1535713b66ff9b840f1138583746bc2bf182b4f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/12/2020
ms.locfileid: "91957069"
---
# <a name="contribute-docs-for-net-code-analysis-rules-to-the-net-docs-repository"></a>Отправка документации по правилам анализа кода .NET в репозиторий документации .NET

Анализаторы .NET Compiler Platform (Roslyn) проверяют качество кода C# или Visual Basic и выявляют в нем проблемы. Начиная с .NET 5.0 эти анализаторы входят в состав [пакета SDK .NET](/dotnet/fundamentals/code-analysis/overview).

- [Анализ качества кода (правила CAxxxx)](/dotnet/fundamentals/code-analysis/overview#code-quality-analysis):
  - Реализация размещена [здесь](https://github.com/dotnet/roslyn-analyzers/tree/master/src/NetAnalyzers) в репозитории `dotnet/roslyn-analyzers`.
  - Документация размещена [здесь](https://github.com/dotnet/docs/blob/master/docs/fundamentals/code-analysis/quality-rules) в репозитории `dotnet/docs`. См. раздел [Отправка документов для правил CAxxxx](#contribute-docs-for-caxxxx-rules).
- [Анализ стиля кода (правила IDExxxx)](/dotnet/fundamentals/code-analysis/overview#code-style-analysis):
  - Реализация размещена [здесь](https://github.com/dotnet/roslyn/tree/master/src/Analyzers) в репозитории `dotnet/roslyn`.
  - Документация размещена [здесь](https://github.com/dotnet/docs/blob/master/docs/fundamentals/code-analysis/style-rules) в репозитории `dotnet/docs`. См. раздел [Отправка документов для правил IDExxxx](#contribute-docs-for-idexxxx-rules).

## <a name="contribute-docs-for-caxxxx-rules"></a>Отправка документов для правил CAxxxx

Выполните следующие шаги, чтобы отправить документацию для правил анализа качества кода в репозиторий [dotnet/docs](https://github.com/dotnet/docs):

1. Определите `Rule ID` и `Category`. Убедитесь, что вам известны идентификатор правила CAxxxx и категория правила, для которого создается документ. Для этого либо анализатор CA должен быть включен в репозиторий [dotnet/roslyn-analyzers](https://github.com/dotnet/roslyn-analyzers), либо у вас должен быть открытый запрос на вытягивание с утвержденными значениями идентификатора и категории, присвоенными этому правилу.
2. Добавьте документацию для правила:
   1. Клонируйте существующий файл правила CA из папки [root](https://github.com/dotnet/docs/blob/master/docs/fundamentals/code-analysis/quality-rules), например `ca1000.md`, и переименуйте его.
   2. Обновите содержимое этого файла соответствующим образом.
3. Добавьте запись для этого файла в следующие таблицы:
   - В файл [таблицы содержимого](https://github.com/dotnet/docs/blob/master/docs/fundamentals/toc.yml) в списке для категории правила. Например если правило CA имеет категорию `Performance`, выполните в этом файле поиск по термину `- name: Performance rules` и добавьте запись в список. Если ничего не найдено, добавьте новую категорию как `- name: Code quality rules`.
   - В файл [индекса правил высшего уровня](https://github.com/dotnet/docs/blob/master/docs/fundamentals/code-analysis/quality-rules/index.md).
   - В файл индекса правил на основе `category`:
     1. Найдите файл индекса на основе категорий в папке [root](https://github.com/dotnet/docs/blob/master/docs/fundamentals/code-analysis/quality-rules). Например, для правила CA с категорией `Performance` этот файл имеет имя `performance-warnings.md`. Если ничего не найдено, создайте новый файл индекса на основе категории путем клонирования любого существующего.
     2. Добавьте в этот файл запись для нужного идентификатора правила.

> [!TIP]
> Выполните в репозитории `dotnet/docs` поиск по известному идентификатору существующего правила CA, чтобы найти все возможные места для обновления сведений о нем. Пример см. в разделе <https://github.com/dotnet/docs/search?q=CA2000>.

## <a name="contribute-docs-for-idexxxx-rules"></a>Отправка документации для правил IDExxxx

Выполните следующие шаги, чтобы отправить документацию для правил анализа стиля кода в репозиторий [dotnet/docs](https://github.com/dotnet/docs):

1. Определите `Rule ID` и варианты стиля кода, если они применяются: Убедитесь, что вам известны идентификатор правила IDExxxx и варианты стиля кода для документируемого правила. Для этого либо анализатор IDE должен быть включен в репозиторий [dotnet/roslyn](https://github.com/dotnet/roslyn), либо у вас должен быть открытый запрос на вытягивание с утвержденными значениями идентификатора и вариантов стиля кода, присвоенными этому правилу.
2. Определите `subcategory` для правила: Все правила IDE имеют категорию `Style`. Выясните подкатегорию правила, изучив вводный раздел, посвященный [правилам стиля кода](/dotnet/fundamentals/code-analysis/style-rules/index). Большинство правил стиля кода IDE относятся к подкатегории `Language`.
3. Определите `preference group` для правила: Определите `preference group` для правила, изучив заголовки предпочтений, указанные [здесь](/dotnet/fundamentals/code-analysis/style-rules/language-rules#net-style-rules).
   - Если с правилом сопоставлены известные варианты стиля кода, группа предпочтений будет соответствовать значению `OptionGroup`, указанному в декларации варианта стиля кода.
   - В противном случае нужно проверить, относится ли это правило к существующей группе предпочтений или для него нужно создать новую группу.
4. Добавьте документацию для правила:
   1. Клонируйте существующий файл правила IDE из папки [root](https://github.com/dotnet/docs/blob/master/docs/fundamentals/code-analysis/style-rules), например `ide0011.md`, и переименуйте его.
   2. Обновите содержимое этого файла соответствующим образом.
5. Добавьте запись для этого правила IDE и (или) вариантов стиля кода в следующие таблицы:
   - В файл [таблицы содержимого](https://github.com/dotnet/docs/blob/master/docs/fundamentals/toc.yml) в список, соответствующий подкатегории и предпочтениям правила. Например, для правила стиля кода IDE с подкатегорией `Language` и группой `Modifier preferences` выполните поиск по термину `- name: Language rules` и дочернему узлу `- name: Modifier preferences` в указанном файле, а затем добавьте запись в найденный список. Если ничего не найдено, создайте новый список как `- name: Code style rules`.
   - В файл [индекса на основе вариантов стиля кода](https://github.com/dotnet/docs/blob/master/docs/fundamentals/code-analysis/style-rules/language-rules.md).
   - В файл [индекса на основе идентификаторов правил](https://github.com/dotnet/docs/blob/master/docs/fundamentals/code-analysis/style-rules/index.md).
   - В файл индекса правил на основе `preferences group`:
     1. Найдите файл индекса на основе групп предпочтений в папке [root](https://github.com/dotnet/docs/blob/master/docs/fundamentals/code-analysis/style-rules). Например, для правила IDE с предпочтениями `Modifier preferences` этот файл имеет имя `modifier-preferences.md`. Если ничего не найдено, создайте новый файл индекса на основе групп предпочтений путем клонирования существующего.
     2. Добавьте в этот файл запись для нужного идентификатора правила.

> [!TIP]
> Выполните в репозитории `dotnet/docs` поиск по известному идентификатору существующего правила IDE и (или) вариантов стиля кода, чтобы найти все возможные места для обновления сведений о нем. Например, см. класс <https://github.com/dotnet/docs/search?q=IDE0011> и тип <https://github.com/dotnet/docs/search?q=csharp_prefer_braces>.

## <a name="see-also"></a>См. также раздел

- [Участие в разработке репозиториев документации по .NET](dotnet-contribute.md)
