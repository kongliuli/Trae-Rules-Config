# WPF MVVM 开发规则

## 架构规范
- **MVVM 模式**: 严格遵守 Model-View-ViewModel 分离原则。View 只负责显示，ViewModel 负责逻辑，Model 负责数据。
- **数据绑定**: 优先使用 `Binding` 和 `Command`，尽量减少 `Code-behind` 中的代码。
- **数据库访问**: 优先使用 **SqlSugar** 进行数据库操作，避免使用原始的 ADO.NET。

## 开发偏好
- **平台**: 默认在 Windows 平台进行 .NET 8 开发。
- **调试**: 偏好使用 .NET Core 控制台进行功能测试和单步调试。
- **UI 优化**: 鼓励使用先进的开源 WPF 插件（如 MaterialDesignInXaml, HandyControl）来美化界面。

## 命名与组织
- ViewModel 必须继承 `INotifyPropertyChanged` 或使用社区库（如 CommunityToolkit.Mvvm）。
- 资源文件（Styles, Templates）应按模块组织在 `Resources` 目录下。
