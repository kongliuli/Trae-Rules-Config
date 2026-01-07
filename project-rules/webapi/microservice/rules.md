# WebAPI 微服务架构开发规则

## 核心组件
- **网关**: 使用 `Yarp` 或 `Ocelot`。
- **服务发现**: 集成 `Consul` 或 `Eureka`。
- **配置中心**: 推荐使用 `Apollo` 或 `Nacos`。
- **消息队列**: 优先选择 `RabbitMQ` 或 `Kafka` 处理异步任务。

## 开发规范
- **健康检查**: 每个服务必须实现 `/health` 接口。
- **日志追踪**: 集成 `SkyWalking` 或 `Jaeger` 进行链路追踪。
- **容器化**: 每个服务必须包含 `Dockerfile` 和 `docker-compose.yml` 片段。

## Solo 模式提效
- "创建一个新的微服务模块 [服务名]，集成 Consul 注册和 Yarp 网关配置。"
- "实现基于 RabbitMQ 的事件发布/订阅逻辑。"
