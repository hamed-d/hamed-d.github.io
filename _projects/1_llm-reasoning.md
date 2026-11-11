---
layout: page
title: Reliable LLM reasoning
description: Telling correct reasoning from errors using how a model's internal representations change across layers.
importance: 1
category: language models
permalink: /projects/llm-reasoning/
---

**Papers:** [Truth as a Trajectory](https://aclanthology.org/2026.acl-long.2073/) (ACL 2026, oral, Best Paper Award nominee) &middot; [Reasoning Errors Have a Region and a Direction in the Residual-Stream Trajectory of LLMs](https://arxiv.org/abs/2608.05660) (preprint, 2026) &middot; [Project page](https://hamed-d.github.io/truth-as-a-trajectory-page/)

### The problem

Language models can produce reasoning that reads well but is wrong. Judging an answer from its text alone tends to pick up superficial lexical cues rather than whether the reasoning is valid.

### The approach

Instead of looking at a single layer, we treat a response as a trajectory through the model's layers and use how its internal representations change across them to distinguish valid reasoning from errors.

The follow-up work combines these changes with coarse regions and directions in the model's internal state space.

### Results

- _Truth as a Trajectory_ reduces reliance on superficial lexical cues and outperforms conventional probes across several benchmarks.
- The follow-up improves answer selection on unseen reasoning benchmarks and generalises to factual tasks.
- _Truth as a Trajectory_ was presented as an oral at ACL 2026 and nominated for the Best Paper Award.
