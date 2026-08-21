# 收录与分类方法论

本文档定义本仓库的收录流程、字段规范与分类体系演化规则。

## 流水线

```
arXiv 每日抓取 → 去重 → LLM 打分（1-10）→ Slack 推送候选
→ 人工 ✅ 确认 → 归类收录进 data/papers.json → 重新生成所有 markdown 清单
```

- 打分规则维护在 agent 仓库的 `skills/paper-ranking/SKILL.md`；
- 只有人工确认过的论文才会被收录，LLM 只负责初筛与建议归类；
- 分类建议、标签、摘要由 LLM 生成，以人工确认为准。

## 论文记录字段（data/papers.json）

| 字段 | 说明 |
| --- | --- |
| `id` | 唯一键：arxiv_id（不含版本号）或 `dblp:<key>`（DBLP 回填的会议论文） |
| `title` / `authors` | 标题与作者列表 |
| `published` | arXiv 首次提交日期 |
| `year` | 发表年份（用于 venues/ 年份索引） |
| `venue` | 发表 venue（Semantic Scholar / DBLP 补充，预印本为 null） |
| `venue_type` | `system` / `architecture` / `robotics` / `preprint` |
| `source` | 收录来源：`arxiv-scout`（日常巡检）/ `dblp-backfill`（历史回填）/ `seed`（人工种子） |
| `directions` | 所属方向 id 列表（对应 taxonomy.json，可多选） |
| `subdirections` | 方向内的子类归属（方向 id → 子类 id，子类定义在 taxonomy.json 各方向的 `subdirections` 中） |
| `milestone_reason` | 里程碑理由（仅 milestone 方向 04 / 05 必填，说明为何属于里程碑级工作） |
| `tags` | 自由技术标签（如 `quantization`、`speculative-decoding`） |
| `code_url` | 官方代码仓库（仅官方实现，第三方复现不收录） |
| `github_stars` | 官方仓库 star 数快照（含抓取日期） |
| `citation_count` | 引用数快照（新论文为 0，仅作长期追踪） |
| `score` / `reason` | 收录时的评分与理由 |
| `summary_zh` | 中文 TL;DR |
| `added` | 收录日期 |

## 收录门槛分层

方向按 `tier` 分为两档（定义见 `data/taxonomy.json`）：

- **core**（01 / 02 / 03 / 06）：按正常评分阈值收录；
- **milestone**（04 / 05）：评分 **≥ 9** 且必须填写 `milestone_reason`，说明该工作如何定义或改写了技术路线；普通增量一律不收。

显式拒收模式（无论分数高低）：

- 仅优化 agent prompt / workflow、无底层技术贡献的论文；
- 无系统或效率贡献的纯算法增量（如常规刷点的策略学习改进）；
- 与 Physical AI Systems / Infra 仅弱相关的应用论文（如把 VLA 当工具用的下游应用）。

## 会议覆盖

- **日常巡检**：靠 arXiv 每日抓取。SOSP / OSDI / ISCA 等会议论文常不上 arXiv，覆盖不全属已知局限，靠下面两条路径弥补；
- **历史回填（dblp-backfill）**：经 DBLP 按会议拉取 2024 年至今的论文列表，按标题与摘要筛选后入库；
- **种子清单（seed）**：人工 curated 的里程碑工作直接入库。

三条路径通过 `source` 字段区分，统一经人工确认后进入 `data/papers.json`。

## 分类体系演化

- 分类定义在 `data/taxonomy.json`，含方向 id、名称、描述、关键词与门槛层级（tier）；
- 收录时若论文与现有方向均不契合，LLM 会提出**增设 / 合并 / 拆分**方向的建议，经人工确认后更新 taxonomy 并回溯重归类受影响论文；
- 一篇论文允许属于多个方向（多标签），前提是在每个方向下承担不同的技术角色；
- 方向的增删与含义变化记录在本文件的 changelog 中。

## 研究组收录

- 研究组数据维护在 `data/groups.json`，按学术实验室 / 工业研究 / 开源生态分类；
- 触发条件：同一团队的工作多次被收录，或单篇工作影响力突出；
- 档案包含：机构、PI / 核心成员、代表方向、代表性收录论文、官方仓库链接。
