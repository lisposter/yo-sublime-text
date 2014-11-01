# 准备工作
在玩转 Sublime Text 之前，我们当然是要准备好必要的东西。

## 下载安装
Sublime Text 是一个跨平台的编辑器，无论你是 Windows、Linux、还是 Mac OS，都能在其官网上找到相应的下载连接。对于我们开发者来说，下载安装根本不是事，在这就不赘述了，访问 Sublime Text 的官网（http://www.sublimetext.com）进行下载安装即可。


## 安装Package Control
Sublime Text 之所以能像现在这样流行，无外乎是因为它拥有不计其数的Package。然后， Sublime Text 自身并没有一个很好的包管理器，因此，我们首先要安装一个包管理器，来管理那些第三方扩展包。Package Control（https://sublime.wbond.net/）便是众望所归的 Sublime Text 包管理器。有趣的是，这个 Sublime Text 最离不开的扩展包却并非是官方开发，而是由第三方社区中的Wbond所开发。

Package Control的安装也很简单：

* 1.使用快捷键 `Ctrl + `` 或者通过菜单 `View > Show Console`打开 Sublime Text 自带的Python终端。
* 2.复制安装代码，然后回车，就会自动安装好 Package Control

__ Sublime Text  3__

```python
import urllib.request,os,hashlib; h = '7183a2d3e96f11eeadd761d777e62404' + 'e330c659d4bb41d3bdf022e94cab3cd0'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

__ Sublime Text  2__

```python
import urllib2,os,hashlib; h = '7183a2d3e96f11eeadd761d777e62404' + 'e330c659d4bb41d3bdf022e94cab3cd0'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); os.makedirs( ipp ) if not os.path.exists(ipp) else None; urllib2.install_opener( urllib2.build_opener( urllib2.ProxyHandler()) ); by = urllib2.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); open( os.path.join( ipp, pf), 'wb' ).write(by) if dh == h else None; print('Error validating download (got %s instead of %s), please try manual install' % (dh, h) if dh != h else 'Please restart  Sublime Text  to finish installation')
```

安装完成后，使用快捷键 `Shift + Ctrl + P`，打开 Sublime Text 的 Command Paletee，输入 *'Package Control Install Package'* 或者 *'pcip'*，等待它加载完索引后，就可以看到，Package Contorl已经列出了可以安装的Package，同样，可以继续输入关键字进行 Package 的搜索，比如 'emmet' 等，选择后回车或者鼠标点击相应的 Package 即可完成安装。
