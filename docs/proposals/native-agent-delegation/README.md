# Native-agent delegation in an owner-authorized workspace

A discussion package for [Rakazo #1479](https://github.com/elie222/rakazo/issues/1479).

**Status: proposal and interactive mockup.** The interface uses fictional fixture data. It does not connect to a machine, run an agent, edit project files, or grant permissions. No implementation PR is included.

| Material | Purpose |
|---|---|
| [Architecture proposal](architecture.md) | Scope, integration points, execution contract, recovery, permissions, and PR sequence |
| [Interaction design](interaction-design.md) | User flow, state transitions, approval behavior, and screenshots |
| [Interactive prototype](prototype.html) | Download the HTML file and open it locally; no server or external dependencies are required |
| [Prototype checks](verification.json) | Local interaction and layout checks, with explicit limits |

The first proposed increment supports a single Linux host, a registered workspace, Codex, restricted SSH, and read-only work initiated by the owner in a direct conversation. Workspace writes with native approvals and outbound enrollment are subsequent increments.

This extends delegated work rather than replacing the bot's primary harness. It does not claim to implement the full computer-host feature in #1479 or the primary-harness selection in [#1379](https://github.com/elie222/rakazo/issues/1379).

The prototype stores only its local demo state in the browser. Its apparent refresh recovery is not a test of backend persistence. GitHub displays the HTML source; download it to interact with the mockup.
