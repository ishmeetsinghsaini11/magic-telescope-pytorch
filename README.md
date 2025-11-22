# MAGIC Gamma Telescope — Gamma Particle Classification

A concise PyTorch project for **gamma vs hadron** particle classification using the MAGIC Gamma Telescope dataset.

## Overview

This repository contains a **simple baseline neural network** trained on tabular astrophysical features to distinguish:

* **Gamma-ray events (signal)**
* **Hadronic cosmic-ray events (background)**

## What’s Included

* Data loading & preprocessing
* Train/test split
* Feature scaling
* A small PyTorch MLP model
* Training + evaluation (loss & accuracy)

## Dataset

Download the dataset manually from the official UCI Machine Learning Repository:

**MAGIC Gamma Telescope Dataset:** [https://archive.ics.uci.edu/dataset/159/magic+gamma+telescope](https://archive.ics.uci.edu/dataset/159/magic+gamma+telescope)

The raw data file is named **`magic.04.data`** on the UCI page — download that file and place it in your project folder (suggested path: `data/magic.04.data`).

The dataset contains 10 numeric features plus the class label (g/h). Example feature names: fLength, fWidth, fSize, fConc, fAlpha, fDist, etc.

### Quick load example

## How to Run

1. Download the MAGIC Gamma dataset separately (not included in this repository).
2. Place the dataset file in the project folder (for example: `data/magic.csv`).
3. Update the notebook path to load your local dataset:

```python
df = pd.read_csv('magic04.data')
```

4. Install dependencies:

```bash
pip install -r requirements.txt
```

5. Open and run the notebook:

```bash
jupyter notebook Magic_Model_pynb.ipynb
```

## Requirements

```text
torch
numpy
pandas
scikit-learn
matplotlib
seaborn
```

## Notes

This project is a **basic baseline**, not a full end‑to‑end pipeline. Ideal for beginners exploring ML on astrophysics data.
