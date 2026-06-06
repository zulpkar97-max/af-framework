# AF v0.3 候选概念索引 / AF v0.3 Candidate Concepts Index

状态 / Status:
中文：候选索引 / 非 canonical
English: candidate index / non-canonical

语言状态 / Language status:
中文：中英双语候选稿，以中文为主。
English: Chinese-first bilingual candidate draft.

来源 / Source:
中文：2026-06-06 AF 自应用对话
English: 2026-06-06 AF self-application dialogue

范围 / Scope:
中文：v0.3+ 审查脚手架
English: v0.3+ review scaffold

## 边界 / Boundary

中文：
本索引只列出候选机制。以下任何条目都不是 canonical AF 规则，也不能被解读为对 AF v0.1.1 或 AF v0.2 的修改。

English:
This index lists candidate mechanisms only. None of the entries below are canonical AF rules. They must not be read as changes to AF v0.1.1 or AF v0.2.

中文：
审查基线是：中文优先术语、不发明曲率公式、不降维为 UX / prompt / agent / memory，并严格保持理论层、协议层、应用层和执行层的区分。

English:
The review baseline is: Chinese-first terminology, no invented curvature formula, no UX/prompt/agent/memory reduction, and strict preservation of theory, protocol, application, and execution layers.

## 中文候选机制表

| 机制 | 状态 | 一句话摘要 | 相关既有 AF 概念 | 为什么尚非 canonical | 开放问题 |
|---|---|---|---|---|---|
| [零曲率基线](zero-curvature-baseline.md) | 候选术语 | 用于判断相对 A->F 压实身份残余偏差的理想基线，不是成功声明。 | A/F 压实；路径身份保真 | 曲率尚未形式化，当前必须保持非数学化。 | 如何在不发明公式的情况下描述残余偏差？ |
| [曲率偏差阈值机制](curvature-deviation-halt.md) | 候选机制 | 低偏差继续，中等偏差再校准/递归展开，高偏差停机或返回人类判断。 | 缺口即停；高质量偏航 | 仍需跨执行层与协议层 case 测试。 | 哪些可观察标志区分低、中、高偏差？ |
| [递归曲率认证](recursive-curvature-certification.md) | 候选机制 | sub-AF / micro-AF 输出在被视为支持父 AF 前，需要回查父 AF。 | 递归压力测试；A/F 身份 | 认证流程尚未稳定。 | 由 AI、人类还是协议记录来认证？ |
| [连接边递归 AF 化](edge-to-af-recursion.md) | 候选机制 | 当 AF 节点之间的关键连接边不能假定为低曲率时，将该连接展开为 micro-AF。 | active graph；A/F 身份；递归压力测试 | 连接展开标准尚未稳定。 | B-E 或 C-D 这类连接何时重要到需要 micro-AF 化？ |
| [事件中心闭合](event-center-closure.md) | 候选机制 | A 侧压实与 F 侧反向必要性在事件中心汇合，并满足低曲率稳定偏差。 | 球形理论 outline；active graph；macro-AF 保真 | 仍需更多 case，才能与叙事重构区分。 | micro-AF 闭合如何回收进 macro-AF 后才允许父 AF 闭合？ |
| [多尺度 AF 封装](multi-scale-af-encapsulation.md) | 候选机制 | macro-AF、sub-AF、micro-AF 可作为可能嵌套单元，但不是每个 sub-AF 都必须封装。 | AF 作为目标单元；跨会话 AF | 封装规则仍是候选。 | 哪些尺度值得协议记录？ |
| [宏观 AF 保真](macro-af-preservation.md) | 候选机制 | 防止局部 sub-AF 成功替代或解决 macro-AF。 | 人类目标所有权；F 身份 | 与 sub-AF 完成的关系仍需明确。 | sub-AF 完成后如何复核 macro-AF？ |
| [F 有效性与 A/F 对应门](f-validity-and-af-correspondence-gate.md) | 候选门 | 区分 F 是否有效，以及 A 是否真的对应 F。 | A/F 压实；路径假扮目标 | 开放 A/F 不能被视为无效。 | 执行前的最小门是什么？ |
| [输入状态门](input-state-gate.md) | 候选门 | 在把用户表达当成可执行任务前，先识别输入状态。 | A0；提示负担纪律 | 输入状态分类仍需更多证据。 | 门控多深才有用且不冒犯？ |
| [载体无关 AF](carrier-agnostic-af.md) | 候选原则 | 在语音、文本、文件、工具、仓库和模型路线之间保持 AF 目标身份。 | 跨会话目标单元 | 载体边界需要实现证据。 | 载体转换应如何记录？ |
| [AF 应用栈](af-application-stack.md) | 候选栈 | 保持理论层、协议层、应用层和执行层区分。 | 协议层 vs 执行层 | 栈边界需要更多例子。 | 产品如何暴露协议层而不降维为 UX？ |

