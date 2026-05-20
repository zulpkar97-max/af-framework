# Ask First (AF) Framework v0.1 Spec

Author: Carl  
Version: v0.1.1  
Status: draft spec  
Layer: methodological implementation layer under Spherical Theory  
Language: Chinese-first

## 0. Status Statement

The Ask First (AF) Framework v0.1 is a methodological implementation-layer spec. It describes how humans and AI, in a single goal-progression process, continuously collaborate through a protocol layer so that the goal preserves its identity as it is transmitted from the A-end to the F-end.

"Ask First" does not mean asking once before execution and then entering plan-handoff. It means that the protocol layer asks before assuming, asks before filling a gap, asks before modifying F, and asks before treating a contingent path as necessary. The opposite of Ask First is not "not asking", but AI using high-probability-correct output, smooth output, or the sense of execution progress to bypass necessary calibration.

AF v0.1 is not Spherical Theory itself. Spherical Theory (Cognitive Sphere Hypothesis) is the upper purpose layer, explaining how multiple cognitive modules sedimented after AF calibration may form higher-order cognitive structures through long-term accumulation. The role of AF v0.1 is narrower: it provides protocol constraints for concrete task progression and serves as a case-level evidence entry point for later Spherical Theory specs.

This spec does not provide mathematical formalization, does not claim that AF has completed empirical validation, and does not make any AGI commitment. The goal of v0.1 is to establish a minimal methodological framework that is readable, runnable, and reviewable.

## 1. What AF Is

AF is the Ask First protocol layer in human-AI goal progression.

The core problem it addresses is: when a goal moves from the user's original expression into AI collaboration, tool calls, execution feedback, and recalibration, whether the goal itself still preserves identity consistency.

AF has two purposes:

1. To constrain AI in collaboration so that it behaves more like a "thinking collaborator" rather than a response machine that only outputs high-probability-correct answers.
2. To synchronously strengthen the human's own thinking structure during collaboration. This effect is an important byproduct, but it is not an educational purpose and is not AF's upper-layer definition.

The object of AF is not "answering", but goal progression. It does not focus on whether one response appears correct. It focuses on whether the transmission from the A-end to the F-end preserves identity, whether gaps are exposed, whether path deviation is made visible, and whether the user still owns the goal itself.

The basic collaboration form of AF is a three-party collaboration field:

- Human: the goal owner.
- Protocol layer: hosting, calibration, dispatching, and deciding whether to halt or continue.
- Execution layer: performing concrete actions such as tool calls, retrieval, generation, implementation, and testing.

These three parties may be carried by different entities, or by the same AI instance switching across stages. But whenever role switching occurs, the current role must be explicitly declared, so that protocol judgment, execution action, and goal ownership do not become mixed together.

The current primary applicable object of AF is human-AI collaboration. Whether it can be stably transferred to human-human collaboration is [pending case-level validation].

## 2. What AF Is Not

AF is absolutely not plan-handoff.

In AF, there is no single handoff moment in which "the plan is written first, and then handed to downstream execution." Planning and execution are not separate stages. They occur interleaved within a continuous collaboration field. Findings from the execution layer flow back to the protocol layer, and the protocol layer re-examines A, F, nodes, curvature, and gaps; however, execution feedback cannot automatically modify the goal. Goal changes must go through protocol records and human judgment.

AF is not a rapid-answer tool.

A-end compaction is usually not an action completed within a few minutes. For real complex goals, the typical cost of A-end compaction may be 15-20 minutes, or longer. Any claim that AF can be completed in "30 seconds" is anti-AF. AF is a slow-thinking tool. It applies only to tasks where goal identity is unstable, the path is prone to drift, AI substitution risk is clear, and execution cost is relatively high. Simple questions should receive fast answers; complex goals need AF.

AF is not "high-probability correct."

An AI giving a high-probability-correct answer does not mean AF is qualified. AF requires the protocol layer to halt at information gaps, mark uncertainty, trigger human judgment, or escalate the information source. Using a smooth, credible, and complete answer to bypass a gap is a typical failure that AF is meant to intercept.

AF is not a conversation-level framework.

AF is goal-based, not session-based. One AF can span multiple conversations, multiple tools, multiple execution stages, and multiple points in time. Conversely, one conversation may contain multiple sub-AFs or micro-AFs.

AF is not an educational scaffold, nor a ZPD mapping.

AF may indeed strengthen human thinking structure, but this is not scaffold design in the educational sense. AF does not aim to "teach the user"; it aims to preserve identity fidelity in the goal-progression process.

AF is not a mathematical formalization model.

