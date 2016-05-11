charles

http://wiki.ele.to:8090/pages/viewpage.action?spaceKey=waimaipingtai&title=Charles+User+Guide




mac
http://webfing.github.io/charles-dubug-http/

唐巧
http://blog.devtang.com/blog/2015/11/14/charles-introduction/




手机设置
首先手机和 mac 在同一个局域网下
之后将手机代理设置成本机IP，端口 8888。（本机 ip 通过 ifconfig）来查看。
￼
￼
之后 charles 会收到一个提醒，点击确定之后就可以看到收到源源不断的请求了。



电脑设置
grant privilege 就可以了，charles 会自己成为系统代理。
但是 chrome 不会自动使用系统的代理，那么就要将其设置为 系统代理，或者 127.0.0.1:8888




https
见唐巧博客或下面
http://blog.csdn.net/jiangwei0910410003/article/details/41620363/




charles 可以代理多个

单纯使用 wifi 下面的代理管理，功能孱弱且麻烦，可以使用一个全局的代理工具。例如 proxyDroid。


善用 breakpoints /map local /map remote






问题：
如何禁止单个的 map local