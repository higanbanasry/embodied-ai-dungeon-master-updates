# W14 公开证据摘要（2026-11-09—2026-11-15）

本页是对本地原始记录的脱敏摘录，不是测试日志、完整产品、源代码或可直接复跑的实验包。“来源标识”是未随 GitHub 提交发布的原工作区相对文件名；SHA-256 用于将本摘要与原件核对。现场照片、音频、设备日志、控制器信息和大型产品 ZIP 均未上传。

| ID | 原件来源标识（未公开） | 原件 SHA-256 | 可公开的结论与限制 |
|---|---|---|---|
| E070 | `D11_WINDOWS_GUIDANCE_REVIEW_AFTER_UBUNTU_20261109/ubuntu_origin_input/UBUNTU_ORIGIN_D11_READONLY_RESULT.json` | `db0ded9f5c1fb734a33e8fb69f9012a4af3dfeba616d36f705a8a7a7031ba0b2` | D11 只读 health/state/query 序列返回，R12 runtime binding 身份匹配；服务端相关性仍需继续核对，模式为 `SYNTHETIC_OFFLINE`，physical I/O 和 Referee commit 为 0。 |
| E071 | `D11R1_UBUNTU_HTML_READONLY_SUPPORT_20261109/evidence/HTML_SOURCE_OFFLINE_RECEIPT.json` | `58ea4ef1012071eb465b23947d8dc5763e056652501849b15662184c50ad509f` | contract/state/handshake/query 源码检查为 `PASS_SOURCE_ONLY_BROWSER_NOT_RUN`；浏览器截图、运动、permit 和 Referee commit 未发生。 |
| E072 | `D12_WINDOWS_INTEGRATED_DEMO_REVIEW_20261110/FINAL_RESULT.json` | `a34046d5e7a7931118589f8fd8e787d3eddfcf9e8f2c0d0ce8a34859e472a7b8` | D12 状态为 `PARTIAL_REAL_PROGRESS`；R12 绑定、三卡 15 阶段计划、launcher/readiness 和本地输入收据形成，但现场识别、实时语音、Ubuntu RGB-D、实体三卡和物理 Referee 未证明。 |
| E073 | `TT_V47_R12_WINDOWS_FULL_PRODUCT_20261111/02_PRODUCT_STATUS.json` | `c2fd968ebf17c1787a816ef4a4069a8b6629218b902b21965d0f8f26a444e82d` | D12R5 软件 smoke `14/14`、D12R6 `5/5`；Unity 全局 PlayMode 状态为 `PROVEN`，但 Ubuntu context 为 `BLOCKED_REAL_CONTEXT_NOT_AVAILABLE`，physical I/O、motion、permit 和 Referee commit 为 0。 |
| E074 | `TT_V47_R12_D12R5_WINDOWS_NATIVE_VERIFIER_GUIDANCE_REVIEW_20261111/05_TASK_RESULT_STATE_CONTRACT.json` | `99fece3df4835e4dcd62c0db29cb33b18f9bfb76da850ca6f655f49f5d384b72` | 原生 verifier 合同候选明确 business `state_version=0–16` 与 Ubuntu 17 supervision phases 分离，并要求 task/epoch/calibration/layout/posterior/STOP 字段；状态为等待 Ubuntu native confirmation，未创建 permit。 |
| E075 | `TT_V47_R12_WINDOWS_P3_FULL_GAME_CONSOLE_UPDATE_20261113/evidence/FULL_STACK_INTEGRATION_RECEIPT.json` | `fd39868665b66c99ba47804e71e0115872b0cfe44be1974fc2cb1af81e6a84d1` | 软件全栈演示包含 3 名玩家、2 个场景、29 个动作和 44 帧；Unity PlayMode `Passed`，44 帧、6 张截图；视觉/ASR/TTS 为合成，Ubuntu、相机、麦克风、机器人和吸取 I/O 未使用。 |
| E076 | `TT_V47_R12_UBUNTU_SUPPLEMENT_AWARE_RETURN_20261115/13_CURRENT_STATUS.md` | `66318af8dae2f53f74bf3bb027313409130374339811cddc44ee77a4f21ab128` | HostPort/result_reader 仍为候选或查询级；R12 实测 calibration、site profile、layout plan、实体 program/plan/waypoint 尚未生成。 |
| E077 | `TT_V47_V3_CURRENT_INTEGRATION_MATERIALS_20261115/04_三类动作定义与示例/ACTION_STATUS_SUMMARY.json` | `840f7ae339a8fec765034bfaeb931f26f2f4405e5cda4b49ed5488190c153607` | 当前 draw/play/discard 均为 Windows software-only；缺少 Ubuntu measured calibration/site profile、当前 R12 layout plan、HostPort production injection 和 native result_reader receipt。 |
| E078 | `TT_V47_R12_HOSTPORT_SENIOR_REVIEW_20261115/19_R12_ARTIFACT_GENERATION_RESULT.json` | `f8200e25217636d443c2c40983e49563c97f1b6632b3d817093c5603c2d4b491` | R12 artifact generation 为 `R12_ARTIFACT_GENERATION_BLOCKED`，原因是 calibration 未测量；未发生 physical I/O、permit、motion 或 Referee commit，禁止历史复用。 |
| E079 | `TT_V47_R12_UBUNTU_ONE_SHOT_MEASURED_CONTEXT_20261115/06_V3_STAGE_UPDATE.json` | `d5f38f4fc46581fd107fc3639b9d9d143fe35333da872fb3c6578308782c009d` | 源码/合同核对通过，HostPort 和 result_reader 仍是 candidate，真实 R12 program/plan/waypoint 阻塞；permit/Dispatch/RGB-D 后验未开始，安全边界全为 false/0。 |

## 证据等级与复现边界

- E070–E079 是只读、静态、软件或候选合同证据；它们不构成 Ubuntu 原生、现场设备或物理 Referee 验收。
- Unity PlayMode 通过只表示私有同版软件工程中的 PlayMode 结果；不表示相机、语音、机械臂或实体卡牌已通过。
- 原始来源仍在私有审阅层；公开仓库只能核对本页文本、来源标识和 SHA-256。
