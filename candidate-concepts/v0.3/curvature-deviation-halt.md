# Curvature Deviation Halt / 曲率偏差阈值机制

Status: candidate mechanism / non-canonical
Language status: English working draft; Chinese-first rewrite required before promotion.
Source: 2026-06-06 AF self-application dialogue; raw elements 2-4, 23-27, 40
Layer: protocol layer
Related existing AF sections: halt on gap; execution feedback cannot rewrite F; high-quality deviation
Summary: A candidate threshold mechanism for responding to curvature deviation from the compressed A/F baseline.
Proposed rule: Deviation from the A/F baseline should not automatically trigger halt. Low deviation may continue with monitoring. Medium deviation should trigger clarification, recursive expansion, or recalibration. High deviation should halt, abort the current path, or return to human judgment before further execution.
Why this matters: Some deviation is normal in exploration and execution. The protocol problem is uncontrolled deviation that preserves local polish while replacing or distorting F.
What this is not: This is not an immediate halt rule for any deviation, not a formulaic threshold, not a general refusal rule, not a ban on exploration, and not a claim that all deviation is failure.
Open questions: What observable markers distinguish low, medium, and high deviation? When should medium deviation become edge-to-AF recursion? How should the system report residual deviation without overloading the user?
Review risks: Turning thresholds into fake precision; halting too aggressively; allowing polished drift under a low-deviation label; hiding execution-layer weakness under protocol language.