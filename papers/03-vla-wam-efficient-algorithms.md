# 03 · VLA/WAM 高效算法

> fast WAM、VLA token 剪枝、量化 / 蒸馏、高效 action head（flow / diffusion 加速）等以效率为目标的算法。核心方向，正常收录门槛。

[← 研究地图](README.md) · [最新收录](LATEST.md)

## 高效动作头（1）

| 论文 | 作者 | 发布 | Venue | 标签 | 代码 | TL;DR |
| --- | --- | --- | --- | --- | --- | --- |
| [FAST: Efficient Action Tokenization for Vision-Language-Action Models](https://arxiv.org/abs/2501.09747) | Karl Pertsch et al. | 2025-01-16 | arXiv | action-tokenization, efficient-vla | - | FAST：高效动作 tokenization，显著加速 VLA 训练与推理。 |

## 其他（5）

| 论文 | 作者 | 发布 | Venue | 标签 | 代码 | TL;DR |
| --- | --- | --- | --- | --- | --- | --- |
| [MINERVA: How Small Can a Manipulation Policy Be and Still Solve LIBERO?](https://arxiv.org/abs/2609.03715) | Kohei Sendai et al. | 2026-09-03 | arXiv | efficient-vla, model-scaling, edge-inference, libero | - | MINERVA 系统测量 LIBERO 基准的任务容量下限：0.54M 参数策略即达 95.1% 成功率，且发现 flow matching 相对 L1 回归无优势而慢 3.8 倍。研究还揭示 LIBERO 指令条件主要是任务记忆选择，为容量感知设计与蒸馏提供了实证基础。 |
| [Knowing When to Stop: Adaptive Action Chunking via Internal Cross-Attention Dynamics in VLAs](https://arxiv.org/abs/2609.00908) | Runze Xu et al. | 2026-09-01 | arXiv | vla, action-chunking, adaptive-inference, training-free | - | 论文发现随预测时域延伸，动作到观测的交叉注意力趋于分散、熵上升至平台期，与预测误差升高相关。据此提出免训练截断机制，检测高熵平台期并动态选择执行时域，在 pi0.5 和 X-VLA 上超越固定时域与自适应基线。 |
| [FlashVLA: Streaming Action Decoding for Fast and Asynchronous VLA Inference](https://arxiv.org/abs/2608.27384) | Zekai Li et al. | 2026-08-27 | arXiv | vla-inference, async-execution, action-chunking, real-time-control | - | FlashVLA 提出流式动作缓冲与分块因果注意力，每次推理产出一个可执行动作块，并隐式保持动作连续性。在仿真与真机实验中实现单 GPU ≥30Hz 的平滑异步控制频率。 |
| [NVIDIA Cosmos-H-Dreams: Real-Time Generative Physics Simulation for Surgical Robotics](https://arxiv.org/abs/2608.24199) | Javier Gamazo Tejero et al. | 2026-08-25 | arXiv | world-model, distillation, real-time-simulation, surgical-robotics, streaming-inference | - | Cosmos-H-Dreams 将动作条件手术视频世界模型经教师-学生蒸馏转化为可控实时模拟器，在单张 RTX PRO 6000 上达 ~160 FPS，支持键盘、VR、手术机器人控制台与闭环策略的实时交互控制。 |
| [ReWorld: An Interactive World Model with Long-Horizon Memory](https://arxiv.org/abs/2608.23565) | Zhifei Chen et al. | 2026-08-24 | arXiv | world-model, kv-cache, distillation, real-time-streaming, long-horizon-memory | - | ReWorld 提出控制与记忆分离的交互式世界模型：训练时用混合注意力窗口与随机 head 路由解耦短时控制与长时记忆，推理时以位姿索引地标库支撑固定预算 KV 缓存。配合 LoRA 分布匹配蒸馏将采样压缩至 4 步，同一骨干同时支持高保真多步模式与实时交互模式，分钟级 rollout 仍能回忆起始画面。 |
