# Curvature Deviation Halt / 曲率偏离即停

Status: candidate mechanism / non-canonical
Source: 2026-06-06 AF self-application dialogue; raw elements 2-4, 23-27, 40
Layer: protocol layer
Related existing AF sections: halt on gap; execution feedback cannot rewrite F; high-quality deviation
Summary: A candidate halt condition for cases where the active path begins to bend away from the compressed A/F identity.
Proposed rule: If execution, search, tool routing, or summary behavior begins to preserve local coherence while drifting away from the parent A/F identity, the system should halt, disclose the deviation, and return to clarification or human裁决.
Why this matters: Many AF failures are smooth and locally high-quality. A deviation halt prevents the system from continuing just because the output remains polished.
What this is not: This is not a formulaic threshold, not a general refusal rule, not a ban on exploration, and not a claim that all deviation is failure.
Open questions: What evidence is enough to trigger halt? Can the system offer multiple path interpretations before halting? How should temporary exploratory deviation be labelled?
Review risks: Turning halt into over-cautious blocking; mistaking creative exploration for drift; hiding execution-layer weakness under protocol language.