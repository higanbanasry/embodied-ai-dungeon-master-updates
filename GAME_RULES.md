# 《遗迹核心：三方夺芯》规则 / Relic Core: Triad Heist Rules

[中文](#中文) · [English](#english)

## 中文

**版本与性质：**下述为 Arena v0.3 的**设计草案摘要**，原设计状态是 `draft-for-paper-playtest`。它解释项目的桌游场景，不宣称全部规则已经写入当前 R12 实体产品，也不宣称已经完成纸面试玩或平衡验收。具体实现若与草案不同，须以同版工程合同和测试为准。

### 目标与摆放

三名玩家在 5×5 正交方格竞技场争夺唯一遗迹核心。核心从 `C3` 开始；P1/P2/P3 的出生点及撤离门分别是 `A3`、`E3`、`C1`。玩家只沿上下左右移动，每格最多一名玩家。游戏最多五轮，设计目标时长 10–15 分钟。机器人担任中立裁判；在人类×2、机器人×1 的演示模式中，也控制 P3。

### 每轮如何进行

1. **环境：**公开一张环境牌，本轮条件在编程前可见。
2. **暗中编程：**每名玩家从六种行动牌中选两张，按顺序放入 `SLOT_1` 和 `SLOT_2`。行动种类在翻牌前隐藏，箭头方向公开。机器人玩家只能读公开信息，不能偷看人类隐藏牌。
3. **同时翻牌与结算：**六张行动牌翻开。通常先结算所有人的第一槽，再结算第二槽；同槽按优先级处理。设计中的“镜像协议”环境牌会交换两槽顺序。每次物理动作后须确认状态；确认失败时停止后续动作，不用预测结果硬接下一步。
4. **轮末：**计分、更新行动牌冷却、轮换先手、检查胜负。用过的两张牌跳过下一轮后才重新可用。

| 行动 | 优先级 | 草案效果 |
|---|---:|---|
| 屏障 / Shield | 6 | 抵挡一次针对自己的震荡、牵引或相邻夺芯 |
| 震荡 / Shock | 5 | 打掉相邻持有者的核心，并尝试推动对方一格 |
| 牵引 / Pull | 4 | 将直线两格内的首个合法目标向自己拉近一格 |
| 步进 / Step | 3 | 沿箭头移动一格 |
| 夺芯 / Seize | 2 | 拿起同格松散核心，或夺取相邻未受屏障保护的持有者核心 |
| 突进 / Dash | 1 | 沿箭头最多两格；携带核心时最多一格 |

同优先级的移动采用同时碰撞规则：争抢同一目标格时相关移动失败；不可穿过已占据格或通过同批交换位置绕过碰撞。卡牌效果、环境牌和冲突细节仍以 v0.3 草案原文为准，公开摘要不代替完整测试用例。

### 核心、得分与胜负

核心可以是松散位于方格、由玩家携带，或在撤离后的当轮等待重生。携带核心进入自己的撤离门得 2 分；未撤离但轮末仍持有核心得 1 分。达到 4 分不立刻中断已锁定的行动，须完成整轮后检查；单独最高且至少 4 分者获胜，否则最多进行五轮。第 5 轮后先比总分，再按草案中的撤离次数、持有状态与适用时的曼哈顿距离等条件决出平局；仍相同可并列。

设计还包含八张公开环境牌，可改变冷却、位移、突进距离、夺芯范围、屏障次数、核心漂移、槽位顺序或轮末携带计分。这些是**规则设计项**，不应据此推断每种效果已有当前实体机器测试。

## English

**Version and status:** This is a readable summary of the Arena v0.3 **design draft**, whose source status is `draft-for-paper-playtest`. It explains the game's intended rules; it does not claim that every rule has been implemented in the current R12 physical product or that paper playtesting and balance acceptance are complete. Same-version engineering contracts and tests take precedence over this design summary when implementation differs.

### Objective and setup

Three players compete for one relic core on a 5×5 orthogonal grid. The core starts at `C3`; P1/P2/P3 start and evacuate at `A3`, `E3`, and `C1`, respectively. Movement is orthogonal, and at most one player occupies a cell. The game lasts at most five rounds, with a design target of 10–15 minutes. The robot is a neutral Referee and can also control P3 in a two-human/one-robot demonstration.

### A round in brief

1. **Environment:** Reveal one public environment card before players program their actions.
2. **Hidden programming:** Each player selects two of six action cards for `SLOT_1` and `SLOT_2`. Action types remain hidden until reveal; arrow directions are public. The robot player can use only public information, never the humans' hidden card identities.
3. **Reveal and resolution:** Reveal all six cards. Normally resolve everyone's first slot, then the second, with action priority within a slot. The draft's “Mirror Protocol” environment swaps slot order. After each physical action the resulting state must be observed; if verification fails, subsequent actions pause rather than relying on prediction.
4. **Round end:** Score, update card cooldowns, rotate initiative, and check for a winner. Used cards skip the next round before becoming available again.

| Action | Priority | Draft effect |
|---|---:|---|
| Shield | 6 | Blocks one Shock, Pull, or adjacent Seize aimed at its owner |
| Shock | 5 | Drops a neighbouring carrier's core and attempts to push them one cell |
| Pull | 4 | Draws the first legal target within two straight-line cells one cell closer |
| Step | 3 | Moves one cell in the arrow direction |
| Seize | 2 | Picks up a loose core on the same cell, or takes it from an adjacent unshielded carrier |
| Dash | 1 | Moves up to two cells in the arrow direction; at most one while carrying |

Equal-priority moves use simultaneous collision rules: competing for the same destination makes the affected moves fail; players cannot pass through occupied cells or bypass collisions by swapping cells in one batch. The source v0.3 draft governs detailed effects, events, and edge cases; this public summary is not a substitute for the full test suite.

### Core, scoring, and victory

The core may be loose on a cell, carried by a player, or awaiting respawn after evacuation. Carrying it into one's own evacuation gate scores 2 points; holding it at round end without evacuating scores 1. Reaching 4 points does not interrupt already locked actions: the full round ends before victory is checked. A sole leader with at least 4 points wins; otherwise play continues for at most five rounds. After round five, ties are resolved using the draft's evacuation count, possession status, and—when applicable—Manhattan distance to a loose core; a complete tie may remain shared.

The draft also defines eight public environment cards affecting cooldowns, movement, dash range, seize range, shield capacity, core drift, slot order, or end-of-round carrier scoring. These are **design rules**, not evidence that every effect has been tested on the current physical machine.
