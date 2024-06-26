# 前言

Django 框架专门设计用于帮助开发人员快速高效地构建强大的 Web 应用程序。它大大减少了繁琐的工作和重复的过程，解决了项目结构、数据库对象关系映射、模板化、表单验证、会话、身份验证、安全、cookie 管理、国际化、基本管理和从脚本访问数据的接口等问题。Django 是建立在 Python 编程语言之上的，Python 本身强制执行清晰易读的代码。除了核心框架，Django 还被设计为使开发人员能够创建可与自己的应用程序一起使用的第三方模块。Django 拥有一个成熟和充满活力的社区，您可以在其中找到源代码、获得帮助并做出贡献。

*Django 3 Web Development Cookbook, Fourth Edition*，将指导您使用 Django 3.0 框架完成 Web 开发过程的每个阶段。我们从项目的配置和结构开始。然后，您将学习如何使用可重用组件定义数据库结构，并在项目的整个生命周期中进行管理。本书将继续介绍用于输入和列出数据的表单和视图。我们将继续使用响应式模板和 JavaScript 来增强用户体验。然后，我们将通过自定义过滤器和标签增强 Django 的模板系统，以便更灵活地进行前端开发。之后，您将调整管理界面，以简化内容编辑者的工作流程。接下来，我们将关注项目的稳定性和健壮性，帮助您保护和优化应用程序。接下来，我们将探讨如何高效地存储和操作分层结构。然后，我们将演示从不同来源收集数据并以各种格式提供您自己的数据比您想象的简单。然后，我们将向您介绍一些用于编程和调试 Django 项目代码的技巧。我们将继续介绍一些可用于测试代码的选项。在本书结束之前，我们将向您展示如何将项目部署到生产环境。最后，我们将通过设置常见的维护实践来完成开发周期。

与许多其他 Django 书籍相比，这些书籍只关注框架本身，而本书涵盖了几个重要的第三方模块，这些模块将为您提供完成网站开发所需的工具。此外，我们提供了使用 Bootstrap 前端框架和 jQuery JavaScript 库的示例，这两者都简化了高级和复杂用户界面的创建。

# 本书适合人群

如果您有 Django 经验并希望提高技能，这本书适合您。我们设计了中级和专业 Django 开发人员的内容，他们的目标是构建多语言、安全、响应迅速且能够随时间推移扩展的强大项目。

# 本书内容包括

第一章，*开始使用 Django 3.0*，说明了任何 Django 项目所需的基本设置和配置步骤。我们涵盖了虚拟环境、Docker 以及跨环境和数据库的项目设置。

第二章，*模型和数据库结构*，解释了如何编写可重用的代码，用于构建模型。新应用程序的首要事项是定义数据模型，这构成了任何项目的支柱。您将学习如何在数据库中保存多语言数据。此外，您还将学习如何使用 Django 迁移管理数据库模式更改和数据操作。

第三章，*表单和视图*，展示了构建用于数据显示和编辑的视图和表单的方法。您将学习如何使用微格式和其他协议，使您的页面对机器更易读，以便在搜索结果和社交网络中表示。您还将学习如何生成 PDF 文档并实现多语言搜索。

第四章，*模板和 JavaScript*，涵盖了一起使用模板和 JavaScript 的实际示例。我们将这些方面结合起来：渲染的模板向用户呈现信息，而 JavaScript 为现代网站提供了关键的增强功能，以实现丰富的用户体验。

第五章，*自定义模板过滤器和标签*，介绍了如何创建和使用自己的模板过滤器和标签。正如您将看到的，默认的 Django 模板系统可以扩展以满足模板开发人员的需求。

第六章，*模型管理*，探讨了默认的 Django 管理界面，并指导您如何通过自己的功能扩展它。

第七章，*安全性和性能*，深入探讨了 Django 内在和外部的几种方式，以确保和优化您的项目。

第八章，*分层结构*，探讨了在 Django 中创建和操作类似树的结构，以及将`django-mptt`或`treebeard`库纳入此类工作流程的好处。本章向您展示了如何同时用于层次结构的显示和管理。

第九章，*导入和导出数据*，演示了数据在不同格式之间的传输，以及在各种来源之间的提供。在本章中，使用自定义管理命令进行数据导入，并利用站点地图、RSS 和 REST API 进行数据导出。

第十章，*花里胡哨*，展示了在日常网页开发和调试中有用的一些额外片段和技巧。

第十一章，*测试*，介绍了不同类型的测试，并提供了一些特征示例，说明如何测试项目代码。

第十二章，*部署*，涉及将第三方应用程序部署到 Python 软件包索引以及将 Django 项目部署到专用服务器。

第十三章，*维护*，解释了如何创建数据库备份，为常规任务设置 cron 作业，并记录事件以供进一步检查。

# 为了充分利用本书

要使用本书中的示例开发 Django 3.0，您需要以下内容：

