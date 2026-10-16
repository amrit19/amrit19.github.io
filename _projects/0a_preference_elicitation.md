---
layout: page
title: Inference-time preference elicitation in multi-agent LLMs
description: Can voting rules beyond majority vote help LLM agents reach the right answer when the strongest agent is outvoted?
importance: 1
category: current research (independent researcher)
---

**Independent research, 2025 to present**

Multi-agent LLM systems usually settle on a final answer by majority vote. That can overrule a stronger agent whenever weaker agents agree with each other. I study whether eliciting richer information from the agents at inference time, namely each agent's ranking of the candidate answers and its prediction of how the group will rank them, lets a _surprisingly popular_ (SP) voting rule recover the correct answer more often than majority vote.

The testbed runs multi-agent debate on verified math problems ([Big-Math-RL-Verified](https://huggingface.co/datasets/SynthLabsAI/Big-Math-RL-Verified)) with ten open models from the Llama, Phi and Qwen families, from 1.5B to 14B parameters. It covers homogeneous ensembles, ensembles with one strong and two weak agents, and cross-family ensembles, under three interaction modes: full debate, no debate, and sharing answers only. Majority and SP voting are compared on the same debates, with ordinal (rank-based) and cardinal (probability-based) versions of SP, and the analysis measures how often agents' predictions actually differ from their own votes, which is what SP relies on.

The framework builds on multi-agent debate ([Du et al., 2023](https://arxiv.org/abs/2305.14325)) and multiagent fine-tuning ([Subramaniam et al., 2025](https://arxiv.org/abs/2501.05707)), and runs on Apple Silicon with MLX.
