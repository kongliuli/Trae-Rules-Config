# 全局 C# 开发规范 (Solo 模式通用)

## 基础环境
- **Target Framework**: .NET 8.0+
- **Language Version**: C# 12.0+
- **Platform**: Windows (针对桌面端) / Linux (针对服务端)

## 代码风格
- **Namespace**: 使用 File-scoped namespace (`namespace MyProject;`)。
- **Nullable**: 必须启用 `Nullable reference types`。
- **Async**: 所有的 I/O 操作必须使用异步方法 (`async/await`)。
- **Naming**: 遵循微软官方命名规范 (PascalCase for classes/methods, camelCase for local variables)。

## Trae Solo 模式协作建议
- **任务拆解**: 建议将复杂功能拆分为多个子任务交给 Trae。
- **上下文提供**: 在开始新功能前，先让 Trae 阅读相关的 `baserule.md`。
- **代码审查**: 即使是 Solo 模式生成的代码，也建议让 Trae 进行一次自我 Review。

## 异常处理
- 严禁使用空的 `catch` 块。
- 业务异常应抛出自定义异常类，并由全局过滤器捕获。
