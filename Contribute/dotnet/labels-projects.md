---
title: 'Стратегия: метки, проекты и вехи'
description: В этой статье объясняется, как метки, проекты и вехи используются в репозитории dotnet/docs.
ms.topic: contributor-guide
ms.prod: non-product-specific
ms.custom: external-contributor-guide
ms.date: 08/06/2020
ms.openlocfilehash: b7c6e4058d802db2e9dc391bfebc9f66b27c4023
ms.sourcegitcommit: fe12c5eef9d05fa598e326c44248c2b9c68cca12
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2020
ms.locfileid: "96755453"
---
# <a name="labels-projects-and-milestones-roadmap"></a><span data-ttu-id="bcb06-103">Стратегия: метки, проекты и вехи</span><span class="sxs-lookup"><span data-stu-id="bcb06-103">Labels, projects, and milestones roadmap</span></span>

<span data-ttu-id="bcb06-104">Команда по разработке документации .NET активно использует [метки GitHub](https://github.com/dotnet/docs/labels) для организации работы.</span><span class="sxs-lookup"><span data-stu-id="bcb06-104">The .NET docs team makes extensive use of [GitHub labels](https://github.com/dotnet/docs/labels) to organize our work.</span></span> <span data-ttu-id="bcb06-105">Путем фильтрации по сочетаниям меток мы можем быстро сосредотачиваться на интересующих нас разделах [веб-сайта документации по .NET](https://docs.microsoft.com/dotnet).</span><span class="sxs-lookup"><span data-stu-id="bcb06-105">By filtering on combinations of labels, we can quickly focus on sections of interest on the [.NET docs website](https://docs.microsoft.com/dotnet).</span></span> <span data-ttu-id="bcb06-106">Например, можно отфильтровать все открытые проблемы с приоритетом `P1`, используя такой запрос: [is:issue is:open label:":books: Area — .NET Architecture Guide"](https://github.com/dotnet/docs/issues?q=is%3Aissue+is%3Aopen+label%3A%22%3Abooks%3A+Area+-+.NET+Architecture+Guide%22).</span><span class="sxs-lookup"><span data-stu-id="bcb06-106">For example, we could filter to all of the open priority one `P1` issues with a query to [is:issue is:open label:":books: Area - .NET Architecture Guide"](https://github.com/dotnet/docs/issues?q=is%3Aissue+is%3Aopen+label%3A%22%3Abooks%3A+Area+-+.NET+Architecture+Guide%22).</span></span>

<span data-ttu-id="bcb06-107">Мы используем [проекты GitHub](https://github.com/dotnet/docs/projects) для организации спринтов и других целевых ситуаций.</span><span class="sxs-lookup"><span data-stu-id="bcb06-107">We use [GitHub projects](https://github.com/dotnet/docs/projects) to organize sprints and other goal-oriented epics.</span></span> <span data-ttu-id="bcb06-108">Для отслеживания работы мы также используем [вехи GitHub](https://github.com/dotnet/docs/milestones).</span><span class="sxs-lookup"><span data-stu-id="bcb06-108">We also use [GitHub milestones](https://github.com/dotnet/docs/milestones) to track work.</span></span> <span data-ttu-id="bcb06-109">Проще всего запомнить, что проекты относятся к планированию (проблемы), а вехи — к работе (запросы на вытягивание).</span><span class="sxs-lookup"><span data-stu-id="bcb06-109">It is best to think of projects for planning (issues), and milestones for work (pull requests).</span></span>

<span data-ttu-id="bcb06-110">В этой стратегии объясняется, как мы используем эти организационные средства, а также есть ссылки на удобные фильтры по некоторым важным областям.</span><span class="sxs-lookup"><span data-stu-id="bcb06-110">This roadmap explains how we use these organizational tools and has links to handy filters we use to find areas of interest.</span></span>

## <a name="labels"></a><span data-ttu-id="bcb06-111">Метки</span><span class="sxs-lookup"><span data-stu-id="bcb06-111">Labels</span></span>

<span data-ttu-id="bcb06-112">Если вы впервые участвуете в работе c [dotnet/docs](https://github.com/dotnet/docs), начните со списка проблем [up-for-grabs](https://github.com/dotnet/docs/labels/up-for-grabs).</span><span class="sxs-lookup"><span data-stu-id="bcb06-112">If this is your first experience contributing to [dotnet/docs](https://github.com/dotnet/docs), start with the [up-for-grabs](https://github.com/dotnet/docs/labels/up-for-grabs) issues.</span></span> <span data-ttu-id="bcb06-113">В него включены проблемы с довольно узкой областью.</span><span class="sxs-lookup"><span data-stu-id="bcb06-113">These are issues that have a more focused scope.</span></span> <span data-ttu-id="bcb06-114">Это отличный путь для первого вклада в работу.</span><span class="sxs-lookup"><span data-stu-id="bcb06-114">They are a great way to make your first contribution.</span></span> <span data-ttu-id="bcb06-115">В представлении "up-for-grabs" вы можете отфильтровать проблемы по областям и приоритетам.</span><span class="sxs-lookup"><span data-stu-id="bcb06-115">From the up-for-grabs view, you can further filter issues based on areas and priority.</span></span> <span data-ttu-id="bcb06-116">Проблемы, которые хорошо подходят для начинающих, мы обозначаем меткой [good-first-issue](https://github.com/dotnet/docs/labels/good-first-issue), и они помогут вам внести первый небольшой вклад.</span><span class="sxs-lookup"><span data-stu-id="bcb06-116">We've identified good issues for beginners with the [good-first-issue](https://github.com/dotnet/docs/labels/good-first-issue) if you want to try a smaller first contribution.</span></span>

<span data-ttu-id="bcb06-117">Мы используем метки для классификации проблем несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="bcb06-117">We use labels to classify issues in many different ways:</span></span>

- <span data-ttu-id="bcb06-118">[руководства по .NET](#find-a-single-net-guide) и [разделы руководства](#search-one-section-of-a-guide);</span><span class="sxs-lookup"><span data-stu-id="bcb06-118">[.NET Guides](#find-a-single-net-guide) and [sections of a guide](#search-one-section-of-a-guide).</span></span>
- [<span data-ttu-id="bcb06-119">Целевой выпуск</span><span class="sxs-lookup"><span data-stu-id="bcb06-119">Target release</span></span>](#releases)
- [<span data-ttu-id="bcb06-120">Приоритет</span><span class="sxs-lookup"><span data-stu-id="bcb06-120">Priority</span></span>](#priority)

<span data-ttu-id="bcb06-121">Объединяя метки из каждого набора (руководство, выпуск, приоритет), вы можете создать узкие срезы для поиска проблем, с которыми вы намерены работать.</span><span class="sxs-lookup"><span data-stu-id="bcb06-121">You can combine a label from each set (guide, release, priority) to create a narrow focus to find issues you want to work on.</span></span>

### <a name="find-a-single-net-guide"></a><span data-ttu-id="bcb06-122">Поиск конкретного руководства по .NET</span><span class="sxs-lookup"><span data-stu-id="bcb06-122">Find a single .NET guide</span></span>

<span data-ttu-id="bcb06-123">Мы используем метки для каждой из электронных книг по архитектуре и для каждого руководства по .NET.</span><span class="sxs-lookup"><span data-stu-id="bcb06-123">We use labels for each of the architecture e-books and for each .NET Guide.</span></span>

<span data-ttu-id="bcb06-124">![:book: руководство на светло-зеленом фоне](./media/labels-projects/guide.png "Префикс для меток руководств по архитектуре")</span><span class="sxs-lookup"><span data-stu-id="bcb06-124">![:book: guide on light green background](./media/labels-projects/guide.png "Prefix for architecture guide labels")</span></span>

<span data-ttu-id="bcb06-125">Электронные книги по архитектуре обозначаются префиксом `:book: guide` и имеют светло-зеленый фон.</span><span class="sxs-lookup"><span data-stu-id="bcb06-125">Architecture e-books are noted with the `:book: guide` prefix and have a light green background.</span></span> <span data-ttu-id="bcb06-126">Это развернутые описания, относящиеся к рекомендуемой архитектуре.</span><span class="sxs-lookup"><span data-stu-id="bcb06-126">These are the long-form areas that cover recommended architecture.</span></span> <span data-ttu-id="bcb06-127">Вот пример списка текущих проблем, которые отфильтрованы по каждому из руководств по архитектуре .NET.</span><span class="sxs-lookup"><span data-stu-id="bcb06-127">Here are current issues filtered for each of the .NET architecture guides.</span></span>

- [<span data-ttu-id="bcb06-128">Веб-приложения ASP.NET Core</span><span class="sxs-lookup"><span data-stu-id="bcb06-128">ASP.NET Core web apps</span></span>](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20ASP.NET%20Core%20web%20apps)
- [<span data-ttu-id="bcb06-129">Blazor</span><span class="sxs-lookup"><span data-stu-id="bcb06-129">Blazor</span></span>](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Blazor)
- [<span data-ttu-id="bcb06-130">Собственные облачные приложения</span><span class="sxs-lookup"><span data-stu-id="bcb06-130">Cloud Native</span></span>](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Cloud%20Native)
- [<span data-ttu-id="bcb06-131">Жизненный цикл Docker</span><span class="sxs-lookup"><span data-stu-id="bcb06-131">Docker lifecycle</span></span>](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Docker%20lifecycle)
- [<span data-ttu-id="bcb06-132">gRPC</span><span class="sxs-lookup"><span data-stu-id="bcb06-132">gRPC</span></span>](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20gRPC)
- [<span data-ttu-id="bcb06-133">Модернизация с помощью контейнеров Windows</span><span class="sxs-lookup"><span data-stu-id="bcb06-133">Modernizing w/ Windows containers</span></span>](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Modernizing%20w%2F%20Windows%20containers)
- [<span data-ttu-id="bcb06-134">Микрослужбы .NET</span><span class="sxs-lookup"><span data-stu-id="bcb06-134">.NET Microservices</span></span>](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20.NET%20Microservices)
- [<span data-ttu-id="bcb06-135">Бессерверные приложения</span><span class="sxs-lookup"><span data-stu-id="bcb06-135">Serverless apps</span></span>](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Serverless%20apps)

<span data-ttu-id="bcb06-136">Этот же стиль меток применяется к [рекомендациям по проектированию платформы](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Framework%20Design%20Guidelines).</span><span class="sxs-lookup"><span data-stu-id="bcb06-136">This label style is also applied to the [Framework design guidelines](https://github.com/dotnet/docs/labels/%3Abook%3A%20guide%20-%20Framework%20Design%20Guidelines).</span></span> <span data-ttu-id="bcb06-137">Для этой области используется та же структура меток, но запросы на вытягивание от сообщества здесь не рекомендуются.</span><span class="sxs-lookup"><span data-stu-id="bcb06-137">This area has the same label design, but community PRs are discouraged.</span></span> <span data-ttu-id="bcb06-138">Эти материалы переиздаются по индивидуальным разрешениям и не должны редактироваться.</span><span class="sxs-lookup"><span data-stu-id="bcb06-138">This is material reprinted with permission and should not be edited.</span></span>

<span data-ttu-id="bcb06-139">![:books: Area на темно-синем фоне](./media/labels-projects/area.png "Префикс для меток области руководства по .NET")</span><span class="sxs-lookup"><span data-stu-id="bcb06-139">![:books: Area on dark blue background](./media/labels-projects/area.png "Prefix for .NET Guide area labels")</span></span>

<span data-ttu-id="bcb06-140">Каждое из руководств по .NET обозначено префиксом `:books: Area` и имеет темно-синий фон.</span><span class="sxs-lookup"><span data-stu-id="bcb06-140">Each .NET Guide is noted with the `:books: Area` prefix and has a dark blue background.</span></span> <span data-ttu-id="bcb06-141">Вот пример списка текущих проблем, которые отфильтрованы по каждому из руководств .NET.</span><span class="sxs-lookup"><span data-stu-id="bcb06-141">Here are current issues filtered for each of the .NET guides.</span></span>

- [<span data-ttu-id="bcb06-142">Справочник по интерфейсам API</span><span class="sxs-lookup"><span data-stu-id="bcb06-142">API Reference</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20API%20Reference)
- <span data-ttu-id="bcb06-143">[Azure .NET SDK](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20Azure%20.NET%20SDk);</span><span class="sxs-lookup"><span data-stu-id="bcb06-143">[Azure .NET SDK](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20Azure%20.NET%20SDk)</span></span>
- [<span data-ttu-id="bcb06-144">Руководство по языку C#</span><span class="sxs-lookup"><span data-stu-id="bcb06-144">C# Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20C%23%20Guide)
- [<span data-ttu-id="bcb06-145">Руководство по языку F#</span><span class="sxs-lookup"><span data-stu-id="bcb06-145">F# Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20F%23%20Guide)
- [<span data-ttu-id="bcb06-146">Руководство по ML.NET</span><span class="sxs-lookup"><span data-stu-id="bcb06-146">ML.NET Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20ML.NET%20Guide)
- <span data-ttu-id="bcb06-147">[Руководство по архитектуре .NET](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20Architecture%20Guide) — может быть удалено</span><span class="sxs-lookup"><span data-stu-id="bcb06-147">[.NET Architecture Guide](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20Architecture%20Guide) - Could be removed</span></span>
- [<span data-ttu-id="bcb06-148">Руководство по .NET Core</span><span class="sxs-lookup"><span data-stu-id="bcb06-148">.NET Core Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20Core%20Guide)
- [<span data-ttu-id="bcb06-149">Руководство по .NET для Apache Spark</span><span class="sxs-lookup"><span data-stu-id="bcb06-149">.NET for Apache Spark Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20for%20Apache%20Spark%20Guide)
- [<span data-ttu-id="bcb06-150">Руководство по .NET Framework</span><span class="sxs-lookup"><span data-stu-id="bcb06-150">.NET Framework Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20Framework%20Guide)
- [<span data-ttu-id="bcb06-151">Руководство по .NET</span><span class="sxs-lookup"><span data-stu-id="bcb06-151">.NET Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20.NET%20Guide)
- <span data-ttu-id="bcb06-152">[Справочник по API Roslyn](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20Roslyn%20API%20Reference) — может быть удален.</span><span class="sxs-lookup"><span data-stu-id="bcb06-152">[Roslyn API Reference](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20Roslyn%20API%20Reference) - could be removed.</span></span>
- [<span data-ttu-id="bcb06-153">Руководство по Visual Basic</span><span class="sxs-lookup"><span data-stu-id="bcb06-153">Visual Basic Guide</span></span>](https://github.com/dotnet/docs/labels/%3Abooks%3A%20Area%20-%20Visual%20Basic%20Guide)

#### <a name="search-one-section-of-a-guide"></a><span data-ttu-id="bcb06-154">Поиск по одному разделу руководства</span><span class="sxs-lookup"><span data-stu-id="bcb06-154">Search one section of a guide</span></span>

<span data-ttu-id="bcb06-155">![:card_file_box: Area на умеренно синем фоне](./media/labels-projects/technology.png "Префикс для меток вложенных областей руководства по .NET")</span><span class="sxs-lookup"><span data-stu-id="bcb06-155">![:card_file_box: Area on medium blue background](./media/labels-projects/technology.png "Prefix for .NET Guide sub-area labels")</span></span>

<span data-ttu-id="bcb06-156">Руководства по .NET достаточно большие, а эти метки позволяют дополнительно ограничить область поиска конкретным разделом руководства.</span><span class="sxs-lookup"><span data-stu-id="bcb06-156">The .NET guides are large, so these labels further limit the scope by a section of a guide.</span></span> <span data-ttu-id="bcb06-157">Каждая из вложенных областей руководств по .NET обозначено префиксом `:card_file_box: Technology` и имеет светло-синий фон.</span><span class="sxs-lookup"><span data-stu-id="bcb06-157">Each .NET Guide subarea is noted with the `:card_file_box: Technology` prefix and has a medium blue background.</span></span> <span data-ttu-id="bcb06-158">Многие из этих меток применяются к нескольким руководствам, а другие — только к одному из них.</span><span class="sxs-lookup"><span data-stu-id="bcb06-158">Many of these labels apply to multiple guides, while others are in only one guide.</span></span> <span data-ttu-id="bcb06-159">Применив фильтр по области, добавьте одну из этих меток, чтобы ограничить область поиска проблем.</span><span class="sxs-lookup"><span data-stu-id="bcb06-159">After filtering on an area, add one of these labels to further limit the scope of issues.</span></span>

- <span data-ttu-id="bcb06-160">AppCompat</span><span class="sxs-lookup"><span data-stu-id="bcb06-160">AppCompat</span></span>
- <span data-ttu-id="bcb06-161">Асинхронная задача</span><span class="sxs-lookup"><span data-stu-id="bcb06-161">Async Task</span></span>
- <span data-ttu-id="bcb06-162">Дополнительные возможности C#</span><span class="sxs-lookup"><span data-stu-id="bcb06-162">C# Advanced concepts</span></span>
- <span data-ttu-id="bcb06-163">Компилятор C#</span><span class="sxs-lookup"><span data-stu-id="bcb06-163">C# compiler</span></span>
- <span data-ttu-id="bcb06-164">Основы C#</span><span class="sxs-lookup"><span data-stu-id="bcb06-164">C# Fundamentals</span></span>
- <span data-ttu-id="bcb06-165">Начало работы с C#</span><span class="sxs-lookup"><span data-stu-id="bcb06-165">C# Get Started</span></span>
- <span data-ttu-id="bcb06-166">Справочник по языку C#</span><span class="sxs-lookup"><span data-stu-id="bcb06-166">C# Language Reference</span></span>
- <span data-ttu-id="bcb06-167">Безопасность значений NULL в C#</span><span class="sxs-lookup"><span data-stu-id="bcb06-167">C# Null safety</span></span>
- <span data-ttu-id="bcb06-168">Новые возможности C#</span><span class="sxs-lookup"><span data-stu-id="bcb06-168">C# What's new</span></span>
- <span data-ttu-id="bcb06-169">CLI</span><span class="sxs-lookup"><span data-stu-id="bcb06-169">CLI</span></span>
- <span data-ttu-id="bcb06-170">Доступ к данным</span><span class="sxs-lookup"><span data-stu-id="bcb06-170">Data Access</span></span>
- <span data-ttu-id="bcb06-171">Docker</span><span class="sxs-lookup"><span data-stu-id="bcb06-171">Docker</span></span>
- <span data-ttu-id="bcb06-172">Установщики</span><span class="sxs-lookup"><span data-stu-id="bcb06-172">Installers</span></span>
- <span data-ttu-id="bcb06-173">LINQ</span><span class="sxs-lookup"><span data-stu-id="bcb06-173">LINQ</span></span>
- <span data-ttu-id="bcb06-174">NCL</span><span class="sxs-lookup"><span data-stu-id="bcb06-174">NCL</span></span>
- <span data-ttu-id="bcb06-175">.NET Standard</span><span class="sxs-lookup"><span data-stu-id="bcb06-175">.NET Standard</span></span>
- <span data-ttu-id="bcb06-176">API Roslyn</span><span class="sxs-lookup"><span data-stu-id="bcb06-176">Roslyn APIs</span></span>
- <span data-ttu-id="bcb06-177">Безопасность</span><span class="sxs-lookup"><span data-stu-id="bcb06-177">Security</span></span>
- <span data-ttu-id="bcb06-178">WCF</span><span class="sxs-lookup"><span data-stu-id="bcb06-178">WCF</span></span>
- <span data-ttu-id="bcb06-179">WF</span><span class="sxs-lookup"><span data-stu-id="bcb06-179">WF</span></span>
- <span data-ttu-id="bcb06-180">WIF</span><span class="sxs-lookup"><span data-stu-id="bcb06-180">WIF</span></span>
- <span data-ttu-id="bcb06-181">WinForms</span><span class="sxs-lookup"><span data-stu-id="bcb06-181">WinForms</span></span>
- <span data-ttu-id="bcb06-182">WPF</span><span class="sxs-lookup"><span data-stu-id="bcb06-182">WPF</span></span>

### <a name="releases"></a><span data-ttu-id="bcb06-183">Выпуски</span><span class="sxs-lookup"><span data-stu-id="bcb06-183">Releases</span></span>

<span data-ttu-id="bcb06-184">![:checkered_flag: Release: на темно-желтом фоне](./media/labels-projects/release.png "Префикс для меток выпуска")</span><span class="sxs-lookup"><span data-stu-id="bcb06-184">![:checkered_flag: Release: on dark yellow](./media/labels-projects/release.png "Prefix for release labels")</span></span>

<span data-ttu-id="bcb06-185">Проблемы, помеченные для конкретного выпуска, обозначаются префиксом `:checkered_flag: Release:` и отображаются на темно-желтом фоне.</span><span class="sxs-lookup"><span data-stu-id="bcb06-185">Issues tagged for a specific release are noted with the `:checkered_flag: Release:` prefix and have a dark yellow background.</span></span>

- <span data-ttu-id="bcb06-186">.NET Core 2.2</span><span class="sxs-lookup"><span data-stu-id="bcb06-186">.NET Core 2.2</span></span>
- <span data-ttu-id="bcb06-187">.NET Core 3.0</span><span class="sxs-lookup"><span data-stu-id="bcb06-187">.NET Core 3.0</span></span>
- <span data-ttu-id="bcb06-188">.NET Framework 4.8</span><span class="sxs-lookup"><span data-stu-id="bcb06-188">.NET Framework 4.8</span></span>
- <span data-ttu-id="bcb06-189">.NET 5</span><span class="sxs-lookup"><span data-stu-id="bcb06-189">.NET 5</span></span>

### <a name="priority"></a><span data-ttu-id="bcb06-190">Приоритет</span><span class="sxs-lookup"><span data-stu-id="bcb06-190">Priority</span></span>

<span data-ttu-id="bcb06-191">Метки приоритета содержат символ `P`, за которым следует одна цифра.</span><span class="sxs-lookup"><span data-stu-id="bcb06-191">Priority labels are all `P` followed by a single digit.</span></span> <span data-ttu-id="bcb06-192">Чем меньше число, тем выше приоритет.</span><span class="sxs-lookup"><span data-stu-id="bcb06-192">Lower numbers are higher priority:</span></span>

- <span data-ttu-id="bcb06-193">P0 — критический приоритет.</span><span class="sxs-lookup"><span data-stu-id="bcb06-193">P0 - Critical priority</span></span>

  <span data-ttu-id="bcb06-194">Проблема безопасности или необходимость выполнить юридическое требование для обеспечения соответствия.</span><span class="sxs-lookup"><span data-stu-id="bcb06-194">Security issue or legally required for compliance.</span></span> <span data-ttu-id="bcb06-195">Исправления вносятся прежде любых других.</span><span class="sxs-lookup"><span data-stu-id="bcb06-195">We drop everything else to fix.</span></span>
  
- <span data-ttu-id="bcb06-196">Р1 — высокий приоритет;</span><span class="sxs-lookup"><span data-stu-id="bcb06-196">P1 - High priority</span></span>

  <span data-ttu-id="bcb06-197">Проблема, которую необходимо устранить для распространенных сценариев.</span><span class="sxs-lookup"><span data-stu-id="bcb06-197">Essential for common scenarios.</span></span> <span data-ttu-id="bcb06-198">Или бросающаяся в глаза ошибка в статье с большим количеством просмотров страницы.</span><span class="sxs-lookup"><span data-stu-id="bcb06-198">Or highly visible error on high page view article.</span></span> <span data-ttu-id="bcb06-199">Исправления вносятся перед устранением проблем категорий P2 и P3.</span><span class="sxs-lookup"><span data-stu-id="bcb06-199">We do these before P2 or P3 work.</span></span>
  
- <span data-ttu-id="bcb06-200">Р2 — средний приоритет;</span><span class="sxs-lookup"><span data-stu-id="bcb06-200">P2 - Medium priority</span></span>

  <span data-ttu-id="bcb06-201">Проблема, которую полезно устранить для распространенных сценариев, но которая не блокирует работу.</span><span class="sxs-lookup"><span data-stu-id="bcb06-201">Helpful for common scenarios but not blocking.</span></span>  <span data-ttu-id="bcb06-202">Исправления вносятся сразу, если это быстро и просто. Или же они откладываются и вносятся после устранения проблем категории P1 в той же статье.</span><span class="sxs-lookup"><span data-stu-id="bcb06-202">We do these if quick and easy, or fit them in while addressing a P1 issue in the same article.</span></span>
  
- <span data-ttu-id="bcb06-203">Р3 — низкий приоритет.</span><span class="sxs-lookup"><span data-stu-id="bcb06-203">P3 - Low priority</span></span>

  <span data-ttu-id="bcb06-204">Проблема, которую полезно устранить для пограничных случаев; обычные ошибки, исправляемые для распространенных сценариев; ошибка в статье с малым количеством просмотров страницы; нерекомендуемая технология.</span><span class="sxs-lookup"><span data-stu-id="bcb06-204">Helpful for edge cases, trivial corrections for common scenarios, low page view article, or deprecated technology.</span></span> <span data-ttu-id="bcb06-205">Исправлению таких ошибок не уделяется специальное время, они устраняются по мере выявления участниками сообщества.</span><span class="sxs-lookup"><span data-stu-id="bcb06-205">Not worth our time but up for grabs for community contribution.</span></span> <span data-ttu-id="bcb06-206">Проблема P3 может быть закрыта, если она не устраняется в течение двух месяцев.</span><span class="sxs-lookup"><span data-stu-id="bcb06-206">A P3 issue may be closed if not addressed after two months.</span></span>

### <a name="what-about-the-other-labels"></a><span data-ttu-id="bcb06-207">Другие метки</span><span class="sxs-lookup"><span data-stu-id="bcb06-207">What about the other labels</span></span>

<span data-ttu-id="bcb06-208">Группы по работе над содержимым используют много других меток для управления разными классификациями проблем.</span><span class="sxs-lookup"><span data-stu-id="bcb06-208">There are many other labels used by the content teams to manage different classifications of issues.</span></span> <span data-ttu-id="bcb06-209">Если вы не входите в такую группу, остальные метки можно смело игнорировать.</span><span class="sxs-lookup"><span data-stu-id="bcb06-209">If you're not on the content team, you can ignore these other labels.</span></span>

## <a name="projects"></a><span data-ttu-id="bcb06-210">Проекты</span><span class="sxs-lookup"><span data-stu-id="bcb06-210">Projects</span></span>

<span data-ttu-id="bcb06-211">Проекты предназначены для планирования. При этом приоритетная работа выполняется автоматически с использованием канбан-доски.</span><span class="sxs-lookup"><span data-stu-id="bcb06-211">Projects are intended for planning purposes, where prioritized work is automated through a Kanban board.</span></span> <span data-ttu-id="bcb06-212">Проекты должны содержать только проблемы GitHub, но _не_ запросы на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="bcb06-212">Projects should only ever contain GitHub issues, _not_ pull requests.</span></span> <span data-ttu-id="bcb06-213">Проекты отличаются от вех тем, что вехи содержат только запросы на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="bcb06-213">Projects differ from milestones, in that milestones only contain pull requests.</span></span>

<span data-ttu-id="bcb06-214">Мы используем проекты двумя способами.</span><span class="sxs-lookup"><span data-stu-id="bcb06-214">We use projects in two ways:</span></span>

- <span data-ttu-id="bcb06-215">Типы проектов `Month YYYY`: это канбан-доски для рабочих планов на каждый месяц.</span><span class="sxs-lookup"><span data-stu-id="bcb06-215">`Month YYYY` project types: These are Kanban boards for each month's working plan.</span></span>
  - <span data-ttu-id="bcb06-216">Примеры: [июль 2020 г.](https://github.com/dotnet/docs/projects/103), [август 2020 г.](https://github.com/dotnet/docs/projects/117) и т. д.</span><span class="sxs-lookup"><span data-stu-id="bcb06-216">Examples, [July 2020](https://github.com/dotnet/docs/projects/103), [August 2020](https://github.com/dotnet/docs/projects/117), and so on.</span></span>
- <span data-ttu-id="bcb06-217">Долговременные ситуации: используются для упорядочения задач, работа над которыми будет продолжаться несколько месяцев.</span><span class="sxs-lookup"><span data-stu-id="bcb06-217">Long-running epics: These are used to organize tasks toward a goal when the work will occur over several months.</span></span>
  - <span data-ttu-id="bcb06-218">Примеры: [.NET 5 Wave — Reorganization](https://github.com/dotnet/docs/projects/105), [.NET Languages (.NET 5 Wave) ](https://github.com/dotnet/docs/projects/106) и т. д.</span><span class="sxs-lookup"><span data-stu-id="bcb06-218">Examples: [.NET 5 Wave - Reorganization](https://github.com/dotnet/docs/projects/105), [.NET Languages (.NET 5 wave) ](https://github.com/dotnet/docs/projects/106), and so on.</span></span>

## <a name="milestones"></a><span data-ttu-id="bcb06-219">Вехи</span><span class="sxs-lookup"><span data-stu-id="bcb06-219">Milestones</span></span>

<span data-ttu-id="bcb06-220">Вехи обычно следуют соглашению об именовании для проектов `Month YYYY`, но они отличаются от проектов.</span><span class="sxs-lookup"><span data-stu-id="bcb06-220">Milestones typically follow the same naming convention of projects `Month YYYY`, but they're different from projects.</span></span> <span data-ttu-id="bcb06-221">Вехи используются для отслеживания завершенной работы.</span><span class="sxs-lookup"><span data-stu-id="bcb06-221">We use milestones to track completed work.</span></span> <span data-ttu-id="bcb06-222">Вехи _не_ должны содержать проблемы (возможная работа), а только запросы на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="bcb06-222">Milestones should _not_ contain issues (potential work), but rather exclusively contain pull requests.</span></span> <span data-ttu-id="bcb06-223">Текущая веха автоматически применяется к новым запросам на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="bcb06-223">The current milestone is automatically applied to new pull requests.</span></span>
