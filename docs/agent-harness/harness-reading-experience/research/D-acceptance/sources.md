# A076–A100：前端验收与可靠阅读研究来源

核查日期：2026-10-07。由 `web.open` 实际打开下列 25 个原作者文档页面，必要时用页内查找定位相关段落；另打开 WCAG 2.2 正文。证据类型为原页文本核查，**未声称对这 25 个源网站完成浏览器操作或视觉测量**。本任务的真实教程 UI 验收由主任务使用唯一浏览器空间执行。

WCAG 的规范基准为 [WCAG 2.2 正文](https://www.w3.org/TR/WCAG22/)。Understanding 是 W3C 的解释文档，页中的成功标准摘述可帮助定位规范，但解释和技术示例并非新增的强制条款。APG 是组件实现指导；MDN、GOV.UK、web.dev 是技术/设计/性能建议。记录中的具体实现阈值还会标注“项目目标”。这些选取标准用于本教程优化，**不是完整 WCAG 合规声明**。

每个页面仅做短转述，不复制长段原文。旧 HTML 诊断来自当前自己的教材文件及颜色公式，未引用旧 learnDSH 内容。

| 记录 | 原页 | 核查范围与性质 |
|---|---|---|
| A076 | [Understanding SC 2.4.1: Bypass Blocks](https://www.w3.org/WAI/WCAG22/Understanding/bypass-blocks.html) | 规范摘述：SC 2.4.1 A；单页内部重复块的跳过入口属于推荐应用；原页成功标准/意图或实现段落文字核查。 |
| A077 | [Understanding SC 2.1.1: Keyboard](https://www.w3.org/WAI/WCAG22/Understanding/keyboard.html) | 规范摘述：SC 2.1.1 A；项目优先原生按键约定；原页成功标准/意图或实现段落文字核查。 |
| A078 | [Understanding SC 2.1.2: No Keyboard Trap](https://www.w3.org/WAI/WCAG22/Understanding/no-keyboard-trap.html) | 规范摘述：SC 2.1.2 A；原页成功标准/意图或实现段落文字核查。 |
| A079 | [Understanding SC 2.4.3: Focus Order](https://www.w3.org/WAI/WCAG22/Understanding/focus-order.html) | 规范摘述：SC 2.4.3 A；具体切章焦点策略是项目目标；原页成功标准/意图或实现段落文字核查。 |
| A080 | [Understanding SC 2.4.7: Focus Visible](https://www.w3.org/WAI/WCAG22/Understanding/focus-visible.html) | 规范摘述：SC 2.4.7 AA；统一样式为项目目标；原页成功标准/意图或实现段落文字核查。 |
| A081 | [Understanding SC 2.4.11: Focus Not Obscured (Minimum)](https://www.w3.org/WAI/WCAG22/Understanding/focus-not-obscured-minimum.html) | 规范摘述：SC 2.4.11 AA；项目采用完整可见的更强目标；原页成功标准/意图或实现段落文字核查。 |
| A082 | [APG Dialog (Modal) Pattern](https://www.w3.org/WAI/ARIA/apg/patterns/dialog-modal/) | APG 实现指导；不等同于一项独立 WCAG 成功标准；原页成功标准/意图或实现段落文字核查。 |
| A083 | [Understanding SC 4.1.2: Name, Role, Value](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html) | 规范摘述：SC 4.1.2 A；原页成功标准/意图或实现段落文字核查。 |
| A084 | [Understanding SC 4.1.3: Status Messages](https://www.w3.org/WAI/WCAG22/Understanding/status-messages.html) | 规范摘述：SC 4.1.3 AA；减少播报噪声是实现指导；原页成功标准/意图或实现段落文字核查。 |
| A085 | [Understanding SC 1.4.3: Contrast (Minimum)](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html) | 规范摘述：SC 1.4.3 AA；项目统一普通文字目标至少 4.5:1；原页成功标准/意图或实现段落文字核查。 |
| A086 | [Understanding SC 1.4.11: Non-text Contrast](https://www.w3.org/WAI/WCAG22/Understanding/non-text-contrast.html) | 规范摘述：SC 1.4.11 AA；并非所有装饰边框都必须达到 3:1；原页成功标准/意图或实现段落文字核查。 |
| A087 | [Understanding SC 1.4.1: Use of Color](https://www.w3.org/WAI/WCAG22/Understanding/use-of-color.html) | 规范摘述：SC 1.4.1 A；原页成功标准/意图或实现段落文字核查。 |
| A088 | [Understanding SC 1.4.4: Resize Text](https://www.w3.org/WAI/WCAG22/Understanding/resize-text.html) | 规范摘述：SC 1.4.4 AA；项目额外提供可选阅读字号；原页成功标准/意图或实现段落文字核查。 |
| A089 | [Understanding SC 1.4.10: Reflow](https://www.w3.org/WAI/WCAG22/Understanding/reflow.html) | 规范摘述：SC 1.4.10 AA，真正需要二维意义的表格/图有例外；原页成功标准/意图或实现段落文字核查。 |
| A090 | [Understanding SC 1.4.12: Text Spacing](https://www.w3.org/WAI/WCAG22/Understanding/text-spacing.html) | 规范摘述：SC 1.4.12 AA；语言不使用的间距特性不强求；原页成功标准/意图或实现段落文字核查。 |
| A091 | [Understanding SC 2.5.8: Target Size (Minimum)](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum.html) | 规范摘述：SC 2.5.8 AA 为 24×24 CSS px 或适用例外；项目主要按钮目标 44px 高；原页成功标准/意图或实现段落文字核查。 |
| A092 | [MDN prefers-reduced-motion](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@media/prefers-reduced-motion) | MDN 技术说明；本项目的克制运动目标；原页成功标准/意图或实现段落文字核查。 |
| A093 | [Understanding SC 1.3.2: Meaningful Sequence](https://www.w3.org/WAI/WCAG22/Understanding/meaningful-sequence.html) | 规范摘述：SC 1.3.2 A；原页成功标准/意图或实现段落文字核查。 |
| A094 | [Understanding SC 2.4.6: Headings and Labels](https://www.w3.org/WAI/WCAG22/Understanding/headings-and-labels.html) | 规范摘述：SC 2.4.6 AA；标题语义本身另涉及 1.3.1；原页成功标准/意图或实现段落文字核查。 |
| A095 | [GOV.UK Design System: Table](https://design-system.service.gov.uk/components/table/) | 设计系统建议与原生表格示例；本项目语义增强目标；原页成功标准/意图或实现段落文字核查。 |
| A096 | [APG Disclosure (Show/Hide) Pattern](https://www.w3.org/WAI/ARIA/apg/patterns/disclosure/) | APG 实现指导；优先原生 HTML 的项目目标；原页成功标准/意图或实现段落文字核查。 |
| A097 | [web.dev: Web Vitals](https://web.dev/articles/vitals) | 性能建议，不是 WCAG 条款；本地实验与真实用户数据需区分；原页成功标准/意图或实现段落文字核查。 |
| A098 | [MDN Printing](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Media_queries/Printing) | MDN CSS/事件说明；本项目打印交付目标；原页成功标准/意图或实现段落文字核查。 |
| A099 | [GOV.UK: Building a robust frontend using progressive enhancement](https://www.gov.uk/service-manual/technology/using-progressive-enhancement) | 服务手册建议；本项目核心阅读可退化目标；原页成功标准/意图或实现段落文字核查。 |
| A100 | [Understanding SC 2.4.4: Link Purpose (In Context)](https://www.w3.org/WAI/WCAG22/Understanding/link-purpose-in-context.html) | 规范摘述：SC 2.4.4 A；哈希历史和分享是项目目标；原页成功标准/意图或实现段落文字核查。 |

## 文字核查后的重要边界

- A076：2.4.1 的规范范围是跨页重复块；本项目为单页内部导航增加跳过入口，是有益的推荐应用，不把缺失入口单独判为该条规范失败。
- A080/A086：可见焦点与非文字对比分别核查；装饰性边框无需全部达到 3:1。当前浅色边框只在它独自承担控件识别时构成实际问题。
- A088/A089：200% 文本放大与 320 CSS px 重排是两项不同验收。把浏览器 viewport 改成 320px 不等于完成真实浏览器放大测试。
- A090：核查用户覆盖后的布局。默认行距很大不能替代间距覆盖；中文不使用的词间距属性不能机械要求。
- A091：24×24 及例外是该项标准要求。44px 是此项目主要触控按钮的舒适目标，不能冒称 WCAG 2.5.8 最低要求。
- A097：本地单次指标与线上真实用户第 75 百分位不同。没有真实访问样本，就不声称 Core Web Vitals 线上通过。
- A098/A099：旧版只是有 print/noJS 代码。新版需实际切换介质或禁用脚本核查；静态源码存在不能写作实测通过。
