# 双仓发布规则 / Dual-repository Publishing Policy

[中文](#中文) · [English](#english)

## 中文

本规则自 2026-11-17 起用于周度归档。原工程仓库是**私有事实源和完整归档**；本仓库是**独立公开展示层**。本仓库从 W13–W15 三周起步，不继承私有仓库的提交历史。

## 每次进展更新的顺序

1. 在私有工程仓库核对来源、周次、证据状态与重复项；写入正式周报、脱敏证据摘要和主证据索引。进行中的周次要明确标为“进行中”，不能提前签成周末验收。
2. 审核公开范围：排除本机绝对路径、私人资料、凭据、真人原始媒体、设备日志、现场配置、大型交付包和未审阅源码。用户现场确认、静态合同、合成测试与动作后机器回执分别表述，不互相替代。
3. 将通过审核的中文周报和证据摘要复制到本仓库，逐文件核对 SHA-256；另写与其事实和限制一致的英文伴随页。项目介绍、规则草案和后续计划也保持中英一致；更新首页、发布清单与必要的状态边界，确认公开提交只含预定文件。
4. 分别提交并核对两个远端的实际提交号与页面。未核实远端前只记“本地已准备”，不能声称两个仓库都已同步。私有仓库的证据索引继续以其自身提交号为准；本仓库不复制完整私有索引或私有 Git 历史。
5. 对外只链接本仓库；私有工程仓库保持 private。本流程由归档主责在用户要求更新时执行，既有只读检查任务不获得 Git 写入权限，也不自动启动跨任务派发或定时上传。

## 当前三周与以后更新

首次公开内容只有 W13、W14 和进行中的 W15。后续每次获准发布都要同步私有完整归档与本仓库的脱敏展示，但**Git 提交历史会累计**：普通删除旧周次文件不能让历史不可见。因此本仓库不承诺永久滚动隐藏到“仅最近三周”。若以后仍须严格只对外展示滚动三周，需要在下一次发布前另行确定新的、无旧历史的公开载体；不得靠强推、改写历史或删除旧提交假装已撤回传播过的内容。

## 证据与复现边界

- 周报日期是发生或归档日期，不把后来取得的结果回填成当时已通过。
- `LIVE` 机器结果需要同一目标设备/主机响应及 task、epoch、标定、布局和停止反馈绑定；用户现场确认可如实记录，但独立机器证据缺失时仍标明缺口。
- 本仓库是进展展示，不是完整产品的安装包、运动许可或实体 Referee 验收。

## English

Since 2026-11-17, the original engineering repository has been the **private source of record and complete archive**; this separate repository is a **selected public display**. It launched with W13, W14, and an explicitly in-progress W15, without importing private Git history.

For each user-requested update:

1. Verify week, sources, evidence level, and duplicate work in the private engineering archive. Mark an ongoing week as **in progress**, never as prematurely accepted.
2. Review publication scope. Exclude local absolute paths, personal information, credentials, real-person raw media, device logs, site configuration, full product deliveries, and unreviewed source. Keep user confirmation, static contracts, synthetic tests, and post-action machine receipts distinct.
3. Copy reviewed Chinese reports/evidence summaries byte-for-byte and verify SHA-256. Write English companion pages with the same facts, numbers, dates, and limitations; keep the bilingual project introduction, rule-draft summary, and next steps aligned. Inspect the exact set of staged public files.
4. Commit and read back each remote's actual SHA and pages. Until both are verified, report **partial sync**, not dual-repository completion. The private primary evidence index continues to use private commit identities; this public repository does not copy its full index or history.
5. Only the designated archive owner performs publication when the user asks. The existing read-only checker gains no Git write rights; no automatic cross-task dispatch or scheduled upload is created.

The initial contents cover three weeks, but ordinary Git history accumulates. Deleting an older week's current files **does not erase old public commits**; this repository cannot promise a permanently rolling three-week-only window. If that strict requirement returns, choose a new history-free public vehicle before the next release rather than rewriting history or pretending previously published content is withdrawn.

`LIVE` machine evidence needs same-task target-device response plus task/epoch, calibration, layout, and stop-feedback binding. The W15 single-card DRAW is user-confirmed real on-site progress, while independent post-action machine evidence remains pending. This repository is a progress display, not a complete product installer, motion authorization, or physical Referee acceptance.
