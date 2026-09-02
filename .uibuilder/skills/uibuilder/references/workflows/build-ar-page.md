# 新建 AR 页面

1. 用 `fetch_context` 确认当前为“AR实景设计规范11”，并读取变量、样式和目标页面。
2. 从 [`../pages/index.md`](../pages/index.md) 选择最接近的页面类型，再依据 [`../pixso-source-map.md`](../pixso-source-map.md) 定位参考 Frame。
3. 明确用户任务、内容来源、页面层级、全局主题、全局视效、必要状态和 1920/1280 两张适配稿。
4. 将每个可见区域映射到 [`../components/index.md`](../components/index.md) 的现有组件；先 `read_components`，再 `query_nodes` 获取真实 GUID、属性和 Variant。
5. 映射完整后复制或继承最接近的规范 Frame。不得从空白画布自由绘制整页。
6. 分别建立 1920 和 1280 Frame，复用同一组件体系和变量模式，只调整规范允许的外部布局、密度、收纳和显隐。
7. 仅写入用户、数据源或规范提供的内容；缺失内容依 [`../content-data-rules.md`](../content-data-rules.md) 处理。没有真实监控画面时读取 [`../assets/image-resources.md`](../assets/image-resources.md)，优先使用 `行业背景2` 作为实景层。
8. 按 [`validate-ar-page.md`](validate-ar-page.md) 验收并交付。

若无合适组件，记录组件名称、业务需要、最接近组件、影响和建议，不自行造组件。