+   Python 3.6 或更高版本

+   用于图像处理的**Pillow**库

+   要么使用 MySQL 数据库和`mysqlclient`绑定库，要么使用带有`psycopg2-binary`绑定库的 PostgreSQL 数据库

+   Docker Desktop 或 Docker Toolbox 用于完整的系统虚拟化，或者内置虚拟环境以保持每个项目的 Python 模块分开

+   用于版本控制的 Git

| **书中涵盖的软件/硬件** | **操作系统建议** |
| --- | --- |

| Python 3.6 或更高版本 Django 3.0.X

PostgreSQL 11.4 或更高版本/MySQL 5.6 或更高版本|任何最近的基于 Unix 的操作系统，如 macOS 或 Linux（尽管也可以在 Windows 上开发）

所有其他特定要求都将在每个配方中单独提到。

**如果您使用的是本书的数字版本，我们建议您自己输入代码或通过 GitHub 存储库访问代码（链接在下一节中提供）。这样做将有助于避免与复制/粘贴代码或不正确缩进相关的任何潜在错误。**

对于编辑项目文件，您可以使用任何代码编辑器，但我们建议使用**PyCharm**（[`www.jetbrains.com/pycharm/`](https://www.jetbrains.com/pycharm/)）或**Visual Studio Code**（[`code.visualstudio.com/`](https://code.visualstudio.com/)）。

如果您成功发布了 Django 项目，我会非常高兴，如果您能通过电子邮件与我分享您的结果、经验和成果，我的电子邮件是 aidas@bendoraitis.lt。

所有代码示例都经过了 Django 3 的测试。但是，它们也应该适用于将来的版本发布。

# 下载示例代码文件

您可以从 [www.packt.com](http://www.packt.com) 的帐户中下载本书的示例代码文件。如果您在其他地方购买了本书，您可以访问 [www.packtpub.com/support](https://www.packtpub.com/support) 并注册，以便直接通过电子邮件接收文件。

您可以按照以下步骤下载代码文件：

1.  在 [www.packt.com](http://www.packt.com) 上登录或注册。

1.  选择 Support 选项卡。

1.  点击 Code Downloads。

1.  在 Search 框中输入书名，然后按照屏幕上的说明进行操作。

一旦文件下载完成，请确保使用最新版本的解压缩或提取文件夹：

+   WinRAR/7-Zip for Windows

+   Zipeg/iZip/UnRarX for Mac

+   7-Zip/PeaZip for Linux

该书的代码包也托管在 GitHub 上，网址为 [`github.com/PacktPublishing/Django-3-Web-Development-Cookbook-Fourth-Edition`](https://github.com/PacktPublishing/Django-3-Web-Development-Cookbook-Fourth-Edition)。如果代码有更新，将在现有的 GitHub 存储库上进行更新。

我们还有其他代码包来自我们丰富的图书和视频目录，可在 **[`github.com/PacktPublishing/`](https://github.com/PacktPublishing/)** 上找到。请查看！

# 使用的约定

本书中使用了许多文本约定。

`CodeInText`：表示文本中的代码词、数据库表名、文件夹名、文件名、文件扩展名、路径名、虚拟 URL、用户输入和 Twitter 句柄。例如："为了使这个配方起作用，您需要安装 `contenttypes` 应用程序。"

代码块设置如下：

```py
# requirements/dev.txt
-r _base.txt
coverage
django-debug-toolbar
selenium
```

当我们希望引起您对代码块的特定部分的注意时，相关行或项目将以粗体显示：

```py
class Idea(CreationModificationDateBase, MetaTagsBase, UrlBase):
    title = models.CharField(
        _("Title"),
        max_length=200,
    )
    content = models.TextField(
        _("Content"),
    )
```

任何命令行输入或输出都以以下方式编写：

```py
(env)$ pip install -r requirements/dev.txt
```

**粗体**：表示新术语、重要单词或屏幕上看到的单词。例如，菜单或对话框中的单词会以这种方式出现在文本中。例如："我们可以看到这里与上传相关的操作按钮也被替换为了一个 Remove 按钮。"

警告或重要说明会以这种方式出现。

技巧和窍门会以这种方式出现。

# 章节

在本书中，您会经常看到几个标题（*准备工作*、*如何做...*、*它是如何工作的...*、*还有更多...* 和 *另请参阅*）。

为了清晰地说明如何完成一个配方，使用以下各节：

# 准备工作

本节告诉您应该期望在配方中发生什么，并描述了为配方设置任何软件或任何必需的预设置所需的步骤。

# 如何做...

本节包含了遵循配方所需的步骤。

# 它是如何工作的...

本节通常包括对前一节中发生的事情的详细解释。

# 还有更多...

本节包括有关配方的其他信息，以增加您对其的了解。

# 另请参阅

本节提供了有关配方的其他有用信息的链接。
