### 步骤：
1. spring initializr，选择 cloud discovery => eureka server
1. spring boot 启动类添加注解：@EnableEurekaServer
1. application.properties 配置上相关属性
1. run启动类，打开链接：http://localhost:10010/

* Spring cloud的服务注册及发现，不仅仅只有eureka，还支持Zookeeper和Consul。默认情况下是eureka，spring 封装了eureka，使其非常简单易用，只需要比传统应用增加一行代码就可以使用了，这一行代码就是一个注解。

* 通过@EnableEurekaServer注解启动一个服务注册中心提供给其他应用进行对话。

* 需要和 eureka client 端配合，运行此项目后，再运行 eureka client 端。  

* 出处：http://blog.didispace.com/spring-cloud-starter-dalston-1/