# 载体无关 AF / Carrier-Agnostic AF

状态 / Status:
中文：候选原则 / 非 canonical
English: candidate principle / non-canonical

语言状态 / Language status:
中文：中英双语候选稿，以中文为主。
English: Chinese-first bilingual candidate draft.

来源 / Source:
中文：2026-06-06 AF 自应用对话；raw elements 5-9, 14-15, 26-29, 38
English: 2026-06-06 AF self-application dialogue; raw elements 5-9, 14-15, 26-29, 38

层级 / Layer:
中文：协议层；应用层
English: protocol layer; application layer

相关既有 AF 概念 / Related Existing AF Sections:
中文：AF 作为目标单元；跨工具执行；上下文披露
English: AF as goal-unit; cross-tool execution; context disclosure

## 摘要 / Summary
中文：
载体无关 AF 指 AF 应在语音、文本、文件、仓库、工具和模型路由等不同载体之间保持目标身份。

English:
Carrier-agnostic AF means AF should preserve goal identity across carriers such as speech, text, files, repositories, tools, and model routes.

## 候选规则 / Proposed Rule
中文：
A/F 身份不应被视为属于某一个载体。语音、prompt、transcript、GitHub 文件、搜索结果、模型路线和执行工件都是证据或状态载体，而不是 F 的自动替代物。

English:
A/F identity should not be treated as belonging to one carrier. Speech, prompt, transcript, GitHub file, search result, model route, and execution artifact are carriers of evidence or state, not automatic replacements for F.

## 为什么重要 / Why This Matters
中文：
许多失败发生在系统把当前载体当成整个目标时，例如把最后一个 prompt 当成 F，或把工具结果当成目标修订。

English:
Many failures occur when the system treats the current carrier as the whole goal, such as treating the latest prompt as F or a tool result as goal revision.

## 这不是什么 / What This Is Not
中文：
这不是记忆系统，不是文件管理规则，不是声称所有载体同等可靠，也不是 UX 抽象。

English:
This is not a memory system, not a file-management rule, not a claim that all carriers are equally reliable, and not a UX abstraction.

## 开放问题 / Open Questions
中文：
载体转换应如何记录？当证据冲突时，哪个载体优先？高密度工作需要多少载体披露？

English:
How should carrier transitions be recorded? Which carrier has priority when evidence conflicts? How much carrier disclosure is needed for high-density work?

## 审查风险 / Review Risks
中文：
把协议降维成上下文管理；用工具细节压垮用户；把 transcript 当成 active graph。

English:
Collapsing protocol into context management; overloading users with tool details; treating transcript as active graph.
