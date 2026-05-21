# AF Project Architecture v0.1

Status: architecture draft  
Author: Carl (Zulpkar Turxun)  
Repository context: Ask First (AF) Framework  
Related current spec: `af-v0.2-spec.md`  
Related case study: `CASE-STUDY-v0.1.1.md` v0.3.2  
License context: v0.2+ documentation/framework text under CC BY-NC 4.0, except where otherwise noted  

---

## 0. Purpose

This document records the current architecture-level relationship between:

- A/F dynamic path
- Ask First protocol control
- human calibration
- execution feedback
- Cognitive Sphere / 球形理论

It does not replace `af-v0.2-spec.md`.

It does not introduce a new release.

It does not mark `CASE-STUDY-v0.1.1.md` as release-ready.

It is an architecture draft used to preserve the currently agreed project map.

---

## 1. Core Relationship

Ask First is not a standalone interaction rule.

Ask First is the protocol-control layer applied to A/F dynamic path generation and execution.

A/F dynamic path defines how a goal progresses from a current anchor/state A toward a target focus/goal F.

Ask First defines when that path must pause, ask, expose gaps, verify boundaries, or return control to the human goal-owner.

In short:

    A/F dynamic path = goal-progression mechanism
    Ask First = protocol-control layer over that mechanism

Without A/F dynamic path, Ask First risks becoming an isolated interaction rule.

Without Ask First, A/F dynamic path risks becoming an ungoverned path-generation process that can silently replace the goal, fill gaps without authorization, or allow execution to overrun protocol judgment.

---

## 2. A/F Dynamic Path

A/F dynamic path is responsible for:

- generating a path from current A to target F
- generating intermediate nodes
- checking whether each node remains connected to F
- evaluating forward value toward F
- evaluating backward consistency with A, root F, and prior constraints
- allowing the current result to become the next A in a subsequent cycle

A/F dynamic path answers:

    Where are we?
    What is the target?
    What nodes are necessary?
    Which path candidates preserve F?
    Which results can become the next A?

---

## 3. Ask First Protocol Control

Ask First is responsible for protocol governance during path generation and execution.

It controls whether the path may proceed.

Ask First is responsible for:

- exposing information gaps
- preventing goal substitution
- preventing unauthorized AI completion
- preserving human goal ownership
- distinguishing protocol layer from execution layer
- verifying evidence boundaries
- verifying question boundaries
- verifying tool capability claims
- stopping or asking before execution when required

Ask First answers:

    Can this node be advanced?
    Is there an unclosed gap?
    Has F been replaced?
    Is the AI making an unauthorized assumption?
    Is the human goal-owner still holding the decision?
    Is execution being mistaken for protocol correctness?

---

## 4. Human Calibration

Human calibration is the decision point where the human goal-owner confirms, rejects, revises, or re-anchors the path.

Human calibration is not a decorative confirmation step.

It is the mechanism that preserves ownership of F.

A valid A/F path unit must include explicit calibration points where the human goal-owner can:

- confirm a node
- reject a node
- revise the path
- re-state F
- expose a missing constraint
- stop execution
- authorize execution

---

## 5. Execution Feedback

Execution feedback is the return channel from action back into the path.

Execution output does not automatically validate the protocol.

A successful execution result still needs to be checked against:

- whether F was preserved
- whether assumptions were authorized
- whether gaps were exposed
- whether the result can become the next A
- whether the human goal-owner accepts the result

Execution feedback allows one completed path segment to become the starting anchor for the next segment.

---

## 6. Minimal Runtime Unit

The minimal runtime unit is:

    A/F Protocol Path Unit =
    A/F dynamic path
    + Ask First protocol control
    + human calibration
    + execution feedback

This unit is the smallest structure that can show how path generation and protocol control work together.

It is not enough to model only the path.

It is not enough to model only the protocol.

The two must be coupled.

---

## 7. Layer Map

    Cognitive Sphere / 球形理论
      ↓
    A/F Protocol Path Unit network
      ↓
    Single A/F Protocol Path Unit
      ↓
    A/F dynamic path + Ask First control + human calibration + execution feedback
      ↓
    Concrete demo / project / task

---

## 8. Relationship to Cognitive Sphere

Cognitive Sphere / 球形理论 is the upper-level structure that may emerge from accumulated, connected, and reusable A/F Protocol Path Units.

A completed A/F Protocol Path Unit can be packaged as a cognitive unit.

A network of such units can preserve:

- path history
- goal identity
- calibration points
- gap records
- execution feedback
- reusable reasoning structure

The Cognitive Sphere is not defined here in full.

This document only states the current operational relationship:

    Multiple A/F Protocol Path Units
      → accumulated cognitive units
      → connected reusable structure
      → lower operational substrate of Cognitive Sphere

---

## 9. Current Repository Coverage

Current `main` covers:

- Ask First protocol layer
- v0.2 license boundary
- partial governance increments
- release-blocked case study

Current `main` does not yet fully cover:

- A/F dynamic path formal model
- A/F Protocol Path Unit full spec
- curvature / forward-backward value model
- cognitive unit packaging
- Cognitive Sphere full theory
- demo implementation
- cognitive operating system

---

## 10. Non-Goals

This document does not:

- redefine AF as anything other than Ask First in the current repository line
- replace `af-v0.2-spec.md`
- mark v0.2 as release-ready
- create a v0.2 tag
- create a v0.2 release
- alter v0.1.1 MIT historical status
- change license terms
- resolve case study blockers
- define the full Cognitive Sphere theory
- implement a demo
- define a cognitive operating system

---

## 11. Open Next Work

Possible next tasks:

1. Define `A/F Protocol Path Unit v0.1` as a fuller spec.
2. Design the minimal demo showing A/F dynamic path and Ask First control together.
3. Define the curvature / forward-backward value model.
4. Define cognitive unit packaging.
5. Expand Cognitive Sphere from outline into a structured theory draft.
6. Decide whether and when this architecture map should be referenced from README.
