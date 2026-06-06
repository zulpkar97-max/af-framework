# 曲率偏差阈值机制 / Curvature Deviation Threshold Mechanism

状态 / Status:
中文：候选机制 / 非 canonical
English: candidate mechanism / non-canonical

语言状态 / Language status:
中文：中英双语候选稿，以中文为主。
English: Chinese-first bilingual candidate draft.

来源 / Source:
中文：2026-06-06 AF 自应用对话；raw elements 2-4, 23-27, 40
English: 2026-06-06 AF self-application dialogue; raw elements 2-4, 23-27, 40

层级 / Layer:
中文：协议层
English: protocol layer

相关既有 AF 概念 / Related Existing AF Sections:
中文：缺口即停；执行反馈不能自动改写 F；高质量偏航
English: halt on gap; execution feedback cannot rewrite F; high-quality deviation

## 摘要 / Summary
中文：
曲率偏差阈值机制是针对偏离 A/F 基线的不同程度，给出继续、校准或停机的候选响应模型。

English:
The curvature deviation threshold mechanism is a candidate response model for different degrees of deviation from the A/F baseline: continue, recalibrate, or halt.

## 候选规则 / Proposed Rule
中文：
偏离 A/F 基线不应自动触发停机。低偏差可以继续并监测；中等偏差应触发澄清、递归展开或再校准；高偏差应停机、中止当前路径，或返回人类判断后再继续。

English:
Deviation from the A/F baseline should not automatically trigger halt. Low deviation may continue with monitoring. Medium deviation should trigger clarification, recursive expansion, or recalibration. High deviation should halt, abort the current path, or return to human judgment before further execution.

## 为什么重要 / Why This Matters
中文：
探索和执行中存在一定偏差是正常的。协议问题不是任何偏差，而是失控偏差：它可能保持局部顺滑和高质量表面，却替换或扭曲 F。

English:
Some deviation is normal in exploration and execution. The protocol problem is uncontrolled deviation that preserves local polish while replacing or distorting F.

## 这不是什么 / What This Is Not
中文：
这不是“任何偏差立即停机”的规则，不是公式化阈值，不是一般拒绝规则，不是禁止探索，也不是声称所有偏差都是失败。

English:
This is not an immediate halt rule for any deviation, not a formulaic threshold, not a general refusal rule, not a ban on exploration, and not a claim that all deviation is failure.

## 开放问题 / Open Questions
中文：
哪些可观察标志区分低、中、高偏差？中等偏差何时应转为连接边递归 AF 化？系统如何报告残余偏差而不过度打扰用户？

English:
What observable markers distinguish low, medium, and high deviation? When should medium deviation become edge-to-AF recursion? How should the system report residual deviation without overloading the user?

## 审查风险 / Review Risks
中文：
把阈值写成虚假精确；过度停机；把顺滑漂移误标成低偏差；用协议语言掩盖执行层能力不足。

English:
Turning thresholds into fake precision; halting too aggressively; allowing polished drift under a low-deviation label; hiding execution-layer weakness under protocol language.
