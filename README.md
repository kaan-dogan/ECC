# ECC Safe

A deliberately small, opt-in fork of Everything Claude Code for Kaan's production voice-agent and web-app work.

## What is included

- `/safe-plan` — create an implementation plan and wait for approval.
- `/safe-research` — verify third-party documentation and integration constraints.
- `/safe-review` — review a diff without modifying it.
- `/safe-security-review` — assess security risks without scanning, installing, or fixing anything.
- `/safe-evaluation-design` — design regression and evaluation cases without creating or running tests.

## What is deliberately excluded

No hooks, rules, installers, MCP servers, agent delegation, automatic memory, background services, automatic updates, permission changes, code execution, file editing, test execution, or network requests are included.

Every command is opt-in and must stop before changing files or external systems. Use the output as a review artifact; carry out any approved implementation in a normal, project-specific Claude Code session.

## Origin and licence

This is a heavily reduced fork of [Everything Claude Code](https://github.com/affaan-m/ECC), retained under its MIT licence. It is not affiliated with or supported by the upstream project.
