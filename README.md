# Trae Rules Configuration

本仓库用于配置和管理各类 Trae 的规则，旨在为不同的 C# 开发场景提供标准化的开发规范和 AI 辅助规则。

## 目录结构

- `userrule/`: 存放按日期格式留档的用户规则。
- `project-rules/`: 存放针对不同项目类型的详细规则描述，按架构划分为独立目录。
    - `winform/`: WinForm 开发规则。
    - `wpf/`: WPF (MVVM) 开发规则，包含企业级应用和工具类应用细分。
    - `webapi/`: WebAPI 开发规则，包含微服务和单体架构细分。
    - `blazor/`: Blazor 开发规则。
    - `maui/`: MAUI 跨平台开发规则。

## 规则分类

### 1. 桌面端开发
- **WinForm**: 传统桌面应用。
- **WPF**: 现代桌面应用，支持 `enterprise-app` (企业级) 和 `tool-app` (工具类) 细分。

### 2. 服务端开发
- **WebAPI**: RESTful 服务，支持 `microservice` (微服务) 和 `monolith` (单体) 细分。

### 3. Web & 跨平台
- **Blazor**: 交互式 Web UI。
- **MAUI**: 跨平台移动与桌面。

## 使用说明

进入对应的架构目录，查看 `baserule.md` 获取基础规则，或进入细分项目目录获取特定场景的规则描述。
