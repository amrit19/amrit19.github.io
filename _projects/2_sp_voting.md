---
layout: page
title: Surprisingly popular voting
description: Recovering the ground truth from crowds of experts and non-experts. NeurIPS 2024, WWW 2025 and KDD 2026.
importance: 2
category: masters @ Penn State
related_publications: true
---

**FAIR Lab, Penn State, Jan 2023 to Dec 2024**

Advised by Dr. Hadi Hosseini; mentored by and in collaboration with Dr. Debmalya Mandal.

When most of a crowd is misinformed, aggregating their votes amplifies the error. The _surprisingly popular_ (SP) algorithm asks each person for their own answer and for a prediction of how others will answer, then picks the answer that is more popular than predicted. That lets it recover the truth even when the experts are a minority. My MS work extended SP from single questions to rankings over many alternatives.

- **Scaling SP to partial preferences (NeurIPS 2024)** {% cite hosseini2024sp %}. Designed Partial-SP and Aggregated-SP, which ask each voter for a vote and a prediction over only a small subset of the alternatives, as a top choice, an approval set or a partial ranking. In a crowdsourcing study with 432 participants on Amazon Mechanical Turk, across geography, movies and paintings, both outperformed classical rules such as Borda, Copeland, Maximin and Schulze at recovering the true ranking. Voter behavior was modeled with a concentric mixture of Mallows models, fit by Bayesian inference (No-U-Turn sampling), and the sample complexity was shown to grow by a factor of k! rather than m! for subsets of size k out of m alternatives.
- **When SP voting works (WWW 2025)** {% cite hosseini2025concentric %}. Proposed concentric mixtures of Mallows and Plackett-Luce models with any number of voter groups, identified expert, intermediate and non-expert groups in real data, and derived the conditions and number of samples under which SP voting recovers the true ranking with high probability.
- **SP-Rank dataset (KDD 2026)** {% cite hosseini2026sprank %}. Released the first large public dataset that pairs ranked votes with predictions of others' votes: 12,384 datapoints from 1,152 participants in nine elicitation formats, with benchmarks for full and subset rank recovery and for modeling voter behavior. [Dataset and code on GitHub](https://github.com/amrit19/SP-Rank-Dataset).

This work formed my MS thesis {% cite puhan2024thesis %}, which won the Best MS Thesis Award in Artificial Intelligence at the Penn State AI Awards. Implementations of the classical voting rules are on [GitHub](https://github.com/amrit19/Vote-Aggregation-Rules).
