---
description: Compare realistic approaches against explicit value, cost, speed, maintainability, risk, and evidence criteria without changing anything.
argument-hint: "[current approach, proposed change, or decision]"
---

# Safe Options Review Command

This command determines whether a realistic alternative is materially better than the current approach or proposed plan. Do not redesign for novelty. If the current approach is good enough, say so clearly.

## What This Command Does

1. **Clarifies the decision** — identifies what the current approach is trying to achieve.
2. **Finds realistic alternatives** — compares no more than two credible options.
3. **Evaluates trade-offs** — uses explicit customer, cost, speed, maintainability, risk, and evidence criteria.
4. **Recommends or preserves** — recommends a change only when the expected gain justifies its complexity.

## When to Use

Use `/safe-options-review` when:

- A design, provider, architecture, or workflow choice will materially affect customers or operations.
- The proposed change adds cost, latency, complexity, or vendor dependency.
- A current solution feels inadequate but the reason is not yet clear.
- You need an evidence-based answer before investing engineering time.

Do not use it for trivial implementation details or to solicit speculative redesigns.

## How It Works

1. Restate the decision and the success criteria.
2. Inspect the available project context and supplied evidence.
3. Identify the current approach and up to two realistic alternatives.
4. Compare each option using the relevant evaluation criteria.
5. State which evidence is verified and which claims remain assumptions.
6. Recommend the current approach or a better option, with a smallest safe validation experiment.

## Scope and boundaries

Inspect the repository and supplied context only with read-only tools. Do not edit files, run mutating commands, install packages, authenticate to services, call production systems, create branches, send messages, or delegate work.

Compare the current approach with no more than two realistic alternatives. Do not invent theoretical options with no credible path to implementation.

## Evaluation criteria

Assess each option against the criteria relevant to the decision:

1. **Customer outcome** — accuracy, reliability, user experience, conversion, and, for voice-agent work, call quality and tone.
2. **Cost** — provider spend, infrastructure cost, engineering time, and ongoing support effort.
3. **Speed** — response latency, time to ship, and manual operational effort.
4. **Maintainability** — ease of understanding, debugging, changing, and handing off.
5. **Risk and reversibility** — privacy, security, blast radius, vendor dependency, and ability to roll back.
6. **Evidence** — distinguish data, tests, or official documentation from assumptions.

Weight the criteria according to the user’s stated priority. If no priority is given, default to customer outcome, risk, and maintainability over novelty.

## Decision Rule

Recommend an alternative only when it has a meaningful advantage in at least one important criterion, no unacceptable downside in the others, and a practical low-risk way to validate the claim.

Otherwise return: **Keep the current approach. The expected gain does not justify added complexity.**

## Output Contract

Return:

1. Current approach and decision context
2. One or two realistic alternatives
3. Concise trade-off comparison
4. Recommendation and rationale
5. Smallest safe validation experiment
6. Confidence level, evidence, and remaining unknowns
