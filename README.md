# Spring Petclinic REST 后端

这是一个兽医诊所管理 REST 服务，提供主人、宠物、兽医、宠物类型、专科和就诊记录的 API。项目使用 Spring Boot，默认通过内存数据库加载示例数据，也可切换到 MySQL 或 PostgreSQL。

## 运行

需要 Java 17 和 Maven。执行 `./mvnw spring-boot:run` 启动服务，默认端口为 9966，接口前缀为 `/petclinic`。运行 `./mvnw test` 可执行基于 H2/HSQLDB 的服务、控制器和持久化测试。

## 主要目录

- `src/main/java/org/springframework/samples/petclinic/rest`：REST 控制器和接口模型
- `src/main/java/org/springframework/samples/petclinic/service`：诊所业务服务
- `src/main/java/org/springframework/samples/petclinic/repository`：JDBC、JPA 与 Spring Data JPA 实现
- `src/main/resources/openapi.yml`：OpenAPI 接口定义
- `src/test`：服务、控制器和仓储测试

安全开关、数据库 profile 和服务端口均在 `src/main/resources` 下的配置文件中管理。
