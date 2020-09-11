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
# <a name="labels-projects-and-milestones-roadmap"></a><span data-ttu-id="b4e97-103">Стратегия: метки, проекты и вехи</span><span class="sxs-lookup"><span data-stu-id="b4e97-103">Labels, projects, and milestones roadmap</span></span>

<span data-ttu-id="b4e97-104">Команда по разработке документации .NET активно использует [метки GitHub](https://github.com/dotnet/docs/labels) для организации работы.</span><span class="sxs-lookup"><span data-stu-id="b4e97-104">The .NET docs team makes extensive use of [GitHub labels](https://github.com/dotnet/docs/labels) to organize our work.</span></span> <span data-ttu-id="b4e97-105">Путем фильтрации по сочетаниям меток мы можем быстро сосредотачиваться на интересующих нас разделах [веб-сайта документации по .NET](https://docs.microsoft.com/dotnet).</span><span class="sxs-lookup"><span data-stu-id="b4e97-105">By filtering on combinations of labels, we can quickly focus on sections of interest on the [.NET docs website](https://docs.microsoft.com/dotnet).</span></span> <span data-ttu-id="b4e97-106">Например, можно отфильтровать все открытые проблемы с приоритетом `P1`, используя такой запрос: [is:issue is:open label:":books: Area — .NET Architecture Guide"](https://github.com/dotnet/docs/issues?q=is%3Aissue+is%3Aopen+label%3A%22%3Abooks%3A+Area+-+.NET+Architecture+Guide%22).</span><span class="sxs-lookup"><span data-stu-id="b4e97-106">For example, we could filter to all of the open priority one `P1` issues with a query to [is:issue is:open label:":books: Area - .NET Architecture Guide"](https://github.com/dotnet/docs/issues?q=is%3Aissue+is%3Aopen+label%3A%22%3Abooks%3A+Area+-+.NET+Architecture+Guide%22).</span></span>

<span data-ttu-id="b4e97-107">Мы используем [проекты GitHub](https://github.com/dotnet/docs/projects) для организации спринтов и других целевых ситуаций.</span><span class="sxs-lookup"><span data-stu-id="b4e97-107">We use [GitHub projects](https://github.com/dotnet/docs/projects) to organize sprints and other goal-oriented epics.</span></span> <span data-ttu-id="b4e97-108">Для отслеживания работы мы также используем [вехи GitHub](https://github.com/dotnet/docs/milestones).</span><span class="sxs-lookup"><span data-stu-id="b4e97-108">We also use [GitHub milestones](https://github.com/dotnet/docs/milestones) to track work.</span></span> <span data-ttu-id="b4e97-109">Проще всего запомнить, что проекты относятся к планированию (проблемы), а вехи — к работе (запросы на вытягивание).</span><span class="sxs-lookup"><span data-stu-id="b4e97-109">It is best to think of projects for planning (issues), and milestones for work (pull requests).</span></span>

<span data-ttu-id="b4e97-110">В этой стратегии объясняется, как мы используем эти организационные средства, а также есть ссылки на удобные фильтры по некоторым важным областям.</span><span class="sxs-lookup"><span data-stu-id="b4e97-110">This roadmap explains how we use these organizational tools and has links to handy filters we use to find areas of interest.</span></span>

## <a name="labels"></a><span data-ttu-id="b4e97-111">Метки</span><span class="sxs-lookup"><span data-stu-id="b4e97-111">Labels</span></span>

<span data-ttu-id="b4e97-112">Если вы впервые участвуете в работе c [dotnet/docs](https://github.com/dotnet/docs), начните со списка проблем [up-for-grabs](https://github.com/dotnet/docs/labels/up-for-grabs).</span><span class="sxs-lookup"><span data-stu-id="b4e97-112">If this is your first experience contributing to [dotnet/docs](https://github.com/dotnet/docs), start with the [up-for-grabs](https://github.com/dotnet/docs/labels/up-for-grabs) issues.</span></span> <span data-ttu-id="b4e97-113">В него включены проблемы с довольно узкой областью.</span><span class="sxs-lookup"><span data-stu-id="b4e97-113">These are issues that have a more focused scope.</span></span> <span data-ttu-id="b4e97-114">Это отличный путь для первого вклада в работу.</span><span class="sxs-lookup"><span data-stu-id="b4e97-114">They are a great way to make your first contribution.</span></span> <span data-ttu-id="b4e97-115">В представлении "up-for-grabs" вы можете отфильтровать проблемы по областям и приоритетам.</span><span class="sxs-lookup"><span data-stu-id="b4e97-115">From the up-for-grabs view, you can further filter issues based on areas and priority.</span></span> <span data-ttu-id="b4e97-116">Проблемы, которые хорошо подходят для начинающих, мы обозначаем меткой [good-first-issue](https://github.com/dotnet/docs/labels/good-first-issue), и они помогут вам внести первый небольшой вклад.</span><span class="sxs-lookup"><span data-stu-id="b4e97-116">We've identified good issues for beginners with the [good-first-issue](https://github.com/dotnet/docs/labels/good-first-issue) if you want to try a smaller first contribution.</span></span>

<span data-ttu-id="b4e97-117">Мы используем метки для классификации проблем несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="b4e97-117">We use labels to classify issues in many different ways:</span></span>

- <span data-ttu-id="b4e97-118">[руководства по .NET](#find-a-single-net-guide) и [разделы руководства](#search-one-section-of-a-guide);</span><span class="sxs-lookup"><span data-stu-id="b4e97-118">[.NET Guides](#find-a-single-net-guide) and [sections of a guide](#search-one-section-of-a-guide).</span></span>
- [<span data-ttu-id="b4e97-119">Целевой выпуск</span><span class="sxs-lookup"><span data-stu-id="b4e97-119">Target release</span></span>](#releases)
- [<span data-ttu-id="b4e97-120">Приоритет</span><span class="sxs-lookup"><span data-stu-id="b4e97-120">Priority</span></span>](#priority)

<span data-ttu-id="b4e97-121">Объединяя метки из каждого набора (руководство, выпуск, приоритет), вы можете создать узкие срезы для поиска проблем, с которыми вы намерены работать.</span><span class="sxs-lookup"><span data-stu-id="b4e97-121">You can combine a label from each set (guide, release, priority) to create a narrow focus to find issues you want to work on.</span></span>

### <a name="find-a-single-net-guide"></a><span data-ttu-id="b4e97-122">Поиск конкретного руководства по .NET</span><span class="sxs-lookup"><span data-stu-id="b4e97-122">Find a single .NET guide</span></span>

<span data-ttu-id="b4e97-123">Мы используем метки для каждой из электронных книг по архитектуре и для каждого руководства по .NET.</span><span class="sxs-lookup"><span data-stu-id="b4e97-123">We use labels for each of the architecture e-books and for each .NET Guide.</span></span>

<span data-ttu-id="b4e97-124">![:book: руководство на светло-зеленом фоне](./media/labels-projects/guide.png "Префикс для меток руководств по архитектуре")</span><span class="sxs-lookup"><span data-stu-id="b4e97-124">![:book: guide on light green background](./media/labels-projects/guide.png "Prefix for architecture guide labels")</span></span>

<span data-ttu-id="b4e97-125">Электронные книги по архитектуре обозначаются префиксом `:book: guide` и имеют светло-зеленый фон.</span><span class="sxs-lookup"><span data-stu-id="b4e97-125">Architecture e-books are noted with the `:book: guide` prefix and have a light green background.</span></span> <span data-ttu-id="b4e97-126">Это развернутые описания, относящиеся к рекомендуемой архитектуре.</span><span class="sxs-lookup"><span data-stu-id="b4e97-126">These are the long-form areas that cover recommended architecture.</span></span> <span data-ttu-id="b4e97-127">Вот пример списка текущих проблем, которые отфильтрованы по каждому из руководств по архитектуре .NET.</span><span class="sxs-lookup"><span data-stu-id="b4e97-127">Here are current issues filtered for each of the .NET architecture guides.</span></span>

- [<span data-ttu-id="b4e97-128">Веб-приложения ASP.NET Core</span><span class="sxs-lookup"><span data-stu-id="b4e97-128">ASP.NET Core web apps</span></span>](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20ASP.NET%20Core%20web%20apps)
- [<span data-ttu-id="b4e97-129">Blazor</span><span class="sxs-lookup"><span data-stu-id="b4e97-129">Blazor</span></span>](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Blazor)
- [<span data-ttu-id="b4e97-130">Собственные облачные приложения</span><span class="sxs-lookup"><span data-stu-id="b4e97-130">Cloud Native</span></span>](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Cloud%20Native)
- [<span data-ttu-id="b4e97-131">Жизненный цикл Docker</span><span class="sxs-lookup"><span data-stu-id="b4e97-131">Docker lifecycle</span></span>](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Docker%20lifecycle)
- [<span data-ttu-id="b4e97-132">gRPC</span><span class="sxs-lookup"><span data-stu-id="b4e97-132">gRPC</span></span>](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20gRPC)
- [<span data-ttu-id="b4e97-133">Модернизация с помощью контейнеров Windows</span><span class="sxs-lookup"><span data-stu-id="b4e97-133">Modernizing w/ Windows containers</span></span>](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Modernizing%20w%2F%20Windows%20containers)
- [<span data-ttu-id="b4e97-134">Микрослужбы .NET</span><span class="sxs-lookup"><span data-stu-id="b4e97-134">.NET Microservices</span></span>](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20.NET%20Microservices)
- [<span data-ttu-id="b4e97-135">Бессерверные приложения</span><span class="sxs-lookup"><span data-stu-id="b4e97-135">Serverless apps</span></span>](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Serverless%20apps)

<span data-ttu-id="b4e97-136">Этот же стиль меток применяется к [рекомендациям по проектированию платформы](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Framework%20Design%20Guidelines).</span><span class="sxs-lookup"><span data-stu-id="b4e97-136">This label style is also applied to the [Framework design guidelines](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Framework%20Design%20Guidelines).</span></span> <span data-ttu-id="b4e97-137">Для этой области используется та же структура меток, но запросы на вытягивание от сообщества здесь не рекомендуются.</span><span class="sxs-lookup"><span data-stu-id="b4e97-137">This area has the same label design, but community PRs are discouraged.</span></span> <span data-ttu-id="b4e97-138">Эти материалы переиздаются по индивидуальным разрешениям и не должны редактироваться.</span><span class="sxs-lookup"><span data-stu-id="b4e97-138">This is material reprinted with permission and should not be edited.</span></span>

<span data-ttu-id="b4e97-139">![:books: Area на темно-синем фоне](./media/labels-projects/area.png "Префикс для меток области руководства по .NET")</span><span class="sxs-lookup"><span data-stu-id="b4e97-139">![:books: Area on dark blue background](./media/labels-projects/area.png "Prefix for .NET Guide area labels")</span></span>

<span data-ttu-id="b4e97-140">Каждое из руководств по .NET обозначено префиксом `:books: Area` и имеет темно-синий фон.</span><span class="sxs-lookup"><span data-stu-id="b4e97-140">Each .NET Guide is noted with the `:books: Area` prefix and has a dark blue background.</span></span> <span data-ttu-id="b4e97-141">Вот пример списка текущих проблем, которые отфильтрованы по каждому из руководств .NET.</span><span class="sxs-lookup"><span data-stu-id="b4e97-141">Here are current issues filtered for each of the .NET guides.</span></span>

- [<span data-ttu-id="b4e97-142">Справочник по интерфейсам API</span><span class="sxs-lookup"><span data-stu-id="b4e97-142">API Reference</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20API%20Reference)
- <span data-ttu-id="b4e97-143">[Azure .NET SDK](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20Azure%20.NET%20SDk);</span><span class="sxs-lookup"><span data-stu-id="b4e97-143">[Azure .NET SDK](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20Azure%20.NET%20SDk)</span></span>
- [<span data-ttu-id="b4e97-144">Руководство по языку C#</span><span class="sxs-lookup"><span data-stu-id="b4e97-144">C# Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20C%23%20Guide)
- [<span data-ttu-id="b4e97-145">Руководство по классическим приложениям</span><span class="sxs-lookup"><span data-stu-id="b4e97-145">Desktop Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20Desktop%20Guide)
- [<span data-ttu-id="b4e97-146">Руководство по языку F#</span><span class="sxs-lookup"><span data-stu-id="b4e97-146">F# Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20F%23%20Guide)
- [<span data-ttu-id="b4e97-147">Руководство по ML.NET</span><span class="sxs-lookup"><span data-stu-id="b4e97-147">ML.NET Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20ML.NET%20Guide)
- <span data-ttu-id="b4e97-148">[Руководство по архитектуре .NET](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20Architecture%20Guide) — может быть удалено</span><span class="sxs-lookup"><span data-stu-id="b4e97-148">[.NET Architecture Guide](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20Architecture%20Guide) - Could be removed</span></span>
- [<span data-ttu-id="b4e97-149">Руководство по .NET Core</span><span class="sxs-lookup"><span data-stu-id="b4e97-149">.NET Core Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20Core%20Guide)
- [<span data-ttu-id="b4e97-150">Руководство по .NET для Apache Spark</span><span class="sxs-lookup"><span data-stu-id="b4e97-150">.NET for Apache Spark Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20for%20Apache%20Spark%20Guide)
- [<span data-ttu-id="b4e97-151">Руководство по .NET Framework</span><span class="sxs-lookup"><span data-stu-id="b4e97-151">.NET Framework Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20Framework%20Guide)
- [<span data-ttu-id="b4e97-152">Руководство по .NET</span><span class="sxs-lookup"><span data-stu-id="b4e97-152">.NET Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20Guide)
- <span data-ttu-id="b4e97-153">[Справочник по API Roslyn](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20Roslyn%20API%20Reference) — может быть удален.</span><span class="sxs-lookup"><span data-stu-id="b4e97-153">[Roslyn API Reference](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20Roslyn%20API%20Reference) - could be removed.</span></span>
- [<span data-ttu-id="b4e97-154">Руководство по Visual Basic</span><span class="sxs-lookup"><span data-stu-id="b4e97-154">Visual Basic Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20Visual%20Basic%20Guide)

#### <a name="search-one-section-of-a-guide"></a><span data-ttu-id="b4e97-155">Поиск по одному разделу руководства</span><span class="sxs-lookup"><span data-stu-id="b4e97-155">Search one section of a guide</span></span>

<span data-ttu-id="b4e97-156">![:card_file_box: Area на умеренно синем фоне](./media/labels-projects/technology.png "Префикс для меток вложенных областей руководства по .NET")</span><span class="sxs-lookup"><span data-stu-id="b4e97-156">![:card_file_box: Area on medium blue background](./media/labels-projects/technology.png "Prefix for .NET Guide sub-area labels")</span></span>

<span data-ttu-id="b4e97-157">Руководства по .NET достаточно большие, а эти метки позволяют дополнительно ограничить область поиска конкретным разделом руководства.</span><span class="sxs-lookup"><span data-stu-id="b4e97-157">The .NET guides are large, so these labels further limit the scope by a section of a guide.</span></span> <span data-ttu-id="b4e97-158">Каждая из вложенных областей руководств по .NET обозначено префиксом `:card_file_box: Technology` и имеет светло-синий фон.</span><span class="sxs-lookup"><span data-stu-id="b4e97-158">Each .NET Guide subarea is noted with the `:card_file_box: Technology` prefix and has a medium blue background.</span></span> <span data-ttu-id="b4e97-159">Многие из этих меток применяются к нескольким руководствам, а другие — только к одному из них.</span><span class="sxs-lookup"><span data-stu-id="b4e97-159">Many of these labels apply to multiple guides, while others are in only one guide.</span></span> <span data-ttu-id="b4e97-160">Применив фильтр по области, добавьте одну из этих меток, чтобы ограничить область поиска проблем.</span><span class="sxs-lookup"><span data-stu-id="b4e97-160">After filtering on an area, add one of these labels to further limit the scope of issues.</span></span>

- <span data-ttu-id="b4e97-161">AppCompat</span><span class="sxs-lookup"><span data-stu-id="b4e97-161">AppCompat</span></span>
- <span data-ttu-id="b4e97-162">Асинхронная задача</span><span class="sxs-lookup"><span data-stu-id="b4e97-162">Async Task</span></span>
- <span data-ttu-id="b4e97-163">Дополнительные возможности C#</span><span class="sxs-lookup"><span data-stu-id="b4e97-163">C# Advanced concepts</span></span>
- <span data-ttu-id="b4e97-164">Компилятор C#</span><span class="sxs-lookup"><span data-stu-id="b4e97-164">C# compiler</span></span>
- <span data-ttu-id="b4e97-165">Основы C#</span><span class="sxs-lookup"><span data-stu-id="b4e97-165">C# Fundamentals</span></span>
- <span data-ttu-id="b4e97-166">Начало работы с C#</span><span class="sxs-lookup"><span data-stu-id="b4e97-166">C# Get Started</span></span>
- <span data-ttu-id="b4e97-167">Справочник по языку C#</span><span class="sxs-lookup"><span data-stu-id="b4e97-167">C# Language Reference</span></span>
- <span data-ttu-id="b4e97-168">Безопасность значений NULL в C#</span><span class="sxs-lookup"><span data-stu-id="b4e97-168">C# Null safety</span></span>
- <span data-ttu-id="b4e97-169">Новые возможности C#</span><span class="sxs-lookup"><span data-stu-id="b4e97-169">C# What's new</span></span>
- <span data-ttu-id="b4e97-170">CLI</span><span class="sxs-lookup"><span data-stu-id="b4e97-170">CLI</span></span>
- <span data-ttu-id="b4e97-171">Доступ к данным</span><span class="sxs-lookup"><span data-stu-id="b4e97-171">Data Access</span></span>
- <span data-ttu-id="b4e97-172">Docker</span><span class="sxs-lookup"><span data-stu-id="b4e97-172">Docker</span></span>
- <span data-ttu-id="b4e97-173">Установщики</span><span class="sxs-lookup"><span data-stu-id="b4e97-173">Installers</span></span>
- <span data-ttu-id="b4e97-174">LINQ</span><span class="sxs-lookup"><span data-stu-id="b4e97-174">LINQ</span></span>
- <span data-ttu-id="b4e97-175">NCL</span><span class="sxs-lookup"><span data-stu-id="b4e97-175">NCL</span></span>
- <span data-ttu-id="b4e97-176">.NET Standard</span><span class="sxs-lookup"><span data-stu-id="b4e97-176">.NET Standard</span></span>
- <span data-ttu-id="b4e97-177">API Roslyn</span><span class="sxs-lookup"><span data-stu-id="b4e97-177">Roslyn APIs</span></span>
- <span data-ttu-id="b4e97-178">Безопасность</span><span class="sxs-lookup"><span data-stu-id="b4e97-178">Security</span></span>
- <span data-ttu-id="b4e97-179">WCF</span><span class="sxs-lookup"><span data-stu-id="b4e97-179">WCF</span></span>
- <span data-ttu-id="b4e97-180">WF</span><span class="sxs-lookup"><span data-stu-id="b4e97-180">WF</span></span>
- <span data-ttu-id="b4e97-181">WIF</span><span class="sxs-lookup"><span data-stu-id="b4e97-181">WIF</span></span>
- <span data-ttu-id="b4e97-182">WinForms</span><span class="sxs-lookup"><span data-stu-id="b4e97-182">WinForms</span></span>
- <span data-ttu-id="b4e97-183">WPF</span><span class="sxs-lookup"><span data-stu-id="b4e97-183">WPF</span></span>

### <a name="releases"></a><span data-ttu-id="b4e97-184">Выпуски</span><span class="sxs-lookup"><span data-stu-id="b4e97-184">Releases</span></span>

<span data-ttu-id="b4e97-185">![:checkered_flag: Release: на темно-желтом фоне](./media/labels-projects/release.png "Префикс для меток выпуска")</span><span class="sxs-lookup"><span data-stu-id="b4e97-185">![:checkered_flag: Release: on dark yellow](./media/labels-projects/release.png "Prefix for release labels")</span></span>

<span data-ttu-id="b4e97-186">Проблемы, помеченные для конкретного выпуска, обозначаются префиксом `:checkered_flag: Release:` и отображаются на темно-желтом фоне.</span><span class="sxs-lookup"><span data-stu-id="b4e97-186">Issues tagged for a specific release are noted with the `:checkered_flag: Release:` prefix and have a dark yellow background.</span></span>

- <span data-ttu-id="b4e97-187">.NET Core 2.2</span><span class="sxs-lookup"><span data-stu-id="b4e97-187">.NET Core 2.2</span></span>
- <span data-ttu-id="b4e97-188">.NET Core 3.0</span><span class="sxs-lookup"><span data-stu-id="b4e97-188">.NET Core 3.0</span></span>
- <span data-ttu-id="b4e97-189">.NET Framework 4.8</span><span class="sxs-lookup"><span data-stu-id="b4e97-189">.NET Framework 4.8</span></span>
- <span data-ttu-id="b4e97-190">.NET 5</span><span class="sxs-lookup"><span data-stu-id="b4e97-190">.NET 5</span></span>

### <a name="priority"></a><span data-ttu-id="b4e97-191">Приоритет</span><span class="sxs-lookup"><span data-stu-id="b4e97-191">Priority</span></span>

<span data-ttu-id="b4e97-192">Метки приоритета содержат символ `P`, за которым следует одна цифра.</span><span class="sxs-lookup"><span data-stu-id="b4e97-192">Priority labels are all `P` followed by a single digit.</span></span> <span data-ttu-id="b4e97-193">Чем меньше число, тем выше приоритет.</span><span class="sxs-lookup"><span data-stu-id="b4e97-193">Lower numbers are higher priority:</span></span>

- <span data-ttu-id="b4e97-194">P0 — проблемы или запросы на вытягивание с критическим приоритетом;</span><span class="sxs-lookup"><span data-stu-id="b4e97-194">P0 - Indicates issues or PRs that are critical priority</span></span>
- <span data-ttu-id="b4e97-195">Р1 — высокий приоритет;</span><span class="sxs-lookup"><span data-stu-id="b4e97-195">P1 - High priority</span></span>
- <span data-ttu-id="b4e97-196">Р2 — средний приоритет;</span><span class="sxs-lookup"><span data-stu-id="b4e97-196">P2 - Medium priority</span></span>
- <span data-ttu-id="b4e97-197">Р3 — низкий приоритет.</span><span class="sxs-lookup"><span data-stu-id="b4e97-197">P3 - Low priority</span></span>

### <a name="what-about-the-other-labels"></a><span data-ttu-id="b4e97-198">Другие метки</span><span class="sxs-lookup"><span data-stu-id="b4e97-198">What about the other labels</span></span>

<span data-ttu-id="b4e97-199">Группы по работе над содержимым используют много других меток для управления разными классификациями проблем.</span><span class="sxs-lookup"><span data-stu-id="b4e97-199">There are many other labels used by the content teams to manage different classifications of issues.</span></span> <span data-ttu-id="b4e97-200">Если вы не входите в такую группу, остальные метки можно смело игнорировать.</span><span class="sxs-lookup"><span data-stu-id="b4e97-200">If you're not on the content team, you can ignore these other labels.</span></span>

## <a name="projects"></a><span data-ttu-id="b4e97-201">Проекты</span><span class="sxs-lookup"><span data-stu-id="b4e97-201">Projects</span></span>

<span data-ttu-id="b4e97-202">Проекты предназначены для планирования. При этом приоритетная работа выполняется автоматически с использованием канбан-доски.</span><span class="sxs-lookup"><span data-stu-id="b4e97-202">Projects are intended for planning purposes, where prioritized work is automated through a Kanban board.</span></span> <span data-ttu-id="b4e97-203">Проекты должны содержать только проблемы GitHub, но _не_ запросы на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="b4e97-203">Projects should only ever contain GitHub issues, _not_ pull requests.</span></span> <span data-ttu-id="b4e97-204">Проекты отличаются от вех тем, что вехи содержат только запросы на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="b4e97-204">Projects differ from milestones, in that milestones only contain pull requests.</span></span>

<span data-ttu-id="b4e97-205">Мы используем проекты двумя способами.</span><span class="sxs-lookup"><span data-stu-id="b4e97-205">We use projects in two ways:</span></span>

- <span data-ttu-id="b4e97-206">Типы проектов `Month YYYY`: это канбан-доски для рабочих планов на каждый месяц.</span><span class="sxs-lookup"><span data-stu-id="b4e97-206">`Month YYYY` project types: These are Kanban boards for each month's working plan.</span></span>
  - <span data-ttu-id="b4e97-207">Примеры: [июль 2020 г.](https://github.com/dotnet/docs/projects/103), [август 2020 г.](https://github.com/dotnet/docs/projects/117) и т. д.</span><span class="sxs-lookup"><span data-stu-id="b4e97-207">Examples, [July 2020](https://github.com/dotnet/docs/projects/103), [August 2020](https://github.com/dotnet/docs/projects/117), and so on.</span></span>
- <span data-ttu-id="b4e97-208">Долговременные ситуации: используются для упорядочения задач, работа над которыми будет продолжаться несколько месяцев.</span><span class="sxs-lookup"><span data-stu-id="b4e97-208">Long-running epics: These are used to organize tasks toward a goal when the work will occur over several months.</span></span>
  - <span data-ttu-id="b4e97-209">Примеры: [.NET 5 Wave — Reorganization](https://github.com/dotnet/docs/projects/105), [.NET Languages (.NET 5 Wave) ](https://github.com/dotnet/docs/projects/106) и т. д.</span><span class="sxs-lookup"><span data-stu-id="b4e97-209">Examples: [.NET 5 Wave - Reorganization](https://github.com/dotnet/docs/projects/105), [.NET Languages (.NET 5 wave) ](https://github.com/dotnet/docs/projects/106), and so on.</span></span>

## <a name="milestones"></a><span data-ttu-id="b4e97-210">Вехи</span><span class="sxs-lookup"><span data-stu-id="b4e97-210">Milestones</span></span>

<span data-ttu-id="b4e97-211">Вехи обычно следуют соглашению об именовании для проектов `Month YYYY`, но они отличаются от проектов.</span><span class="sxs-lookup"><span data-stu-id="b4e97-211">Milestones typically follow the same naming convention of projects `Month YYYY`, but they're different from projects.</span></span> <span data-ttu-id="b4e97-212">Вехи используются для отслеживания завершенной работы.</span><span class="sxs-lookup"><span data-stu-id="b4e97-212">We use milestones to track completed work.</span></span> <span data-ttu-id="b4e97-213">Вехи _не_ должны содержать проблемы (возможная работа), а только запросы на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="b4e97-213">Milestones should _not_ contain issues (potential work), but rather exclusively contain pull requests.</span></span> <span data-ttu-id="b4e97-214">Текущая веха автоматически применяется к новым запросам на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="b4e97-214">The current milestone is automatically applied to new pull requests.</span></span>
