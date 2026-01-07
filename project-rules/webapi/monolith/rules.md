# WebAPI 单体架构开发规则

## 架构设计
- **三层架构**: Controller -> Service -> Repository (SqlSugar)。
- **依赖注入**: 构造函数注入是唯一推荐方式。
- **实体映射**: 使用 `AutoMapper` 或 `Mapster` 进行 Entity 与 DTO 的转换。

## 数据库规范
- **ORM**: 强制使用 **SqlSugar**。
- **Code First**: 优先使用 Code First 模式，由 Trae 生成实体类和迁移逻辑。

## Solo 模式提效
- "为 [实体名] 生成完整的 CRUD 接口，包含分页查询和条件过滤。"
- "集成 Swagger 并配置 JWT 认证。"
