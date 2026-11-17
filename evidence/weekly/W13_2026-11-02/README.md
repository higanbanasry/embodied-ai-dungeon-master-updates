# W13 公开证据摘要（2026-11-02—2026-11-08）

本页是对本地原始记录的脱敏摘录，不是测试日志、完整产品、源代码或可直接复跑的实验包。“来源标识”是未随 GitHub 提交发布的原工作区相对文件名；SHA-256 用于将本摘要与原件核对。原始图像、音频、设备日志、现场配置、控制器信息和大型产品 ZIP 均未上传。

| ID | 原件来源标识（未公开） | 原件 SHA-256 | 可公开的结论与限制 |
|---|---|---|---|
| E065 | `V47_R56L_WINDOWS_MULTILINE_EXECUTION_20261105/MULTI_LINE_STATUS.json` | `2bbe3ccee63f57eea757ee4c6e0a372f4e8e1f599b29c445746ab19c6a8ba3c2` | 三卡五阶段 Windows 软件链记录到 `state_version=15`；状态 `WINDOWS_MULTILINE_PARTIAL_GUIDANCE_REQUIRED`，Ubuntu 回包为 `NOT_RECEIVED`，多卡物理为 `NOT_PROVEN`。 |
| E066 | `V47_R56L_WINDOWS_FINAL_GAPS_REPAIR_20261106/WINDOWS_RETURN.json` | `0f70450a44395355f54cd4d2d65e22a0ce556b9311936a5a507bf6bd785b9be3` | Windows 多卡软件状态链和 Headless HTML 阶段捕获完成；Unity PlayMode 为 `BLOCKED`，R5 精确绑定、TopCamera/Ubuntu 深度、会议音频和 Ubuntu 回包仍缺失，物理多卡未证明。 |
| E067 | `V47_R56L_GIT_GOVERNANCE_RETURN_20261106/GIT_STATE_RECEIPT.json` | `6b7a85ad4099e418f19782db8d2443672be2ab79a1c2973cdfa2fe60ddf4b14c` | V47 独立来源治理收据为 `CLEAN`；只证明来源治理和 readback 范围，不代表完整 V47 产品已进入公开仓库。 |
| E068 | `V47_R56L_D0_WINDOWS_AUTOMATION_RETURN_20261107/P3_STATUS.json` | `bc8029997a4852b16c20016260ca0b48f03bca1d729b80b7292253f44302f7d8` | P3 软件候选包含 Tag 124/125/126，并记录 hand/discard 区域；`REACHABILITY_UNKNOWN`，`physical_io=false`，没有 permit。 |
| E069 | `V47_R56L_D10_WINDOWS_RETURN_20261108/P3_STATE_MACHINE_RECEIPT.json` | `3bc21762bd16ae5ace4de34ed49d90959e9d60f8d57639085ec7fc1fdc51e51b` | 请求驱动软件状态机接受 `15` 次转移，最终状态版本为 `16`，覆盖 DRAW/IDENTIFY/PLAY/RESOLVE/DISCARD；无物理 I/O、运动许可或 Referee commit。 |

## 证据等级与复现边界

- E065–E069 是软件、静态、Headless 或来源治理证据；测试数和状态只属于对应历史收据，不代表本次归档重新运行。
- 本页不能证明 Ubuntu 原生启动、Unity PlayMode、真实视觉/音频、机械臂运动或物理 Referee 提交。
- 原始来源仍在私有审阅层；公开仓库只能核对本页文本、来源标识和 SHA-256。
