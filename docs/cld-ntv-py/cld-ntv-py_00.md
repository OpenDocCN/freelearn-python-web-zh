# 前言

如今的企业发展如此迅速，以至于拥有自己的基础架构来支持扩张已经不可行。因此，它们一直在利用云的弹性来提供一个构建和部署高度可扩展应用的平台。

这本书将是你学习如何在 Python 中构建云原生架构的一站式书籍。它将首先向你介绍云原生架构，并帮助你分解它。然后你将学习如何使用事件驱动方法在 Python 中构建微服务，并构建 Web 层。接下来，你将学习如何与数据服务交互，并使用 React 构建 Web 视图，之后我们将详细了解应用安全性和性能。然后，你还将学习如何将你的服务 Docker 化。最后，你将学习如何在 AWS 和 Azure 平台上部署应用。我们将以讨论一些关于部署后应用可能出现的问题的概念和技术来结束本书。

这本书将教会你如何构建作为小型标准单元的应用，使用所有经过验证的最佳实践，并避免通常的陷阱。这是一本实用的书；我们将使用 Python 3 及其令人惊叹的工具生态系统来构建一切。本书将带你踏上一段旅程，其目的地是基于云平台的微服务构建完整的 Python 应用程序。

# 本书涵盖的内容

第一章《介绍云原生架构和微服务》讨论了基本的云原生架构，并让你准备好构建应用程序。

第二章《使用 Python 构建微服务》为你提供了构建微服务和根据你的用例扩展它们的完整知识。

第三章《使用 Python 构建 Web 应用程序》构建了一个与微服务集成的初始 Web 应用程序。

第四章《与数据服务交互》让你亲自了解如何将你的应用迁移到不同的数据库服务。

第五章《使用 React 构建 Web 视图》讨论了如何使用 React 构建用户界面。

第六章《使用 Flux 创建可扩展的 UI》让你了解了用于扩展应用的 Flux。

第七章《学习事件溯源和 CQRS》讨论了如何以事件形式存储交易以提高应用性能。

第八章《保护 Web 应用程序》帮助你保护应用程序免受外部威胁。

第九章《持续交付》让你了解频繁应用发布的知识。

第十章《将你的服务 Docker 化》讨论了容器服务和在 Docker 中运行应用程序。

第十一章《在 AWS 平台上部署》教会你如何在 AWS 上为你的应用构建基础架构并设置生产环境。

第十二章《在 Azure 平台上实施》讨论了如何在 Azure 上为你的应用构建基础架构并设置生产环境。

第十三章《监控云应用》让你了解不同的基础架构和应用监控工具。

# 你需要为这本书做好什么准备

您需要在系统上安装 Python。最好使用文本编辑器 Vim/Sublime/Notepad++。在其中一章中，您可能需要下载 POSTMAN，这是一个强大的 API 测试套件，可作为 Chrome 扩展程序使用。您可以在[`chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop?hl=en`](https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop?hl=en)下载。

除了这些之外，如果您在以下网络应用程序上有账户，那将是很好的：

+   Jenkins

+   Docker

+   亚马逊网络服务

+   Terraform

如果您没有账户，这本书将指导您，或者至少指导您如何在先前提到的网络应用程序上创建账户。

# 这本书是为谁写的

这本书适用于具有 Python 基础知识、命令行和基于 HTTP 的应用程序原理的开发人员。对于那些想要学习如何构建、测试和扩展他们的基于 Python 的应用程序的人来说，这本书是理想的选择。不需要有 Python 编写微服务的先前经验。 

# 约定

在这本书中，您将找到一些文本样式，用于区分不同类型的信息。以下是一些样式的示例及其含义的解释。

文本中的代码单词、数据库表名、文件夹名、文件名、文件扩展名、路径名、虚拟 URL、用户输入和 Twitter 用户名显示如下：“创建一个`signup`路由，该路由将使用`GET`和`POST`方法读取页面，并将数据提交到后端数据库。”

代码块设置如下：

```py
    sendTweet(event){
      event.preventDefault();
      this.props.sendTweet(this.refs.tweetTextArea.value); 
      this.refs.tweetTextArea.value = '';
    } 

```

任何命令行输入或输出都以以下方式编写：

```py
$ apt-get install nodejs

```

**新术语**和**重要单词**以粗体显示。您在屏幕上看到的单词，例如菜单或对话框中的单词，会以这种方式出现在文本中：“单击“创建用户”按钮，用户将被创建，并且策略将附加到其中。”

警告或重要说明会以这种方式出现。

技巧和窍门会以这种方式出现。
