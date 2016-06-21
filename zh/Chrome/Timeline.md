# Timeline
Timeline可以记录下页面上的各种行为情况，我们可以分析这些行为来提高页面的运行时性能。

第一次看到timeline panel的时候，我是懵逼的，想到了那个歌词：红的黄的蓝的绿的......

![Timeline](../../images/chrome/timeline.png)

## 怎么看性能 How to look at performance
不要觉得performance很简单，只是一些简单的dos和don'ts.

规则会更新，规则也会很容易使用错。

我们应该更关注我们的用户，用户对页面的感觉如何比什么准则都重要

### The RAIL Performance Model
RAIL是一个以用户为中心的性能模型，主要的目的就是用户不要总说到网站“慢”，让用户开心。

**Response**
对于用户的一个操作，要能在100毫秒内响应，避免用户不知道是否自己的操作是否成功。
比如用户点击了提交的按钮，不能点了后有延迟什么反应也没有。
如果操作比较耗时，需要添加load的效果或者类似的提示。

**Animation**
每个动画的帧需需要在16毫秒
* visual animation：显示到屏幕上的动画、从屏幕上退出的动画
* scrolling：用户滚动后页面响应的效果
* drag

**IDLE**

需要在50毫秒里完成

** Load
给用户看到第一个有意义的界面需要的时候要控制在1秒内。

注意事项：
1. 不要再macbook pro这样的机器上测试性能，这不能代表真实的用户。一般的手机比电脑要慢几十倍
2. Nexus 4是一个比较适合测试的机器
3. 推荐用3G网络来测试性能
4. 

### 怎么使用Timeline工具
可以用来记录和分析我们的应用跑起来的所有活动，也是我们可以用来解决性能问题比较好的地方。






面板上分为几个部分
Main
Raster
GPU
ScriptsStreamerThread








## 分析运行时性能
用户期望页面是响应很快的

```
不要写那些会重新计算布局的JavaScript代码
不要过度复杂化css代码，使用较少的css代码，并且使用的选择器尽可能的简单
尽量避免重新布局，选择使用那些不会触发重新布局的css属性
页面绘制会比其他的渲染活动更加的消耗时间，小心瓶颈
```

### JavaScript
有些js代码会需要修改页面上显示的修改，会给性能带来负面影响。
不要让不需立即执行的代码或者需要运行很长的代码影响用户的正常交互操作。

### Style

### Layout

### Paint and composite


# 实践
假如页面中有个function运行很久时间
假如使用了效率低的css属性和值

# 参考
[Introducing RAIL: A User-Centric Model For Performance](https://www.smashingmagazine.com/2015/10/rail-user-centric-model-performance/)