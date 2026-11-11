---
layout: page
title: Model editing with task vectors
description: Separating shared and task-specific parts of task vectors for more targeted model editing.
importance: 3
category: language models
permalink: /projects/task-vector-editing/
---

**Paper:** [Decomposing Task Vectors for Refined Model Editing](https://arxiv.org/abs/2512.22511) (preprint, 2025)

### The problem

Task vectors are the weight differences between a fine-tuned model and its base. They let you add or remove behaviour by arithmetic on weights, but each vector mixes knowledge shared across tasks with knowledge specific to one task. Editing with the whole vector can therefore change more than intended.

### The approach

We decompose task vectors into shared and task-specific components, so edits can target only the part that matters.

### Results

- The decomposition supports controlled model merging, diffusion style mixing and toxicity reduction.
- In experiments, it lowered toxicity by 47% while preserving performance on general-knowledge tasks.
