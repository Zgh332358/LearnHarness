# R15｜Learn Git Branching

核查日期：2026 年 10 月 7 日。研究范围：教材展现与交互方法；不是 Harness 教程定稿。

一手页面：[实际文章/产品页](https://learngitbranching.js.org/?locale=en)。
补充一手页面：[同站官方关卡文档](https://learngitbranching.js.org/generatedDocs/levels.html)。

## 证据状态与限制

主交互页欢迎文字与同站官方关卡文档已读取。未输入命令，未验证通关判定或动画。关卡文本中的历史技术说明不当作当前 Git 官方事实。

所有观察的 observed_mode 都为 text（此处仅文本）。交互项记录页面明示的操作设计，不代表已经操作验证。

## 独立具体观察

### R15-O01｜入场即说明学习路径（display）

- 页面观察：欢迎页分别建议初学者从第一关开始，熟悉者选择后续关卡。
- 证据位置：主站 welcome 文字。 [一手页面](https://learngitbranching.js.org/?locale=en)。
- 观察方式：页面文本及控件标签；尚未操作。
- 迁移假设：教程应告诉读者沿什么主线学习，而不是让目录承担全部导学责任。
- 限制：不能照搬大量关卡入口；用户要完整读通文档，主线必须足够明确。

### R15-O02｜可查询允许操作的范围（interaction）

- 页面观察：欢迎页提供 show commands 查看命令的入口说明。
- 证据位置：主站 welcome 提示可在终端查看命令。 [一手页面](https://learngitbranching.js.org/?locale=en)。
- 观察方式：页面文本及控件标签；尚未操作。
- 迁移假设：把工具说明视为模型可用动作的明确列表，并就近支持查看。
- 限制：没有实际操作验证；Harness 教材不应要求读者先学习命令语法。

### R15-O03｜图中的对象有稳定编号（display）

- 页面观察：第一关用 C0、C1 标识提交，解释箭头表示祖先关系。
- 证据位置：官方关卡文档 Introduction to Git Commits。 [一手页面](https://learngitbranching.js.org/generatedDocs/levels.html)。
- 观察方式：页面文本及控件标签；尚未操作。
- 迁移假设：请求和结果用稳定编号配对；下一轮可直接指认使用了哪项记录。
- 限制：提交祖先与工具请求因果不同，图例应按 Harness 实际关系重写。

### R15-O04｜示范后立即做小任务（interaction）

- 页面观察：首关演示一次 commit，再让读者自行做两次完成目标。
- 证据位置：官方文档 Git Commits 的示范命令与结束任务。 [一手页面](https://learngitbranching.js.org/generatedDocs/levels.html)。
- 观察方式：页面文本及控件标签；尚未操作。
- 迁移假设：先演示一轮，再让读者识别另一轮由哪项结果触发，使理解可检查。
- 限制：未实测通关；不能把点击下一步的完成当成学习目标达成。

### R15-O05｜用常见错误揭示隐藏状态（interaction）

- 页面观察：分支例子先展示 main 变化而 newImage 未动，再解释当前分支并切换。
- 证据位置：官方关卡文档 Branching in Git 的两组命令与解释。 [一手页面](https://learngitbranching.js.org/generatedDocs/levels.html)。
- 观察方式：页面文本及控件标签；尚未操作。
- 迁移假设：让读者预测查询请求是否已经获得结果，再揭示真实阶段，纠正常见混淆。
- 限制：错误要有明确原因与修正；不能制造无关挫折或用惩罚性反馈。

### R15-O06｜结束目标写成具体状态（display）

- 页面观察：分支与相对引用关卡写明应创建、切换或移动到的目标。
- 证据位置：官方文档 Branching、Relative Refs #2 的完成条件。 [一手页面](https://learngitbranching.js.org/generatedDocs/levels.html)。
- 观察方式：页面文本及控件标签；尚未操作。
- 迁移假设：自测写成可观察判断，例如指出请求的执行者与尚未知的事实。
- 限制：不应把完成指定命令序列视为唯一正确推理路径。

### R15-O07｜公开说明颜色对应规则（display）

- 页面观察：合并关卡解释分支颜色及提交颜色混合所代表的关系。
- 证据位置：官方文档 Merging in Git 的颜色说明。 [一手页面](https://learngitbranching.js.org/generatedDocs/levels.html)。
- 观察方式：页面文本及控件标签；尚未操作。
- 迁移假设：如果给状态着色，必须说明含义并让文字或标记同时承载关系。
- 限制：混色容易增加解释负担，Harness 更适合少量稳定状态标签。

### R15-O08｜允许回看当前任务（interaction）

- 页面观察：合并关卡提示可用 objective 重新显示要求。
- 证据位置：官方文档 Merging in Git 的结束提示。 [一手页面](https://learngitbranching.js.org/generatedDocs/levels.html)。
- 观察方式：页面文本及控件标签；尚未操作。
- 迁移假设：交互进行中仍能随时查看目标和约束，不让读者凭记忆完成。
- 限制：未输入命令验证；宜用简单可见按钮，而非隐蔽口令。

## 不直接迁移的理由

不复制原页面的完整视觉或全部控件。只保留能服务于一个具体学习问题的方法；采用与否需要后续研究—对照—判断循环，再由根代理核查实际操作状态。复杂度、可访问性与技术等同关系均要单独判断。

## 根代理统一浏览器核查建议

根代理在同一空间进入第一关，观察示范后的图，再自行输入两次 git commit 检查目标与通关；第二关可观察创建分支后提交，main 移动而新分支未动的对照。
