# 进展与后续 / Progress and Next Steps

[中文](#中文) · [English](#english)

状态日期 / Status date: `2026-11-17`。本页是公开进展导航，不是新的工程授权、固定日期承诺或实体安全放行。

## 中文

### 已有进展

| 领域 | 有记录的进展 | 不能由此推出 |
|---|---|---|
| 规则/软件 | 早期 Arena 状态与 Referee 软件基线有离线证据；W13 多卡五阶段软件链到 `state_version=16` | 完整 Arena 规则、当前 R12 源码或物理结算已全部公开/验收 |
| 数字界面 | W13 Headless HTML 有阶段捕获；W14 R12 私有工程的 Unity 全局 PlayMode 有同版收据 | 相机、语音或机器人实机链已通过 |
| 双机/原生接口 | W14 有只读序列和 HostPort/result_reader 候选合同；W15 动作前 Permit 路径对账有收据 | 原生结果生产链、现场标定和动作后验证已齐备 |
| 现场实体动作 | W15 用户确认实体单张 DRAW 已在现场完成 | 同一动作的完整独立机器回执、连续三卡或实体整局已验收 |

### 下一步验收方向

1. **单张 DRAW 证据收口：**核对同一 task/epoch、目标设备响应、标定/布局、动作后原生结果、RGB-D 后验和停止反馈。缺任一关键绑定时如实保留 `UNKNOWN`，不把动作前 Permit 包当成动作完成回执。
2. **当前现场输入：**取得同版、实测的 calibration、site profile、layout 与 waypoint；历史坐标和软件候选不能直接作为新现场真值。
3. **连续桌游流程：**在单张动作闭环证实后，分开验证出牌、弃牌、连续三卡、数字/物理状态一致以及 Referee 提交；每一步有独立可核证据。
4. **游戏质量与公开可复现性：**规则草案仍需纸面试玩、平衡和边界测试；只有通过公开范围审查的代码/资产才能加入展示仓库。当前报告不是完整可复现产品。
5. **持续双仓更新：**每次用户要求归档时，先核私有事实源与主索引，再发布中英一致的脱敏展示并读回两个远端。W15 周末前仍标“进行中”；不得提前补写验收结果。

优先看 [W15 进行中记录](reports/W15_2026-11-16_2026-11-22.md) 与 [证据](evidence/weekly/W15_2026-11-16/README.md)；W14 的结论是此前时间截面，不能因 W15 新进展而回写成“当时已完成”。

## English

This page is a public navigation aid, not a new engineering authorization, fixed-date promise, or physical safety release.

### Evidenced progress

| Area | Recorded progress | Does **not** imply |
|---|---|---|
| Rules/software | An earlier Arena state/Referee baseline has offline evidence; W13's five-stage multi-card software flow reached `state_version=16` | All Arena rules, current R12 source, or physical adjudication are published/accepted |
| Digital interface | W13 captured Headless HTML stages; W14 has same-version global Unity PlayMode receipts from the private R12 product | Camera, speech, or physical robot flow passed |
| Dual-host/native interface | W14 has a read-only sequence and candidate HostPort/result_reader contracts; W15 has a pre-action Permit-path reconciliation receipt | Native result production, measured site calibration, or post-action verification is complete |
| Physical action | In W15, the user confirmed that a physical single-card DRAW was completed on site | The same action has a full independent machine receipt, or continuous three-card/full-game acceptance |

### Next acceptance directions

1. **Close the single-DRAW evidence gap:** Match the same task/epoch, target-device response, calibration/layout, post-action native result, RGB-D observation, and stop feedback. If key bindings are missing, keep the result `UNKNOWN`; a pre-action Permit package is not a completion receipt.
2. **Obtain current measured site inputs:** Bind same-version calibration, site profile, layout, and waypoints. Historical coordinates or software candidates are not new on-site measurements.
3. **Validate a continuous tabletop flow:** After the single-action loop is evidenced, separately test play, discard, consecutive cards, digital/physical state consistency, and Referee submission. Each requires its own auditable evidence.
4. **Improve game quality and public reproducibility:** The rule draft still needs paper playtests, balance review, and edge-case tests. Only source/assets that pass publication review may be added here. Current reports are not a complete reproducible product.
5. **Maintain dual-repository updates:** On each user-requested archive update, verify the private source and primary index first, then publish consistent Chinese/English redacted pages and read back both remotes. W15 remains “in progress” until its week closes; acceptance must not be backdated.

See the [W15 in-progress report](reports/W15_2026-11-16_2026-11-22.en.md) and [evidence summary](evidence/weekly/W15_2026-11-16/README.en.md). W14 is an earlier historical snapshot and must not be rewritten as if W15's progress had already happened.
