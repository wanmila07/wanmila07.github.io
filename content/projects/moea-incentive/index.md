---
title: "Multi-Objective Evolutionary Algorithm for Informal Business Incentive Distribution"
summary: "PhD research project developing a MOEA with adaptive operators to solve the NP-hard problem of incentive allocation among informal sector SMEs, using World Bank enterprise survey data."
tags:
- Evolutionary Optimisation
- Multi-Objective Optimisation
- NSGA-II
- Python
- Operations Research
- Decision Support
date: "2026-03-18T00:00:00Z"
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

This project is the computational core of my PhD thesis, addressing the NP-hard problem of distributing limited government incentives among informal sector businesses in a fair, efficient, and sustainable manner.

## Problem Statement

Informal sector SMEs form a significant portion of developing economies but are frequently excluded from formal incentive programmes due to the lack of systematic allocation frameworks. Distributing limited incentives across thousands of businesses with heterogeneous needs and constraints is a combinatorial optimisation problem that cannot be solved optimally by traditional methods at scale.

## Approach

A Multi-Objective Evolutionary Algorithm (MOEA) with adaptive operators was developed to simultaneously optimise three competing objectives:

- Efficiency: maximising economic impact per incentive unit
- Equity: ensuring fair distribution across business segments
- Sustainability: prioritising businesses with long-term viability

Key algorithmic contributions:

- Adaptive operator selection mechanism that dynamically adjusts crossover and mutation rates based on population diversity
- Constraint handling for budget limits, eligibility criteria, and minimum allocation thresholds
- Pareto front generation enabling policy-makers to explore trade-off solutions

## Dataset

World Bank Indonesian Survey of Informal Sector Enterprises (ISES 2023) - 5,352 enterprises, 191 variables covering business characteristics, financial performance, access to services, and growth indicators.

## Technical Stack

- Core Algorithm: Python (NumPy, SciPy)
- Data Processing: Pandas, Pathlib
- Statistical Analysis: SciPy (Mann-Whitney U, Kruskal-Wallis, Spearman correlation, Bonferroni)
- ML Components: Scikit-learn, Keras
- Visualisation: Matplotlib, Plotly
- API Layer: FastAPI
- Dashboard: Streamlit

## Status

Algorithm development and experimental evaluation complete. Manuscript under review. Dashboard and API layer in active development.

## Research Output

- PhD Thesis: Multi-Objective Evolutionary Algorithm with Adaptive Operators for Informal Business Incentive Distribution Modelling (completed, pending submission)
- Journal manuscript under review