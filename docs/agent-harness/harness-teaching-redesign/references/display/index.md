# 展现方法索引

建立日期：2026 年 10 月 7 日。组织单位是展现方法，不是网站或作者。

本组文件读取 [结构化研究观察](../evidence/observations.json) 中的 16 个案例记录，提炼为 7 项独立方法。它不改写当前教程大纲，不实施 HTML，也不把原站的操作说明当成本轮实际操作证明。浏览器核验由根代理在既有空间统一进行。

每篇都包含目标问题、具体图文结构、原案例观察 ID、Harness 适用及不适用处、手机与静态回退、未来验收要求。结构方案属于设计推断；研究记录不是学习效果已经成立的证明。

## 按学习问题选择

| 方法 | 要解决的读者问题 | 使用时的关键约束 |
| --- | --- | --- |
| [D01 固定对象分区与因果方向](D01-fixed-objects-causal-direction.md) | 谁把什么传给谁，反馈进入哪里？ | 逻辑位置不等于物理部署；直接答复分支保持可见。 |
| [D02 步骤数据表与稳定编号](D02-step-data-ledger.md) | 具体做了什么，现在到了哪里，依据来自哪项记录？ | 公开事件不等于模型内部思考；状态不能合成一个成功。 |
| [D03 同一输入的最小差异对照](D03-same-input-minimal-difference.md) | 为什么结果不同，到底改了哪个条件？ | 固定任务、起点与数据；一次只改一个关键条件。 |
| [D04 就近图文解释与同事件多表示](D04-nearby-explanation-linked-representations.md) | 这一句解释的是图中哪个对象和哪项数据？ | 图文与数据共享对象和编号；减少无必要的并列表示。 |
| [D05 完整主线与按需细节](D05-mainline-on-demand-details.md) | 怎样沿完整主线读懂，再查看必要细节？ | 必要的授权、失败、未知和验收不折叠隐藏。 |
| [D06 学习目标、阅读路径与可判断终点](D06-learning-goals-reading-path.md) | 读完要能判断什么，初读与回查怎样走？ | 操作完成不等于理解；目标用可观察判断验收。 |
| [D07 明确图例、简化与证据边界](D07-legends-simplification-evidence-boundaries.md) | 图例是什么意思，哪些被省略，哪些仍未知？ | 文字与线型同时编码；示意图也必须准确。 |

## 方法之间怎样配合

D01 决定图中的对象和方向，D02 给每个事件可查的数据，D03 用固定输入突出某一条件的作用。D04 把这些对象与文字放到同一局部解释里，D05 确保深度不打断主线，D06 明确读者要做到什么，D07 限制图和教学例的误导范围。这是展现规格的配合关系，不规定教材章节顺序。

不需要每张图同时采用七种方法。先确定一个学习问题，再选择能回答它的方法；如果仅用文字或小表能完整表达，就不增加流程图或交互。

## 来源覆盖

以下覆盖 16 个案例、52 条不同观察 ID；全量研究流有 127 条记录。选择数量只说明可追溯覆盖，不说明学习质量。

| 案例 | 展现方法引用 | 原案例证据 |
| --- | --- | --- |
| R01 Red Blob Games：A* | D02、D03 | [案例记录](../evidence/R01-red-blob-a-star.md) |
| R02 Bret Victor：Explorable Explanations | D04、D05、D07 | [案例记录](../evidence/R02-bret-victor-explorable-explanations.md) |
| R03 Seeing Theory：基础概率 | D04 | [案例记录](../evidence/R03-seeing-theory-basic-probability.md) |
| R04 Bartosz Ciechanowski：Gears | D07 | [案例记录](../evidence/R04-ciechanowski-gears.md) |
| R05 Nicky Case：The Evolution of Trust | D02、D05 | [案例记录](../evidence/R05-The-Evolution-of-Trust.md) |
| R06 Nicky Case：The Wisdom and/or Madness of Crowds | D01、D06、D07 | [案例记录](../evidence/R06-The-Wisdom-and-or-Madness-of-Crowds.md) |
| R07 Nicky Case：LOOPY | D05、D06、D07 | [案例记录](../evidence/R07-LOOPY-Explorable-Introduction.md) |
| R08 Nicky Case 与 Vi Hart：Parable of the Polygons | D03、D05 | [案例记录](../evidence/R08-Parable-of-the-Polygons.md) |
| R09 Georgia Tech：Interactive Linear Algebra | D01、D04、D05、D06 | [案例记录](../evidence/R09-Georgia-Tech-Interactive-Linear-Algebra.md) |
| R10 Immersive Math：向量章 | D03、D04、D05 | [案例记录](../evidence/R10-Immersive-Math.md) |
| R11 Python Tutor | D01、D02、D07 | [案例记录](../evidence/R11-Python-Tutor.md) |
| R12 javascript.info：浏览器事件 | D03、D04、D05、D06 | [案例记录](../evidence/R12-javascript-info-Browser-Events.md) |
| R13 Distill：Augmented RNNs | D01、D03、D04、D07 | [案例记录](../evidence/R13-Distill-分层机制解释.md) |
| R14 TensorFlow Playground | D01、D05、D07 | [案例记录](../evidence/R14-TensorFlow-可控实验台.md) |
| R15 Learn Git Branching | D02、D06、D07 | [案例记录](../evidence/R15-LearnGitBranching-示范到任务.md) |
| R16 The Pudding：文本预测 | D02、D03、D04、D07 | [案例记录](../evidence/R16-Pudding-预测依据揭示.md) |

## 共用验收边界

- 每条方法都应对应一个读者能完成的判断，不以动画数量、图的复杂度或页面长度计效果。
- 宽屏、窄屏与静态回退表达同一机制；必要信息不依赖悬停、颜色、连续运动或手动展开。
- 来源证据与本教材设计推断分开。真实调用、教学模拟、产品事实和部署归纳各有标记。
- 后续对照现有教程时，记录具体问题与改动理由；本组方法文件本身不替代该审阅。

## 本轮产物边界

已完成方法综合与文件检查。尚未完成方法在 Harness 教材中的实际实现、浏览器验收或真实非技术读者测试。没有据此声称某方法已经改善本教材学习效果。