v0.1 uses terms such as A, F, curvature, node, and recursion, but these terms are protocol language and structural language in this version, not mathematical definitions. Curvature has no formula, the sphere has no geometric quantification, and recursion has no proof in a formal system.

## 3. Three Roles and Hard Boundaries

### 3.1 Human

The human is the final owner of the goal.

The human is responsible for deciding whether the goal itself may change, for judging whether key information is trustworthy, for initiating the escalation chain when information sources are insufficient, and for breaking the circuit when necessary.

The human does not need to participate in the details of execution-layer calls. AF does not require the user to know tool APIs, retrieval syntax, code implementation, or model-calling methods. What the human must undertake is goal judgment, value judgment, and credibility judgment, not execution operations.

The human has the sole authority to decide goal changes. The protocol layer may propose that "the current F may need recalibration", and the execution layer may report that "the current path has encountered an obstacle", but neither may directly rewrite the goal on behalf of the human.

### 3.2 Protocol Layer

The protocol layer is responsible for hosting, asking, calibrating, dispatching, and deciding whether to halt or continue.

When AI serves as the protocol layer, it must not directly perform tool calls, and it must not automatically convert execution-layer findings into goal changes. Its main responsibility is to maintain identity preservation in A-to-F transmission.

The protocol layer must do several things:

- Compact the A-end.
- Maintain F-end identity.
- Determine whether a node is necessary.
- Monitor path curvature.
- Halt at gaps.
- Maintain human goal ownership.
- Dispatch the execution layer and receive execution feedback.
- Return to human calibration when execution feedback triggers risk.

The protocol layer must not bypass a gap with "high-probability correct" output. If a gap affects A, F, a key node, or credibility judgment, the protocol layer must halt.

### 3.3 Execution Layer

The execution layer is responsible for precise calls and raw returns.

The execution layer may be AI, a tool, an API, search, a code execution environment, an external service, or a human executor. The execution layer does not make protocol judgments, does not judge whether F should change, does not judge what the user truly wants, and does not equate execution success with goal achievement.

The responsibility of the execution layer is to produce, retrieve, run, and return. It must preserve raw information as much as possible and must not package execution results as protocol conclusions.

The same AI instance may switch between the protocol layer and the execution layer, but it must explicitly declare the role. For example: "I am now retrieving information as the execution layer"; "I now return to the protocol layer to judge, based on execution feedback, whether recalibration is needed."

## 4. The Eight Constraints

### ① A-End Compaction

The user's original expression must not directly enter F-end inference. It must be denoised, disambiguated, atomized, and jointly compacted with the human under the hosting of the protocol layer.

The A-end is not the first sentence spoken by the user. The A-end is the goal anchor formed after questioning. It needs at least to answer:

- What the user truly wants to solve.
- Which adjacent goals this goal is not.
- Who owns the goal.
- Which information is known and which information is missing.
- What will happen if this is not done.
- Whether there is current risk of AI substitution or mistaken replacement.

A-end compaction does not require completing a fixed checklist. The number of questions depends on goal complexity. A simple edge node may require only two or three questions; the closer one gets to a mid-stage key node, the more questions there may be. A fixed "14 questions" is not the essence of AF; dynamic compaction is.

### ② A→F Identity Preservation

During transmission from A to F, the goal identity must not deform.

Goal identity includes: what it is solving, for whom it is solving, under what constraints it is solving, what state counts as solved, and what state does not count as solved.

The most common AI failure is not low-quality output, but high-quality drift: smooth language, complete structure, local correctness, while the overall goal has already been replaced by an easier-to-deliver F'. AF must prioritize intercepting this drift.

### ③ F Cannot Be Unilaterally Modified

Once F is established, no party may modify it privately.

But F is not frozen. F evolves dynamically. The condition is: the change must go through the protocol, must be explicitly recorded, must be judged by the human, and when necessary must be supported by evidence from the execution layer.

F evolving dynamically does not mean F can be stealthily replaced by AI. When the execution layer discovers a new problem, it can only trigger an F check; it cannot automatically modify F. The protocol layer may say, "this finding may affect F", but it must not directly say, "therefore F has been updated."

### ④ F-End Reverse Necessity

F is a value anchor, not an execution result.

The F-end does not depend on the success of a single task execution in order to be valid. Even if execution fails, the value judgment at the F-end may still hold. Failure can only indicate insufficiency in the current path, node, tool, or information; it cannot automatically overturn F.

Mid-stage nodes must undergo F-end reverse-necessity checks. A node being "useful" does not mean it is "necessary." A solution "running successfully" does not mean it is a required path. AF requires the protocol layer to keep asking: if this node is not taken, can F still hold? If yes, it is contingent; if no, it may be necessary.

