# A 组：中文排版、字级与图文语法研究

核查日期：2026-10-07。共 25 个不同设计判断，使用 14 个实际打开并取得正文的一手来源页面。

证据边界：本组通过联网页面原文抽取核查规范、示例内容和代码结构；未对这些原站做浏览器截图、键盘或响应式操作。`current_diagnosis` 基于修改前的本项目 HTML 静态 DOM/CSS；`acceptance` 是后续验收目标，不表示已经通过。

来源建议不是本项目的既定结论：英文行宽与行距不能直接当中文标准；W3C CLReq 本次是工作草案；面向政府服务的品牌约束没有移植为本项目的强制规则。

## 来源与核查方式

### S01 · [USWDS Typography](https://designsystem.digital.gov/components/typography/)

- 核查方式：实际打开原作者/官方页面，取得页面正文；官方设计系统指导原文核查。
- 定位内容：Font size / Text alignment / Measure / Line height / Whitespace / Font style。
- 对应判断：A05、A20。

### S02 · [USWDS Using type](https://designsystem.digital.gov/design-tokens/typesetting/overview/)

- 核查方式：实际打开原作者/官方页面，取得页面正文；官方设计系统指导原文核查。
- 定位内容：Normalization / Fonts at native size / Typesetting with tokens。
- 对应判断：A08。

### S03 · [IBM Carbon Typography](https://www.carbondesignsystem.com/building-blocks/foundations/typography/overview)

- 核查方式：实际打开原作者/官方页面，取得页面正文；官方设计系统指导原文核查。
- 定位内容：Productive and expressive type sets / Scale / Weights / Type color。
- 对应判断：A06、A07、A14。

### S04 · [Butterick — Line length](https://practicaltypography.com/line-length.html)

- 核查方式：实际打开原作者/官方页面，取得页面正文；原作者教材原文核查。
- 定位内容：字符数作为行宽度量 / 45–90 characters / 页边距与响应式行宽。
- 对应判断：A02。

### S05 · [Butterick — Line spacing](https://practicaltypography.com/line-spacing.html)

- 核查方式：实际打开原作者/官方页面，取得页面正文；原作者教材原文核查。
- 定位内容：110%、135%、170%三段相同示例 / CSS unitless line-height。
- 对应判断：A03。

### S06 · [W3C 中文排版需求（工作草案）](https://www.w3.org/TR/clreq/)

- 核查方式：实际打开原作者/官方页面，取得页面正文；W3C工作草案内容核查。
- 定位内容：6.1.1 行首行尾禁则 / 6.2.2.1 中文书籍两端对齐 / 6.3.3 中西文混排；本次版本标为2026-10-07工作草案。
- 对应判断：A11、A12、A13。

### S07 · [ONS Accessible text formatting](https://service-manual.ons.gov.uk/brand-guidelines/typography/accessible-text-formatting)

- 核查方式：实际打开原作者/官方页面，取得页面正文；官方设计指导原文核查。
- 定位内容：Layout and structure / Consider reading order / One single column / Text formatting。
- 对应判断：A18、A19。

### S08 · [Digital Scotland Typography](https://designsystem.gov.scot/styles/typography)

- 核查方式：实际打开原作者/官方页面，取得页面正文；官方设计系统指导原文核查。
- 定位内容：小屏与大屏字级表 / Headings / Small type / Links / Lists。
- 对应判断：A01、A10、A21、A25。

### S09 · [IBM Carbon Spacing](https://www.carbondesignsystem.com/building-blocks/foundations/spacing/overview)

- 核查方式：实际打开原作者/官方页面，取得页面正文；官方设计系统指导原文核查。
- 定位内容：Spacing scale / Creating relationships / Creating hierarchy / White space。
- 对应判断：A16、A17。

### S10 · [USWDS Using color](https://designsystem.digital.gov/design-tokens/color/overview/)

- 核查方式：实际打开原作者/官方页面，取得页面正文；官方设计系统指导原文核查。
- 定位内容：项目角色色token / Start in black and white / Put practical before emotional。
- 对应判断：A15。

### S11 · [USWDS Table](https://designsystem.digital.gov/components/table/)

- 核查方式：实际打开原作者/官方页面，取得页面正文；官方设计系统指导与示例代码原文核查。
- 定位内容：Borderless table / When to consider something else / Usability guidance。
- 对应判断：A24。

### S12 · [Digital Scotland Images](https://designsystem.gov.scot/styles/images)

- 核查方式：实际打开原作者/官方页面，取得页面正文；官方设计系统指导原文核查。
- 定位内容：When to use images / Designing illustrations / Images do not replace text。
- 对应判断：A22、A23。

### S13 · [Butterick — Headings](https://practicaltypography.com/headings.html)

- 核查方式：实际打开原作者/官方页面，取得页面正文；原作者教材原文核查。
- 定位内容：Fewer levels, subtler emphasis / space above and below / 不用比例公式替代视觉判断。
- 对应判断：A09。

### S14 · [Butterick — Space between paragraphs](https://practicaltypography.com/space-between-paragraphs.html)

- 核查方式：实际打开原作者/官方页面，取得页面正文；原作者教材原文核查。
- 定位内容：段间距替代段首缩进 / 不用额外回车 / 用CSS margin表达。
- 对应判断：A04。

## 不计入证据的页面

- Apple HIG Typography：打开后只有“requires JavaScript”提示，未取得指导正文，不能据此声称其具体排版方法。
- GOV.UK Typography：抓取失败，未作为任何记录依据。
- Carbon Color usage 的猜测路径返回404，未作为颜色证据；颜色规则使用已打开的 USWDS 正文。

## 本项目修改前的静态基线

- 正文17px/1.9，窄屏16px；main最大800px；目录13px。
- 九幅机制图、二十六张表；关键箭头标签部分为.67rem，在默认16px根字号下约10.72px。
- 这些是源代码事实，实际渲染宽度、对比度、缩放及触摸操作应在主任务统一浏览器验收中测量。
