# 递归曲率认证 / Recursive Curvature Certification

状态 / Status:
中文：候选机制 / 非 canonical
English: candidate mechanism / non-canonical

语言状态 / Language status:
中文：中英双语候选稿，以中文为主。
English: Chinese-first bilingual candidate draft.

来源 / Source:
中文：2026-06-06 AF 自应用对话；raw elements 14-17, 34, 48-50
English: 2026-06-06 AF self-application dialogue; raw elements 14-17, 34, 48-50

层级 / Layer:
中文：协议层；适用于 macro-AF、sub-AF 与 micro-AF
English: protocol layer; applies across macro-AF, sub-AF, and micro-AF

相关既有 AF 概念 / Related Existing AF Sections:
中文：递归压力测试；A/F 身份保真；AF 作为目标单元
English: recursive pressure testing; A/F identity preservation; AF as goal-unit

## 摘要 / Summary
中文：
递归曲率认证是一个候选审查步骤，用于检查 sub-AF 或 micro-AF 的输出是否仍然支持父 AF。

English:
Recursive curvature certification is a candidate review step that checks whether sub-AF or micro-AF outputs still support the parent AF.

## 候选规则 / Proposed Rule
中文：
在一个 sub-AF 结果被视为父 AF 的进展之前，系统应认证该子结果是否保留父 A/F 身份、暴露未解决缺口，并且没有用局部成功工件替换 macro 目标。

English:
Before a sub-AF result is treated as progress for a parent AF, the system should certify that the sub-result preserves the parent A/F identity, exposes unresolved gaps, and does not replace the macro goal with a locally successful artifact.

## 为什么重要 / Why This Matters
中文：
子任务可能成功，但父目标仍然漂移。递归认证防止局部成功变成 macro 层替换。

English:
Subtasks can succeed while the parent goal drifts. Recursive certification keeps local success from becoming macro-level substitution.

## 这不是什么 / What This Is Not
中文：
这不是要求每个子任务都成为正式 AF，不是数学证明，也不是 agent planner 校验。

English:
This is not a demand that every subtask become a formal AF, not a mathematical proof, and not agent-planner validation.

## 开放问题 / Open Questions
中文：
认证需要什么最小记录？低风险 micro-AF 中认证能否隐式发生？认证失败应如何报告？

English:
What minimal record is needed for certification? Can certification be implicit in low-risk micro-AF? How should failed certification be reported?

## 审查风险 / Review Risks
中文：
把每一步官僚化；用自动认证替代人类裁决；把递归 AF 混同为普通任务拆解。

English:
Bureaucratizing every step; replacing human judgment with automated certification; confusing recursive AF with ordinary task decomposition.
