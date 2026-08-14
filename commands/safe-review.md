---
description: Review local changes or a specified pull request without modifying anything.
argument-hint: "[PR URL or blank for local diff]"
---

# Safe Review

Read the requested diff and surrounding code. Report only well-supported findings with file locations, a concrete failure mode, severity, and suggested next step. Include missing tests and user-facing regressions.

Do not edit files, run fixers, commit, push, comment on a pull request, or alter any external system. A clean review is a valid result.
