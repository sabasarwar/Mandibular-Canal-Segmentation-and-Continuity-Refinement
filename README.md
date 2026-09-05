# Mandibular Canal Segmentation and Continuity Refinement

## Overview

Accurate localization of the inferior alveolar nerve (IAN) within the mandibular canal is essential for safe dental implant planning — a gap in a segmented canal corresponds to an unknown nerve position and is clinically unusable. This project presents a novel mandibular canal segmentation pipeline for 3D CBCT scans, built in two stages: a supervised 3D nnU-Net model, trained using a progressive, model-assisted annotation strategy, followed by a training-free post-processing refinement stage that restores anatomical continuity to the model's predictions. The refinement traces minimum-cost paths through the network's own probability field to bridge genuine gaps, while a conservative, ground-truth-free safety rule declines to bridge canals that are truly disrupted by pathology and flags them for clinician review instead.

Despite achieving strong overlap-based accuracy, we found that high-Dice segmentations can still be discontinuous — a failure mode invisible to standard metrics but critical for clinical use. This repository accompanies our paper (in preparation), which details the method, dataset, and full experimental results.

## Repository Contents

This repository shares a representative subset of data and outputs — **not the full dataset or codebase** (code to be released separately).
## Citation

A paper describing this work is in preparation. Citation details will be added here upon publication.

## License

See [LICENSE](LICENSE) for details.