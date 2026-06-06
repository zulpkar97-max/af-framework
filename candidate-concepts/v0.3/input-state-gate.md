# 输入状态门 / Input-State Gate

状态 / Status:
中文：候选门 / 非 canonical
English: candidate gate / non-canonical

语言状态 / Language status:
中文：中英双语候选稿，以中文为主。
English: Chinese-first bilingual candidate draft.

来源 / Source:
中文：2026-06-06 AF 自应用对话；raw elements 5-9, 18-20, 22-25
English: 2026-06-06 AF self-application dialogue; raw elements 5-9, 18-20, 22-25

层级 / Layer:
中文：协议层；关联应用层
English: protocol layer; application-layer relevance

相关既有 AF 概念 / Related Existing AF Sections:
中文：提示负担纪律；缺口即停；人类目标所有权
English: prompt burden discipline; gap halt; human goal ownership

## 摘要 / Summary
中文：
输入状态门用于在执行前区分原始表达、探索、修正、证据、拒绝和任务输入。

English:
The input-state gate distinguishes raw expression, exploration, correction, evidence, refusal, and task input before execution.

## 候选规则 / Proposed Rule
中文：
系统不应假设每个用户输入都是可执行任务。它应先识别输入是 A0、澄清、证据、分支激活、命令、修正、边界设定还是拒绝。

English:
The system should not assume every user input is an executable task. It should first identify whether the input is A0, clarification, evidence, branch activation, command, correction, boundary-setting, or refusal.

## 为什么重要 / Why This Matters
中文：
自然表达经常是在生成问题，而不是陈述完成的任务。把所有输入都当成任务，会导致过早执行和高质量偏航。

English:
Natural expression often generates the problem rather than stating a finished task. Treating all input as task input causes premature execution and high-quality deviation.

## 这不是什么 / What This Is Not
中文：
这不是用户分类，不是人格模型，不是问卷，也不是把 prompt engineering 负担推给用户。

English:
This is not user classification, not a personality model, not a questionnaire, and not a prompt-engineering burden pushed onto the user.

## 开放问题 / Open Questions
中文：
哪些输入状态是必要的？这个门如何保持轻量？什么时候系统应该询问，而不是静默分类？

English:
What input states are necessary? How can the gate stay lightweight? When should the system ask rather than classify silently?

## 审查风险 / Review Risks
中文：
制造侵入式审问；用系统标签替代用户意图；把 AF 降维成 UX 输入处理。

English:
Creating intrusive interrogation; replacing user intent with system labels; reducing AF to UX input handling.
