# 一、五种工作方式
1. 简单队列模式

模式组成结构：一个生产者，一个队列，一个消费者

2. Work模式：分布式消费方式

模式组成：一个生产者，一个队列，多个消费者

3. 发布/订阅模式（Exchange-fanout）

模式组成：一个生产者，一个fanout Exchange，多个队列，多个消费者

4. Routing模式（Exchange-Direct）发布消息时指定消息key

模式组成：一个生产者，一个Direct exchange，多个队列，多个消费者，（每个消息要有指定key，exchange根据key发送到具体队列）

5. Topic模式（通配符模式）：

模式组成：一个生产者，一个Direct exchange，多个队列，多个消费者，（每个消息要有指定key，exchange根据key发送到具体队列，只要消息的key符合绑定到exchange的queue通配符规则，就降消息转发到相应队列）

