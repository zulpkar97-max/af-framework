# Edge-to-AF Recursion / 连接边递归 AF 化

Status: candidate mechanism / non-canonical
Language status: English working draft; Chinese-first rewrite required before promotion.
Source: 2026-06-06 AF self-application dialogue; raw elements 10-17, 24-27, 34, 48-50
Layer: protocol layer; can trigger application-layer work
Related existing AF sections: A/F identity preservation; recursive pressure testing; active graph; macro-AF / sub-AF / micro-AF distinction
Summary: A candidate mechanism for expanding a key connection between two AF nodes into a micro-AF when that connection cannot be assumed as low-curvature.
Proposed rule: When a connection edge between two AF nodes, such as B-E or C-D, carries non-trivial assumptions, hidden evidence requirements, disputed necessity, or possible path substitution, the connection itself may be recursively expanded into a micro-AF for clarification before the parent AF treats the edge as stable.
Why this matters: The risk is not mainly an edge case or anomaly. The risk is that a connection that looks like a simple low-curvature bridge may actually contain unresolved A/F correspondence, evidence, or necessity questions. Expanding the edge protects macro-AF continuity without pretending the connection is already certified.
What this is not: This is not ordinary edge-case handling, not issue triage, not a claim that every connection must become an AF, and not a license for infinite recursion.
Open questions: What makes a connection edge sufficiently important to expand? How should B-E or C-D style links be named in public Chinese-first terminology? How does the parent AF remain recoverable while the edge is expanded?
Review risks: Reverting to edge-case language; expanding every link into protocol overhead; losing macro-AF continuity; treating connection expansion as canonical rather than candidate.