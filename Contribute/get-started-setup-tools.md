---
title: Установка средств для создания содержимого
description: Эта статья поможет вам скачать и установить клиентские средства, необходимые для редактирования файлов Markdown и работы с Git.
ms.topic: contributor-guide
ms.prod: non-product-specific
ms.custom: external-contributor-guide
author: jasonwhowell
ms.author: jasonh
ms.date: 04/30/2018
ms.openlocfilehash: ba7e511d756f43acfa5cfbbd228f793d7fbce727
ms.sourcegitcommit: cfba5ad25b898bfed76046126ce8ff4871910701
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/04/2020
ms.locfileid: "78331867"
---
# <a name="install-content-authoring-tools"></a>Установка средств для создания содержимого

В этой статье объясняется, как установить клиентские средства Git и Visual Studio Code в интерактивном режиме.
> [!div class="checklist"]
> * Установка [Git](https://git-scm.com/)
> * Установка [Visual Studio Code](https://code.visualstudio.com/).
> * Установка [пакета создания документации](https://marketplace.visualstudio.com/items?itemName=docsmsft.docs-authoring-pack).

>[!IMPORTANT]
> Если вы вносите в статью лишь небольшие изменения, вам *не* нужно выполнять описанные здесь шаги. Вы можете сразу перейти к [рабочему процессу по внесению быстрых изменений](index.md#quick-edits-to-existing-documents).
>
> Участникам, которые вносят много изменений, рекомендуется выполнить инструкции, которые позволят применить [рабочий процесс по внесению значительных или времязатратных изменений](how-to-write-workflows-major.md). Даже если у вас есть разрешения на запись в основном репозитории, *настоятельно рекомендуется (и в этом руководстве предполагается, что вы это сделаете) создать вилку и клон репозитория*, чтобы у вас были права на чтение и запись для хранения в этой вилке предлагаемых вами изменений.

## <a name="install-git-client-tools"></a>Установка клиентских средств для Git 

 Установите последнюю версию [клиентских средств Git от Software Freedom Conservancy](https://git-scm.com/download/) для своей платформы. 

* [Git для Windows](https://git-scm.com/download/win). Пакет установки включает систему управления версиями Git и приложение командной строки Git Bash, используемое для взаимодействия с локальным репозиторием Git.
* Git для Mac предоставляется как часть средств командной строки Xcode. Просто запустите `git` из командной строки. При необходимости вам будет предложено установить средства командной строки. Вы также можете скачать [Git для Mac](https://git-scm.com/download/mac) из Software Freedom Conservancy.
* [Git для Linux и Unix](https://git-scm.com/download/linux)

Если вы предпочитаете использовать графический пользовательский интерфейс вместо интерфейса командной строки, см. сведения о часто используемых параметрах на странице [доступных средств графического пользовательского интерфейса Software Freedom Conservancy](https://git-scm.com/downloads/guis), на сайте [версии GitHub для настольного компьютера](https://desktop.github.com/) или на сайте [Visual Studio Code](https://www.visualstudio.com/products/code-vs.aspx).

Следуйте инструкциям по установке и настройке для выбранного клиента.

В следующей статье вы [настроите локальный репозиторий Git](get-started-setup-local.md).

   Дополнительные ресурсы по Git см. здесь: [Глоссарий GitHub ](https://help.github.com/articles/github-glossary) | [Базовые возможности Git](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics) | [Обучающие ресурсы по Git и GitHub](https://help.github.com/articles/good-resources-for-learning-git-and-github/).

## <a name="understand-markdown-editors"></a>Сведения о редакторах Markdown

Markdown — это упрощенный язык разметки, который легко использовать и осваивать. Поэтому он быстро стал отраслевым стандартом. Чтобы писать статьи на языке Markdown, мы рекомендуем скачать и установить Markdown editor.  [Visual Studio Code](https://code.visualstudio.com/) — предпочтительное средство для редактирования разметки Markdown в Майкрософт. [Atom](https://atom.io) — еще одно популярное средство для редактирования разметки Markdown.

Тексты с разметкой Markdown сохраняются в файлы с расширением MD.

Дополнительные сведения о написании кода на языке Markdown, включая основные сведения о Markdown и функциях, которые поддерживаются настраиваемыми расширениями OPS для Markdown, см. в статье [Справочник по Markdown](markdown-reference.md).

## <a name="visual-studio-code"></a>Visual Studio Code

[Visual Studio Code](https://code.visualstudio.com/) (также называется VS Code) — это простой редактор, который работает в Windows, Linux и Mac. Он включает интеграцию с Git и поддержку расширений.

Скачайте и установите [VS Code](https://code.visualstudio.com/). На главной странице VS Code должна правильно определиться ваша операционная система:

- [Windows](https://code.visualstudio.com/docs/setup/windows);
- [Mac](https://code.visualstudio.com/docs/setup/mac);
- [Linux](https://code.visualstudio.com/docs/setup/linux).

> [!TIP]
> Чтобы запустить VS Code и открыть текущую папку, выполните команду `code .` в командной строке или оболочке Bash. Если текущая папка содержится в локальном репозитории Git, в Visual Studio Code автоматически отобразятся данные об интеграции с GitHub.

## <a name="docs-authoring-pack"></a>Пакет создания документации
Установите пакет Docs Authoring Pack для создания документации для Visual Studio Code. Этот набор расширений предоставляет основные средства для редактирования документов на языке Markdown и включает функцию предварительного просмотра, которая позволяет оценить соответствие стилю docs.microsoft.com.

   На странице [Marketplace](https://marketplace.visualstudio.com/items?itemName=docsmsft.docs-authoring-pack) выберите **Install** (Установить) или в VS Code в списке расширений найдите `docsmsft.docs-authoring-pack`.   

   В VS Code пакет Docs Authoring Pack можно открыть с помощью клавиш ALT+M. Панель инструментов по умолчанию скрыта. Чтобы отобразить ее, измените настройки VS Code (CTRL+запятая) при помощи настраиваемого параметра "markdown.showToolbar": true.

   Дополнительные сведения см. на странице справки по [Docs Authoring Pack](how-to-write-docs-auth-pack.md).


## <a name="next-steps"></a>Дальнейшие действия

Теперь все готово к [настройке локального репозитория](get-started-setup-local.md).
