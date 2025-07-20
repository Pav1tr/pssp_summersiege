# Protein Secondary Structure Prediction (PSSP)

This repository contains code and models for **Protein Secondary Structure Prediction** using deep learning techniques like 1D Convolution and attention-based layers. Built with the help of PyTorch and Scikit-Learn libraries, the notebook demonstrates the full pipeline from preprocessing to evaluation using Q3 accuracy metrics.

---

## Files

| File | Description |
|------|-------------|
| `PSSP_PS4.ipynb` | Main Jupyter Notebook with code for loading data, building models, training, and evaluating Q3 performance. |

---

## Problem Statement

Develop a high-accuracy machine learning model to predict the three-state secondary structure (α-helix [H], β-sheet [E], or coil [C]) of individual amino acids in a protein using only its raw sequence data, without requiring evolutionary or homologous sequence information. The model should address key challenges in computational biology while minimizing reliance on domain-specific biological knowledge.

---

## Model Architecture

- **Input**: Encoded amino acid sequences
- **Layers**:
  - Embedding / Dense Layer
  - 1D Convolution Layer
  - Dropout Layer
- **Output**: Per-residue prediction of secondary structure (Q3 and Q8)
- **Dataset Used**: CB513 dataset found online. Also provided in the repository.

---

## Evaluation Metrics

- **Q3 and Q8 Accuracy** – Overall correctness of predicted secondary structure
- **Per-Class Accuracy** – Performance on all secondary structures (H, E, and C for Q3; H, B, E, G, I, T, S, and -(unknown) for Q8)

---
