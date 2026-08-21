# 02 · VLA/WAM 加速器与架构

> 面向机器人 / 多模态 / VLA 的芯片与架构设计、存算一体、稀疏架构；主要来自 ISCA / MICRO / HPCA / ASPLOS。核心方向，正常收录门槛。

[← 研究地图](README.md) · [最新收录](LATEST.md)

## 机器人计算（动力学 / 控制 / 规划）（3）

| 论文 | 作者 | 发布 | Venue | 标签 | 代码 | TL;DR |
| --- | --- | --- | --- | --- | --- | --- |
| [DRACO: A Hardware-Efficient Robot Rigid Body Dynamics Accelerator with Precision-Aware Quantization Framework](https://dblp.org/rec/conf/hpca/LiuLZDMYXZ26.html) | Xingyu Liu et al. | 2026 | HPCA | robot-dynamics, rigid-body, quantization | - | 精度感知量化框架的硬件高效机器人刚体动力学加速器。 |
| [Dadu-Corki: Algorithm-Architecture Co-Design for Embodied AI-powered Robotic Manipulation](https://dblp.org/rec/conf/isca/HuangH0Y0M00L0G25.html) | Yiyang Huang 0002 et al. | 2025 | ISCA | embodied-ai, manipulation, algorithm-architecture-codesign | - | 面向具身 AI 机器人操作的算法-架构协同设计加速器。 |
| [HiPER: Hierarchically-Composed Processing for Efficient Robot Learning-Based Control](https://dblp.org/rec/conf/isca/Ting0ZSZ25.html) | Justin Ting et al. | 2025 | ISCA | robot-control, robot-learning, accelerator | - | 分层组合处理架构加速基于机器人学习的控制。 |

## 感知与 SLAM 加速（8）

| 论文 | 作者 | 发布 | Venue | 标签 | 代码 | TL;DR |
| --- | --- | --- | --- | --- | --- | --- |
| [SPLATONIC: Architectural Support for 3D Gaussian Splatting SLAM via Sparse Processing](https://dblp.org/rec/conf/hpca/HuangZMXLHGLLFG26.html) | Xiaotong Huang et al. | 2026 | HPCA | 3dgs, slam, sparse-processing | - | 面向 3D 高斯泼溅 SLAM 的稀疏处理架构支持。 |
| [RTGS: Real-Time 3D Gaussian Splatting SLAM via Multi-Level Redundancy Reduction](https://dblp.org/rec/conf/micro/LiQ0WQHZZC0Z25.html) | Leshu Li et al. | 2025 | MICRO | 3dgs, slam, real-time | - | 多级冗余削减实现实时 3D 高斯泼溅 SLAM。 |
| [GCC: A 3DGS Inference Architecture with Gaussian-Wise and Cross-Stage Conditional Processing](https://dblp.org/rec/conf/micro/Pei0SZMWSL025.html) | Minnan Pei et al. | 2025 | MICRO | 3dgs, inference-architecture | - | 高斯级与跨阶段条件处理的 3DGS 推理架构。 |
| [REACT3D: Real-time Edge Accelerator for Incremental Training in 3D Gaussian Splatting based SLAM Systems](https://dblp.org/rec/conf/micro/WangZZXWYY0025.html) | Hongyi Wang et al. | 2025 | MICRO | 3dgs, slam, edge-accelerator | - | 面向 3DGS SLAM 系统增量训练的实时边缘加速器。 |
| [SuperNoVA: Algorithm-Hardware Co-Design for Resource-Aware SLAM](https://dblp.org/rec/conf/asplos/KimHNDS25.html) | Seah Kim et al. | 2025 | ASPLOS | slam, algorithm-hardware-codesign | - | 资源感知 SLAM 的算法-硬件协同设计。 |
| [HgPCN: A Heterogeneous Architecture for E2E Embedded Point Cloud Inference](https://dblp.org/rec/conf/micro/GaoJPCPL24.html) | Yiming Gao et al. | 2024 | MICRO | point-cloud, embedded, heterogeneous | - | 面向嵌入式端到端点云推理的异构架构。 |
| [GauSPU: 3D Gaussian Splatting Processor for Real-Time SLAM Systems](https://dblp.org/rec/conf/micro/WuZHZCZ24.html) | Lizhou Wu et al. | 2024 | MICRO | 3dgs, slam, processor | - | 面向实时 SLAM 系统的 3D 高斯泼溅处理器。 |
| [SPADE: Sparse Pillar-based 3D Object Detection Accelerator for Autonomous Driving](https://dblp.org/rec/conf/hpca/LeePKYLCKKC24.html) | Minjae Lee et al. | 2024 | HPCA | 3d-detection, autonomous-driving, accelerator | - | 面向自动驾驶的稀疏柱体 3D 目标检测加速器。 |

## 具身系统与可靠性（3）

| 论文 | 作者 | 发布 | Venue | 标签 | 代码 | TL;DR |
| --- | --- | --- | --- | --- | --- | --- |
| [CREATE: Cross-Layer Resilience Characterization and Optimization for Efficient yet Reliable Embodied AI Systems](https://dblp.org/rec/conf/asplos/XieQWWDWCLJWWL26.html) | Tong Xie et al. | 2026 | ASPLOS | embodied-ai, resilience, reliability | - | 面向高效可靠具身 AI 系统的跨层韧性刻画与优化。 |
| [ReCA: Integrated Acceleration for Real-Time and Efficient Cooperative Embodied Autonomous Agents](https://dblp.org/rec/conf/asplos/WanDIQJZKRR25.html) | Zishen Wan et al. | 2025 | ASPLOS | embodied-agents, real-time, cooperative | - | 面向实时高效协作具身自主智能体的一体化加速架构。 |
| [AnA: An Attentive Autonomous Driving System](https://dblp.org/rec/conf/asplos/ChoeWL25.html) | Wonkyo Choe et al. | 2025 | ASPLOS | autonomous-driving, attention, system | - | 注意力驱动的自动驾驶系统。 |

## 多模态 / 视频加速器（1）

| 论文 | 作者 | 发布 | Venue | 标签 | 代码 | TL;DR |
| --- | --- | --- | --- | --- | --- | --- |
| [V-Rex: Real-Time Streaming Video LLM Acceleration via Dynamic KV Cache Retrieval](https://dblp.org/rec/conf/hpca/KimYSK26.html) | Donghyuk Kim et al. | 2026 | HPCA | video-llm, streaming, kv-cache-retrieval | - | 动态 KV cache 检索实现实时流式视频 LLM 加速。 |
