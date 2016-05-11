# Sources
可以通过设置断点来debug我们的js代码

### 通过断点来debug
DevTools里面包含了非常强大的断点的技术，可以用来检查代码的逻辑错误

使用alert('ok so far')或者alert('x = ' + x);还是有点原始的。

怎么设置断点呢？

断点按照类型分为四种
* Breakpoints
* DOM Breakpoints
* XHR Breakpoints
* Event Listener Breakpoints

### debug压缩过的代码
* 先将代码格式化
* 用source maps将编译压缩过的代码和源代码对应上

### 通过DevTools Workspaces来保存变动
当我们修改了DOM、样式，我们的确可以在页面上看到改动的结果。
可是，当我们刷新了浏览器后，改动就全部丢掉了，除非每次改完把修改复制到我们自己的代码编辑器里面

我们可以通过Workspaces来做到这一点