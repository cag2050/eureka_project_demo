### 步骤：
1. spring initializr，选择 cloud discovery => eureka discovery
1. spring boot 启动类添加注解：@EnableDiscoveryClient，该注解能激活Eureka中的DiscoveryClient实现，这样才能实现Controller中对服务信息的输出。
1. application.properties 配置上相关属性
1. 再次访问server链接：http://localhost:10010/，服务被成功注册了
1. 访问：http://localhost:2001/dc，将client实例打印出来了

* Spring cloud的服务注册及发现，不仅仅只有eureka，还支持Zookeeper和Consul。默认情况下是eureka，spring 封装了eureka，使其非常简单易用，只需要比传统应用增加一行代码就可以使用了，这一行代码就是一个注解。

* 需要和 eureka server 端配合，运行此项目前，eureka server 端需要先运行。  

* 出处：http://blog.didispace.com/spring-cloud-starter-dalston-1/