# 插件推荐

本章会推荐一些常用的插件，并做一些简单的介绍。

### AnvancedNewFile

增强版的新建文件，和自带的区别在于，使用 ANF，路径可以是 Tab 补全，另外，可以自定义一些路径别名，并且可以根据不同平台的系统，补全不同的路径

### All Autocomplete Sublime Text

增强了自带的补全，使得 Sublime 可以搜寻已打开的文件，来推荐补全内容，默认情况下，Sublime 只会补全出现在当前文件中的字词。


### AutoFileName

这个插件，可以让你在写路径的时候，帮你补全文件名，这在书写 `<img src="some/path/to/img">` 或者 `background: url(some/path/to/img)` 这样的代码的时候，尤为有用。

### BracketHighlighter

顾名思义，为各种括号以及引号，HTML 标签对进行匹配和高亮，这在函数式编程的时候会非常方便。


### CodeFormatter

代码格式化插件，虽然它格式化的比较机械化，人为的一些空行之类的往往无法很好的辨认，但是，在对一些被压缩过的代码，或者一长串 json 字符串没法看的时候，格式化一下，马上就很清晰了。

### Color Highlighter

如果你是一个前端，那么，你肯定会经常和一大堆颜色值打交道，使用这个插件，可以把类似于 `#02a3c6` 这样的颜色值的真是颜色显示出来，在写样式的时候，就不用来回切浏览器来看这个颜色对应哪个值了。


### DocBlockr

这个插件可以让你很轻松的写出如下格式的代码注释：

```js
/**
 * [function_name description]
 * @param  {[type]} argument [description]
 * @return {[type]}          [description]
 */
```

### EditorConfig

[EditorConfig](http://editorconfig.org/) 是一个统一编辑器配置的插件，利用这个插件，可以规范特定的项目在每个人的编辑器中采取同样的配置，例如缩进是 tab 还是 space，缩进长度是多少等等。并且使用这个插件并不会永久修改你的编辑器配置，因此，你在这个项目之外的地方，配置还是和你原来的一样。

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

这个插件可以让你选择两个 tab 的内容进行 diff 操作，很简单却实用的功能。

### FixMyJs

这个是在 jshint 出品的 fixmyjs 的基础上开发的 Sublime 插件，可以根据你的 .jshintrc 配置来一键修复代码中的 jshint 错误。
