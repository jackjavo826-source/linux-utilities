# Linux Utilities

Personal Linux tooling focused on repeatable troubleshooting and desktop automation.

**Status: documentation stage.** This repository defines the project areas and the evidence required for a source release. It does not currently contain installable scripts.

## Project areas

| Area | Problem | Planned evidence |
| --- | --- | --- |
| Display layout | Restore a multi-monitor layout after reconnecting displays | Session type, connector mapping, before/after layout, and rollback behavior |
| Audio routing | Select the intended output consistently | Detected devices, selected output, and recovery after reconnecting |
| Desktop visualization | Explore an audio spectrum widget with efficiency modes | Signal path, idle behavior, CPU use, and fullscreen pause behavior |
| Diagnostics | Collect useful information without exposing personal system details | Sanitized sample output and explicit read/write behavior |

## Engineering approach

Start with read-only inspection. Make configuration explicit, keep changes reversible, and document the environment where each utility was checked.

Linux desktop behavior can depend on the distribution, desktop version, session type, graphics driver, and connected hardware. Compatibility must be recorded per tool rather than assumed.

## Source release requirements

- State dependencies, required permissions, and all persistent changes.
- Provide a minimal example configuration without personal paths or network details.
- Document installation, removal, and recovery.
- Test normal operation, missing devices, invalid configuration, and repeated runs.
- Record actual results, including any unavailable environments.

## Verification record

No runtime or performance results have been published in this repository yet. Future results should name the tested commit, software versions, procedure, expected behavior, and observed outcome.

See the [portfolio documentation standards](https://github.com/jackjavo826-source/jackjavo826-source/blob/main/PORTFOLIO_STANDARDS.md).
