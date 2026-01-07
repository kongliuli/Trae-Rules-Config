# WPF 企业级应用规则

## 核心要求
- **模块化**: 使用 Prism 或 Caliburn.Micro 进行模块化开发。
- **权限控制**: 集成 RBAC (Role-Based Access Control) 权限管理系统。
- **日志**: 必须集成 Serilog 或 NLog，记录详细的运行日志和异常堆栈。

## 数据处理
- 大数据量展示必须使用虚拟化技术 (UI Virtualization)。
- 复杂报表建议集成 FastReport 或类似的第三方报表工具。
