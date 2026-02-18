# PROJECTS.md

> 工作区项目清单（执行版）

## A. 工作内容（genov）

### fomox-evm
- **路径：** `/home/ubuntu/github/genov/fomox-evm`
- **类型：** Monorepo（EVM 合约 + 前后端）
- **状态：** 已上线 BSC 测试网 / 主网，持续迭代新功能
- **优先级：** 高
- **部署（后端）：** AWS EC2 + Docker Compose + Nginx 反代蓝绿双实例
- **生产 EC2 公网 IP：** `54.179.70.89`
- **测试 EC2 公网 IP：** `13.212.215.250`
- **环境变量：**
  - Staging: `/home/ubuntu/fomox-evm-api/.env.staging`
  - Production: `/home/ubuntu/fomox-evm-api/.env.prod`
- **项目文档：** 仓库 `docs/` 目录
- **下一步（默认）：**
  1. 按需求拆分迭代任务并评估影响面
  2. 变更后执行最小必要验证（合约/前端/后端）
  3. 更新发布与回归记录

## B. 独立开发（reapp）

### reapp.top
- **路径：** `/home/ubuntu/github/reapp/reapp.top`
- **类型：** 纯前端网页应用（Next.js）
- **状态：** 开发中，目标先上线“仅图片压缩工具”MVP
- **优先级：** 高
- **当前已完成：** UI 优化、图片压缩能力（Squoosh 引擎优化）、SEO 基础方案（`docs/SEO_GUIDE.md`）
- **当前阶段目标（MVP 上线前）：**
  1. Landing 保留压缩工具可用，其他工具入口显示 `Coming Soon`
  2. 全站品牌从 OneImage 彻底 Rebrand 为 `ReImage`
  3. 导航移除 Blogs，补齐 About / Contact / Privacy / Terms 页面
  4. 压缩工具页补齐营销文案（工具区之外），基于 oneimage 对标并优化
  5. 规划并接入 9 语言 i18n 框架（首版可先保留英文文案）
- **下一步（执行中）：** 输出分阶段实施计划并按子代理并行推进

### mini-tarot
- **路径：** `/home/ubuntu/github/reapp/mini-tarot`
- **类型：** 纯前端网页应用
- **状态：** 开发中，未上线
- **优先级：** 中

## C. 合作项目（defintech）

### fakt
- **路径：** `/home/ubuntu/github/defintech/fakt`
- **类型：** 与朋友合作项目
- **状态：** 规划中（目录已建，暂无代码）
- **优先级：** 低

## 维护约定
- 当前活跃仓库变化时，第一时间更新本文件。
- 每个项目保留“路径 / 状态 / 优先级 / 关键部署信息 / 下一步”。
- 不写冗长背景，保持可执行。