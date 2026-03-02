---
title: "Tencent Advertising Algorithms Competition (Top 10%)"
excerpt: "Built a multi-modal generative recommendation system and achieved 3.3x score improvement."
collection: portfolio
date: 2025-09-01
---

In Tencent's next-item prediction challenge, I designed a recommendation system beyond a standard dual-tower setup.

- Adapted HSTU-style sequence modeling with relative attention bias for long-range dependencies.
- Extended a SASRec baseline to a three-tower architecture (user, item, sequence).
- Added InfoNCE-based contrastive learning and cross-time negative sampling.
- Optimized preprocessing and temporal pipeline:
  - Training time per epoch: 1h -> 15min
  - Inference time: 1h -> 20min
- Final result: score improved from `0.023` to `0.076` (`3.3x`), ranking in the top 10% among 2000+ teams.
