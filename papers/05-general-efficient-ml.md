# 05 · 通用高效 ML 方法

> FlashAttention、经典量化 / 稀疏化方法、投机解码等被广泛采用的里程碑工作。**仅收录里程碑级工作，普通增量不收**。

[← 研究地图](README.md) · [最新收录](LATEST.md)

## 量化（3）

| 论文 | 作者 | 发布 | Venue | 标签 | 代码 | TL;DR |
| --- | --- | --- | --- | --- | --- | --- |
| [AWQ: Activation-aware Weight Quantization for On-Device LLM Compression and Acceleration](https://dblp.org/rec/conf/mlsys/0002TTYCWXDG024.html) | Ji Lin 0002 et al. | 2024 | MLSys | quantization, awq, on-device, llm | - | 激活感知权重量化（AWQ）实现端侧 LLM 压缩与加速，已被主流推理框架广泛集成。 |
| [SmoothQuant: Accurate and Efficient Post-Training Quantization for Large Language Models](https://arxiv.org/abs/2211.10438) | Guangxuan Xiao et al. | 2022-11-18 | arXiv | quantization, w8a8 | [code](https://github.com/mit-han-lab/smoothquant) | SmoothQuant：精确高效的 LLM 后训练量化。 |
| [GPTQ: Accurate Post-Training Quantization for Generative Pre-trained Transformers](https://arxiv.org/abs/2210.17323) | Elias Frantar et al. | 2022-10-31 | arXiv | quantization, post-training | [code](https://github.com/IST-DASLab/gptq) | GPTQ：精确的一次性后训练量化方法。 |

## 投机解码（3）

| 论文 | 作者 | 发布 | Venue | 标签 | 代码 | TL;DR |
| --- | --- | --- | --- | --- | --- | --- |
| [Medusa: Simple LLM Inference Acceleration Framework with Multiple Decoding Heads](https://arxiv.org/abs/2401.10774) | Tianle Cai et al. | 2024-01-19 | arXiv | speculative-decoding, decoding-heads | [code](https://github.com/FasterDecoding/Medusa) | Medusa：多解码头的简易 LLM 推理加速框架。 |
| [SpecInfer: Accelerating Large Language Model Serving with Tree-based Speculative Inference and Verification](https://dblp.org/rec/conf/asplos/MiaoOZCWZWZYSSC24.html) | Xupeng Miao et al. | 2024 | ASPLOS | speculative-decoding, tree-based, llm-serving | - | 树状投机推理与验证加速 LLM serving，投机解码系统化的代表作。 |
| [Fast Inference from Transformers via Speculative Decoding](https://arxiv.org/abs/2211.17192) | Yaniv Leviathan et al. | 2022-11-30 | arXiv | speculative-decoding, draft-verify | - | 投机解码：通过草稿-验证加速 Transformer 推理的开创性工作。 |

## 注意力与 Kernel（4）

| 论文 | 作者 | 发布 | Venue | 标签 | 代码 | TL;DR |
| --- | --- | --- | --- | --- | --- | --- |
| [FlashInfer: Efficient and Customizable Attention Engine for LLM Inference Serving](https://dblp.org/rec/conf/mlsys/00010LLZW0KGKC25.html) | Zihao Ye 0001 et al. | 2025 | MLSys | attention-kernel, llm-serving, gpu-kernel | - | 高效可定制的 LLM 推理 attention 引擎，已被 vLLM/SGLang 等主流框架集成为默认 kernel 后端。 |
| [FlashAttention-3: Fast and Accurate Attention with Asynchrony and Low-precision](https://arxiv.org/abs/2407.08608) | Jay Shah et al. | 2024-07-11 | arXiv | attention, low-precision, hopper | - | FlashAttention-3：异步与低精度加速的注意力实现。 |
| [FlashAttention-2: Faster Attention with Better Parallelism and Work Partitioning](https://arxiv.org/abs/2307.08691) | Tri Dao | 2023-07-17 | arXiv | attention, parallelism | - | FlashAttention-2：更优并行与工作划分的注意力实现。 |
| [FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness](https://arxiv.org/abs/2205.14135) | Tri Dao et al. | 2022-05-27 | arXiv | attention, io-aware, gpu-kernel | - | FlashAttention：IO 感知的快速精确注意力，成为全行业标准实现。 |

## 稀疏化（2）

| 论文 | 作者 | 发布 | Venue | 标签 | 代码 | TL;DR |
| --- | --- | --- | --- | --- | --- | --- |
| [A Simple and Effective Pruning Approach for Large Language Models](https://arxiv.org/abs/2306.11695) | Mingjie Sun et al. | 2023-06-20 | arXiv | pruning, activation-aware | [code](https://github.com/locuslab/wanda) | Wanda：简单有效的 LLM 剪枝方法。 |
| [SparseGPT: Massive Language Models Can Be Accurately Pruned in One-Shot](https://arxiv.org/abs/2301.00774) | Elias Frantar et al. | 2023-01-02 | arXiv | pruning, one-shot | [code](https://github.com/IST-DASLab/sparsegpt) | SparseGPT：大模型一次性精确剪枝。 |
