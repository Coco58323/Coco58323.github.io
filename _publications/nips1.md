---
title: "Learning Topology-Agnostic EEG Representations with Geometry-Aware Modeling"
collection: publications
permalink: /publication/nips1
excerpt: 'TL;DR: This paper is about how to spatial model EEG data with pre-training schema. The new pre-training schema is topology-agnostic, facilitating usage of EEG data in different tasks.'
date: 2023-09-23
venue: 'NeurIPS'
# paperurl: 'http://academicpages.github.io/files/paper1.pdf'
citation: 'Ke Yi, Yansen Wang, Ren Kan, Dongshen Li. NeurIPS 2023 (poster)'
---

## Abstract

Large-scale pre-training has shown great potential to enhance the models on the downstream task in vision and language. Developing similar techniques for scalp electroencephalogram (EEG) is suitable since unlabelled data is plentiful. Meanwhile, various sampling channels selection and inherent structural and spatial information bring challenges and avenues to improve existing pre-training strategies further. In order to break the boundaries between different EEG resources and facilitate cross-dataset EEG pre-training, we propose to map all kinds of channel selections to a unified topology. We further introduce MMM, a pre-training framework with Multi-dimensional position encoding,Multi-level channel hierarchy, Multi-stage pre-training strategy built on the unified topology to obtain topology-agnostic representations. Experiments demonstrate that our approach yields impressive improvements over previous state-of-the-art techniques on emotional recognition benchmark datasets.

## Key words
Electroencephalogram, EEG Pre-training, EEG-based emotion recognition