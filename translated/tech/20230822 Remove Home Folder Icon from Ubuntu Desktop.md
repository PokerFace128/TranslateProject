[#]: subject: "Remove Home Folder Icon from Ubuntu Desktop"
[#]: via: "https://itsfoss.com/ubuntu-remove-home-icon/"
[#]: author: "Abhishek Prakash https://itsfoss.com/author/abhishek/"
[#]: collector: "lujun9972"
[#]: translator: "geekpi"
[#]: reviewer: " "
[#]: publisher: " "
[#]: url: " "

从 Ubuntu 桌面上删除主文件夹图标
======

Ubuntu 使用定制的 GNOME 版本，由于侧边启动器，它的外观与旧的 Unity 桌面有些相似。

普通 GNOME 和 Ubuntu 的 GNOME 之间的另一个区别是桌面上主文件夹和回收站的使用。这些图标就在那里，以便你可以快速访问它们。

![Home folder icon on Ubuntu desktop][1]

如果你觉得不美观，可以从桌面视图中删除主文件夹。

让我分享一下 GUI 和命令行方法。

### 在 Ubuntu 中隐藏桌面上的主文件夹图标

这是你需要做的。

**在 Ubuntu 中按 Super + D [键盘快捷键][2]访问桌面**。

现在**右键单击桌面上的空白区域**。

从右键单击上下文菜单中，**选择桌面图标设置**。

![Right click on the desktop and click the Desktop Icons Settings][3]

它将在“设置”应用中打开 Ubuntu 桌面设置选项。你也可以通过打开“设置”应用并转到侧边栏中的“Ubuntu 桌面”选项来访问它。

在这里，你将看到**显示个人文件夹的切换选项**。将其关闭以禁用桌面上的主文件夹图标。

![Disable the Show Personal folder button][4]

💡

想要恢复主文件夹图标吗？ 再次切换它。

### 使用命令行禁用主文件夹图标

是的，你可以从命令行完全禁用主文件夹图标。

打开终端并使用以下命令。

```

    gsettings set org.gnome.shell.extensions.ding show-home false

```

效果将是立竿见影的。

要恢复图标，请使用相同的命令，但使用 `true` 而不是 `false`：

```

    gsettings set org.gnome.shell.extensions.ding show-home true

```

看到那有多简单了吗？ 也可以采取类似的步骤来删除回收站图标。

![][5]

--------------------------------------------------------------------------------

via: https://itsfoss.com/ubuntu-remove-home-icon/

作者：[Abhishek Prakash][a]
选题：[lujun9972][b]
译者：[geekpi](https://github.com/geekpi)
校对：[校对者ID](https://github.com/校对者ID)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://itsfoss.com/author/abhishek/
[b]: https://github.com/lujun9972
[1]: https://itsfoss.com/content/images/2023/08/home-folder-icon-on-ubuntu-desktop.png
[2]: https://itsfoss.com/ubuntu-shortcuts/
[3]: https://itsfoss.com/content/images/2023/08/access-ubuntu-desktop-icon-settings.png
[4]: https://itsfoss.com/content/images/2023/08/disable-home-folder-icon-on-ubuntu-desktop.png
[5]: https://itsfoss.com/content/images/size/w256h256/2022/12/android-chrome-192x192.png
