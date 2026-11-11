---
layout: page
title: Partial-LoRA
description: Fine-tuning with up to 87% fewer trainable parameters while maintaining or improving accuracy.
importance: 2
category: language models
permalink: /projects/partial-lora/
---

**Paper:** [The Quest for Winning Tickets in Low-Rank Adapters](https://arxiv.org/abs/2512.22495) (preprint, 2025)

### The problem

Low-rank adapters (LoRA) made fine-tuning large pretrained models much cheaper. This work asks whether even sparser adapters can match their accuracy.

### The approach

Partial-LoRA searches for "winning tickets" inside low-rank adapters, meaning small subsets of adapter parameters that can be trained on their own.

### Results

Partial-LoRA reduced trainable parameters by up to 87% while maintaining or improving accuracy, in experiments across 8 vision and 12 language tasks.
