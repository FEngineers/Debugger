# 
Profiler - 分析器

![Profiles panel](../../images/chrome/profiles-panel.png)

通过Profiles panel可以做的事情，
* Timeline提供的信息不能满足需求，获取一些更多的信息
* 可以用来分析内存泄漏的原因

# 给JavaScript代码提速
可以通过Chrome DevTools CPU分析器，来查看哪些方法耗时很久

![CPU Profiler](../../images/chrome/profiles-cpu-profile.png)


### Record a CPU profile
如果要查看JavaScript的运行情况，我们可以收集一个JavaScript CPU profile.
CPU profile会告诉我们页面上的执行时间花在哪些代码里。

1. 去到 **Profiles** 的面板下
2. 选中单选框 **Collect JavaScript CPU Profile**
3. 点击 **Start**
4. 接下来看我们想分析的是什么数据，可以整个reload页面，在页面上交互，或者
 


### View CPU profile



### View CPU profile as Flame Chart



