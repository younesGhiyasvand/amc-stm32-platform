# Validation Strategy

Version: 1.0

Status: Draft

Last Updated: 2026-06-25

---

# Objective

Define the validation methodology used for evaluating the Automatic Modulation Classification (AMC) system.

The goal is to evaluate model performance under both ideal and real-world conditions.

---

# Overview

The validation strategy is divided into two separate datasets:

- Standard Dataset (Benchmark)
- Hardware Dataset (Real-world)

This separation ensures both theoretical correctness and practical performance evaluation.

---

# Standard Dataset Validation

## Dataset

A publicly available AMC dataset will be used:

- RadioML XXXX.XX
- RadioML XXXX.XX
- RadioML XXXX.XX

---

## Purpose

- Model training
- Baseline performance evaluation
- Comparison with existing research

---

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- Confusion Matrix
- F1 Score

---

## Expected Outcome

High accuracy under controlled and clean simulation conditions.

---

# Hardware Dataset Validation

## Dataset Source

Real signals generated using the developed AMC hardware platform:

- STM32 TX/RX boards
- DAC and ADC interface board
- Analog transmission channel

---

## Purpose

- Evaluate real-world performance
- Measure robustness to hardware imperfections
- Validate generalization capability

---

## Characteristics

- Noise from analog components
- Clock jitter effects
- ADC quantization effects
- Channel distortions

---

## Evaluation Metrics

Same metrics as standard dataset:

- Accuracy
- Precision
- Recall
- Confusion Matrix
- F1 Score

---

# Comparison Strategy

The main research contribution is based on comparison between:

Standard Dataset Performance

VS

Hardware Dataset Performance

---

# Analysis Goals

- Measure performance degradation in real conditions
- Identify sensitivity to noise and hardware impairments
- Evaluate robustness of feature extraction methods
- Compare classifier generalization capability

---

# Final Decision

The AMC system will be validated using both simulated standard datasets and real-world hardware-generated datasets.

The comparison between these two domains will serve as a key evaluation metric for the project and potential publication.