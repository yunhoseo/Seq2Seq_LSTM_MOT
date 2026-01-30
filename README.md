# Seq2Seq_LSTM_MOT
## Seq2Seq LSTM-Based Multi-Object Tracking for Occlusion Handling in Manufacturing Environments

# Seq2Seq_LSTM_MOT

This repository contains an experimental implementation of a **Seq2Seq + LSTM-based Multi-Object Tracking (MOT)** framework.  
The project focuses on learning temporal motion patterns from object trajectories and applying sequence-to-sequence modeling for tracking tasks.

---

## 📌 Project Overview

- **Task**: Multi-Object Tracking (MOT)
- **Core Model**: Seq2Seq architecture with LSTM
- **Input**: Object trajectory sequences extracted from video
- **Output**: Predicted future trajectories / motion sequences
- **Purpose**: Research and experimentation on sequence modeling for object tracking

---

## 📁 Repository Structure

```text
.
├── videos/                 # Large video files (managed with Git LFS)
│   ├── train_video.mp4
│   └── test_video.mp4
├── src/                    # (Optional) source code directory
├── README.md
└── .gitattributes          # Git LFS configuration
