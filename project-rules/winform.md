# WinForm 开发规则

## 核心原则
- **控件命名**: 遵循 `btnSubmit`, `lblStatus`, `txtInput` 等前缀命名法。
- **事件处理**: 避免在 UI 线程执行耗时操作，使用 `Task.Run` 或 `BackgroundWorker`。
- **界面布局**: 优先使用 `TableLayoutPanel` 和 `FlowLayoutPanel` 保证界面的自适应性。

## 推荐实践
- 使用分层架构，将业务逻辑从 `Form.cs` 中剥离。
- 窗体间通信建议使用事件委托或中介者模式。
- 资源管理：确保 `IDisposable` 控件在窗体关闭时正确释放。
