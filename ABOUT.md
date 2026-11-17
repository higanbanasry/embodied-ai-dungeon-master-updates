# 项目介绍 / About the Project

[中文](#中文) · [English](#english)

## 中文

《遗迹核心：三方夺芯》（Relic Core: Triad Heist）是一个具身智能桌游项目：三名玩家围绕棋盘中央的核心竞争，其中一个席位可以由 Agent 控制。项目同时研究可确定复现的规则裁判、受隐藏信息约束的决策、桌面观察、数字界面，以及在安全门控下的实体卡牌/棋子操作。目标不是让机器人凭一帧图像自行“猜”结果，而是让每一步观察、合法行动、规则状态与物理反馈有明确的责任边界。

| 层 | 职责 | 当前公开边界 |
|---|---|---|
| 规则与 Referee | 保存唯一权威棋盘状态、检查合法行动和阶段转换 | 早期 Arena 软件基线曾离线验证；这里未发布完整产品源码 |
| Agent | 只读取允许公开的玩家视图，提出行动候选 | 不能读取对手隐藏牌，也不能直接改写裁判状态 |
| Perception | 从相机/标签等输入形成带来源的观察候选 | 识别框不自动等于卡牌身份、毫米坐标或抓取成功 |
| Unity | 显示同版软件事件、界面和阶段反馈 | PlayMode 软件结果不等于物理执行 |
| Robot / Ubuntu | 在受控现场范围内操作，并返回动作及停止反馈 | 单张 DRAW 有用户现场确认；完整动作后机器回执仍待核 |

公开信息按证据等级阅读：`SYNTHETIC_OFFLINE` 是合成/离线，`STATIC` 是静态来源或合同，`NOT_RUN_BLOCKED` 是未运行且有阻塞，`UNKNOWN` 是尚不能判断。真实动作需要目标设备、task/epoch、标定、布局和停止反馈等同一任务绑定；用户现场确认会如实标明，但不冒充独立机器验收。

本仓库是**精选展示**，不是完整代码库。它从 W13–W15 起步，提供中英双语导航、游戏规则草案、当前进展和脱敏周报/证据摘要。私有工程仓库保留正式归档、主证据索引、可复现软件切片与未公开的原件；私有媒体、设备日志、现场配置、凭据和完整交付包不会因本展示而公开。项目会持续推进，后续进展也将按发布规则更新。

建议阅读：[桌游规则](GAME_RULES.md) → [进展与后续](ROADMAP.md) → [W13–W15 周报](README.md#当前可见的三个周次) → [发布规则](PUBLISHING_POLICY.md)。

## English

*Relic Core: Triad Heist* is an embodied-AI tabletop project. Three players compete for a central relic core; one seat may be controlled by an agent. The project connects deterministic game adjudication, decisions constrained by hidden information, tabletop observation, a digital interface, and safety-gated physical card/piece handling. Its objective is not to infer an entire game from one image: each observation, legal action, authoritative state transition, and physical feedback has a defined owner.

| Layer | Responsibility | Public evidence boundary |
|---|---|---|
| Rules and Referee | Own the authoritative board state, validate actions, advance phases | An earlier Arena software baseline was tested offline; the complete current product source is not published here |
| Agent | Propose actions from an allowed public player view | Cannot inspect opponents' hidden cards or directly edit Referee state |
| Perception | Produce provenance-bound observation candidates from cameras/tags | A detection box alone is not card identity, millimetre pose, or a successful pick |
| Unity | Display same-version software events and phase feedback | PlayMode software evidence is not physical execution evidence |
| Robot / Ubuntu | Act within a bounded on-site scope and return action/stop feedback | A single DRAW is user-confirmed; its full independent post-action machine receipt remains pending |

Read evidence by scope: `SYNTHETIC_OFFLINE` means synthetic/offline, `STATIC` means static source or contract, `NOT_RUN_BLOCKED` means not run because a prerequisite is missing, and `UNKNOWN` means unresolved. A live machine claim needs same-task target-device response, task/epoch, calibration, layout, and stop-feedback binding. A user's on-site confirmation is recorded honestly but is not relabelled as independent machine acceptance.

This is a **selected public showcase**, not the full code repository. It begins with W13–W15 and provides bilingual navigation, a game-rule draft, current progress, and redacted weekly reports/evidence summaries. The private engineering archive retains the formal history, primary evidence index, reproducible software slices, and unpublished originals. Private media, device logs, site configuration, credentials, and complete delivery packages are not exposed here. The project continues beyond any single presentation or application cycle.

Suggested reading: [Game rules](GAME_RULES.md) → [Progress and next steps](ROADMAP.md) → [W13–W15 reports](README.md#english) → [Publishing policy](PUBLISHING_POLICY.md).
