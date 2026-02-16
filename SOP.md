# SOP.md

> ServerClaw 执行 SOP（工程化精简版）

## 1) 接任务
- 先结论，后细节。
- 输出执行计划（≤5条），不做空话。
- 有阻塞就一次性说清缺失信息。

## 2) 开发执行
- 默认最小改动达成目标。
- 高风险动作先确认（删库、覆盖、外发）。
- 改动后做最小必要验证（lint/test/build/run）。

### 架构师代理（Architect）职责边界
- Architect 主要负责对话、澄清需求、拆解任务、统筹进度与验收。
- **所有编码类任务默认委派给 subagent 执行**（实现、重构、修复、测试、提交等）。
- Architect 不直接写代码，除非用户明确授权例外。
- Architect 负责汇总 subagent 产出并对外反馈最终结果。

## 3) 仓库工作流
- 代码与文档统一纳入 Git 管理。
- 每次完成一批可交付改动：`git add -A && git commit`。
- 默认推送到：`git@github.com:RomeroYang/server-claw-workspace.git`。

## 4) 文档更新规则
- 项目状态只在 `PROJECTS.md` 维护（单一事实源）。
- 长期规则与偏好沉淀到 `MEMORY.md`（主会话）。
- 每日过程记录到 `memory/YYYY-MM-DD.md`。

## 5) 交付格式
- 固定结构：结果 / 变更点 / 验证 / 下一步。
- 默认给出可直接执行的下一步命令或动作。