## English Candidate Mechanisms Table

| Mechanism | Status | One-line summary | Related existing AF concept | Why not canonical yet | Open questions |
|---|---|---|---|---|---|
| [Zero-Curvature Baseline](zero-curvature-baseline.md) | Candidate term | Ideal baseline for judging residual deviation from compressed A->F identity, not a success claim. | A/F compression; path identity preservation | Curvature has not been formalized and must remain non-mathematical for now. | How can residual deviation be described without inventing formulas? |
| [Curvature Deviation Threshold Mechanism](curvature-deviation-halt.md) | Candidate mechanism | Low deviation continues, medium deviation recalibrates or expands, high deviation halts or returns to human judgment. | Halt on gap; high-quality deviation | Needs case testing across execution and protocol layers. | What observable markers distinguish low, medium, and high deviation? |
| [Recursive Curvature Certification](recursive-curvature-certification.md) | Candidate mechanism | Check sub-AF and micro-AF outputs against parent AF before treating them as support. | Recursive pressure testing; A/F identity | Certification procedure is not yet stable. | Who certifies: AI, user, or protocol record? |
| [Edge-to-AF Recursion](edge-to-af-recursion.md) | Candidate mechanism | Expand a key connection edge between AF nodes into a micro-AF when the connection cannot be assumed low-curvature. | Active graph; A/F identity; recursive pressure testing | Connection-expansion criteria are not yet stable. | When is a B-E or C-D style connection important enough to become micro-AF? |
| [Event-Center Closure](event-center-closure.md) | Candidate mechanism | A-side compaction and F-side reverse necessity converge on an event center under low-curvature stable deviation. | Cognitive sphere outline; active graph; macro-AF preservation | Needs more cases before it can be separated from narrative reconstruction. | How is micro-AF closure recovered into macro-AF before parent closure? |
| [Multi-Scale AF Encapsulation](multi-scale-af-encapsulation.md) | Candidate mechanism | Treat macro-AF, sub-AF, and micro-AF as possible nested units without requiring every sub-AF to be encapsulated. | AF as goal-unit; cross-session AF | Encapsulation rules remain candidate. | Which scales deserve protocol records? |
| [Macro-AF Preservation](macro-af-preservation.md) | Candidate mechanism | Prevent local sub-AF success from replacing or resolving the macro-AF. | Human goal ownership; F identity | Needs clearer relation to sub-AF completion. | How should macro-AF be rechecked after sub-AF completion? |
| [F Validity and A/F Correspondence Gate](f-validity-and-af-correspondence-gate.md) | Candidate gate | Distinguish F validity from whether A actually corresponds to F. | A/F compression; path masquerading as goal | Open A/F must not be treated as invalid. | What is the minimal gate before execution? |
| [Input-State Gate](input-state-gate.md) | Candidate gate | Classify input state before treating user expression as an executable task. | A0; prompt burden discipline | Input-state categories need more evidence. | How much gating is useful before it becomes intrusive? |
| [Carrier-Agnostic AF](carrier-agnostic-af.md) | Candidate principle | Preserve AF across speech, text, files, tools, repositories, and model routes. | AF as goal-unit beyond a conversation | Carrier boundaries need implementation evidence. | How should carrier shifts be recorded? |
| [AF Application Stack](af-application-stack.md) | Candidate stack | Keep theory, protocol, application, and execution layers distinct in AF applications. | Protocol layer vs execution layer | Stack boundaries need more examples. | How should products expose the stack without reducing AF to UX? |

## 审查规则 / Review Rule

中文：
任何候选机制被提升前，都必须通过 `review/v0.3-candidate-review-checklist.md`，并映射回既有 AF 概念；不得重写历史版本。

English:
Before any candidate is promoted, it must pass `review/v0.3-candidate-review-checklist.md` and be mapped back to existing AF concepts without rewriting historical versions.
