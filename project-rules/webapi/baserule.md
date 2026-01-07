# WebAPI MVC 开发规则

## 接口规范
- **RESTful**: 遵循标准的 HTTP 方法（GET, POST, PUT, DELETE）。
- **响应格式**: 统一使用 `ApiResponse<T>` 包装类，包含 `Code`, `Message`, `Data` 字段。
- **版本控制**: 建议在 URL 中包含版本号，如 `/api/v1/resource`。

## 技术栈
- **依赖注入**: 充分利用内置的 DI 容器进行服务注册。
- **ORM**: 推荐使用 Entity Framework Core 或 SqlSugar。
- **文档**: 必须集成 Swagger (Swashbuckle) 并编写完整的 XML 注释。

## 安全与性能
- 使用 `DTO` (Data Transfer Objects) 进行数据传输，避免直接暴露实体模型。
- 实现全局异常过滤器 (Exception Filter) 统一处理错误。
