# Macro-AF Preservation / 宏观 AF 保真

Status: candidate mechanism / non-canonical
Language status: English working draft; Chinese-first rewrite required before promotion.
Source: 2026-06-06 AF self-application dialogue; raw elements 2-4, 10-11, 27, 34, 42
Layer: protocol layer
Related existing AF sections: F identity; human goal ownership; execution feedback cannot modify goal
Summary: A candidate preservation rule that prevents sub-AF progress from replacing the macro-AF.
Proposed rule: Completion, failure, or tool feedback from a sub-AF must be mapped back to the macro-AF before it is treated as resolving, modifying, or invalidating the macro goal.
Why this matters: Local success is one of the easiest ways to create high-quality deviation: the artifact works, but the original F has been replaced.
What this is not: This is not resistance to useful subgoals, not a denial of execution-layer value, and not a claim that macro-AF is immutable.
Open questions: What is the minimum macro-AF recheck after sub-AF completion? How should macro-F changes be recorded when the human intentionally changes F?
Review risks: Freezing macro goals too rigidly; making sub-AF work appear unimportant; confusing preservation with refusal to adapt.