# D05｜完整主线与按需细节

方法类型：展现（display）。综合日期：2026 年 10 月 7 日。

本文根据 16 个案例的研究记录提炼展现规格，不是现有教程大纲审阅或 HTML 实现。来源部分是已有页面观察；下面的迁移方案、排版与检查均为基于需求基线的设计推断，尚未经过目标读者实验。部分源观察属于交互，但本文只提炼它们需要怎样显示对象、数据与解释。

## 目标问题

教材要有深度，但读者是否被不影响当前问题的协议选项打断？反过来，折叠是不是藏掉了授权、失败或未知这些必须知道的内容？

## 排版与图的具体结构

1. 主线直接给该例的对象、核心过程、关键条件、结果与边界。一个默认例即使完全不展开、也不操作，仍有完整解释。

2. 补充内容按用途命名，例如“查看实际返回字段”“为什么这里不重试”“来源与产品差异”。名称说明展开后能解决什么问题，不只写“高级内容”。

3. 可延后的内容包括协议更多选项、替代实现和扩展实验。授权要求、已发动作的状态、未知事实、验收条件与当前例的必要假设在主线保持可见。

4. 熟悉操作与对象后再增加条件。自由配置或完整实验台作为扩展入口，不让读者刚入场就先学全部设置。

5. 展开内容保留当前阅读位置及其对应对象，并提供回到主线的明确办法。折叠是一种阅读选择，不代表内容不存在，也不减少应有技术深度。

## 来源案例与观察 ID

| 观察 ID | 原案例与可追溯页面 | 能证实的方法证据 | 证据边界 |
| --- | --- | --- | --- |
| R02-O06 | [Bret Victor：Explorable Explanations](https://worrydream.com/ExplorableExplanations/)；[本地案例记录](../evidence/R02-bret-victor-explorable-explanations.md) | 作者要求静态解释成立，读者按自己的疑问再交互。 | text；这是作者陈述的设计原则；本轮未做静态或可访问性验证。默认文字不能只说“看上图”，必须包含必要关系。 |
| R05-O08 | [Nicky Case：The Evolution of Trust](https://ncase.me/trust/words.html)；[本地案例记录](../evidence/R05-The-Evolution-of-Trust.md) | 完整参数实验放末尾且可跳过。 | text；可跳过的是扩展实验，工具执行、状态和验收等核心内容不能因此省略。 |
| R08-O08 | [Nicky Case 与 Vi Hart：Parable of the Polygons](https://ncase.me/polygons/)；[本地案例记录](../evidence/R08-Parable-of-the-Polygons.md) | 引导实验结束后才给开放沙箱。 | text；文字说明真实情境更复杂；不代表所有简化都适用于工具副作用或恢复。 |
| R09-O07 | [Georgia Tech：Interactive Linear Algebra](https://textbooks.math.gatech.edu/ila/vectors.html#subsection-9)；[本地案例记录](../evidence/R09-Georgia-Tech-Interactive-Linear-Algebra.md) | 点与向量解释后，符号习惯放在 Remark，另一种理解放在 Note。 | text；这里只确认独立块组织，不声称这些块可折叠。 |
| R09-O08 | [Georgia Tech：Interactive Linear Algebra](https://textbooks.math.gatech.edu/ila/vectors.html)；[本地案例记录](../evidence/R09-Georgia-Tech-Interactive-Linear-Algebra.md) | HTML 中多个 Example 入口带 knowl 标识和对应示例地址；线性组合也保留独立内嵌图。 | text；确认了 HTML 入口及地址，没有点击展开；不能据此断言无跳转或无加载故障。 |
| R10-O07 | [Immersive Math：向量章](https://immersivemath.com/ila/ch02_vectors/ch02.html)；[本地案例记录](../evidence/R10-Immersive-Math.md) | 定义长度后，正文把 scalar 解释为普通数字，并把具体长度计算延后。 | text；不意味着所有细节都可推迟；关键执行条件不能隐藏。 |
| R12-O06 | [javascript.info：浏览器事件](https://javascript.info/introduction-browser-events)；[本地案例记录](../evidence/R12-javascript-info-Browser-Events.md) | addEventListener 的 options 列表解释基本用途，把捕获和默认行为链接到后续章节。 | text；重要授权、错误和状态条件仍需当前可见，不能一并延后。 |
| R14-O08 | [TensorFlow Playground](https://playground.tensorflow.org/)；[本地案例记录](../evidence/R14-TensorFlow-可控实验台.md) | 作者提供隐藏可见功能并保存特定课题链接的说明。 | text；尚未确认具体开关；完整仪表盘会使读者先学会调参而非看懂机制。 |
| R07-O05 | [Nicky Case：LOOPY](https://ncase.me/loopy/)；[本地案例记录](../evidence/R07-LOOPY-Explorable-Introduction.md) | 先嵌示例，再给从零创建入口。 | text；iframe 被列出不等于嵌入示例已可运行，加载、交互和窄屏状态未验证。 |

这里保留的是研究流记录的证据模式；即使原文介绍了控件，本文件也不新增“已操作可用”的结论。后续浏览器核验应补在案例证据中，再引用核验结果。

## Harness 中适用与不适用的地方

**适用：** 适合正文保留运行与责任解释，协议字段、SDK 用法、替代部署和测量细节按需查看。也适合让不同经验读者阅读同一文本，而不把非技术版本缩成类比摘要。

**不适用：** 不适合把模型提出动作与工具执行的分界、未确认副作用或知识日期塞进折叠区。原例中的 Remark、Note 或 Example 入口不能一概称为已验证的可折叠控件。

## 手机与静态回退

**手机：** 摘要标题可整行点击且有明确展开状态；展开后先说明关联的例和问题。避免嵌套多层折叠与独立内部滚动，让返回主线不依赖精确拖动。

**静态回退：** 导出时将细节移为就近附注或独立补充节，并保留互相指向的编号。默认主线应完整；展开内容以“补充”标题区分，不能被导出遗漏。

## 使用本方法时的检查

- 不展开任何内容仍能区分请求、执行、结果与未知。
- 补充入口名称说明用途，而非制造技术等级门槛。
- 静态导出包含全部必要边界和全部补充来源。

这些检查是未来教材与实现的验收要求，不是已经通过的测试。

