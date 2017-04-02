# 学习关系型数据库的贴士和技巧 {#-}

Karl 将指导你学习这门课程的关系数据库部分。在学习之前，请阅读一些实用的虚拟机资源，这些资源将在你成为后端程序员的过程中帮助到你。

## 什么是虚拟机？ {#-}

在这门课程中，Karl 使用 Vagrant 创建了虚拟机。虚拟机是一种存在于本地机器上的虚拟计算机系统。它具有虚拟硬件设备，就像在实际的机器上运行一样。这种虚拟计算机系统会通过单独的窗口运行于当前的操作系统上，对于 Vagrant 来说，通过命令行来运行。

### Vagrant：你需要了解的所有知识！ {#vagrant-}

Vagrant 是一个与[VirtualBox](https://www.virtualbox.org/)产生接口的命令行工具，使得配置和创建虚拟机变得异常简单。

### 为何要使用 Vagrant？ {#-vagrant-}

因为 Vagrant 操作简单，易于使用。它符合行业标准，可以帮助你习惯于在命令行中操作！

### 指令概述 {#-}

下面是使用 Vagrant 时需要知道的基本指令：

* `vagrant init`：在当前目录下创建新的 Vagrantfile
* `vagrant up`: 启动虚拟机
* `vagrant ssh`: 通过 SSH 连接到虚拟机
* `vagrant halt`: 停止虚拟机
* `vagrant destroy`: 停止并删除虚拟机（将删除所有相关的文件）
* `vagrant status`：显示虚拟机的状态

在终端中输入`vagrant help`即可了解详情！

### 常见问题解答 {#-}

虽然我们喜欢 Vagrant，因为它使用简单。但是也会出现问题。下面是一些常见问题和相应的解决方案：

* “我在我的项目目录下运行了
  `vagrant up && vagrant ssh`，但是现在当我输入`ls`，我看不到任何文件！什么情况？”
  * 你的所有操作都是正确的，你只是没有位于虚拟机中希望位于的文件夹中。直接输入
    `cd /vagrant`即可查看你的项目文件。你也可以使用`pwd`随时检查你是否位于正确的位置！
* “当我运行
  `vagrant ssh`时，为何什么也没发生/为何出现错误消息？”
  * 检查确保你位于正确的目录下！通过`cd`指令进入包含你要使用的 Vagrant 文件的文件夹中。此外，确保 VirtualBox 正常运行，处于快速`vagrant 状态`！
* “我使用的是 Windows 机器，当我运行任何指令时，Vagrant 似乎都卡住了，什么情况？”
  * 该问题通常都是许可权限造成的；也许你以管理员的身份启动了 VirtualBox 并尝试以普通用户的身份使用 Vagrant，或者是相反的情况。解决办法很简单：关闭所有虚拟机，关闭 VirtualBox，然后以运行 Vagrant 时希望成为的身份重新打开 VirtualBox。另请参阅[这篇](http://windows.microsoft.com/en-us/windows7/how-do-i-run-an-application-once-with-a-full-administrator-access-token)关于如何以管理员的身份运行应用程序的文章。
* “DNS 不能运行，请帮助我！”
  * 要解决 DNS 问题，可能需要启用代理。请参阅[这个很棒的讨论话题](https://serverfault.com/questions/453185/vagrant-virtualbox-dns-10-0-2-3-not-working)以获取帮助！

要了解更多内容，请参阅下面的资源：

1. [Vagrant 教程](http://blog.osteel.me/posts/2015/01/25/how-to-use-vagrant-for-local-web-development.html)
2. [Vagrant 功能网络直播](https://plus.google.com/events/ca6ndfsdj4timcjplsfcqlh1vmc?authkey=CLCDip6m-KmeBQ)
3. [官方 Vagrant 文档](https://www.vagrantup.com/docs/)
4. [《关系数据库入门》之如何设置 Vagrant](https://www.udacity.com/wiki/ud197/install-vagrant)

现在你已经深入了解虚拟机器了，我们开始学习关系数据库吧！

