# 教学交互与信息状态：一手来源核查

本文件对应 A51–A75 的 25 条研究与设计判断。核查日期：2026-10-07。共实际打开并读取 15 个一手页面，14 个用于记录，1 个作为未采用方向的补充核查。

核查方式是 `web.run` 的原页 `open`，再以 `find` 与定位 `open` 阅读相关章节。这里的证据是原作者文本规范或教程结构；没有在这些源网站点击控件、截取视觉对照或开展用户测试。当前项目诊断来自本轮阅读 HTML 源码，涉及类名、DOM 结构与事件逻辑，不能据此宣称已经浏览器实测。源文档中的组件测试结果也不能替代我们页面的验收。

源文档提供组件职责和约束；本项目的使用方式、位置、颜色强度与验收条件是针对非技术读者的推导。我们不照搬 Carbon 的完整产品控制台，也不照搬 USWDS 的政府表单布局。

| 编号 | 实际打开的一手页面 | 核查章节与实际取得的证据 | 对应记录 |
| --- | --- | --- | --- |
| C-S01 | [Carbon：Button](https://www.carbondesignsystem.com/building-blocks/core/components/button/guidelines) | Overview、Emphasis、Content、Overflow、Best practices；区分动作与导航、动词对象、强调层级，阅读页不一定需要主按钮。 | A51–A54 |
| C-S02 | [Carbon：Content switcher](https://www.carbondesignsystem.com/building-blocks/core/components/content-switcher/guidelines) | Overview、When not to use、Low contrast、Interactions；同类视图切换、层级与低强调。 | A59 |
| C-S03 | [Carbon：Notification](https://www.carbondesignsystem.com/building-blocks/core/components/notification/guidelines) | Inline、Dismissal、Callout formatting；上下文位置、持续反馈、克制使用提示。 | A60–A62 |
| C-S04 | [USWDS：Accordion](https://designsystem.digital.gov/components/accordion/) | Guidance；主体信息需要阅读时使用正文，披露标题的可触达范围。 | A68、A69 |
| C-S05 | [USWDS：Table](https://designsystem.digital.gov/components/table/) | Guidance；简单样式、列的统一单位、短表头、避免长文塞进表格、不同窄屏形式。 | A70、A71 |
| C-S06 | [USWDS：Step indicator](https://designsystem.digital.gov/components/step-indicator/) | Guidance；线性过程定位、当前项和总数、非线性场景限制。 | A66、A67 |
| C-S07 | [USWDS：Radio buttons](https://designsystem.digital.gov/components/radio-buttons/) | Guidance；互斥选择、默认偏置、竖排与标签触发、fieldset/legend。 | A56、A57 |
| C-S08 | [USWDS：Checkbox](https://designsystem.digital.gov/components/checkbox/) | Guidance；独立多选、明确状态文字与整体标签。 | A58 |
| C-S09 | [USWDS：Select](https://designsystem.digital.gov/components/select/) | Guidance；少量选项的替代形式、持续标签、避免自动提交与依赖选择。 | A55 |
| C-S10 | [USWDS：Tooltip](https://designsystem.digital.gov/components/tooltip/) | Guidance；仅适合非关键短帮助，关键说明不应藏在悬停里。已读取，但25条中的披露与图解规则已覆盖此限制，没有再拆出一条重复计数。 | 补充核查，不计数 |
| C-S11 | [Carbon：Code snippet](https://www.carbondesignsystem.com/building-blocks/core/components/code-snippet/guidelines) | Overview、Formatting、Copy to clipboard；只读片段、长度变体、复制为可选并需确认。 | A72、A73 |
| C-S12 | [Carbon：Inline loading](https://www.carbondesignsystem.com/building-blocks/core/components/inline-loading/guidelines) | When to use、Placement、States、Interactions；等待适用范围、原位反馈、动作文字。 | A63、A64 |
| C-S13 | [Carbon：Tag](https://www.carbondesignsystem.com/building-blocks/core/components/tag/guidelines) | Variants、States、Read-only tag；只读与可操作标签的区分。 | A65 |
| C-S14 | [Red Blob Games：Introduction to the A* Algorithm](https://www.redblobgames.com/pathfinding/a-star/introduction.html) | Representing the map、Breadth First Search；先讲输入与输出，再逐步观察同一个机制。 | A75 |
| C-S15 | [USWDS：Data visualizations](https://designsystem.digital.gov/components/data-visualizations/) | General guidance；一个中心意思、有限颜色、文字结论与不只依赖颜色。原页说明本组件是 guidance-only；没有组件代码。 | A74 |

以上都是原作者/设计系统页面的短原创摘要，未复制整段指南，未保存原站图片。Carbon 页面在本次读取时使用 `/building-blocks/core/components/.../guidelines` 路径，记录使用实际打开的当前路径。

## 对当前教材最值得落实的五个改动

1. **稳定实验观察区。** 输入、输出、执行者、已知与未知保持固定观察槽位，事件变化不能挤走操作按钮。
2. **让主次动作有差别。** 每个当前实验仅一个局部主动作；回看与重置降低视觉强调，章节阅读继续保持文档气质。
3. **信息状态比装饰更清楚。** “选择已改变但未组装”“未发送”“尚未获得结果”贴近预览或数据；短状态与长教学原因分层。
4. **表格与代码服务理解。** 真正的跨列比较保留表格；来源、术语目录在窄屏可按字段堆叠。工作单和 JSON 均有用途标签，不能暗示必须运行。
5. **主体可直接阅读。** 答案与补充资料可以披露，核心解释保持展开；不给每段加卡片，不用消失的 toast 承载原因，不加入假等待。

## 验收口径

记录中的 `acceptance` 是待执行的项目标准，不是已通过结果。后续验收应检查桌面/窄屏截图、键盘焦点、每项实验状态变化、禁用原因、长内容换行与页面溢出。简单好看由正文连续性、结构一致和观察成本共同决定，不能只用圆角、背景、动画数量衡量。
