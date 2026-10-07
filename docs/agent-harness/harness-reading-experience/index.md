# Harness 教材阅读体验改造

本轮以非技术背景读者为对象，优化完整教材的阅读、定位、图文层级和实验操作。内容主线仍是“输入、输出、执行”，并解释 Harness 的技术逻辑、架构位置和当前产品分工。

研究与方案比较开始于 2026-10-07，最终实现和浏览器复验完成于 2026-10-08。技术正文的一手资料核查日期仍为 2026-10-07。

## 先看结果

采用**暖白编辑式阅读**：暖白底、深墨正文、少量墨绿强调；系统中文无衬线正文，章题带少量文集气质。目录按学习阶段分组，全文与本章定位分开，本地搜索进入原文，阅读设置控制字号和全文展开。图解保持二维、可选择文字，实验保持原生控件和明确反馈。

- [最终桌面阅读预览](evidence/final-desktop-reading.png) · [手机阅读](evidence/final-mobile-reading.png) · [手机查找](evidence/final-mobile-search.png)
- [三种美学方向的独立比较](design/01-独立设计评审.md)
- [最终设计选择与规格](design/02-方案选择与设计规格.md)
- [最终前端验收报告](validation/02-前端最终验收.md)

## 100 轮怎样计数

完成 **A001–A100，共 100 条有来源的前端研究与设计判断**，形成 100 张方法卡。记录关联 **69 个不同一手来源 URL**；同一个来源可以支持不同问题。最终取舍为 **26 条采纳、64 条调整采用、10 条舍弃**。

每条记录说明原页方法、证据范围、旧版具体问题、本项目适配方式和验收条件。100 轮不是 100 个网站、100 套视觉主题、100 次浏览器测试或真人测试。方法的研究取舍和成品的实际验证是两种证据，分开保存。

- [受众与验收基线](00-阅读体验与验收基线.md)
- [百轮执行规则](01-百轮研究执行规则.md)
- [100 张方法卡索引](methods/index.md)
- [最终记录注册表](loops/registry.json) · [原候选快照](loops/candidate-registry.json)
- [独立复核后的五项修订](loops/修订记录.md)
- [100 条研究独立复核](validation/00-研究独立复核.md)

## 按方法类型查阅

|范围|关注点|原页与研究记录|
|---|---|---|
|A001–A025|中文排版、层级、留白、颜色、图表语法|[排版与视觉](research/A-typography/sources.md)|
|A026–A050|目录、局部路线、搜索、历史与连续阅读|[导航与组织](research/B-navigation/sources.md)|
|A051–A075|动作主次、反馈、选择、表格与实验边界|[交互与反馈](research/C-interaction/sources.md)|
|A076–A100|键盘、焦点、对比、重排、退化与性能|[前端验收](research/D-acceptance/sources.md) · [验收矩阵](research/D-acceptance/acceptance-matrix.md)|

这些原页来自 W3C/WCAG/APG、USWDS、GOV.UK、Carbon、Docusaurus、VitePress、MDN、React、Diátaxis 等一手文档。研究结合规范说明、原站示例和本教材诊断；不将英语字号、品牌字体或 API 站点的信息密度直接套给中文长文。

## 成品证据

- [原站实际浏览器观察与截图](evidence/01-原站浏览器观察.md)
- [成品独立设计复核](validation/01-成品独立复核.md)
- [完整性与颜色计算](validation/static-results.json)
- [50 个响应式测量点](validation/responsive-results.json)
- [14 项导航与键盘检查](validation/navigation-results.json)
- [7 组实验回归](validation/lab-results.json)
- [6 组放大、间距、打印媒体与退化检查](validation/extended-results.json)
- [5 组焦点、刷新与资源专项检查](validation/special-results.json)

当前验收未发现阻断交付的问题。验证范围是本机 Chromium 渲染和列明的操作样本；未将它称为完整 WCAG 认证、跨浏览器全面测试或真人学习效果研究。范围和限制在最终验收报告中逐项说明。