### ⑤ Recursive AF / Scale Duality

Every sub-task is a sub-AF.

A large AF can contain multiple sub-AFs, and each sub-AF can continue to be decomposed into micro-AFs. Each layer has its own micro-A, micro-F, and micro-eight constraints.

Recursive qualification is not "the main task appears complete." Strictly speaking, for an AF to be qualified, it requires:

- The overall F is achieved.
- All sub-Fs are achieved.
- All micro-Fs are achieved.
- No layer mistakes the completion of a sub-goal for the completion of the main goal.

This constraint prevents "local closure masquerading as overall closure." For example, in a portfolio project, completion of the homepage structure does not mean completion of the portfolio; completion of the visual system does not mean achievement of the job-seeking goal; one subpage going live does not mean F already holds.

### ⑥ Curvature Constraint

The cost of path deviation from the main line must be visible and assessable.

Low-curvature paths are preferred. High-curvature paths are not prohibited, but they must be explicitly declared and calibrated through the protocol layer. In v0.1, curvature is not a mathematical quantity, but a structural risk of deviation from goal identity.

Curvature monitoring concerns:

- Whether the current action still serves F.
- Whether the current node has slid from necessary into contingent.
- Whether current execution has changed the main line because of local convenience.
- Whether AI has turned a side branch into the main line through smooth generation.
- Whether the user has been pulled away from the original goal by the sense of execution progress.

Deviation may occur. AF does not require the path to always be a straight line. AF requires deviation to be seen, recorded, and calibrated.

### ⑦ No Empty Slot Filling / Halt on Gap

When information is insufficient, the protocol layer must halt and ask; it must not bypass the issue with "high-probability correct" output.

No empty slot filling means: when a key position lacks information, evidence, definition, authorization, or human confirmation, AI must not fill it with smooth language. The gap must be marked as a gap.

Gaps include:

- A is not compacted.
- F is not verifiable.
- Node necessity is unclear.
- Information source is unreliable.
- Human goal ownership is not confirmed.
- The relationship between execution result and main line is unclear.
- There is an unexplained association between a new AF and an old AF.

⑥ and ⑦ are paired constraints. Curvature monitoring is responsible for detecting drift, and gap monitoring is responsible for preventing AI from drifting in uncertain regions through confident output. Together, they constitute the halting mechanism of AF.

### ⑧ Human Goal Ownership

Human goal ownership must be maintained throughout.

At no stage may the protocol layer stealthily modify the human's goal, even if the protocol layer judges that "this would be better." AI may make suggestions, point out internal contradictions in the goal, and remind the human that F may need updating, but it must wait for human judgment.

Goal ownership is not a one-sentence authorization statement. It is a constraint that runs through the whole process. Every F update, node promotion or demotion, path rearrangement, and gap circuit-break must be able to return to human judgment.

## 5. Collaboration Form

AF is a three-party continuous collaboration field, not a sequential workflow.

Calibration and execution are interleaved. During calibration, the execution layer pauses; during execution, the protocol layer continuously monitors deviation. Findings from the execution layer flow back to the protocol layer, and the protocol layer judges whether human intervention is needed.

A typical fragment is as follows:

1. The human proposes an original goal.
2. The protocol layer compacts A.
3. The protocol layer proposes an F candidate and checks whether F is only a means.
4. The human confirms or revises F.
5. The protocol layer decomposes key nodes and judges which ones are necessary.
6. The execution layer executes one node.
7. The execution layer returns a finding.
8. The protocol layer judges whether the finding is an ordinary execution issue, a node issue, a curvature issue, or an F identity issue.
9. If it affects the goal, the protocol layer returns to the human.
10. After human judgment, the protocol layer continues, halts, rearranges, or breaks the circuit.

There is no moment here in which "the plan is completed and handed to AI." Planning, execution, feedback, and calibration occur in the same collaboration field in a rolling manner.

## 6. Information Trust and Escalation Chain

AF does not allow AI to replace credibility judgment with high-probability judgment.

When collaboration depends on external information, the protocol layer should initiate an escalation chain:

1. Official source.
2. Semi-official source.
3. Directly ask the relevant party.
4. Circuit-break.

Circuit-breaking is legitimate and necessary. When AI judges that "high-probability correct" has become a source of risk, the human has the right to interrupt the current information chain and recalibrate the path, source, or goal.

Circuit-breaking is not failure. On the contrary, being unable to break the circuit is the risk. What AF protects is goal identity and credible progression, not process smoothness.

