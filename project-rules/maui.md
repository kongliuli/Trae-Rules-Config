# MAUI 开发规则

## 跨平台适配
- **平台特有代码**: 优先使用 `OnPlatform` 或 `OnIdiom` 标记，必要时使用 `Platforms` 文件夹下的条件编译。
- **布局**: 优先使用 `Grid` 和 `FlexLayout` 以适应不同屏幕尺寸。

## 架构与性能
- **MVVM**: 同样遵循 MVVM 模式，推荐结合 `CommunityToolkit.Mvvm`。
- **资源管理**: 图像资源应使用 `MauiImage` 以实现自动缩放。
- **启动优化**: 减少启动时的同步初始化操作，使用异步加载。

## 硬件访问
- 使用 `Microsoft.Maui.Devices` 等内置 API 访问硬件功能，确保跨平台兼容性。
