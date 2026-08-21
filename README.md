# Awesome Physical AI Infra Papers

一份持续演化的 **Physical AI Systems / Infra** 研究图谱：VLA/WAM 的推理系统与 serving、加速器与计算架构、高效算法，以及与之相邻的 LLM / 多模态推理系统。

本仓库由自动化巡检 agent 维护：arXiv 每日抓取 → LLM 打分筛选 → Slack 人工 ✅ 确认 → 归类收录。分类体系会随领域发展持续审视与调整。

## 📊 概览

| 指标 | 当前值 |
| --- | --- |
| 收录论文 | 249 |
| 研究方向 | 6 |
| 追踪会议 | 15（系统 6 · 架构 4 · 机器人 4 · arXiv / Others） |
| 追踪研究组 | 14 |
| 最近更新 | 2026-08-21 |

## 🧭 研究地图

完整地图与分类说明见 [papers/README.md](papers/README.md)；另提供 [按会议 / 年份索引](venues/README.md)。

| # | 方向 | 门槛 | 论文数 |
| ---: | --- | --- | ---: |
| 01 | [VLA/WAM 系统与 Serving](papers/01-vla-wam-systems-serving.md) | core | 0 |
| 02 | [VLA/WAM 加速器与架构](papers/02-vla-wam-accelerators.md) | core | 15 |
| 03 | [VLA/WAM 高效算法](papers/03-vla-wam-efficient-algorithms.md) | core | 1 |
| 04 | [VLA/WAM 基座模型](papers/04-vla-wam-foundation-models.md) | milestone | 16 |
| 05 | [通用高效 ML 方法](papers/05-general-efficient-ml.md) | milestone | 12 |
| 06 | [通用 ML 系统与 Serving](papers/06-general-ml-systems.md) | core | 205 |

## 🆕 最新收录

见 [papers/LATEST.md](papers/LATEST.md)。

## 🏛️ 会议索引

按年份 × 追踪会议浏览收录论文，见 [venues/README.md](venues/README.md)。

## 🧑‍🔬 领先研究组

领域内有影响力的实验室、公司与开源生态，见 [groups/README.md](groups/README.md)。

## 🗂️ 仓库结构

| 位置 | 用途 |
| --- | --- |
| `papers/` | 按方向组织的论文清单 + 最新收录 |
| `venues/` | 年份 × 会议索引 |
| `groups/` | 领先研究组 / 公司 / 开源生态索引 |
| `data/papers.json` | 机器可读的论文数据库（**唯一数据源**） |
| `data/taxonomy.json` | 分类体系定义（可演化） |
| `data/groups.json` | 机器可读的研究组数据 |
| `docs/` | 收录与分类方法论 |

所有 markdown 清单均由 `data/` 下的 JSON 数据生成，请勿手工编辑表格内容。

## 🔎 收录原则

- 质量优先，不设数量指标；
- 收录门槛分层：core 方向正常评分阈值，milestone 方向（04 / 05）仅收里程碑级工作；
- 每篇论文须有明确的技术定位（方向 + 子类 + 标签）；
- 代码链接仅收录官方实现；
- 分类体系随收录持续审视：不合身的归类会被修正，新方向会被增设。

详细规则见 [docs/METHODOLOGY.md](docs/METHODOLOGY.md)。
