# W15 In-progress Public Evidence Summary (updated 2026-11-17)

[中文原文 / Chinese source](README.md) · [English report](../../../reports/W15_2026-11-16_2026-11-22.en.md)

This page records publishable source identities and claim boundaries. It excludes private product source, full handoff packages, raw media, and device logs. A source identifier below is **not a GitHub-openable path**; SHA-256 is for a project member holding the original. W15 is ongoing, not an end-of-week acceptance report.

| ID | Private source identifier (not published) | Original SHA-256 | Public conclusion and limit |
|---|---|---|---|
| E080 | `V47_PRIVATE_REPO/evidence/r12-single-draw-status-20261116/R12_SINGLE_DRAW_STATUS.json` | `993cc8b6c5c4e6897ff637378e6fb3daba5dd45245ec9fed6ffa3b40eff4c5ac` | Private status `USER_CONFIRMED_SINGLE_DRAW_COMPLETED`; the user reconfirmed on 2026-11-17 that a physical single-card DRAW was completed on site. The private record notes no independent post-action RGB-D frame in the repository. Not a complete machine-result receipt. |
| E081 | `R12_PERMIT_PATH_RECONCILIATION_READY_20261116.zip` | `a2446be202aed001bf38cbaedaa1bef1ded0412ff7a040a80af829ce32b23d5d` | Return ZIP passed CRC; Permit path status `NEW_TASK_READY_NO_DISPATCH`, with `used=false`, `physical_io=false`, `motion_calls=0`, and Referee commit 0. This is pre-action support, not independent acceptance of the later on-site action. |
| E082 | `V47_PRIVATE_REPO/apps/windows-authority/source_snapshot/tabletop_agent/v47_rebuild/server.py` | `b09d03c25b4c2ba0ecb2df388d8ea1d68b35c75910f12be793d5c54c44f0759a` | Private source shows HTML project sessions, Permit/Dispatch routes, and task identity alignment. This archive checked source identity read-only; no renewed dual-host/device execution, and source is not uploaded. |

E080 is **user confirmation of a real on-site event**; independent machine-result verification remains `UNKNOWN`. E081 and E082 are pre-action/static evidence, not a `LIVE` post-action result. Consecutive three-card handling, play, discard, a full game, post-action RGB-D, and physical Referee acceptance are outside this completed scope.
