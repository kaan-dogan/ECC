---
description: Design read-only regression and evaluation cases before a change.
argument-hint: "[feature, call flow, or prompt change]"
---

# Safe Evaluation Design

Design a test and evaluation plan for the requested change. Cover success paths, failure paths, boundary cases, regressions, observability, acceptance criteria, and a minimal rollout or rollback signal.

For voice-agent work, include realistic conversation scenarios, handling of uncertainty, escalation behaviour, latency and tone considerations, and privacy-safe test data. Do not create tests, run tests, touch production data, or change any files.
