<h1 align="center">Seq2Seq_LSTM_MOT</h1>

<p align="center">
  <em>Seq2Seq + LSTM trajectory modeling for Multi-Object Tracking under occlusion</em>
</p>

<p align="center">
  <img alt="Python" src="https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white">
  <img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-2.0%2B-EE4C2C?logo=pytorch&logoColor=white">
  <img alt="Task" src="https://img.shields.io/badge/Task-Multi--Object%20Tracking-555">
  <img alt="Status" src="https://img.shields.io/badge/Status-Research-yellow">
</p>

---

## Overview

This repository contains an experimental implementation of a **Seq2Seq + LSTM-based Multi-Object Tracking (MOT)** framework. The project studies how temporal motion patterns can be learned directly from object trajectories and used to maintain identities through occlusion — a recurring failure mode of appearance-only association in manufacturing and logistics scenes.

| Aspect | Detail |
| --- | --- |
| **Task** | Multi-Object Tracking (motion-only association) |
| **Core model** | Sequence-to-Sequence encoder–decoder with LSTM cells |
| **Input** | Object trajectory sequences extracted from video |
| **Output** | Predicted future trajectories / motion sequences |
| **Purpose** | Research on sequence modeling as an alternative to appearance-based association |

## Repository Structure

```text
.
├── videos/             # Large video files (managed with Git LFS)
│   ├── train_video.mp4
│   └── test_video.mp4
├── src/                # Source code (model, training, inference)
├── README.md
└── .gitattributes      # Git LFS configuration
```

> Video assets are tracked with [Git LFS](https://git-lfs.com). Run `git lfs install` once before cloning so the binaries are fetched correctly.

## Motivation

Appearance-based association breaks down when targets are visually similar or occluded for many frames. By treating each track as a sequence problem and letting an LSTM encoder–decoder learn the underlying motion grammar, the tracker can hypothesize trajectories across occlusion gaps without relying on re-identification features.

## Status

Active research code — interfaces and configurations are subject to change. Released alongside ongoing work at SOS Lab on appearance-free multi-camera multi-object tracking.

## Author

**Yunho Seo** — MS student, SOS Lab, Kyonggi University  
[@yunhoseo](https://github.com/yunhoseo) · yunho.seo@kyonggi.ac.kr · [Google Scholar](https://scholar.google.com/citations?user=6oiCOa8AAAAJ&hl=ko) · [ORCID](https://orcid.org/0009-0008-2599-6824)
