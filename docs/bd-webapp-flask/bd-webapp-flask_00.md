# 前言

在我们“现在的世界”中，人们几乎无法开发新的应用程序而不将许多技术粘合在一起，无论是新趋势数据库，消息系统还是各种语言。 谈到 Web 开发，事情可能会变得稍微复杂，因为你不仅必须将许多技术混合在一起，而且它们还必须与访问它们的应用程序（也称为 Web 浏览器）良好地配合。 它们还应与您的部署服务器兼容，这本身又是另一回事！

在 Python 世界中，人们遵循 Python 之禅和 PEP8 等伟大准则，交付令人惊叹的桌面软件，我们可以利用各种库和框架来创建出色的 Web 应用程序，每个都有其自己的哲学。 例如，Django 是一个捆绑解决方案； 它为您做出了关于项目应该如何看起来，应该有什么，以及应该如何完成事情的选择。 Web2py 是另一个框架解决方案，甚至将 IDE 与其捆绑在一起。 这些都是很好的概念，但如果您想创建一些简单的东西，我建议您在其他地方做。 它们通常是很好的选择，但有时它们只是太多了（最新的 Django 版本似乎决定改变这一点； 让我们密切关注进一步的发展）。

Flask 定位自己不是像 Django 和 Web2py 那样的开箱即用的解决方案，而是一个最简解决方案，你只得到最基本的东西，然后选择其他所有的东西。 当你想要对应用程序进行细粒度控制时，当你想要精确选择你的组件时，或者当你的解决方案很简单时（不是简化的，好吗？）。

这本书是对 Web 世界中美丽代码和许多选择的情景的回应。 它试图解决与 Web 开发相关的主要问题，从安全性到内容交付，从会话管理到 REST 服务和 CRUD。 还涵盖了重要的现代概念，如过度工程，质量和开发过程，以便从第一天起获得更好的结果。 为了使学习过程顺利进行，主题都是在不着急的情况下呈现，并附有注释示例。 该书还旨在为读者提供有关如何预防代码常见问题的现实建议。

来学习如何创建出色的 Flask 应用程序，为您的项目和客户提供价值！

# 本书涵盖的内容

第一章《Flask in a Flask, I Mean, Book》向你介绍了 Flask，解释了它是什么，它不是什么，以及它在 Web 框架世界中的定位。

第二章《First App, How Hard Could it Be?》涵盖了通往 Flask 开发的第一步，包括环境设置，你自己的“Hello World”应用程序，以及模板如何进入这个方程式。 这是一个轻松的章节！

第三章《Man, Do I Like Templates!》介绍了面部标签和过滤器在 Jinja2 模板引擎中的进展，以及它如何与 Flask 集成。 从这里开始事情开始变得有点严肃！

第四章《Please Fill in This Form, Madam》讨论了如何处理表单（因为表单是 Web 开发生活中的一个事实），并使用 WTForms 以其全部荣耀来对待它们！

第五章《Where Do You Store Your Stuff?》介绍了关系型和非关系型数据库的概念，涵盖了如何处理这两种情况，以及何时处理。

第六章《But I Wanna REST Mom, Now!》是关于创建 REST 服务的一章（因为 REST 的热情必须得到满足），手动创建和使用令人惊叹的 Flask-Restless。

第七章，“如果没有经过测试，就不是游戏，兄弟！”，是我们以质量为中心的章节，您将学习通过适当的测试、TDD 和 BDD 方式提供质量！

第八章，“技巧和窍门或 Flask 魔法 101”，是一个密集的章节，涵盖了良好的实践、架构、蓝图、调试和会话管理。

第九章，“扩展，我是如何爱你”，涵盖了到目前为止尚未涉及的所有伟大的 Flask 扩展，这些扩展将帮助您实现现实世界对您的生产力要求。

第十章，“现在怎么办？”，结束了我们的开发之旅，涵盖了健康部署的所有基础知识，并指引您在 Flask 世界中迈出下一步。

# 您需要为本书做好准备

为了充分利用阅读体验，读者应该准备一台安装了 Ubuntu 14.x 或更高版本的机器，因为示例是为这种设置设计的，还需要对 Python 有基本的了解（如果您没有，请先参考[`learnxinyminutes.com/docs/python/`](http://learnxinyminutes.com/docs/python/)），以及一个带有您喜欢的高亮显示的文本编辑器（LightTable，Sublime，Atom）。其他所需软件将在各章讨论中介绍。

# 这本书是为谁准备的

本书面向 Python 开发人员，无论是有一些或没有 Web 开发经验的人，都希望创建简约的 Web 应用程序。它专注于那些希望成为 Web 开发人员的人，因为所有基础知识都在一定程度上得到了涵盖，也专注于那些已经熟悉使用其他框架进行 Web 开发的人，无论是基于 Python 的框架，如 Django、Bottle 或 Pyramid，还是其他语言的框架。 

同样重要的是，您要对用于构建网页的 Web 技术有基本的了解，比如 CSS、JavaScript 和 HTML。如果这不是您的背景，请查看 W3Schools 网站（[`w3schools.com/`](http://w3schools.com/)），因为它涵盖了使用这些技术的基础知识。此外，如果您熟悉 Linux 终端，整本书的学习将会更加轻松；如果不是这种情况，请尝试链接[`help.ubuntu.com/community/UsingTheTerminal`](https://help.ubuntu.com/community/UsingTheTerminal)。

尽管如此，请放心，如果您对 Python 有基本的了解，您完全有能力理解示例和章节；在本书结束时，您将创建出表现良好且易于维护的令人惊叹的 Web 应用程序。

# 约定

在本书中，您将找到一些区分不同信息类型的文本样式。以下是一些这些样式的示例，以及它们的含义解释。

文本中的代码单词、数据库表名、文件夹名、文件名、文件扩展名、路径名、虚拟 URL、用户输入和 Twitter 句柄显示如下：“进入新项目文件夹并创建`main.py`文件”。

代码块设置如下：

```py
# coding:utf-8
from flask import Flask
app = Flask(__name__)

@app.route("/")
def hello():
    return "Hello World!"

if __name__ == "__main__":
    app.run()
```

任何命令行输入或输出都以以下形式编写：

```py
sudo pip install virtualenvwrapper

```

**新术语**和**重要单词**以粗体显示。您在屏幕上看到的单词，比如菜单或对话框中的单词，会以这样的形式出现在文本中：“您有没有想象过在网站上填写表单并在末尾点击那个花哨的**发送**按钮时会发生什么？”。

### 注意

警告或重要说明会以这样的方式出现在框中。

### 提示

提示和技巧会以这样的方式出现。