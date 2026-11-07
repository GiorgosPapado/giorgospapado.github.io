---
layout: default
title: Projects
permalink: /projects/
---

# Projects

## vit-thesis

Code for my MSc thesis, *Vision Transformer for Gesture Recognition from EMG Signals* (Aristotle University of Thessaloniki). It compares Vision Transformers (fine-tuned from a Google checkpoint, and trained from scratch) against a PCA+SVM baseline on gesture recognition and user identification, using the GRABMyo EMG data with participant-grouped splits. A separate ViT-GPT2 image-captioning pipeline lives in the same repository.

Caveats, as stated in the repository: the thesis reports a better result for the ViT, but this code does not reproduce those numbers, and nothing has been re-run end to end on the real data since the refactor. TODO(author): dataset licence and how to obtain the data.

[Repository](https://github.com/GiorgosPapado/vit-thesis)

## vr-gesture-recognition

Real-time VR controller gesture recognition. Models are trained in Python (Hydra, Nevergrad, sktime), exported to ONNX and run in Unity (C#/ML.NET) or in the browser (WebXR). The repository also contains tooling and baselines for a cleaned 24-class hand-gesture set.

Caveats: the recordings are not included in the repository, and the baselines (logistic regression 0.371 and LDA 0.355 test accuracy, session-grouped splits) are weak starting points, not good models. TODO(author): model details (classes, input shape, accuracy) and paper reference.

[Repository](https://github.com/GiorgosPapado/vr-gesture-recognition)

## Tower-Defence

A 3D tower defence game made in Unity: eight waves of three enemy types, three turret types (Standard, Missile, Laser) and a small neural-network builder AI (about 1.4k parameters) trained with evolution strategies inside Unity. The AI also works as a balance-testing harness.

Caveats: in the repository's own evaluation the learned policy only ties a tuned hand-written baseline, and the game is effectively solved by spamming the cheap Standard turret. TODO(author): gameplay GIF or build link.

[Repository](https://github.com/GiorgosPapado/Tower-Defence)

## efficient-inference

Efficient transformer inference experiments: ONNX Runtime optimisation and benchmarks (BERT QA, M2M100), a thermal person-detection ONNX/INT8 study, and an in-progress Once-for-All-style elastic transformer for EMG. All results so far are sanity-level, not final.

The repository is not public yet. TODO(author): add the link when it is published.

## SADAMB paper

Papadopoulos, Drakoulis, Ntovas, Doumanoglou and Zarpalas, *Computers* (MDPI) 2025, 14(10), 413. DOI 10.3390/computers14100413: [read the paper](https://www.mdpi.com/2073-431X/14/10/413). TODO(author): one-line description of the paper and my role.
