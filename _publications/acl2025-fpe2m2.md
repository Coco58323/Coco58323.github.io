---
title: "FPE2M2: Approaching Lossless and Efficient Quantization with Native Floating Point"
collection: publications
permalink: /publication/acl2025-fpe2m2
excerpt: 'A novel FPE2M2 floating-point quantization format that achieves near-lossless accuracy with efficient CUDA implementation for LLM weight-only quantization.'
date: 2025-02-01
venue: 'ACL'
citation: '<b>Ke Yi</b>, Jianwei Zhang, Jia Li, Junyang Lin, Jingren Zhou. <b>ACL 2025</b>'
---

## Abstract

In the decoding phase, the system bottleneck lies in weight transfer bandwidth. Weight quantization can improve system throughput under bandwidth constraints. Current mainstream weight quantization uses 4-bit with calibration algorithms, but calibration is time-consuming and prone to overfitting. 

We propose the **FPE2M2** floating-point quantization format with efficient CUDA implementation for FPE2M2 to FP16/FP8 conversion. The operator overhead approaches 4-bit quantization while achieving **near-lossless** accuracy on downstream tasks.

## Key Contributions

- Novel FPE2M2 floating-point quantization format
- Efficient CUDA kernel implementation
- Near-lossless accuracy with 4-bit-level efficiency

