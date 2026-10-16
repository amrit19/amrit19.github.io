---
layout: page
title: Improving LLMs through multi-agent fine-tuning
description: Choosing fine-tuning data from LLM debates with better aggregation rules than majority vote.
importance: 2
category: current research (independent researcher)
---

**Independent research, 2025 to present**

[Multiagent fine-tuning](https://arxiv.org/abs/2501.05707) improves a group of LLMs by fine-tuning each one on data from their own debates: generator agents learn from reasoning traces that reached the consensus answer, and critic agents learn from cases where an agent revised its answer toward the consensus. The consensus is chosen by majority vote, so when the majority is wrong, the agents are trained on wrong answers.

I have built the pipeline that turns debate logs into generator and critic fine-tuning data, and I am extending it so that the consensus used to select training data can come from SP voting and other aggregation rules instead of majority vote. The goal is to see whether better aggregation leads to better training data, and whether that improvement compounds over several rounds of fine-tuning.
