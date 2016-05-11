# Console
console是一个非常完善的终端，在终端里我们可以和page进行交互，比如选中DOM元素，profile the CPU, 监控事件等等。

### 求出表达式的值 Evaluate Expressions
我们可以在console里写一些JavasSript的代码，并查看运行结果。
而且console里还提供了一些功能来支持我们更好的运行JavaScript.

当我们按下回车键的时候，console就会运行我们的js代码。

* 表达式导航
```
当我们在敲代码的时候，会提示我们可能相关的属性名，也有自动补全和tab补全的功能。
如果有多个匹配的，我们可以使用上、下箭头，来查看所有可能的选项；我们也可以使用右箭头来选中当前的选项。
如果只给了一个建议的选项，使用tab可以选中。
```

* 选中元素
```
$()   document.querySelector的简写，返回第一个满足css选择器的元素
$$()  document.querySelectorAll的简写，返回所有满足css选择器的的元素
$x()  传入XPath，返回满足条件的元素
```
例如
```
$('code') // Returns the first code element in the document.
$$('figure') // Returns an array of all figure elements in the document.
$x('html/body/p') // Returns an array of all paragraphs in the document body.
```

### 监控事件
可以监听页面上的某个元素的某件事情

监听事件
```
monitorEvents(document.body, "click");
```
取消监听事件
```
unmonitorEvents(document.body);
```

### API
```
$_
$0 - $4
$(selector)
$$(selector)
$x(path)
clear()
copy(object)
debug(function)
dir(object)
dirxml(object)
inspect(object/function)
getEventListeners(object)
keys(object)
monitor(function)
monitorEvents(object[, events])
profile([name]) and profileEnd([name])
table(data[, columns])
undebug(function)
unmonitor(function)
unmonitorEvents(object[, events])
values(object)
```