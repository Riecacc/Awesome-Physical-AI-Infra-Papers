# 01 · VLA/WAM 系统与 Serving

> VLA（Vision-Language-Action）与 WAM（World-Action Model / world model）的推理运行时、serving、调度、实时控制回路、端云协同部署。核心方向，正常收录门槛。

[← 研究地图](README.md) · [最新收录](LATEST.md)

## 其他（5）

| 论文 | 作者 | 发布 | Venue | 标签 | 代码 | TL;DR |
| --- | --- | --- | --- | --- | --- | --- |
| [FluxVLA Engine: A One-Stop VLA Engineering Platform for Embodied Intelligence](https://arxiv.org/abs/2609.17210) | Yinhao Li et al. | 2026-09-15 | arXiv | vla-serving, deployment-platform, real-time-chunking, open-source | [code](https://github.com/FluxVLA/FluxVLA) | FluxVLA Engine 是一个开放的、配置驱动的 VLA 工程平台，标准化数据集、模型、动作头、分布式训练、仿真评估与机器人执行的接口。集成实时分块、加速推理后端与轻量远程 GPU serving，打通离线学习、仿真验证、在线纠错与真机执行的完整链路。 |
| [FlashVLA: Streaming Action Decoding for Fast and Asynchronous VLA Inference](https://arxiv.org/abs/2608.27384) | Zekai Li et al. | 2026-08-27 | arXiv | vla-inference, async-execution, action-chunking, real-time-control | - | FlashVLA 提出流式动作缓冲与分块因果注意力，每次推理产出一个可执行动作块，并隐式保持动作连续性。在仿真与真机实验中实现单 GPU ≥30Hz 的平滑异步控制频率。 |
| [NVIDIA Cosmos-H-Dreams: Real-Time Generative Physics Simulation for Surgical Robotics](https://arxiv.org/abs/2608.24199) | Javier Gamazo Tejero et al. | 2026-08-25 | arXiv | world-model, distillation, real-time-simulation, surgical-robotics, streaming-inference | - | Cosmos-H-Dreams 将动作条件手术视频世界模型经教师-学生蒸馏转化为可控实时模拟器，在单张 RTX PRO 6000 上达 ~160 FPS，支持键盘、VR、手术机器人控制台与闭环策略的实时交互控制。 |
| [PonderPounce: A Pretrained MLLM as an Episode Context Engine for Robot Control](https://arxiv.org/abs/2608.24115) | Suhwan Choi et al. | 2026-08-25 | arXiv | vla-serving, async-inference, episodic-memory, dual-system, low-latency | - | PonderPounce 复用 MLLM 原生因果上下文作为机器人情景记忆，System2 异步生成认知 token 供 System1 VLA 消费，优化后支持 20Hz 动作回放，在 RoboMME 上大幅超越基线。 |
| [ReWorld: An Interactive World Model with Long-Horizon Memory](https://arxiv.org/abs/2608.23565) | Zhifei Chen et al. | 2026-08-24 | arXiv | world-model, kv-cache, distillation, real-time-streaming, long-horizon-memory | - | ReWorld 提出控制与记忆分离的交互式世界模型：训练时用混合注意力窗口与随机 head 路由解耦短时控制与长时记忆，推理时以位姿索引地标库支撑固定预算 KV 缓存。配合 LoRA 分布匹配蒸馏将采样压缩至 4 步，同一骨干同时支持高保真多步模式与实时交互模式，分钟级 rollout 仍能回忆起始画面。 |
