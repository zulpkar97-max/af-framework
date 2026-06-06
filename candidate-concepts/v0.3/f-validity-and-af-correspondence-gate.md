# F Validity and A/F Correspondence Gate / F 有效性与 A/F 对应门

Status: candidate gate / non-canonical
Language status: English working draft; Chinese-first rewrite required before promotion.
Source: 2026-06-06 AF self-application dialogue; raw elements 1-4, 19, 22-24
Layer: protocol layer
Related existing AF sections: A/F compression; target/path distinction; human goal ownership
Summary: A candidate gate that separates whether F is valid from whether A actually corresponds to F.
Proposed rule: Before execution treats user expression as a settled target, the protocol should check whether the apparent F is physically, logically, and value-wise meaningful, and whether A corresponds to that F rather than to a path masquerading as F.
Why this matters: It protects real F from being killed by a failed path, while also preventing impossible or contradictory paths from being promoted into valid goals.
What this is not: This is not a claim that open A/F is invalid, not a demand for full formal proof, and not a refusal mechanism for unusual goals.
Open questions: What is the minimal correspondence check? How should uncertain F be preserved without executing prematurely? How should human裁决 be recorded?
Review risks: Treating uncertainty as invalidity; over-policing exploratory goals; letting the AI impose its own value judgment as F validity.