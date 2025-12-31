---
title: "Learning Topology-Agnostic EEG Representations with Geometry-Aware Modeling"
collection: publications
permalink: /publication/nips2023-eeg
excerpt: 'A topology-agnostic EEG pre-training framework that enables cross-dataset pre-training with multi-dimensional position encoding and multi-stage training strategy.'
date: 2023-09-23
venue: 'NeurIPS'
citation: '<b>Ke Yi</b>, Yansen Wang, Ren Kan, Dongshen Li. <b>NeurIPS 2023</b>'
---

## Abstract

Large-scale pre-training has shown great potential to enhance models on downstream tasks in vision and language. Developing similar techniques for scalp electroencephalogram (EEG) is suitable since unlabelled data is plentiful. Meanwhile, various sampling channel selections and inherent structural and spatial information bring challenges and avenues to improve existing pre-training strategies.

To break the boundaries between different EEG resources and facilitate cross-dataset EEG pre-training, we propose to map all kinds of channel selections to a unified topology. We further introduce **MMM**, a pre-training framework with:
- **M**ulti-dimensional position encoding
- **M**ulti-level channel hierarchy  
- **M**ulti-stage pre-training strategy

Experiments demonstrate that our approach yields impressive improvements over previous state-of-the-art techniques on emotional recognition benchmark datasets.

## Keywords

Electroencephalogram, EEG Pre-training, EEG-based emotion recognition

