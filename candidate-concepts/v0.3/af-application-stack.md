# AF Application Stack / AF 应用栈

Status: candidate stack / non-canonical
Source: 2026-06-06 AF self-application dialogue; raw elements 21, 26-30, 33-40, 41-42
Layer: theory layer, protocol layer, application layer, execution layer
Related existing AF sections: protocol layer vs execution layer; human goal ownership; tool route disclosure
Summary: A candidate stack for keeping AF theory, protocol, application, and execution layers distinct when AF is applied to products or workflows.
Proposed rule: AF applications should state which layer is being discussed: theory explains candidate structure; protocol governs A/F preservation and halt conditions; application designs product or workflow behavior; execution performs tool/model/file actions.
Why this matters: Without layer separation, AF is easily absorbed into UX, prompt engineering, agent planning, model routing, or memory systems.
What this is not: This is not a product architecture mandate, not an agent-planner design, and not a reduction of AF to an implementation stack.
Open questions: How should products expose protocol-layer behavior without turning it into visible UI clutter? How should execution feedback return to protocol without rewriting F?
Review risks: Making AF look like software architecture only; hiding protocol decisions inside product UX; treating execution success as protocol success.