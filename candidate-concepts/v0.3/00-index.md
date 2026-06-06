# AF v0.3 Candidate Concepts Index

Status: candidate index / non-canonical
Language status: English working draft; Chinese-first rewrite required before promotion.
Source: 2026-06-06 AF self-application dialogue
Scope: v0.3+ review scaffold

## Boundary

This index lists candidate mechanisms only. None of the entries below are canonical AF rules. They must not be read as changes to AF v0.1.1 or AF v0.2.

The review baseline is: Chinese-first terminology, no invented curvature formula, no UX/prompt/agent/memory reduction, and strict preservation of theory, protocol, application, and execution layers.

## Candidate Mechanisms

| Mechanism | Status | One-line summary | Related existing AF concept | Why not canonical yet | Open questions |
|---|---|---|---|---|---|
| [Zero-curvature baseline](zero-curvature-baseline.md) | Candidate term | Ideal baseline for judging residual deviation from compressed A->F identity, not a success claim. | A/F compression; path identity preservation | Curvature has not been formalized and must remain non-mathematical for now. | How can residual deviation be described without inventing formulas? |
| [Curvature deviation halt](curvature-deviation-halt.md) | Candidate mechanism | Threshold response model: low deviation continues, medium deviation recalibrates, high deviation halts or returns to human judgment. | Halt on gap; high-quality deviation | Needs case testing across execution and protocol layers. | What observable markers distinguish low, medium, and high deviation? |
| [Recursive curvature certification](recursive-curvature-certification.md) | Candidate mechanism | Check sub-AF and micro-AF outputs against parent AF before treating them as support. | Recursive pressure testing; A/F identity | Certification procedure is not yet stable. | Who certifies: AI, user, or protocol record? |
| [Edge-to-AF recursion](edge-to-af-recursion.md) | Candidate mechanism | Expand a key connection edge between AF nodes into a micro-AF when the connection cannot be assumed low-curvature. | Active graph; A/F identity; recursive pressure testing | Connection-expansion criteria are not yet stable. | When is a B-E or C-D style connection important enough to become micro-AF? |
| [Event-center closure](event-center-closure.md) | Candidate mechanism | Closure condition where A-side compaction and F-side reverse necessity converge on an event center under low-curvature stable deviation. | Cognitive sphere outline; active graph; macro-AF preservation | Needs more cases before it can be separated from narrative reconstruction. | How is micro-AF closure recovered into macro-AF before parent closure? |
| [Multi-scale AF encapsulation](multi-scale-af-encapsulation.md) | Candidate mechanism | Treat macro-AF, sub-AF, and micro-AF as possible nested units without requiring every sub-AF to be encapsulated. | AF as goal-unit; cross-session AF | Encapsulation rules remain candidate. | Which scales deserve protocol records? |
| [Macro-AF preservation](macro-af-preservation.md) | Candidate mechanism | Prevent local sub-AF success from replacing or resolving the macro-AF. | Human goal ownership; F identity | Needs clearer relation to sub-AF completion. | How should macro-AF be rechecked after sub-AF completion? |
| [F validity and A/F correspondence gate](f-validity-and-af-correspondence-gate.md) | Candidate gate | Distinguish F validity from whether A actually corresponds to F. | A/F compression; path masquerading as goal | Open A/F must not be treated as invalid. | What is the minimal gate before execution? |
| [Input-state gate](input-state-gate.md) | Candidate gate | Classify input state before treating user expression as an executable task. | A0; prompt burden discipline | Input-state categories need more evidence. | How much gating is useful before it becomes intrusive? |
| [Carrier-agnostic AF](carrier-agnostic-af.md) | Candidate principle | Preserve AF across speech, text, files, tools, repositories, and model routes. | AF as goal-unit beyond a conversation | Carrier boundaries need implementation evidence. | How should carrier shifts be recorded? |
| [AF application stack](af-application-stack.md) | Candidate stack | Keep theory, protocol, application, and execution layers distinct in AF applications. | Protocol layer vs execution layer | Stack boundaries need more examples. | How should products expose the stack without reducing AF to UX? |

## Review Rule

Before any candidate is promoted, it must pass `review/v0.3-candidate-review-checklist.md` and be mapped back to existing AF concepts without rewriting historical versions.