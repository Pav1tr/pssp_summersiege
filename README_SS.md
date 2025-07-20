# Protein Secondary Structure Prediction (PSSP)

This repository contains code and models for **Protein Secondary Structure Prediction** using deep learning techniques like BiLSTM, CNN, and attention-based layers. Built with TensorFlow/Keras, the notebook demonstrates the full pipeline from preprocessing to evaluation using Q3 accuracy metrics.

---

## Files

| File | Description |
|------|-------------|
| `PSSP_PS4.ipynb` | Main Jupyter Notebook with code for loading data, building models, training, and evaluating Q3 performance. |

---

## Problem Statement

Develop a high-accuracy machine learning model to predict the three-state secondary structure (α-helix [H], β-sheet [E], or coil [C]) of individual amino acids in a protein using only its raw sequence data, without requiring evolutionary or homologous sequence information. The model should address key challenges in computational biology while minimizing reliance on domain specific biological knowledge.

---

## Model Architecture

- **Input**: Encoded amino acid sequences with optional physicochemical features
- **Layers**:
  - Embedding / Dense Layer
  - 1D Convolution Layer
  - Bi-directional LSTM
  - Dropout Layer
  - TimeDistributed Dense with Softmax
- **Output**: Per-residue prediction of secondary structure (Q3)

---

## Evaluation Metrics

- **Q3 Accuracy** – Overall correctness of predicted secondary structure
- **Per-Class Accuracy** – Performance on Helix (H), Sheet (E), Coil (C)

---
