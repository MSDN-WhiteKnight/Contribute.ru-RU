---
title: Процедура участия в разработке репозиториев документации по PowerShell
description: В этой статье описывается процедура участия в разработке репозиториев документации по PowerShell. Вы узнаете об используемых репозиториях, процессе организации содержимого и политиках управления примерами кода и другими ресурсами.
ms.topic: contributor-guide
ms.prod: non-product-specific
ms.custom: external-contributor-guide
author: sdwheeler
ms.author: sewhee
ms.date: 10/07/2019
ms.openlocfilehash: 9802942dccbfad2cb860739ffba4b30d2b0af0c9
ms.sourcegitcommit: ca84e542b081e145052f38967e826f6ef25da1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/12/2019
ms.locfileid: "72290203"
---
# <a name="process-for-contributing-to-powershell-docs"></a><span data-ttu-id="8525c-104">Процесс участия в составлении документации по PowerShell</span><span class="sxs-lookup"><span data-stu-id="8525c-104">Process for contributing to PowerShell docs</span></span>

<span data-ttu-id="8525c-105">Мы ценим вклад сообщества в составление документации. Ниже приводятся правила, которых следует придерживаться при составлении документации по PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8525c-105">We appreciate community contributions to docs. The following list shows some guiding rules that you should keep in mind when you're contributing to the PowerShell documentation:</span></span>

