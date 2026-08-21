# 04 · VLA/WAM 基座模型

> π 系列、GR00T 系列、OpenVLA、RT 系列、Cosmos-Policy 等定义或改写技术路线的模型。**仅收录里程碑级工作，普通增量不收**。

[← 研究地图](README.md) · [最新收录](LATEST.md)

| 论文 | 作者 | 发布 | Venue | 标签 | 代码 | TL;DR |
| --- | --- | --- | --- | --- | --- | --- |
| [GigaBrain-WBC-0.5: A Behavior World Model for Robust Whole-Body Control with Environment Interaction](https://arxiv.org/abs/2608.18234) | Ziyang Cheng et al. | 2026-08-18 | arXiv | world-model, whole-body-control, humanoid | - | 提出 GigaBrain-WBC-0.5，首个用于人形机器人全身控制的行为世界模型，通过因果 Transformer 联合预测动作、状态和行为命令分布，并自动标注 3D 地形接触几何。地形交互成功率 81.3%（4.3 倍于基线），跌倒恢复 99.3%，真机验证可跨本体迁移。 |
| [Hydra-0: Action Flow for Generalist World Modeling and Control](https://arxiv.org/abs/2608.18077) | Hongyu Li et al. | 2026-08-18 | arXiv | world-model, action-flow, nvidia | - | 提出 Hydra-0，以动作流（将机器人动作表示为像素运动）为条件的通用世界模型，实现跨本体、任务、环境的通用建模与控制，机器人运动误差降低 90.4%。还涌现逆向模式：从人类演示的物体流预测兼容的机器人动作，无需任务专家演示。 |
| [From Foundation to Application: Improving VLA Models in Practice](https://arxiv.org/abs/2607.06403) | Wei Wu et al. | 2026-07-07 | arXiv | vla, sparse-moe, cross-embodiment | [code](https://github.com/robbyant/lingbot-vla-v2) | LingBot-VLA 2.0：稀疏 MoE 架构、6 万小时数据的跨本体 VLA。 |
| [World Action Models are Zero-shot Policies](https://arxiv.org/abs/2602.15922) | Seonghyeon Ye et al. | 2026-02-17 | arXiv | world-action-model, zero-shot, nvidia | - | DreamZero：14B 世界动作模型，联合预测视频与动作实现零样本策略。 |
| [A Pragmatic VLA Foundation Model](https://arxiv.org/abs/2601.18692) | Wei Wu et al. | 2026-01-26 | arXiv | vla, real-world-data, dual-arm | [code](https://github.com/Robbyant/lingbot-vla) | LingBot-VLA：2 万小时真机预训练的务实 VLA 基础模型。 |
| [Cosmos Policy: Fine-Tuning Video Models for Visuomotor Control and Planning](https://arxiv.org/abs/2601.16163) | Moo Jin Kim et al. | 2026-01-22 | arXiv | cosmos, video-model, visuomotor | - | Cosmos Policy：将视频模型微调为视觉运动控制与规划策略。 |
| [$π_{0.5}$: a Vision-Language-Action Model with Open-World Generalization](https://arxiv.org/abs/2504.16054) | Physical Intelligence et al. | 2025-04-22 | arXiv | vla, generalization | - | π0.5：具备开放世界泛化能力的 VLA 模型。 |
| [GR00T N1: An Open Foundation Model for Generalist Humanoid Robots](https://arxiv.org/abs/2503.14734) | NVIDIA et al. | 2025-03-18 | arXiv | humanoid, foundation-model, nvidia | - | GR00T N1：NVIDIA 开源通用人形机器人基础模型。 |
| [FAST: Efficient Action Tokenization for Vision-Language-Action Models](https://arxiv.org/abs/2501.09747) | Karl Pertsch et al. | 2025-01-16 | arXiv | action-tokenization, efficient-vla | - | FAST：高效动作 tokenization，显著加速 VLA 训练与推理。 |
| [Cosmos World Foundation Model Platform for Physical AI](https://arxiv.org/abs/2501.03575) | NVIDIA et al. | 2025-01-07 | arXiv | world-model, synthetic-data, nvidia | [code](https://github.com/nvidia-cosmos/cosmos-predict1) | Cosmos：面向 Physical AI 的世界基础模型平台。 |
| [$π_0$: A Vision-Language-Action Flow Model for General Robot Control](https://arxiv.org/abs/2410.24164) | Kevin Black et al. | 2024-10-31 | arXiv | vla, flow-matching, generalist-policy | - | π0：基于 flow matching 的通用机器人控制 VLA 模型。 |
| [OpenVLA: An Open-Source Vision-Language-Action Model](https://arxiv.org/abs/2406.09246) | Moo Jin Kim et al. | 2024-06-13 | arXiv | open-source, vla | - | OpenVLA：开源 VLA 模型代表作。 |
| [Octo: An Open-Source Generalist Robot Policy](https://arxiv.org/abs/2405.12213) | Octo Model Team et al. | 2024-05-20 | arXiv | open-source, generalist-policy | - | Octo：开源通用机器人策略。 |
| [Open X-Embodiment: Robotic Learning Datasets and RT-X Models](https://arxiv.org/abs/2310.08864) | Open X-Embodiment Collaboration et al. | 2023-10-13 | arXiv | dataset, cross-embodiment | - | Open X-Embodiment / RT-X：跨本体机器人数据集与模型。 |
| [RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control](https://arxiv.org/abs/2307.15818) | Anthony Brohan et al. | 2023-07-28 | arXiv | vla, web-knowledge, google | - | RT-2：将网络知识迁移到机器人控制的 VLA 模型奠基作。 |
| [RT-1: Robotics Transformer for Real-World Control at Scale](https://arxiv.org/abs/2212.06817) | Anthony Brohan et al. | 2022-12-13 | arXiv | robotics-transformer, real-world | - | RT-1：大规模真实世界控制的机器人 Transformer。 |
