# Carrier-Agnostic AF / 载体无关 AF

Status: candidate principle / non-canonical
Language status: English working draft; Chinese-first rewrite required before promotion.
Source: 2026-06-06 AF self-application dialogue; raw elements 5-9, 14-15, 26-29, 38
Layer: protocol layer; application layer
Related existing AF sections: AF as goal-unit; cross-tool execution; context disclosure
Summary: A candidate principle that AF should preserve goal identity across carriers such as speech, text, files, repositories, tools, and model routes.
Proposed rule: A/F identity should not be treated as belonging to one carrier. Speech, prompt, transcript, GitHub file, search result, model route, and execution artifact are carriers of evidence or state, not automatic replacements for F.
Why this matters: Many failures occur when the system treats the current carrier as the whole goal, such as treating the latest prompt as F or a tool result as goal revision.
What this is not: This is not a memory system, not a file-management rule, not a claim that all carriers are equally reliable, and not a UX abstraction.
Open questions: How should carrier transitions be recorded? Which carrier has priority when evidence conflicts? How much carrier disclosure is needed for high-density work?
Review risks: Collapsing protocol into context management; overloading users with tool details; treating transcript as active graph.