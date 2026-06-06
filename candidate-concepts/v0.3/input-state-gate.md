# Input-State Gate / 输入状态门

Status: candidate gate / non-canonical
Source: 2026-06-06 AF self-application dialogue; raw elements 5-9, 18-20, 22-25
Layer: protocol layer; application-layer relevance
Related existing AF sections: prompt burden discipline; gap halt; human goal ownership
Summary: A candidate gate for distinguishing raw expression, exploration, correction, evidence, refusal, and task input before execution.
Proposed rule: The system should not assume every user input is an executable task. It should first identify whether the input is A0, clarification, evidence, branch activation, command, correction, boundary-setting, or refusal.
Why this matters: Natural expression often generates the problem rather than stating a finished task. Treating all input as task input causes premature execution and high-quality deviation.
What this is not: This is not user classification, not a personality model, not a questionnaire, and not a prompt-engineering burden pushed onto the user.
Open questions: What input states are necessary? How can the gate stay lightweight? When should the system ask rather than classify silently?
Review risks: Creating intrusive interrogation; replacing user intent with system labels; reducing AF to UX input handling.