- <span data-ttu-id="8525c-106">**НЕ** удивляйте нас огромными запросами на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="8525c-106">**DON'T** surprise us with large pull requests.</span></span> <span data-ttu-id="8525c-107">Лучше сообщите о проблеме и начните обсуждение, чтобы мы согласовали направление, прежде чем вы потратите свое время.</span><span class="sxs-lookup"><span data-stu-id="8525c-107">Instead, file an issue and start a discussion so we can agree on a direction before you invest a large amount of time.</span></span>
- <span data-ttu-id="8525c-108">**Следуйте** этим инструкциям и руководствам по стилю при написании [кода](powershell-style-code.md) и [справки](powershell-style-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8525c-108">**DO** follow these instructions and the [code](powershell-style-code.md) and [reference](powershell-style-reference.md) style guides..</span></span>
- <span data-ttu-id="8525c-109">**Используйте** файл [шаблона](powershell-style-basic-markdown.md) в качестве отправной точки.</span><span class="sxs-lookup"><span data-stu-id="8525c-109">**DO** use the [template](powershell-style-basic-markdown.md) file as the starting point of your work.</span></span>
- <span data-ttu-id="8525c-110">**Создайте** отдельную ветвь в вилке, прежде чем приступить к работе над статьями.</span><span class="sxs-lookup"><span data-stu-id="8525c-110">**DO** create a separate branch on your fork before working on the articles.</span></span>
- <span data-ttu-id="8525c-111">**Следуйте** [рабочему процессу GitHub](../how-to-write-workflows-major.md).</span><span class="sxs-lookup"><span data-stu-id="8525c-111">**DO** follow the [GitHub Flow workflow](../how-to-write-workflows-major.md).</span></span>
- <span data-ttu-id="8525c-112">**Делайте записи** в блоге или Twitter (или на других платформах) о своем вкладе.</span><span class="sxs-lookup"><span data-stu-id="8525c-112">**DO** blog and tweet (or whatever) about your contributions, frequently!</span></span>

<span data-ttu-id="8525c-113">Эти рекомендации облегчат работу и вам, и нам.</span><span class="sxs-lookup"><span data-stu-id="8525c-113">Following these guidelines ensures a better experience for you and for us.</span></span>

## <a name="make-a-contribution-to-powershell-docs"></a><span data-ttu-id="8525c-114">Участие в составлении документации по PowerShell</span><span class="sxs-lookup"><span data-stu-id="8525c-114">Make a contribution to PowerShell docs</span></span>

<span data-ttu-id="8525c-115">Вы можете выбрать одну из интересующих вас [проблем](https://github.com/MicrosoftDocs/PowerShell-Docs/issues/new/choose).</span><span class="sxs-lookup"><span data-stu-id="8525c-115">You can choose from existing [issues](https://github.com/MicrosoftDocs/PowerShell-Docs/issues/new/choose).</span></span>
<span data-ttu-id="8525c-116">Они делятся на следующие категории:</span><span class="sxs-lookup"><span data-stu-id="8525c-116">Depending on your interests and level of commitment, the efforts fall into the following categories:</span></span>

- <span data-ttu-id="8525c-117">**Незначительные изменения**.</span><span class="sxs-lookup"><span data-stu-id="8525c-117">**Small changes**.</span></span> <span data-ttu-id="8525c-118">Если это незначительные изменения, см. инструкции по редактированию в GitHub на [домашней странице](../index.md#quick-edits-to-existing-documents) руководства для участников.</span><span class="sxs-lookup"><span data-stu-id="8525c-118">For small changes, see the instructions on editing in GitHub on the [home page](../index.md#quick-edits-to-existing-documents) of the contributor guide.</span></span> <span data-ttu-id="8525c-119">В число незначительных изменений входят:</span><span class="sxs-lookup"><span data-stu-id="8525c-119">Small changes include:</span></span>

  - <span data-ttu-id="8525c-120">исправление опечаток и орфографических ошибок;</span><span class="sxs-lookup"><span data-stu-id="8525c-120">Fixing typos and spelling errors</span></span>
  - <span data-ttu-id="8525c-121">улучшение грамматики или форматирования;</span><span class="sxs-lookup"><span data-stu-id="8525c-121">Improving grammar or formatting</span></span>
  - <span data-ttu-id="8525c-122">небольшие изменения технического или фактического характера.</span><span class="sxs-lookup"><span data-stu-id="8525c-122">Minor technical or factual edits</span></span>

- <span data-ttu-id="8525c-123">**Обслуживание**.</span><span class="sxs-lookup"><span data-stu-id="8525c-123">**Maintenance**.</span></span> <span data-ttu-id="8525c-124">В эту категорию входят довольно простые проблемы, например исправление нерабочих или некорректных ссылок, добавление отсутствующих примеров кода или решение проблем с ограниченным содержимым.</span><span class="sxs-lookup"><span data-stu-id="8525c-124">This category includes fairly simple contributions, such as fixing broken or incorrect links, adding missing code examples, or addressing limited content issues.</span></span> <span data-ttu-id="8525c-125">В некоторых случаях эти проблемы затрагивают большое количество файлов.</span><span class="sxs-lookup"><span data-stu-id="8525c-125">In some cases, these issues may concern large numbers of files.</span></span> <span data-ttu-id="8525c-126">В такой ситуации сообщите нам, над чем вы хотите поработать, прежде чем начать.</span><span class="sxs-lookup"><span data-stu-id="8525c-126">In that case, you should let us know what you'd like to work on before you begin.</span></span> <span data-ttu-id="8525c-127">Напишите комментарий к проблеме, чтобы уведомить нас, что работаете над ней.</span><span class="sxs-lookup"><span data-stu-id="8525c-127">Add a comment on the issue to tell us that you are working on it.</span></span>

- <span data-ttu-id="8525c-128">**Обновление содержимого**.</span><span class="sxs-lookup"><span data-stu-id="8525c-128">**Content updates**.</span></span> <span data-ttu-id="8525c-129">Поскольку объем документации очень большой, содержимое часто устаревает и требует пересмотра.</span><span class="sxs-lookup"><span data-stu-id="8525c-129">Given the enormity of the doc set, content easily becomes outdated and requires revision.</span></span> <span data-ttu-id="8525c-130">Кроме того по разным причинам одно и то же содержимое может быть представлено дважды, а то и трижды.</span><span class="sxs-lookup"><span data-stu-id="8525c-130">In addition, for a variety of reason, some content has been duplicated or even triplicated.</span></span> <span data-ttu-id="8525c-131">При обновлении содержимого следует убедиться, что отдельные темы не потеряли актуальность, и рекомендуем пересматривать содержимое в специальной области, чтобы избежать повторения и гарантировать, что все уникальное содержимое хранится в небольшом наборе документации.</span><span class="sxs-lookup"><span data-stu-id="8525c-131">Updating content involves making sure that individual topics are current or revising content in a feature area to eliminate duplication and ensure that all unique content is preserved in the smaller documentation set.</span></span>

- <span data-ttu-id="8525c-132">**Создание нового содержимого**.</span><span class="sxs-lookup"><span data-stu-id="8525c-132">**New content authoring**.</span></span> <span data-ttu-id="8525c-133">Если вы хотите написать свою статью, в проблемах найдите тему, которой нам не хватает в документации.</span><span class="sxs-lookup"><span data-stu-id="8525c-133">If you're interested in authoring your own topic, these issues list topics that we know we'd like to add to our doc set.</span></span> <span data-ttu-id="8525c-134">Не забудьте предварительно сообщить нам, что собираетесь работать над этой темой.</span><span class="sxs-lookup"><span data-stu-id="8525c-134">Let us know before you begin working on a topic, though.</span></span> <span data-ttu-id="8525c-135">Если вы хотите написать статью на тему, которой здесь нет, откройте проблему.</span><span class="sxs-lookup"><span data-stu-id="8525c-135">If you're interested in writing a topic that isn't listed here, open an issue.</span></span>

<span data-ttu-id="8525c-136">Выбрав задачу, следуйте руководству [по началу работы](../get-started-setup-github.md), чтобы создать учетную запись GitHub и настроить среду.</span><span class="sxs-lookup"><span data-stu-id="8525c-136">Once you've picked a task to work on, follow the [get started](../get-started-setup-github.md) guide to create a GitHub account and setup your environment.</span></span>

### <a name="making-large-changes"></a><span data-ttu-id="8525c-137">Внесение крупных изменений</span><span class="sxs-lookup"><span data-stu-id="8525c-137">Making large changes</span></span>

<span data-ttu-id="8525c-138">**Шаг 1:** Если вы хотите написать новую статью или существенно исправить уже опубликованную, откройте проблему с описанием ваших намерений.</span><span class="sxs-lookup"><span data-stu-id="8525c-138">**Step 1:** If you're interested in writing new content or in thoroughly revising existing content, open an issue describing what you want to do.</span></span>

<span data-ttu-id="8525c-139">**Шаг 2:** Создайте вилку в репозитории `MicrosoftDocs/PowerShell-Docs`, а затем создайте рабочую ветвь для своих изменений.</span><span class="sxs-lookup"><span data-stu-id="8525c-139">**Step 2:** Fork the `MicrosoftDocs/PowerShell-Docs` repository and create a working branch for your changes.</span></span>

<span data-ttu-id="8525c-140">**Шаг 3:** Внесите изменения в новой ветви.</span><span class="sxs-lookup"><span data-stu-id="8525c-140">**Step 3:** Make the changes in this new branch.</span></span>

<span data-ttu-id="8525c-141">Если это новая статья, используйте шаблон из [руководства по стилю](powershell-style-basic-markdown.md) в качестве отправной точки.</span><span class="sxs-lookup"><span data-stu-id="8525c-141">If it's a new topic, use the template in the [style guide](powershell-style-basic-markdown.md) as your starting point.</span></span> <span data-ttu-id="8525c-142">Руководство по стилю содержит рекомендации по написанию и разъяснения по метаданным, необходимым для каждой статьи.</span><span class="sxs-lookup"><span data-stu-id="8525c-142">The style guide contains the writing guidelines and explains the metadata required for each article.</span></span>

<span data-ttu-id="8525c-143">Перейдите в папку, руководствуясь оглавлением, как описано в шаге 1.</span><span class="sxs-lookup"><span data-stu-id="8525c-143">Navigate to the folder that corresponds to the TOC location determined for your article in step 1.</span></span>
<span data-ttu-id="8525c-144">Папка содержит файлы Markdown для всех статей в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="8525c-144">That folder contains the Markdown files for all articles in that section.</span></span> <span data-ttu-id="8525c-145">При необходимости создайте новую папку, чтобы поместить в нее файлы для вашей статьи.</span><span class="sxs-lookup"><span data-stu-id="8525c-145">If necessary, create a new folder to place the files for your content.</span></span> <span data-ttu-id="8525c-146">Основная статья этого раздела называется *index.md*.</span><span class="sxs-lookup"><span data-stu-id="8525c-146">The main article for that section is called *index.md*.</span></span>
<span data-ttu-id="8525c-147">Изображения и другие статические ресурсы размещайте во вложенной папке **media** внутри папки с вашей статьей. Создайте эту папку, если она еще не существует.</span><span class="sxs-lookup"><span data-stu-id="8525c-147">For images and other static resources, create a subfolder called **media** inside the folder that contains your article, if it doesn't already exist.</span></span> <span data-ttu-id="8525c-148">В папке **media** создайте вложенную папку с названием статьи (за исключением файла index).</span><span class="sxs-lookup"><span data-stu-id="8525c-148">Inside the **media** folder, create a subfolder with the article name (except for the index file).</span></span>

<span data-ttu-id="8525c-149">Обязательно соблюдайте синтаксис Markdown.</span><span class="sxs-lookup"><span data-stu-id="8525c-149">Be sure to follow the proper Markdown syntax.</span></span> <span data-ttu-id="8525c-150">Подробные инструкции и примеры см. в [руководстве по стилю](powershell-style-basic-markdown.md).</span><span class="sxs-lookup"><span data-stu-id="8525c-150">Please read the [style guide](powershell-style-basic-markdown.md) for detailed instructions and examples.</span></span>

<span data-ttu-id="8525c-151">**Пример структуры**</span><span class="sxs-lookup"><span data-stu-id="8525c-151">**Example structure**</span></span>

```
reference
  /docs-conceptual
    /learn
      /remoting
        managing-remote-sessions.md
        /images
          /managing-remote-sessions
            sesssion-list.png
```

<span data-ttu-id="8525c-152">**Шаг 4:** Отправьте запрос на вытягивание из вашей рабочей ветви в *промежуточную* ветвь.</span><span class="sxs-lookup"><span data-stu-id="8525c-152">**Step 4:** Submit a Pull Request (PR) from your working branch to the *staging* branch.</span></span>

<span data-ttu-id="8525c-153">Каждый запрос на вытягивание обычно относится к одной проблеме.</span><span class="sxs-lookup"><span data-stu-id="8525c-153">Normally, a PR should address one issue at a time.</span></span> <span data-ttu-id="8525c-154">Запрос на вытягивание может менять один или несколько файлов.</span><span class="sxs-lookup"><span data-stu-id="8525c-154">The PR can modify one or multiple files.</span></span> <span data-ttu-id="8525c-155">Если вы работаете с несколькими исправлениями в разных файлах, создайте отдельные запросы на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="8525c-155">If you're addressing multiple fixes on different files, separate PRs are preferred.</span></span>

<span data-ttu-id="8525c-156">Если ваш запрос на вытягивание исправляет существующую проблему, добавьте ключевое слово `Fixes #Issue_Number` в сообщение о фиксации или описание запроса на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="8525c-156">If your PR fixes an existing issue, add the `Fixes #Issue_Number` keyword to the commit message or PR description.</span></span> <span data-ttu-id="8525c-157">Таким образом проблема будет автоматически закрыта при слиянии запроса на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="8525c-157">That way, the issue is automatically closed when the PR is merged.</span></span> <span data-ttu-id="8525c-158">Дополнительные сведения см. в разделе [Закрытие проблем с помощью сообщений о фиксации](https://help.github.com/articles/closing-issues-via-commit-messages/).</span><span class="sxs-lookup"><span data-stu-id="8525c-158">For more information, see [Closing issues via commit messages](https://help.github.com/articles/closing-issues-via-commit-messages/).</span></span>

<span data-ttu-id="8525c-159">Команда PowerShell рассмотрит ваш запрос на вытягивание и сообщит вам, нужны ли дополнительные изменения для его одобрения.</span><span class="sxs-lookup"><span data-stu-id="8525c-159">The PowerShell team reviews your PR and lets you know if there are any other changes necessary in order to approve it.</span></span>

<span data-ttu-id="8525c-160">**Шаг 5:** Внесите необходимые изменения в вашу ветвь по рекомендациям команды.</span><span class="sxs-lookup"><span data-stu-id="8525c-160">**Step 5:** Make any necessary updates to your branch as discussed with the team.</span></span>

<span data-ttu-id="8525c-161">После одобрения запроса на вытягивание наша команда объединит ваш запрос на вытягивание с *промежуточной* ветвью.</span><span class="sxs-lookup"><span data-stu-id="8525c-161">Once the PR is approved, the maintainers merge your PR into the *staging* branch.</span></span> <span data-ttu-id="8525c-162">Мы периодически отправляем все фиксации из *промежуточной* ветви в *активную* ветвь.</span><span class="sxs-lookup"><span data-stu-id="8525c-162">We periodically push all commits from *staging* branch into the *live* branch.</span></span> <span data-ttu-id="8525c-163">После публикации вашего вклада его можно увидеть на [сайте документации по PowerShell](https://docs.microsoft.com/PowerShell/).</span><span class="sxs-lookup"><span data-stu-id="8525c-163">Once your contribution is live, you can see it in the [PowerShell docs site](https://docs.microsoft.com/PowerShell/).</span></span> <span data-ttu-id="8525c-164">Обычно мы публикуем изменения два или три раза в течение рабочей недели.</span><span class="sxs-lookup"><span data-stu-id="8525c-164">Typically, we publish a two to three times during the work week.</span></span>

## <a name="contributor-license-agreement"></a><span data-ttu-id="8525c-165">Лицензионное соглашение с участником</span><span class="sxs-lookup"><span data-stu-id="8525c-165">Contributor license agreement</span></span>

<span data-ttu-id="8525c-166">Подпишите [лицензионное соглашение с участником](https://cla.opensource.microsoft.com/MicrosoftDocs/PowerShell-Docs) до слияния вашего запроса на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="8525c-166">You must sign the [Contribution License Agreement (CLA)](https://cla.opensource.microsoft.com/MicrosoftDocs/PowerShell-Docs) before your PR is merged.</span></span> <span data-ttu-id="8525c-167">При работе над нашей документацией это достаточно сделать один раз.</span><span class="sxs-lookup"><span data-stu-id="8525c-167">This is a one-time requirement when contributing to our documentation.</span></span>

<span data-ttu-id="8525c-168">Не нужно подписывать соглашение заранее.</span><span class="sxs-lookup"><span data-stu-id="8525c-168">You don't have to sign the agreement up-front.</span></span> <span data-ttu-id="8525c-169">Вы может клонировать, создать вилку и отправить запрос на вытягивание, как обычно.</span><span class="sxs-lookup"><span data-stu-id="8525c-169">You can clone, fork, and submit your PR as usual.</span></span>
<span data-ttu-id="8525c-170">При создании запроса на вытягивание он классифицируется ботом лицензионного соглашения с участником.</span><span class="sxs-lookup"><span data-stu-id="8525c-170">When your PR is created, it is classified by a CLA bot.</span></span> <span data-ttu-id="8525c-171">Если изменение незначительное (например, вы исправили опечатку), запрос на вытягивание помечается тегом `cla-not-required`.</span><span class="sxs-lookup"><span data-stu-id="8525c-171">If the change is small (for example, you fixed a typo), then the PR is labeled with `cla-not-required`.</span></span> <span data-ttu-id="8525c-172">В противном случае он классифицируется как `cla-required`.</span><span class="sxs-lookup"><span data-stu-id="8525c-172">Otherwise, it's classified as `cla-required`.</span></span> <span data-ttu-id="8525c-173">Когда вы подпишете лицензионное соглашение с участником, текущий и все последующие запросы на вытягивание помечаются тегом `cla-signed`.</span><span class="sxs-lookup"><span data-stu-id="8525c-173">Once you signed the CLA, the current and all future pull requests are labeled as `cla-signed`.</span></span>