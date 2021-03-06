# config-server
Spring Cloud Config 是Spring Cloud 团队创建的一个全新项目，用来为分布式系统中的基础设施和微服务应用提供集中化的外部配置支持，它分为服务端与客户端两个部分。

其中服务端也称为分布式配置中心，它是一个独立的微服务应用，用来连接配置仓库并为客户端提供获取配置信息、加密/解密信息等访问接口；

而客户端则是微服务架构中的各个微服务应用或基础设施，它们通过指定的配置中心来管理应用资源与业务相关的配置内容，并在启动的时候从配置中心获取和加载配置信息。

Spring Cloud Config 实现了对服务端和客户端中环境变量和属性配置的抽象映射，所以它除了适用于Spring 构建的应用程序之外，也可以在任何其他语言运行的应用程序中使用。

由于Spring Cloud Config 实现的配置中心默认采用Git 来存储配置信息，所以使用Spring Cloud Config 构建的配置服务器，天然就支持对微服务应用配置信息的版本管理，并且可以通过Git 客户端工具来方便的管理和访问配置内容。当然它也提供了对其他存储方式的支持，比如：SVN 仓库、本地化文件系统。


# Reference

[Spring Cloud Config](https://cloud.spring.io/spring-cloud-config/spring-cloud-config.html)