# ERRATA

本文档记录对仓库内已提交内容的更正与澄清。所有历史 commit 保持不变,作为公开记录;本文件仅记录在后续 commit 中被取代或澄清的内容。

This document records corrections and clarifications to materials previously committed in this repository. All historical commits remain unchanged as part of the public record; this file documents only what has been superseded or clarified in subsequent commits.

---

## 2026-05-20 — AF Framework 命名 / Naming of the AF Framework

### 中文

**问题。** 英文版球形 outline(文件:`cognitive-sphere-v0.0-outline.en.md`,commit `71dcbb24992f985b4d9b9a226fb87ade69c0b589`,2026-05-20)在标题和正文中将 AF Framework 英文展开为 **"Anchored Flow Framework"**。此英文展开是翻译过程中由 AI 助手提出的,**不是作者的原始命名**。

**更正。** 作者对该框架的原始命名是 **Ask First (AF) Framework**。"Ask First" 描述协议层最核心的行为约束:在假设之前、在填补信息缺口之前、在修改目标之前、在把可选路径当成必要路径之前,协议层必须先问,不先答。

**影响范围。**
- 中文版球形 outline(`cognitive-sphere-v0.0-outline.md`,commit `e8a96a514ef7c479d956db0d893fb1e742e6aaec`)只使用符号 "AF",无英文展开,**不受影响**。
- 英文版球形 outline(`71dcbb24...`)是唯一含错误命名的文件。
- AF v0.1 起的所有 commit(`af-v0.1-spec.md`,commit `5fbe6cf5ac103af9e7b1cea209dde3952502de48`,及之后)使用规范命名 **Ask First (AF) Framework**。

**处理原则。** 较早的英文 outline commit `71dcbb24...` **不被重写**,保留在仓库中作为历史记录,本 errata 作为正式更正声明。对外引用本框架时应使用 **Ask First (AF) Framework** 为规范名。

### English

**Issue.** The English translation of the Cognitive Sphere v0.0 outline (file: `cognitive-sphere-v0.0-outline.en.md`, commit `71dcbb24992f985b4d9b9a226fb87ade69c0b589`, 2026-05-20) refers to the AF Framework as **"Anchored Flow Framework"** in its title and body. This English expansion was proposed by an AI assistant during the translation step and was **not the author's original naming**.

**Correction.** The author's original naming of the framework is **Ask First (AF) Framework**. "Ask First" describes the protocol layer's core behavioral constraint: before assuming, before filling information gaps, before modifying the goal, and before treating a contingent path as a necessary one, the protocol layer must ask, not answer.

**Scope of the error.**
- The Chinese Cognitive Sphere outline (`cognitive-sphere-v0.0-outline.md`, commit `e8a96a514ef7c479d956db0d893fb1e742e6aaec`) uses only the symbol "AF" without English expansion and is **unaffected**.
- The English Cognitive Sphere outline (`71dcbb24...`) is the only file containing the incorrect expansion.
- All commits from AF v0.1 onward (`af-v0.1-spec.md`, commit `5fbe6cf5ac103af9e7b1cea209dde3952502de48`, and later) use the canonical name **Ask First (AF) Framework**.

**Policy.** The earlier English outline commit `71dcbb24...` is **not rewritten** and remains in the repository as a historical record, with this errata serving as the formal correction. Any external citation of the framework should use **"Ask First (AF) Framework"** as the canonical name.

---

## Maintenance / 维护

新的 errata 条目按倒序时间追加。每条记录:受影响的文件或 commit、问题、更正、影响范围、对历史 commit 的处理原则。

New errata entries will be appended to this file in reverse chronological order. Each entry records: the file or commit affected, the issue, the correction, the scope, and the policy decision regarding historical commits.
