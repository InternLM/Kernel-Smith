# Kernel-Smith

**Kernel-Smith** is a GPU kernel generation system developed by the Shanghai Artificial Intelligence Laboratory and MetaX. The technical report is available [here](https://arxiv.org/pdf/2603.28342).

> We do not currently plan to release the Kernel-Smith model weights or agent code. For now, this repository will focus on sharing generated kernels, benchmarks, and related documentation. Stay tuned.

## 🌟 Highlights

- Uses an evolution-based optimization loop with stable evaluation on both **NVIDIA Triton** and **MetaX MACA** backends.
- Trains for kernel improvement by rewarding correctness-preserving changes that increase performance.
- Outperforms frontier models like Gemini-3.0-pro and Claude-4.6-opus on KernelBench.

## 🚀 Production-Level Deployment

Kernel-Smith generated kernels have already been integrated into several open-source projects:

| Project | Optimized Kernel | Impact | Pull Request |
| :--- | :--- | :--- | :--- |
| **SGLang** | `normal_decode_set_metadata` | **4.78x** kernel acceleration | [#20778](https://github.com/sgl-project/sglang/pull/20778) |
| **LMDeploy** | DeepSeek MoE Routing | **1.36x** kernel acceleration | [#4345](https://github.com/InternLM/lmdeploy/pull/4345) |
| **DLBlas** | DeepSeek Engram kernels | Accelerated architecture research | [#102](https://github.com/DeepLink-org/DLBlas/pull/102) |

## 🌐 Try It Out

[Kernel-Smith Online Demo](https://chat.intern-ai.org.cn/kernel-smith)