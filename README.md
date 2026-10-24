# 大模型推理优化专家 (LLM Inference Optimization Expert)

专注大模型（LLM）推理降本提速的 AI 专家：量化与压缩、推理引擎部署、KV Cache 与连续批处理、吞吐与首字延迟（TTFT）调优，给出可量化落地的工程方案。

## 类型

Agent 型（单个 AI 专家）

## 核心能力

- **量化与压缩**：GPTQ / AWQ / GGUF / NF4 / HQQ，4bit·8bit 选型与精度评估
- **推理引擎部署**：vLLM / TensorRT-LLM / SGLang / llama.cpp / Ollama 拓扑与并行策略
- **注意力与调度优化**：PagedAttention、KV Cache 量化、连续批处理、推测解码、前缀缓存
- **性能剖析调优**：TTFT / TPOT / P99 瓶颈定位与参数调优
- **蒸馏与小型化**：知识蒸馏、结构化剪枝、LoRA 替代全量

## 试试这样问我

- 帮我把一个 7B 模型量化到 4bit，并评估精度与显存变化
- 用 vLLM 部署 Qwen，在固定显存下把吞吐拉到最高
- 分析我的推理服务 P99 延迟瓶颈，给出优化方案

## 本地安装（WorkBuddy 我的专家）

将本目录放到专家目录下并注册：

```
C:\Users\Administrator\.workbuddy\plugins\marketplaces\my-experts\plugins\llm-inference-optimization-expert\
```

```bash
python3 scripts/register_expert.py <expert-dir>
```

## 从 GitHub 安装

```bash
git clone https://github.com/dzp181/llm-inference-optimization-expert.git
cp -r llm-inference-optimization-expert \
  ~/.workbuddy/plugins/marketplaces/my-experts/plugins/
python3 scripts/register_expert.py \
  ~/.workbuddy/plugins/marketplaces/my-experts/plugins/llm-inference-optimization-expert
```

## 打包分享

```bash
python3 scripts/package_expert.py llm-inference-optimization-expert
```

## 头像

头像位于 `avatars/expert.png`（512×512，≤500KB）。如需替换，要求：PNG（推荐）或 JPG，512×512 px，单张不超过 500KB。
