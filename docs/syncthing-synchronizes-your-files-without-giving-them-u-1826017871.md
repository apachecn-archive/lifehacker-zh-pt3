# 使用 Syncthing 同步您的文件，而无需将它们交给第三方服务

> 原文:[https://life hacker . com/sync thing-synchronizes-your-files-without-giving-them-u-1826017871](https://lifehacker.com/syncthing-synchronizes-your-files-without-giving-them-u-1826017871)

Dropbox、Google Drive 或任何你用来将文件备份到云并在你的多台台式机和笔记本电脑之间保持同步的流行服务本身没有任何问题。然而，数据隐私正变得越来越重要，如果你准备好从这些类型的服务中跳出来，我们不会质疑你。

Watch

开源实用工具 Syncthing 是一种很好的方式，可以获得本地文件同步的所有好处，而不必将您的数据交给另一家公司(无论他们多么承诺永远不会查看这些数据)。代价是 Syncthing 比 Dropbox 这样的服务更难管理，这使得在所有设备上上传、下载和同步文件变得非常容易。

### 切换到 Syncthing 需要一些设置

首先，前往 Syncthing 的网站 并寻找 [SyncTrayzor](https://github.com/canton7/SyncTrayzor/releases/tag/v1.1.21) 的链接，这是一个 windows 实用程序，允许你通过漂亮的 GUI 而不是令人头痛的命令行来使用该程序。下载适合您的 Windows PC (32 位或 64 位)的版本，或者如果您想与众不同，可以下载便携式版本，然后安装(或运行)该应用程序。在每台想要纳入大型文件同步计划的计算机上重复该过程。

当您启动 SyncTrayzor 时，您首先需要将所有发送和接收文件的不同系统连接在一起。为了简单起见，我们将假设我们正在链接两台 Windows 桌面 PC:系统 A 和系统 b。

在系统 A 上，单击“添加远程设备”按钮。在系统 B 上，单击右上角的 Actions 按钮并选择“Show ID”将系统 B 中过长的设备识别码复制到系统 a 的设备 ID 字段中。输入系统 B 的设备名称(如“Laptop”)点击保存。

现在，反向重复此过程—使用系统 A 的设备 ID 将系统 A 添加到系统 B 的 SyncTrayzor 版本中。把这个过程想象成在你的两个设备之间建立友谊。如果双方都不想成为朋友，他们就不会交换秘密。但是，如果每个人都能认出对方，他们就会一直聊下去。

明白了吗？现在，在你的一台电脑(比如说系统 A)上安装 SyncTrayzor，点击应用程序左上角的“添加文件夹”按钮。选择您想要在多个系统之间同步的文件夹，给它一个您可以识别的文件夹标签(名称)，然后选择您想要共享该文件夹的设备。对每个你想要同步的文件夹重复这个过程(或者只是在某个地方创建一个名为“Sync”的新文件夹，把你所有的东西都放在那里，Dropbox 风格)。

从理论上讲，SyncTrayzor 现在应该开始在您选择的所有系统上自动转储您的同步文件夹。如果它完全搞砸了，或者看起来不起作用，请确保您没有某种 [内部网络问题](https://docs.syncthing.net/users/firewall.html#firewall-setup) 把事情搞砸了。您也可以从“操作”菜单重新启动 SyncTrayzor，这可能会解决任何(或所有)系统上的问题。