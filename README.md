# Trae Rules Configuration

本仓库用于配置和管理各类 Trae 的规则，旨在为不同的 C# 开发场景提供标准化的开发规范和 AI 辅助规则。特别针对 **Trae Solo 模式** 进行了优化，以实现极速开发和高质量代码产出。

## 目录结构

- `global-rules/`: **（新增）** 全局通用的 C# 开发规范和 Solo 模式协作建议。
- `userrule/`: 存放按日期格式留档的用户规则。
- `project-rules/`: 存放针对不同项目类型的详细规则描述。
    - `winform/`: WinForm 开发规则。
    - `wpf/`: WPF (MVVM) 开发规则，包含 `enterprise-app` 和 `tool-app`。
    - `webapi/`: WebAPI 开发规则，包含 `microservice` 和 `monolith`。
    - `blazor/`: Blazor 开发规则。
    - `maui/`: MAUI 跨平台开发规则。

## 核心特色

1. **Solo 模式适配**：每个规则文件都包含了针对 Trae Solo 模式的指令建议，帮助 AI 更好地理解您的意图。
2. **技术栈聚焦**：深度集成 **SqlSugar**, **HandyControl**, **.NET 8** 等高效工具。
3. **调试友好**：强调控制台先行验证的开发习惯，提升调试效率。

## 使用说明

1. **全局配置**：首先参考 `global-rules/csharp-standard.md` 设定项目基调。
2. **场景选择**：根据项目类型进入 `project-rules/` 下的对应目录。
3. **AI 引导**：将规则内容告知 Trae，或将其作为项目初始化时的 `.cursorrules` (或 Trae 对应配置) 参考。
