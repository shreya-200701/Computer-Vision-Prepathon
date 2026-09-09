# Computer-Vision-Prepathon
# Computer Vision Prepathon

This repository contains my solutions for the Computer Vision Prepathon.

## Tasks

### Task A — Automated Segmentation of Solar Filaments

The objective is to segment solar filaments from full-disk H-alpha solar images.

Approach:
- U-Net based semantic segmentation
- Baseline BCE + Dice loss
- Edge-aware loss using Sobel edge information
- Pixel-level and instance-level evaluation
- Threshold and multi-scale analysis
- Failure-case visualization

Main metrics:
- IoU
- Precision
- Recall
- AP@IoU 0.5
- Hit Rate
- Miss Rate
- Multi-scale IoU (MIoU)

Notebook:
`Task_A_Solar_Filament_Segmentation/Task_A.ipynb`

---

### Task B — Diagnosing Object Hallucination in Vision-Language Models

The objective is to reduce object hallucination in Vision-Language Models using the POPE benchmark.

Model:
- BLIP VQA

Approaches evaluated:
- Baseline VLM
- Naive prompting
- Confidence-based decision thresholding

Evaluation metrics:
- Accuracy
- Precision
- Recall
- F1 Score
- False Positive Rate (FPR)
- Confusion Matrix

The confidence-based approach was evaluated at multiple thresholds and a threshold of 0.70 was selected as the final operating point.

Notebook:
`Task_B_VLM_Hallucination/Task_B.ipynb`

---

## Repository Structure

```text
Computer-Vision-Prepathon/
│
├── Task_A_Solar_Filament_Segmentation/
│   └── Task_A.ipynb
│
├── Task_B_VLM_Hallucination/
│   └── Task_B.ipynb
│
├── results/
│   ├── Task_A/
│   └── Task_B/
│
├── README.md
└── report.pdf
