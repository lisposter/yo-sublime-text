# 插件推荐

Sublime Text 能有今天的人气，除去她本身优秀的外表之外，也脱离不了众多社区提供的插件，通过插件这样的机制，可以让众多开发者能为 Sublime Text 曾贴众多功能。本章会推荐一些常用的插件，并做一些简单的介绍。

### AnvancedNewFile

增强版的新建文件，和自带的区别在于，使用 ANF，路径可以是 Tab 补全，另外，可以自定义一些路径别名，并且可以根据不同平台的系统，补全不同的路径，在开发大型项目时候，需要建立文件于深层目录的时候，补全将会是很有用的功能，同时也能避免一些输入错误带来的问题。虽然插件名字叫做 AnvancedNewFile，但是其实除了新建文件，该插件还提供了‘删除’，‘重命名’，‘复制’这些常用的功能。

### All Autocomplete Sublime Text

增强了自带的补全，使得 Sublime 可以搜寻已打开的文件，来推荐补全内容。在默认情况下，Sublime 只会补全出现在当前文件中的字词。在安装这个插件之后，Sublime 便会在所打开的所有文件中搜索可用于补全当前输入的内容。


### AutoFileName

这个插件，可以让你在写路径的时候，帮你补全文件名，这在书写 `<img src="some/path/to/img">` 或者 `background: url(some/path/to/img)` 这样的代码的时候，尤为有用。

### BracketHighlighter

顾名思义，为各种括号以及引号，HTML 标签对进行匹配和高亮，这在函数式编程的时候会非常方便。其也提供了丰富的配置选项，可以让你自定义匹配的括号类型，样式，颜色等。


### CodeFormatter

代码格式化插件，虽然它格式化的比较机械化，人为的一些空行之类的往往无法很好的辨认，但是，在对一些被压缩过的代码，或者一长串 json 字符串没法看的时候，格式化一下，马上就很清晰了。


### Color Highlighter

如果你是一个前端，那么，你肯定会经常和一大堆颜色值打交道，使用这个插件，可以把类似于 `#02a3c6` 这样的颜色值的真是颜色显示出来，在写样式的时候，就不用来回切浏览器来看这个颜色对应哪个值了。插件支持多种颜色的书写方式，例如 rgb，hex 等，可以满足大部分的编程时候对颜色值的需求。


### DocBlockr

代码注释是平时开发中很重要却又不受大家喜欢的环节，这个插件可以让你很轻松的写出如下 js doc 格式的代码注释：

```js
/**
 * [function_name description]
 * @param  {[type]} argument [description]
 * @return {[type]}          [description]
 */
```

### EditorConfig

[EditorConfig](http://editorconfig.org/) 是一个统一编辑器配置的插件，利用这个插件，可以规范特定的项目在每个人的编辑器中采取同样的配置，例如缩进是 tab 还是 space，缩进长度是多少等等。并且使用这个插件并不会永久修改你的编辑器配置，因此，你在这个项目之外的地方，配置还是和你原来的一样。

插件使用方式很简单，在 Sublime 中装完插件本身后，启用即可。然后在项目根目录中创建 `.editorconfig` 文件（也可以放置于用户家目录，这样会做为全局的配置，在这里，还是推荐大家在项目中单独配置，并纳入版本库中），即可配置一些共通的选项，具体可以配置的项，可以参考其官网。

### Emmet

Emmet 可以说是前端必备的工具了，他曾经的名字是 zen-coding，相信不少人听过了。他提供了大量快捷书写 html，css 代码的方式，例如：

```
section.nav>ul>li*5>a
```
按下 tab 键，可以出来如下的 html：

```html
<section class="nav">
    <ul>
        <li><a href=""></a></li>
        <li><a href=""></a></li>
        <li><a href=""></a></li>
        <li><a href=""></a></li>
        <li><a href=""></a></li>
    </ul>
</section>
```

### FileDiffs

这个插件可以让你选择两个 tab 的内容进行 diff 操作，很简单却实用的功能。安装完成后，通过右键点击文件标签栏或者使用命令都可以进行文件 diff 对比。

### FixMyJs

这个是在 jshint 出品的 fixmyjs 的基础上开发的 Sublime 插件，可以根据你的 .jshintrc 配置来一键修复代码中的 jshint 错误。虽然处理一些复杂的不规范问题的时候还是欠缺了点，但是，补全一下分号之类的，绰绰有余了。


### Git

Sublime 中最好的 git 集成套件，可以通过 Sublime 的 Command Plate 进行大部分的 Git 操作。笔者常用的功能是 Blame，在 Sublime 中使用 Blame，高亮等都舒服。

### GitGutter

在使用 Git 的时候，我们往往想要知道自己改了些什么内容，最简单的办法是使用 git diff 命令，但是每次都需要跑一个命令，总不是很方便的感觉，这个插件可以在左侧行号区域显示文件的 git diff 信息，这可以让你很清楚自己对文件修改了什么。增删改都有不同的标志显示。

### JavaScriptNext

增强了 JS 的高亮，特别是对 ES 6/ES 2015 的支持。

### Markdown Extended

对 markdown 语法的增强，可以对类似于标题，代码等进行高亮。

### Markndown Preview

快速预览一个 markdown 文件渲染后的结果，可以通过浏览器预览

### SideBarEnhancements

增强 Sublime 的侧边栏，增加了大量的操作在右键菜单中，类似于拷贝文件，拷贝路径，新建文件，等等。

### SublimeLinter

强大的代码错误检查，这是它的主体，如果你需要使用 lint，还需要安装一些插件，例如 'SublimeLinter-jshint' 等。

### Vintageous

比自带的 Vintage 更贴近 Vim 的插件，例如增加了 Command 条等。
