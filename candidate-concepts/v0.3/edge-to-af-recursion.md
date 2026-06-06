# 连接边递归 AF 化 / Edge-to-AF Recursion

状态 / Status:
中文：候选机制 / 非 canonical
English: candidate mechanism / non-canonical

语言状态 / Language status:
中文：中英双语候选稿，以中文为主。
English: Chinese-first bilingual candidate draft.

来源 / Source:
中文：2026-06-06 AF 自应用对话；raw elements 10-17, 24-27, 34, 48-50
English: 2026-06-06 AF self-application dialogue; raw elements 10-17, 24-27, 34, 48-50

层级 / Layer:
中文：协议层；可触发应用层工作
English: protocol layer; can trigger application-layer work

相关既有 AF 概念 / Related Existing AF Sections:
中文：A/F 身份保真；递归压力测试；active graph；macro-AF / sub-AF / micro-AF 区分
English: A/F identity preservation; recursive pressure testing; active graph; macro-AF / sub-AF / micro-AF distinction

## 摘要 / Summary
中文：
连接边递归 AF 化指：当两个 AF 节点之间的关键连接边不能被假定为低曲率时，该连接本身可以被展开为一个 micro-AF。

English:
Edge-to-AF recursion means that when a key connection edge between two AF nodes cannot be assumed to be low-curvature, the connection itself may be expanded into a micro-AF.

## 候选规则 / Proposed Rule
中文：
当两个 AF 节点之间的连接边，例如 B-E 或 C-D，承载非平凡假设、隐藏证据要求、有争议的必要性，或可能发生路径替换时，该连接本身可以递归展开为 micro-AF，在父 AF 把该连接视为稳定之前先进行澄清。

English:
When a connection edge between two AF nodes, such as B-E or C-D, carries non-trivial assumptions, hidden evidence requirements, disputed necessity, or possible path substitution, the connection itself may be recursively expanded into a micro-AF for clarification before the parent AF treats the edge as stable.

## 为什么重要 / Why This Matters
中文：
风险不主要来自 edge case 或异常，而是来自看似简单的低曲率连接。该连接内部可能包含未解决的 A/F 对应、证据或必要性问题。展开连接边可以保护 macro-AF 连贯性，同时不假装连接已经被认证。

English:
The risk is not mainly an edge case or anomaly. The risk is that a connection that looks like a simple low-curvature bridge may actually contain unresolved A/F correspondence, evidence, or necessity questions. Expanding the edge protects macro-AF continuity without pretending the connection is already certified.

## 这不是什么 / What This Is Not
中文：
这不是“边缘到 AF 递归”，不是普通 edge case 处理，不是 issue triage，不是声称每条连接都必须成为 AF，也不是允许无限递归。

English:
This is not ordinary edge-case handling, not issue triage, not a claim that every connection must become an AF, and not a license for infinite recursion.

## 开放问题 / Open Questions
中文：
什么使一条连接边重要到需要展开？B-E 或 C-D 这类连接如何用公开的中文优先术语命名？连接展开期间，父 AF 如何保持可回收？

English:
What makes a connection edge sufficiently important to expand? How should B-E or C-D style links be named in public Chinese-first terminology? How does the parent AF remain recoverable while the edge is expanded?

## 审查风险 / Review Risks
中文：
退回 edge case 语言；把每条连接都扩张成协议负担；丢失 macro-AF 连贯性；把连接展开误当成 canonical 规则。

English:
Reverting to edge-case language; expanding every link into protocol overhead; losing macro-AF continuity; treating connection expansion as canonical rather than candidate.
