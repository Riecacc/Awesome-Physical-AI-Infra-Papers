# 🧭 研究地图

> 251 篇论文 · 6 个研究方向 · 每篇论文可属于多个方向

[**📚 最新收录**](LATEST.md) · [**🏛️ 按会议 / 年份索引**](../venues/README.md) · [**🧩 JSON**](../data/papers.json) · [**🏷️ 分类定义**](../data/taxonomy.json)

## 按方向浏览

| # | 研究方向 | 门槛 | 论文数 |
| ---: | --- | --- | ---: |
| 01 | [**VLA/WAM 系统与 Serving**](01-vla-wam-systems-serving.md) | core | 0 |
| 02 | [**VLA/WAM 加速器与架构**](02-vla-wam-accelerators.md) | core | 15 |
| 03 | [**VLA/WAM 高效算法**](03-vla-wam-efficient-algorithms.md) | core | 1 |
| 04 | [**VLA/WAM 基座模型**](04-vla-wam-foundation-models.md) | milestone | 16 |
| 05 | [**通用高效 ML 方法**](05-general-efficient-ml.md) | milestone | 12 |
| 06 | [**通用 ML 系统与 Serving**](06-general-ml-systems.md) | core | 205 |

另提供 [按会议 / 年份索引](../venues/README.md)：系统（MLSys / SOSP / OSDI 等）、架构（ISCA / MICRO / HPCA / ASPLOS）、机器人（RSS / CoRL / ICRA / IROS）三个会议群，外加 arXiv / Others。

## 门槛分层

- **core**（01 / 02 / 03 / 06）：方向内论文按正常评分阈值收录；
- **milestone**（04 / 05）：仅收录定义或改写技术路线的里程碑级工作，评分 ≥ 9 且须给出里程碑理由，普通增量不收。

## 分类的演化

分类体系定义在 [`data/taxonomy.json`](../data/taxonomy.json)，不是一成不变的：

- 每篇论文收录时由 LLM 按当前分类体系归类（方向 + 子类 + 标签）；
- 若论文与任何现有方向都不契合，会提出增设 / 合并 / 拆分方向的建议，经人工确认后更新分类并重新归类受影响的论文；
- 一篇论文在技术角色确实不同的情况下，允许出现在多个方向下。