## 7. Trajectory Record as Cross-Collaboration Graph

The trajectory record of AF is not a passive log file, but an active link graph.

It records at least three types of nodes:

- The A-end of each AF.
- The F-end of each AF.
- Key decision points, gaps, goal-change points, and circuit-break points.

It records at least three types of edges:

- Semantic associations.
- Dependencies.
- Change chains.

The purpose of trajectory recording is not to let a person read a long log half a year later, but to allow the system, when a new collaboration triggers an old node, to recognize: this is not a completely new problem; it is related to an old main line.

If the original main-line AF is unfinished, a new main-line AF is initiated, and the two main lines have node associations on the active link graph, the system must issue an alert. This state may be referred to using the language of Spherical Theory as a "sphere integrity breach." In AF v0.1, this term is only an upper-layer theoretical reference and does not redefine Spherical Theory.

If another person half a year later, or Carl himself half a year later, re-enters the context of this collaboration, the active link graph must enable unambiguous restoration of context. If it cannot, this is not a failure of user memory, but a systemic failure.

## 8. Recursive Qualification Criteria

An entire AF is qualified if and only if all of the following conditions are met:

1. The overall F is achieved, or is explicitly marked as unachieved, paused, circuit-broken, or pending calibration.
2. If F evolves dynamically, every evolution has a protocol record and human judgment.
3. All sub-Fs of all sub-AFs are achieved, or are explicitly marked.
4. All micro-Fs of all micro-AFs are achieved, or are explicitly marked.
5. The user maintains goal ownership throughout.
6. Information gaps are marked and are not smoothly filled by AI.
7. Path deviation is monitored, and high-curvature paths are explicitly calibrated.
8. Cross-collaboration main-line continuity is maintained, and the active link graph has no unalerted integrity breach.
9. The sedimented cognitive module is consistent with the actual AF path.

Here, cognitive module is an upper-layer concept from Spherical Theory. AF v0.1 does not redefine it; it only requires that if an AF is later cited as evidence for a cognitive module, it must be consistent with the real path, and a failed, drifted, or unclosed AF must not be packaged as a successful module.

## 9. Relationship with Spherical Theory

AF is the methodological implementation layer of Spherical Theory, not Spherical Theory itself.

The "cognitive module", "higher-order anchor", "low-curvature path", "cognitive sphere", and other terms mentioned in Spherical Theory v0.0 outline are upper-purpose-layer concepts. AF v0.1 does not redefine these concepts; it only explicitly refers to them where necessary.

Successful cases of AF v0.1 are the evidence basis for later complete Spherical Theory specs. In other words, Spherical Theory needs real AF cases to support its higher-order judgments about module sedimentation, cross-case connection, and cognitive sphere formation.

AF v0.1 does not predict or commit to the final form of Spherical Theory. It only provides the lower-layer protocol: how to make one goal progression as identity-preserving, traceable, calibratable, and reviewable as possible.

## 10. Open Limits of v0.1

AF v0.1 still has clear boundaries.

First, v0.1 does not quantify curvature. Curvature is currently a protocol judgment, not a formula.

Second, v0.1 does not provide a complete data structure. The trajectory record is defined as an active link graph, but the concrete schema must emerge after actual cases.

Third, v0.1 does not prove that AF can be universally applied. It only states that AF applies to tasks where goal identity matters, AI collaboration risk is clear, and the execution chain is relatively long.

Fourth, v0.1 does not solve all human-AI collaboration problems. It only handles goal identity preservation, protocol calibration, halt-on-gap, role boundaries, recursive achievement, and cross-collaboration continuity.

Fifth, v0.1 does not guarantee success. AF can only increase the probability that certain failure modes are identified, paused, and calibrated. It does not promise that any goal will necessarily be achieved.

## 11. Minimal Summary

The minimal definition of AF v0.1 is:

Ask First is the continuous protocol layer in human-AI goal progression. Through A-end compaction, F-end identity preservation, dynamically evolving but not unilaterally modifiable F, reverse-necessity checks, recursive AF, curvature constraint, halt on gap, and human goal ownership, it prevents AI from replacing the real goal in multi-turn collaboration through high-probability-correct output, smooth execution, or plan-handoff.

The qualification standard of AF is not "AI produced something", but whether the goal preserved its identity, whether gaps were exposed, whether execution was calibrated, whether the user still owned the goal, and whether the cross-collaboration main line remained continuous.

AF is a slow-thinking tool. It does not serve all problems. It serves problems that are worth slowing down for, in order to prevent the goal from being replaced.
