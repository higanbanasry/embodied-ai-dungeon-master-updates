# W13 Public Evidence Summary (2026-11-02–2026-11-08)

[中文原文 / Chinese source](README.md) · [English report](../../../reports/W13_2026-11-02_2026-11-08.en.md)

This is a redacted summary of private originals, **not** raw test logs, product source, or a directly reproducible experiment package. “Private source identifier” is a relative identifier for an original **not available in this GitHub repository**. A SHA-256 lets someone holding that original compare bytes; it does not prove the reported event on its own. Raw images/audio, device logs, site/controller configuration, and large product ZIPs are excluded.

| ID | Private source identifier (not published) | Original SHA-256 | Public conclusion and limit |
|---|---|---|---|
| E065 | `V47_R56L_WINDOWS_MULTILINE_EXECUTION_20261105/MULTI_LINE_STATUS.json` | `2bbe3ccee63f57eea757ee4c6e0a372f4e8e1f599b29c445746ab19c6a8ba3c2` | The Windows three-card/five-stage software flow reached `state_version=15`; status `WINDOWS_MULTILINE_PARTIAL_GUIDANCE_REQUIRED`. Ubuntu return `NOT_RECEIVED`; physical multi-card `NOT_PROVEN`. |
| E066 | `V47_R56L_WINDOWS_FINAL_GAPS_REPAIR_20261106/WINDOWS_RETURN.json` | `0f70450a44395355f54cd4d2d65e22a0ce556b9311936a5a507bf6bd785b9be3` | Windows multi-card software flow and Headless HTML stage capture completed. Unity PlayMode `BLOCKED`; exact R5 binding, top-camera/Ubuntu depth, meeting audio, and Ubuntu return missing. Physical multi-card unproven. |
| E067 | `V47_R56L_GIT_GOVERNANCE_RETURN_20261106/GIT_STATE_RECEIPT.json` | `6b7a85ad4099e418f19782db8d2443672be2ab79a1c2973cdfa2fe60ddf4b14c` | Independent V47 source governance receipt was `CLEAN`. This proves only that source/readback scope, not public availability of the complete V47 product. |
| E068 | `V47_R56L_D0_WINDOWS_AUTOMATION_RETURN_20261107/P3_STATUS.json` | `bc8029997a4852b16c20016260ca0b48f03bca1d729b80b7292253f44302f7d8` | P3 software candidate included Tags 124/125/126 and hand/discard zones. `REACHABILITY_UNKNOWN`, `physical_io=false`, no permit. |
| E069 | `V47_R56L_D10_WINDOWS_RETURN_20261108/P3_STATE_MACHINE_RECEIPT.json` | `3bc21762bd16ae5ace4de34ed49d90959e9d60f8d57639085ec7fc1fdc51e51b` | Request-driven software machine accepted `15` transitions, ending at `state_version=16`, covering DRAW/IDENTIFY/PLAY/RESOLVE/DISCARD. No physical I/O, motion permit, or Referee commit. |

E065–E069 document software, static, Headless, or source-governance scope from historical receipts; they were **not rerun** for this archive update. They do not prove Ubuntu native startup, Unity PlayMode, live perception/audio, robot motion, or physical Referee submission. Only this summary, source identifiers, and hashes can be checked publicly.
