# 🧑‍🔬 领先研究组与生态

> 追踪 Physical AI Systems / Infra 方向有持续高影响力产出的学术实验室、工业研究团队与开源生态。
> 数据维护在 [`data/groups.json`](../data/groups.json)，此页由其生成；代表论文均链回本仓库收录记录。

[← 返回首页](../README.md)

## 学术实验室

### UC Berkeley Sky Computing Lab

- **方向**：LLM serving 系统与开源机器人模型
- **简介**：vLLM 谱系（SLoRA / Punica / SkyServe 等）与 Octo 通用机器人策略。
- **链接**：[主页](https://sky.cs.berkeley.edu)
- **代表论文（6）**：[SLoRA: Scalable Serving of Thousands of LoRA Adapters](https://dblp.org/rec/conf/mlsys/0007CLHLYCZZK0S24.html)；[Punica: Multi-Tenant LoRA Serving](https://dblp.org/rec/conf/mlsys/Chen0WZCK24.html)；[SkyServe: Serving AI Models across Regions and Clouds with Spot Instances](https://dblp.org/rec/conf/eurosys/MaoXWCGBYSS25.html)；[MoE-Lightning: High-Throughput MoE Inference on Memory-constrained GPUs](https://dblp.org/rec/conf/asplos/CaoLGSL0GZS25.html)；[NEO: Saving GPU Memory Crisis with CPU Offloading for Online LLM Inference](https://dblp.org/rec/conf/mlsys/JiangZCSY25.html)；[Octo: An Open-Source Generalist Robot Policy](https://arxiv.org/abs/2405.12213)

### MIT HAN Lab（Song Han）

- **方向**：高效推理与量化（AWQ / QServe / SmoothQuant / LServe）
- **简介**：端侧量化与长序列 serving 的系列奠基工作，开源生态影响力大。
- **链接**：[主页](https://hanlab.mit.edu)
- **代表论文（4）**：[AWQ: Activation-aware Weight Quantization for On-Device LLM Compression and Acceleration](https://dblp.org/rec/conf/mlsys/0002TTYCWXDG024.html)；[QServe: W4A8KV4 Quantization and System Co-design for Efficient LLM Serving](https://dblp.org/rec/conf/mlsys/0001TYZX0025.html)；[SmoothQuant: Accurate and Efficient Post-Training Quantization for Large Language Models](https://arxiv.org/abs/2211.10438)；[LServe: Efficient Long-sequence LLM Serving with Unified Sparse Attention](https://dblp.org/rec/conf/mlsys/YangGT0XT0L0025.html)

### IST Austria（Frantar / Alistarh）

- **方向**：量化与剪枝方法（GPTQ / SparseGPT）
- **简介**：一次性后训练压缩路线的开创团队。
- **链接**：[主页](https://ista.ac.at)
- **代表论文（2）**：[GPTQ: Accurate Post-Training Quantization for Generative Pre-trained Transformers](https://arxiv.org/abs/2210.17323)；[SparseGPT: Massive Language Models Can Be Accurately Pruned in One-Shot](https://arxiv.org/abs/2301.00774)

### CMU（Catalyst / Kolter 等）

- **方向**：投机推理与 serving 系统
- **简介**：SpecInfer / SpotServe / Helix（Jia Zhihao 组）与 Wanda 剪枝。
- **链接**：[主页](https://catalyst.cs.cmu.edu)
- **代表论文（4）**：[SpecInfer: Accelerating Large Language Model Serving with Tree-based Speculative Inference and Verification](https://dblp.org/rec/conf/asplos/MiaoOZCWZWZYSSC24.html)；[SpotServe: Serving Generative Large Language Models on Preemptible Instances](https://dblp.org/rec/conf/asplos/MiaoSDXL0J24.html)；[Helix: Serving Large Language Models over Heterogeneous GPUs and Network via Max-Flow](https://dblp.org/rec/conf/asplos/Mei0MYJV25.html)；[A Simple and Effective Pruning Approach for Large Language Models](https://arxiv.org/abs/2306.11695)

### SJTU IPADS

- **方向**：端侧与机密推理系统
- **简介**：PowerInfer、PipeLLM 等端侧/机密 LLM 推理工作。
- **链接**：[主页](https://ipads.se.sjtu.edu.cn)
- **代表论文（2）**：[PowerInfer: Fast Large Language Model Serving with a Consumer-grade GPU](https://dblp.org/rec/conf/sosp/SongMX024.html)；[PipeLLM: Fast and Confidential Large Language Model Services with Speculative Pipelined Encryption](https://dblp.org/rec/conf/asplos/0005TM025.html)
## 工业研究

### Physical Intelligence (π)

- **方向**：VLA 基座模型（π 系列）
- **简介**：π0 / π0.5 / FAST 作者团队，通用机器人控制基础模型的定义者之一。
- **链接**：[主页](https://www.physicalintelligence.company)
- **代表论文（3）**：[$π_0$: A Vision-Language-Action Flow Model for General Robot Control](https://arxiv.org/abs/2410.24164)；[$π_{0.5}$: a Vision-Language-Action Model with Open-World Generalization](https://arxiv.org/abs/2504.16054)；[FAST: Efficient Action Tokenization for Vision-Language-Action Models](https://arxiv.org/abs/2501.09747)

### NVIDIA（GEAR / Isaac / Cosmos）

- **方向**：机器人基座模型与世界模型（GR00T / Cosmos / DreamZero）
- **简介**：GR00T 人形基座、Cosmos 世界模型平台与 DreamZero WAM，Physical AI 模型侧最完整的工业布局。
- **链接**：[主页](https://research.nvidia.com)
- **代表论文（4）**：[GR00T N1: An Open Foundation Model for Generalist Humanoid Robots](https://arxiv.org/abs/2503.14734)；[Cosmos World Foundation Model Platform for Physical AI](https://arxiv.org/abs/2501.03575)；[Cosmos Policy: Fine-Tuning Video Models for Visuomotor Control and Planning](https://arxiv.org/abs/2601.16163)；[World Action Models are Zero-shot Policies](https://arxiv.org/abs/2602.15922)

### 蚂蚁灵波 Robbyant

- **方向**：VLA 基座模型（LingBot 系列）
- **简介**：LingBot-VLA 系列以大规模真机数据与稀疏 MoE 路线著称，模型与数据均开源。
- **链接**：[主页](https://github.com/robbyant)
- **代表论文（2）**：[A Pragmatic VLA Foundation Model](https://arxiv.org/abs/2601.18692)；[From Foundation to Application: Improving VLA Models in Practice](https://arxiv.org/abs/2607.06403)

### Google DeepMind Robotics

- **方向**：RT 系列与 VLA 范式
- **简介**：RT-1/RT-2/RT-X 奠定 VLA 范式；投机解码原始论文同样出自 Google。
- **链接**：[主页](https://deepmind.google)
- **代表论文（4）**：[RT-1: Robotics Transformer for Real-World Control at Scale](https://arxiv.org/abs/2212.06817)；[RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control](https://arxiv.org/abs/2307.15818)；[Open X-Embodiment: Robotic Learning Datasets and RT-X Models](https://arxiv.org/abs/2310.08864)；[Fast Inference from Transformers via Speculative Decoding](https://arxiv.org/abs/2211.17192)

### Microsoft Research

- **方向**：LLM 推理系统（PD 分离 / 调度 / 量化 / 集群能效）
- **简介**：Splitwise、Sarathi-Serve、T-MAC、DynamoLLM 等，推理系统方向产出最密集的团队之一。
- **链接**：[主页](https://www.microsoft.com/en-us/research)
- **代表论文（6）**：[Splitwise: Efficient Generative LLM Inference Using Phase Splitting](https://dblp.org/rec/conf/isca/PatelCZSGMB24.html)；[Taming Throughput-Latency Tradeoff in LLM Inference with Sarathi-Serve](https://dblp.org/rec/conf/osdi/AgrawalKPMKGTR24.html)；[DynamoLLM: Designing LLM Inference Clusters for Performance and Energy Efficiency](https://dblp.org/rec/conf/hpca/StojkovicZGTC25.html)；[T-MAC: CPU Renaissance via Table Lookup for Low-Bit LLM Deployment on Edge](https://dblp.org/rec/conf/eurosys/WeiCCMWZY25.html)；[vAttention: Dynamic Memory Management for Serving LLMs without PagedAttention](https://dblp.org/rec/conf/asplos/PrabhuNMRP25.html)；[POD-Attention: Unlocking Full Prefill-Decode Overlap for Faster LLM Inference](https://dblp.org/rec/conf/asplos/KamathPM0RP25.html)

### ByteDance（Seed / Infra）

- **方向**：超大规模训练与推理基础设施（MegaScale 系列）
- **简介**：MegaScale 家族（训练 / Infer / Omni / Data）与万卡级生产系统实践。
- **链接**：[主页](https://team.doubao.com)
- **代表论文（3）**：[MegaScale: Scaling Large Language Model Training to More Than 10, 000 GPUs](https://dblp.org/rec/conf/nsdi/JiangLZHCZPLXNJ24.html)；[MegaScale-Infer: Efficient Mixture-of-Experts Model Serving with Disaggregated Expert Parallelism](https://dblp.org/rec/conf/sigcomm/ZhuJJWSWZZWCXZL25.html)；[Robust LLM Training Infrastructure at ByteDance](https://dblp.org/rec/conf/sosp/WanLSWZSWWWLYZJ25.html)

### Alibaba

- **方向**：数据中心网络与生产级 LLM serving
- **简介**：HPN 训练网络、Aegaeon GPU 池化、Llumnix 动态调度等生产系统。
- **链接**：[主页](https://www.alibabagroup.com)
- **代表论文（4）**：[Alibaba HPN: A Data Center Network for Large Language Model Training](https://dblp.org/rec/conf/sigcomm/QianXCGXGFSZMWW24.html)；[Aegaeon: Effective GPU Pooling for Concurrent LLM Serving on the Market](https://dblp.org/rec/conf/sosp/Xiang0QYZYZL0025.html)；[Llumnix: Dynamic Scheduling for Large Language Model Serving](https://dblp.org/rec/conf/osdi/SunHZXZL024.html)；[ServeGen: Workload Characterization and Generation of Large Language Model Serving in Production](https://dblp.org/rec/conf/nsdi/XiangLQZYZJZ26.html)
## 开源生态

### FlashInfer

- **方向**：注意力 kernel 生态
- **简介**：被 vLLM / SGLang 等主流 serving 框架集成的 attention kernel 库。
- **链接**：[主页](https://github.com/flashinfer-ai/flashinfer)
- **代表论文（1）**：[FlashInfer: Efficient and Customizable Attention Engine for LLM Inference Serving](https://dblp.org/rec/conf/mlsys/00010LLZW0KGKC25.html)

### KTransformers

- **方向**：CPU/GPU 混合 MoE 推理
- **简介**：端侧 MoE 推理的热门开源框架（清华 MADSV 等）。
- **链接**：[主页](https://github.com/kvcache-ai/ktransformers)
- **代表论文（1）**：[KTransformers: Unleashing the Full Potential of CPU/GPU Hybrid Inference for MoE Models](https://dblp.org/rec/conf/sosp/ChenXZTWDCYLQZO25.html)
