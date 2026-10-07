# 长篇教材导航研究：A26–A50

核查日期：2026-10-07。范围：章节导航、局部定位、渐进展示、回查与连续阅读。

本批为 25 条不同的研究与设计判断，使用 18 个实际打开的有效一手页面。记录见 [records.json](records.json)。每条都有来源、当前诊断、adopt / adapt / reject 决定、实现建议与验收条件。验收字段为实施后需要执行的条件，本批没有把它标成已通过。

## 核查方法和证据边界

- 网页工具直接打开原作者、项目官方、官方设计系统或标准解释页，读取正文和官方配置/HTML 示例。搜索仅找正确页面；搜索摘要不作为判断证据。
- 网页结构观察只指提取到的标题、列表与位置顺序，不证明视觉颜色、尺寸或交互结果。本批未操作来源站点的搜索、抽屉、折叠或历史返回。
- W3C Understanding 页面是非规范性解释。GOV.UK 的组件要求也不自动成为本项目的强制规则。
- 当前诊断来自开始时 HTML 的静态 DOM、CSS 和脚本阅读。已存在而有效的部分明确保留；代码风险没有伪称浏览器失败。
- 来源采用短篇原创转述，不复制整页。实现及验收为本项目的适配判断。

## 当前版本基线

文件：Agent-Harness图解阅读版.html。

SHA-256：1bcc11d753a38253449b052e70450f78ea904d46f060726411bfbba34189312a。

静态检查：18 个阅读章节，73 个 h3（包括实验标题），只有整本章目录，没有当前章局部目录、搜索输入、跳过导航链接。第 2、7 章各有 8 个 h3。已有学习问题卡片、章末描述性前后链接、当前章 aria-current 及按 hash 显示所属章的能力。

待实测的代码风险：全文滚动只更新目录高亮，没有更新 currentIndex；全文开关复用旧索引/hash；全部 hashchange 强制 scrollIntoView 可能覆盖历史滚动恢复。这些不是已操作测试的结论。

## 已打开的一手来源

| 编号 | 来源 | 关联记录 | 实际核查 |
|---|---|---|---|
| N01 | [Sidebar | Docusaurus](https://docusaurus.io/docs/sidebar) | A26 | 打开原页，读取有序树与前后页导航说明。 |
| N02 | [Sidebar items | Docusaurus](https://docusaurus.io/docs/sidebar/items) | A27 | 打开原页，核查 label、sidebar_label、category 的说明。 |
| N03 | [Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn_web_development) | A28、A40 | 打开原页，读取 In this article 与不同起点的课程入口；网页文本结构观察。 |
| N04 | [Default Theme Config | VitePress](https://vitepress.dev/reference/default-theme-config) | A29、A30 | 打开原页并定位 outline、sidebarMenuLabel，读取级别与移动标签配置。 |
| N05 | [ARIA: aria-current | MDN](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Reference/Attributes/aria-current) | A31 | 打开原页，读取 page、location、step 的含义。 |
| N06 | [Choosing the State Structure | React](https://react.dev/learn/choosing-the-state-structure) | A32、A38 | 打开原页，读取避免矛盾和重复状态原则；阅读模式是本项目工程适配。 |
| N07 | [Headings and Table of contents | Docusaurus](https://docusaurus.io/docs/markdown-features/toc) | A33 | 打开原页并定位 Heading IDs，读取显式 ID 与保持旧链接的说明。 |
| N08 | [Search | VitePress](https://vitepress.dev/reference/default-theme-search) | A34、A47、A48 | 打开原页，核查浏览器索引、标题权重、带 hash 的文档 ID；未操作该站搜索。 |
| N09 | [Prev Next Links | VitePress](https://vitepress.dev/reference/default-theme-prev-next-links) | A35 | 打开原页，核查相邻页文字和目标可单独定制。 |
| N10 | [Pagination | GOV.UK](https://design-system.service.gov.uk/components/pagination/) | A36、A37 | 打开原页，核查内容页导航的垂直排列、上下文题目及无限滚动限制。 |
| N11 | [History: scrollRestoration | MDN](https://developer.mozilla.org/en-US/docs/Web/API/History/scrollRestoration) | A39 | 打开原页正文，读取 auto/manual；本教材后退风险来自代码审阅，未据此假称实测。 |
| N12 | [Tutorials | Diátaxis](https://diataxis.fr/tutorials/) | A41 | 打开原作者页，读取具体任务、成果与避免过早选项的说明。 |
| N13 | [Quick Start | React](https://react.dev/learn) | A42 | 打开原页，观察学习点先于示例的网页文本结构，不作为页面美学截图证明。 |
| N14 | [Explanation | Diátaxis](https://diataxis.fr/explanation/) | A43 | 打开原作者页，读取建立联系、背景与主题边界的说明。 |
| N15 | [Accordion | GOV.UK](https://design-system.service.gov.uk/components/accordion/) | A44、A46 | 打开原页，核查核心信息默认可见与避免嵌套建议。 |
| N16 | [Details | GOV.UK](https://design-system.service.gov.uk/components/details/) | A45 | 打开原页，核查补充信息及简短描述性标签，读取官方 HTML 示例。 |
| N17 | [Understanding SC 2.4.11 | W3C](https://www.w3.org/WAI/WCAG22/Understanding/focus-not-obscured-minimum.html) | A49 | 打开官方解释页，读取遮挡准则与固定层风险。Understanding 是非规范性解释。 |
| N18 | [Understanding SC 2.4.1 | W3C](https://www.w3.org/WAI/WCAG22/Understanding/bypass-blocks.html) | A50 | 打开官方解释页，读取跳过重复导航及单页也有帮助的注记，不宣称整体合规。 |

## 优先落实的导航骨架

1. 全书按任务分组并缩短目录标签，当前章再给独立的小节目录。
2. 章号、章名、小节、高亮、前后章链接从统一的导航状态派生。
3. 全文模式、深链接、主动跳转与历史返回分别处理，保持正在读的段落。
4. 本地搜索先解决章题/小节回查，不加聊天问答和外部检索服务。
5. 核心解释保持可见，补充仅一层展开；窄屏入口有文字，键盘可跳过导航。

这是优先级建议，不要求 23 个 adopt / adapt 各自增加一个控件。条目可合并到少量组件中，由最终方案选择和浏览器验收决定落实范围。

## 未计为有效证据的访问

VitePress 的 /reference/default-theme-outline 与 /reference/default-theme-doc-footer 没有返回有效正文，已改用本表 N04、N09。GitBook 的 /docs/publishing-documentation/site-structure/navigation 与 /table-of-contents 返回不可访问，未用于任何记录，未声称操作或视觉核查成功。
