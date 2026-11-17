# W15 进行中证据摘要（更新至 2026-11-17）

本页仅记录可公开的来源身份与结论边界，不包含私有产品源码、完整交接包、原始媒体或设备日志。“原件来源标识”不是 GitHub 可打开的路径；SHA-256 供持有私有原件的项目成员核对。W15 尚未结束，本页不是周末验收。

| ID | 原件来源标识（未公开） | 原件 SHA-256 | 可公开的结论与限制 |
|---|---|---|---|
| E080 | `V47_PRIVATE_REPO/evidence/r12-single-draw-status-20261116/R12_SINGLE_DRAW_STATUS.json` | `993cc8b6c5c4e6897ff637378e6fb3daba5dd45245ec9fed6ffa3b40eff4c5ac` | 私有记录状态为 `USER_CONFIRMED_SINGLE_DRAW_COMPLETED`；用户又在 11 月 17 日明确确认实体单张 DRAW 已完成。该记录注明仓库内没有独立的动作后 RGB-D 帧；本项不是完整机器结果回执。 |
| E081 | `R12_PERMIT_PATH_RECONCILIATION_READY_20261116.zip` | `a2446be202aed001bf38cbaedaa1bef1ded0412ff7a040a80af829ce32b23d5d` | 返回包 CRC 通过，Permit 路径对账状态为 `NEW_TASK_READY_NO_DISPATCH`；包内 `used=false`、`physical_io=false`、`motion_calls=0`、Referee commit 为 0。它支持动作前链路准备，不证明后续现场动作已由机器独立验收。 |
| E082 | `V47_PRIVATE_REPO/apps/windows-authority/source_snapshot/tabletop_agent/v47_rebuild/server.py` | `b09d03c25b4c2ba0ecb2df388d8ea1d68b35c75910f12be793d5c54c44f0759a` | 私有来源仓库存在 HTML 项目会话、Permit/Dispatch 路由和任务身份对齐的源提交；本次只读核对源码身份，没有重新运行双机或现场测试，源码未上传。 |

## 分级说明

- E080 的事实是“用户现场确认实体单张 DRAW 完成”；独立机器结果验证仍为 `UNKNOWN`。这不是把真实事件降为软件模拟，而是区分现场确认与可独立复核的机器证据。
- E081、E082 是动作前对账与静态源码证据，不是 `LIVE` 动作结果。
- 连续三卡、出牌、弃牌、完整对局、动作后 RGB-D 与实体 Referee 不在本次完成范围。
