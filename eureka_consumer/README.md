* 这个例子，通过LoadBalancerClient接口来获取某个服务的具体实例，并根据实例信息来发起服务接口消费请求。
但是这样的做法需要我们手工的去编写服务选取、链接拼接等繁琐的工作，对于开发人员来说非常的不友好。所以，下来我们看看Spring Cloud中针对客户端负载均衡的工具包：Ribbon。

* consumer：消费eureka_client提供的接口

* 先启动 eureka server 和 client 端，再启动此项目。  
访问地址：http://localhost:2002/consumer  

* 出处：http://blog.didispace.com/spring-cloud-starter-dalston-2-1/