5.整个事件关联的关键点可以总结如下：

在事件发生时，即源端在产生事件的时候要raise一个event, 监听端使用监听函数如：listenTo()不断监听端口，有消息进来，则建立连接，存放于对应字典，同时将handler注册到_eventMixin_handlers这个列表中。
