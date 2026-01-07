# Blazor 开发规则

## 组件化开发
- **组件拆分**: 保持组件功能单一，复杂页面应拆分为多个子组件。
- **参数传递**: 使用 `[Parameter]` 属性，并注意参数的单向数据流。
- **UI 库**: 推荐使用 Ant Design Blazor 或 MudBlazor。

## 状态管理
- 简单状态使用 `CascadingParameters`。
- 复杂状态建议使用单例服务或专门的状态管理库。

## 性能优化
- 避免在 `OnParametersSet` 中执行过重的逻辑。
- 合理使用 `@key` 指令优化列表渲染。
- 针对 WebAssembly 模式，注意裁剪发布包大小。
