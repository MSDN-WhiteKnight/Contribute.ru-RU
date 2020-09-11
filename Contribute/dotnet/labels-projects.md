---
title: 'Стратегия: метки, проекты и вехи'
description: В этой статье объясняется, как метки, проекты и вехи используются в репозитории dotnet/docs.
ms.topic: contributor-guide
ms.prod: non-product-specific
ms.custom: external-contributor-guide
ms.date: 08/06/2020
ms.openlocfilehash: b8e9f2a33f9b4a8025aa36a890bff1017cf132c6
ms.sourcegitcommit: abcc67cb3ec1f635a6374d7c47a4831e3eee9050
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/08/2020
ms.locfileid: "89559270"
---
# <a name="labels-projects-and-milestones-roadmap"></a>Стратегия: метки, проекты и вехи

Команда по разработке документации .NET активно использует [метки GitHub](https://github.com/dotnet/docs/labels) для организации работы. Путем фильтрации по сочетаниям меток мы можем быстро сосредотачиваться на интересующих нас разделах [веб-сайта документации по .NET](https://docs.microsoft.com/dotnet). Например, можно отфильтровать все открытые проблемы с приоритетом `P1`, используя такой запрос: [is:issue is:open label:":books: Area — .NET Architecture Guide"](https://github.com/dotnet/docs/issues?q=is%3Aissue+is%3Aopen+label%3A%22%3Abooks%3A+Area+-+.NET+Architecture+Guide%22).

Мы используем [проекты GitHub](https://github.com/dotnet/docs/projects) для организации спринтов и других целевых ситуаций. Для отслеживания работы мы также используем [вехи GitHub](https://github.com/dotnet/docs/milestones). Проще всего запомнить, что проекты относятся к планированию (проблемы), а вехи — к работе (запросы на вытягивание).

В этой стратегии объясняется, как мы используем эти организационные средства, а также есть ссылки на удобные фильтры по некоторым важным областям.

## <a name="labels"></a>Метки

Если вы впервые участвуете в работе c [dotnet/docs](https://github.com/dotnet/docs), начните со списка проблем [up-for-grabs](https://github.com/dotnet/docs/labels/up-for-grabs). В него включены проблемы с довольно узкой областью. Это отличный путь для первого вклада в работу. В представлении "up-for-grabs" вы можете отфильтровать проблемы по областям и приоритетам. Проблемы, которые хорошо подходят для начинающих, мы обозначаем меткой [good-first-issue](https://github.com/dotnet/docs/labels/good-first-issue), и они помогут вам внести первый небольшой вклад.

Мы используем метки для классификации проблем несколькими способами:

- [руководства по .NET](#find-a-single-net-guide) и [разделы руководства](#search-one-section-of-a-guide);
- [Целевой выпуск](#releases)
- [Приоритет](#priority)

Объединяя метки из каждого набора (руководство, выпуск, приоритет), вы можете создать узкие срезы для поиска проблем, с которыми вы намерены работать.

### <a name="find-a-single-net-guide"></a>Поиск конкретного руководства по .NET

Мы используем метки для каждой из электронных книг по архитектуре и для каждого руководства по .NET.

![:book: руководство на светло-зеленом фоне](./media/labels-projects/guide.png "Префикс для меток руководств по архитектуре")

Электронные книги по архитектуре обозначаются префиксом `:book: guide` и имеют светло-зеленый фон. Это развернутые описания, относящиеся к рекомендуемой архитектуре. Вот пример списка текущих проблем, которые отфильтрованы по каждому из руководств по архитектуре .NET.

- [Веб-приложения ASP.NET Core](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20ASP.NET%20Core%20web%20apps)
- [Blazor](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Blazor)
- [Собственные облачные приложения](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Cloud%20Native)
- [Жизненный цикл Docker](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Docker%20lifecycle)
- [gRPC](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20gRPC)
- [Модернизация с помощью контейнеров Windows](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Modernizing%20w%2F%20Windows%20containers)
- [Микрослужбы .NET](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20.NET%20Microservices)
- [Бессерверные приложения](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Serverless%20apps)

Этот же стиль меток применяется к [рекомендациям по проектированию платформы](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Framework%20Design%20Guidelines). Для этой области используется та же структура меток, но запросы на вытягивание от сообщества здесь не рекомендуются. Эти материалы переиздаются по индивидуальным разрешениям и не должны редактироваться.

![:books: Area на темно-синем фоне](./media/labels-projects/area.png "Префикс для меток области руководства по .NET")

Каждое из руководств по .NET обозначено префиксом `:books: Area` и имеет темно-синий фон. Вот пример списка текущих проблем, которые отфильтрованы по каждому из руководств .NET.

- [Справочник по интерфейсам API](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20API%20Reference)
- [Azure .NET SDK](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20Azure%20.NET%20SDk);
- [Руководство по языку C#](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20C%23%20Guide)
- [Руководство по классическим приложениям](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20Desktop%20Guide)
- [Руководство по языку F#](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20F%23%20Guide)
- [Руководство по ML.NET](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20ML.NET%20Guide)
- [Руководство по архитектуре .NET](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20Architecture%20Guide) — может быть удалено
- [Руководство по .NET Core](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20Core%20Guide)
- [Руководство по .NET для Apache Spark](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20for%20Apache%20Spark%20Guide)
- [Руководство по .NET Framework](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20Framework%20Guide)
- [Руководство по .NET](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20Guide)
- [Справочник по API Roslyn](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20Roslyn%20API%20Reference) — может быть удален.
- [Руководство по Visual Basic](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20Visual%20Basic%20Guide)

#### <a name="search-one-section-of-a-guide"></a>Поиск по одному разделу руководства

![:card_file_box: Area на умеренно синем фоне](./media/labels-projects/technology.png "Префикс для меток вложенных областей руководства по .NET")

Руководства по .NET достаточно большие, а эти метки позволяют дополнительно ограничить область поиска конкретным разделом руководства. Каждая из вложенных областей руководств по .NET обозначено префиксом `:card_file_box: Technology` и имеет светло-синий фон. Многие из этих меток применяются к нескольким руководствам, а другие — только к одному из них. Применив фильтр по области, добавьте одну из этих меток, чтобы ограничить область поиска проблем.

- AppCompat
- Асинхронная задача
- Дополнительные возможности C#
- Компилятор C#
- Основы C#
- Начало работы с C#
- Справочник по языку C#
- Безопасность значений NULL в C#
- Новые возможности C#
- CLI
- Доступ к данным
- Docker
- Установщики
- LINQ
- NCL
- .NET Standard
- API Roslyn
- Безопасность
- WCF
- WF
- WIF
- WinForms
- WPF

### <a name="releases"></a>Выпуски

![:checkered_flag: Release: на темно-желтом фоне](./media/labels-projects/release.png "Префикс для меток выпуска")

Проблемы, помеченные для конкретного выпуска, обозначаются префиксом `:checkered_flag: Release:` и отображаются на темно-желтом фоне.

- .NET Core 2.2
- .NET Core 3.0
- .NET Framework 4.8
- .NET 5

### <a name="priority"></a>Приоритет

Метки приоритета содержат символ `P`, за которым следует одна цифра. Чем меньше число, тем выше приоритет.

- P0 — проблемы или запросы на вытягивание с критическим приоритетом;
- Р1 — высокий приоритет;
- Р2 — средний приоритет;
- Р3 — низкий приоритет.

### <a name="what-about-the-other-labels"></a>Другие метки

Группы по работе над содержимым используют много других меток для управления разными классификациями проблем. Если вы не входите в такую группу, остальные метки можно смело игнорировать.

## <a name="projects"></a>Проекты

Проекты предназначены для планирования. При этом приоритетная работа выполняется автоматически с использованием канбан-доски. Проекты должны содержать только проблемы GitHub, но _не_ запросы на вытягивание. Проекты отличаются от вех тем, что вехи содержат только запросы на вытягивание.

Мы используем проекты двумя способами.

- Типы проектов `Month YYYY`: это канбан-доски для рабочих планов на каждый месяц.
  - Примеры: [июль 2020 г.](https://github.com/dotnet/docs/projects/103), [август 2020 г.](https://github.com/dotnet/docs/projects/117) и т. д.
- Долговременные ситуации: используются для упорядочения задач, работа над которыми будет продолжаться несколько месяцев.
  - Примеры: [.NET 5 Wave — Reorganization](https://github.com/dotnet/docs/projects/105), [.NET Languages (.NET 5 Wave) ](https://github.com/dotnet/docs/projects/106) и т. д.

## <a name="milestones"></a>Вехи

Вехи обычно следуют соглашению об именовании для проектов `Month YYYY`, но они отличаются от проектов. Вехи используются для отслеживания завершенной работы. Вехи _не_ должны содержать проблемы (возможная работа), а только запросы на вытягивание. Текущая веха автоматически применяется к новым запросам на вытягивание.
