---
title: "Temporal-Aware Encoder for Egocentric Video Retrieval"
excerpt: "Final year project — tripled video-text retrieval baseline on EPIC-Kitchens-100 with temporal adapters on frozen vision-language backbones."
collection: portfolio
date: 2026-03-01
---

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)

My final year project at the University of Bristol, supervised by [Shawn Shen](https://shawnshenjx.github.io). The goal is to improve video-text retrieval on egocentric videos by adding temporal modeling to frozen vision-language backbones.

- Identified that CLIP/PE text encoders give **0.97+ cosine similarity** between temporal opposites like "open fridge" vs "close fridge", and mean pooling over frames destroys temporal order.
- Designed and compared four temporal adapter architectures (MLP, Transformer, Conv1D, ST-Adapter) on frozen Perception Encoder features.
- Best model (ST-Adapter with middle fusion) **tripled zero-shot baseline R@1** on EPIC-Kitchens-100 (V2T R@1: 1.09% → 2.78%).
- Ran verb-aware hard negative ablation — negative result showing the bottleneck is in the frozen text encoder, not the training loss.
- Evaluated on [EPIC-Kitchens-100](https://epic-kitchens.github.io/2025) and [Ego4D](https://ego4d-data.org) egocentric video benchmarks.
