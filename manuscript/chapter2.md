# 相关概念和信息

## 用户数据目录
初次运行 Sublime Text 的时候，会在你的系统中创建一个`用户数据目录`，用来存储一些用户的设置、扩展包，扩展包的设置信息等。不同的系统拥有不同的路径：

* Windows: %APPDATA%\Sublime Text 3
* Linux: ~/.config/sublime-text-3”
* OS X: ~/Library/Application Support/Sublime Text 3

在该目录下面，可能会存在以下几个主要的目录：

* Installed Packages: 这里一般是一些自带的或者自行安装的第三方的扩展包文件，一般是「打包」后的文件，以 `.sublime-package` 为后缀名。
* Packages：这里存的一般是一些没有被「打包」的扩展。
* Local：这里存储了一些回话信息，用户实现 Sublime Text 独有的「热重启」功能等（后续讲到）。

随着你安装的第三方扩展增多，这个`用户数据目录`下面可能还会有其他的目录出现，不过那些目录一般不会是我们的主要关注点。

日常使用中，我们需要关注的目录，其实就是 `Packages` 这一个，也就是可以直接从 Sublime Text 菜单栏打开的目录（如果你使用的是 Mac OS X 系统，那么你可以按这样的步骤快速打开这个目录：Sublime Text - Preferences - Browser Packages）。

特别的，在这个目录中有一个比较特殊的目录，叫做 `User`，这个目录中包含了所有的你的个人设置，包括 Sublime Text 本身的配置信息，以及各种扩展插件的设置，亦或者是你自己定制的主题等等。你会在 Sublime Text 的菜单中轻易地发现，无论是 Sublime Text 自己，还是其他的各种扩展插件，它们的「设置」菜单一般都会包含两项「Settings - Default」，「Settings - User」，其中 Default，顾名思义是默认的配置，那么 User 即是我们自己的配置了。所有你点开 User 这一项后进行的设置，对应的设置文件都会存于上述的 `Packages/User` 目录下。

## 小技巧

### 如何配置
如上文所说，编辑器本身和插件都会含有 Default 和 User 两项配置菜单，当你点击 User 这一项后，编辑器会打开一个文件供你编辑，当你执行保存操作后，编辑器会自行在 `Packages/User` 目录下生成一个后缀名为 `.sublime-settings` 配置文件。在绝大多数的时间里，这个文件会是空白的，那么，最简单的方法就是同时再点击 Default 打开一份它的默认配置，然后将其全选，复制到 User 那个空白文件中，这样，后面再进行调整的时候，即可以直接修改 User 那份了。当然，有经验的用户也可以直接手动编写 User 那份配置文件，在 Sublime Text 的世界里，配置文件一般都是 JSON 文件，相信很多人都不陌生了。

要注意的是，千万不要直接编辑 Default 那份配置文件，因为一旦编辑器和插件更新，这个 Default 对应的文件会被直接覆盖，只有 `User/Packages` 下面的文件才不会被覆盖掉。


### 如何同步配置
有了上面的基础，相信你应该大概知道如何备份了

__Git__
如果你想要使用 Git 来同步备份设置，只需将 User 目录创建为 repo ，然后执行同步即可。

__Dropbox__
使用同步网盘就更简单了，在 Dropbox 中创建目录 `User` 将 `Packages/User` 下文件全部复制到 Dropbox 下的 User 目录中，然后删除 `Packages` 下的 `User` 目录，最后创建软连接，eg: `ln -s ~/Dropbox/User ~/Library/Application Support/Sublime Text 3/Packages/`。
