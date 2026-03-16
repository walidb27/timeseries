# Time Series Classification on LSST

This repository contains our deep learning experiments on the **LSST** multivariate time-series classification dataset from the **UEA/UCR archive**.  
The project compares several neural architectures trained **from scratch** under a shared experimental setup:

- **LSTM baseline**
- **Deeper LSTM**
- **Class-weighted LSTM**
- **1D CNN**
- **Transformer**

The goal is to study how recurrent, convolutional, and attention-based models behave on a **short, multivariate, and imbalanced** time-series classification task.

## Authors

- **Mathys Pordié**
- **Walid Bel Adef**

## Repository

GitHub repository: [walidb27/timeseries](https://github.com/walidb27/timeseries)

---

## Project Overview

Although the initial assignment mentioned adapting a foundation model, the implementation in this repository focuses on a fair comparison between several supervised models trained from scratch.

The **Transformer** is therefore presented as the **strong competitor**, while the **1-layer LSTM** serves as the **decent baseline**.

The dataset used is **LSST**, a multivariate time-series benchmark with:

- **2,459 training samples**
- **2,466 test samples**
- **36 time steps**
- **6 channels**
- **14 classes**

Because the dataset is **imbalanced**, we evaluate models with both:

- **Accuracy**
- **Macro-F1**

---

## Repository Structure

```text
timeseries/
├── lsst_CNN_1D.ipynb
├── lsst_lstm_base_.ipynb
├── lsst_lstm_compromis.ipynb
├── lsst_lstm_desequilibre.ipynb
├── lsst_Transformer.ipynb
├── report_timeseries.pdf
└── README.md
