---
title: "Rotated Runtime Smooth: Training-Free Activation Smoother for Accurate INT4 Inference"
collection: publications
permalink: /publication/iclr2025-rrs
excerpt: 'A novel training-free activation smoothing method that enables accurate INT4 inference for LLMs by handling outliers in real-time.'
date: 2025-01-01
venue: 'ICLR'
citation: '<b>Ke Yi</b>, Zengke Liu, Jianwei Zhang, Chengyuan Li, Tong Zhang, Junyang Lin, Jingren Zhou. <b>ICLR 2025</b>'
---

## Abstract

When using 4-bit quantization for both activations and weights in LLM inference, matrix operations can achieve higher computational throughput. However, outliers compress the representation space of normal values during quantization, leading to significant accuracy degradation. We propose a real-time outlier smoothing operator that efficiently integrates with existing computation frameworks. With only **1% additional overhead**, we improve the 4-bit inference perplexity (PPL) of LLaMA3-70B from **49.73** to **6.87**.

## Key Contributions

- Training-free activation smoothing for INT4 inference
- Real-time outlier handling with minimal overhead
- Significant accuracy improvement on large language models

