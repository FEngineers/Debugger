# Network
在Network面板下面，可以看看页面上请求的资源，我们也可以根据Network提供的信息来优化页面的加载性能

Network面板由5个部分组成

* Controls
可以用来控制整个Network面板长什么样子，已经有哪些功能
* Filters
用Filter的选项来控制显示在Requests Table显示哪些资源；也可以通过按住cmd，然后点击filter选项，
这样可以一次选中多个filter
* Overview
显示加载资源的timeline，如果看到有bar是垂直重叠的，说明有同时加载的情况。
* Requests Table
资源列表，默认情况下按照加载的顺序来排序，最早加载的资源在最顶部。
点击某一个资源，可以看到关于这个资源的更多信息。
我们也可以通过在表头右击（除了Timeline的表头区域），可以来控制增加或删除某一列的信息。
* Summary
一些总结的信息，请求资源的总数，请求数据的总大小，以及加载时间。


![Network Panel](../../images/chrome/chrome-network-panel.png)

### 记录network的活动

### 捕捉屏幕截图

### 查看DOMContentLoaded和load两个事件的信息
Network会高亮显示两个事件：DOMContentLoaded和load

* DOMContentLoaded
发生在页面上的markup被解析以后。在Network的面板有两个地方会显示，在Overview界面的垂直的蓝色的线，
以及在Summary的部分也可以看到准确的时间
* load
load会在页面已经完全load后触发，会在三个地方显示：
红色的垂直的线；在资源列表里面的垂直的红色的线；在Summary的部分里面

### 查看某一个请求的资源的细节
* Headers
* Preview
* Response
* Cookies
* Timing