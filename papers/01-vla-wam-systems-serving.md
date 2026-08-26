# 01 · VLA/WAM 系统与 Serving

> VLA（Vision-Language-Action）与 WAM（World-Action Model / world model）的推理运行时、serving、调度、实时控制回路、端云协同部署。核心方向，正常收录门槛。

[← 研究地图](README.md) · [最新收录](LATEST.md)

## 其他（1）

| 论文 | 作者 | 发布 | Venue | 标签 | 代码 | TL;DR |
| --- | --- | --- | --- | --- | --- | --- |
| [ReWorld: An Interactive World Model with Long-Horizon Memory](https://arxiv.org/abs/2608.23565) | Zhifei Chen et al. | 2026-08-24 | arXiv | world-model, kv-cache, distillation, real-time-streaming, long-horizon-memory | - | ReWorld 提出控制与记忆分离的交互式世界模型：训练时用混合注意力窗口与随机 head 路由解耦短时控制与长时记忆，推理时以位姿索引地标库支撑固定预算 KV 缓存。配合 LoRA 分布匹配蒸馏将采样压缩至 4 步，同一骨干同时支持高保真多步模式与实时交互模式，分钟级 rollout 仍能回忆起始画面。 |
