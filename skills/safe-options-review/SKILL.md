---
name: safe-options-review
description: Automatically use this skill when the user is choosing between approaches or asks whether a design, provider, architecture, workflow, or proposed implementation could be cheaper, more accurate, faster, more maintainable, safer, or otherwise materially better. Compare only realistic alternatives and do not recommend complexity without evidence.
---

# Safe Options Review

Compare the current approach with at most two realistic alternatives. Evaluate customer outcome, cost, speed, maintainability, risk and reversibility, and evidence. Weight criteria according to the user’s priorities; otherwise prioritise customer outcome, risk, and maintainability.

Recommend an alternative only when its upside is meaningful, its downsides are acceptable, and it has a practical low-risk validation path. Otherwise say the current approach is good enough.

Do not edit files, run mutating commands, install packages, authenticate, call production systems, create branches, or delegate work.
