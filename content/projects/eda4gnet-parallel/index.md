---
title: "Enhancing Computational Performance of EDA4GNet Through Parallel Processing"
summary: "Computational performance study on EDA4GNet smart grid intrusion detection — achieved 3.34x speedup via multiprocessing on IEC 61850 GOOSE traffic. Currently enhancing detection performance toward conference publication."
tags:
- Parallel Processing
- Network Security
- Anomaly Detection
- Smart Grid
- IEC 61850
- Python
- Performance Optimisation
date: "2025-12-01T00:00:00Z"
external_link: ""
image:
  caption: ""
  focal_point: Smart
links: []
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""
---

## Overview

Final Year Project (BSc Computer Science — Networks, UiTM) investigating computational bottlenecks in EDA4GNet, an anomaly detection system for IEC 61850 smart grid networks, and resolving them through parallel processing architecture.

## Problem Statement

EDA4GNet monitors IEC 61850 station bus traffic for GOOSE message attacks. The sequential processing architecture created bottlenecks when handling large volumes of GOOSE messages, compromising real-time detection capability at industrial scale.

## Objectives

- Design parallel processing models for EDA4GNet — threading, multiprocessing, and hybrid approaches
- Develop and implement each model
- Evaluate computational effectiveness using three metrics: speedup factor, throughput, and CPU utilisation

## Methodology

Based on the CRISP-DM framework adapted for network traffic analysis:

- **Data:** ERENO dataset (2,305,746 records, 9 classes)
- **Baseline:** EDA4GNet with ARFIMA + State-Space AR implementation
- **Parallel models:** Three approaches designed and implemented — threading, multiprocessing, hybrid
- **Evaluation:** Four progressive stages — Proof of Concept, Algorithm Refinement, Performance Validation, Production Evaluation

## Results

| Approach | Speedup Factor | Throughput (samples/sec) | CPU Utilisation |
|---|---|---|---|
| Sequential | 1.00x | 214.09 | 24.10% |
| Threading | 0.834x | 178.62 | 28.70% |
| **Multiprocessing** | **3.34x** | **715.15** | **89.40%** |
| Hybrid | 2.30x | 492.84 | 76.80% |

**Detection accuracy preserved at 85.92%** across all parallel implementations.

Total experimental runtime: 98+ hours of real-time validation.

## Key Findings

- Multiprocessing achieved the highest speedup (3.34x) by leveraging CPU-bound parallelism for ARFIMA calculations and EM algorithm operations
- Threading underperformed due to Python GIL limitations on CPU-intensive tasks
- Hybrid approach provided a balance between speedup and resource usage
- Industrial-scale validation confirmed real-time processing capability

## Significance

- Quantitative benchmarks established for future EDA4GNet research
- Demonstrated industrial relevance for smart grid cybersecurity
- Contributed multi-scale validation methodology

## Future Work

- GPU acceleration implementation
- Distributed computing architecture
- Real-world smart grid deployment

## Status

Core parallel processing study completed as part of BSc FYP (UiTM, 2025). Currently 
undertaking enhancement work targeting improved detection performance. 
Conference publication planned upon completion.