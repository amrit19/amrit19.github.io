---
layout: page
title: Better preference labels for RLHF
description: Using surprisingly popular voting to label reward-model data when most labelers are wrong. Part of my MS thesis.
importance: 1
category: masters @ Penn State
---

**[FAIR Lab](https://faculty.ist.psu.edu/hadi/lab.html), Penn State, Nov 2023 to Aug 2024**

In reinforcement learning from human feedback (RLHF), a reward model learns from preference labels that are usually aggregated from many annotators by majority vote. If most annotators are wrong, the reward model learns the wrong preferences, and the language model fine-tuned against it follows them.

In a chapter of my MS thesis, I tested whether _surprisingly popular_ (SP) voting can produce better labels. Weaker language models (GPT-2, DistilBERT, DistilGPT-2) stood in for non-expert annotators and stronger ones (Llama 3 8B, Mistral 7B v0.3, DeBERTa, Phi-3) for experts. Each model picked the correct ending for commonsense questions from the SWAG dataset and predicted how the other models would vote, with many more samples drawn from the weaker models than from the stronger ones. In these preliminary experiments, SP voting improved label accuracy by 9% on average over standard voting rules.

I built the full pipeline with Hugging Face TRL: supervised fine-tuning, preference data generation, reward modeling and PPO. Related code: [supervised fine-tuning of BERT, RoBERTa and DeBERTa, with and without PEFT](https://github.com/amrit19/Supervised-Fine-Tuning-Language-Models).
