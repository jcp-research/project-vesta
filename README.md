# Project Vesta

Project Vesta is an exploratory research project studying operator-spectral diagnostics for transformer attention dynamics.

The core idea is to extract attention matrices from transformer models, convert them into symmetric surrogate operators, and analyze their eigenvalue spectra, spectral gaps, and layer/head perturbation patterns.

This project is currently exploratory. It does not claim that transformers are quantum systems or that spectral gaps directly encode semantic truth. The goal is to test whether operator-theoretic signatures can reveal meaningful internal structure in transformer computation.

---

## Current Experiment

Model: DistilGPT2

Method:

1. Extract attention matrix A
2. Construct symmetric surrogate operator:

   H = 1/2(A + A^T)

3. Compute eigenvalues and spectral gap
4. Track layer-wise and head-wise spectral behavior
5. Compare coherent vs corrupted prompts

---

## Preliminary Findings

Current experiments suggest:

- spectral gaps vary across transformer layers
- later layers show stronger mean spectral organization
- perturbing semantic coherence produces localized spectral changes
- some heads appear more spectrally sensitive than others

These findings are preliminary and require further testing.

---

## Repository Structure

- `notebooks/` — Colab notebooks and experiments
- `papers/` — exploratory writeups and PDFs
- `figures/` — plots and heatmaps
- `notes/` — research notes and definitions

---

## Status

Early exploratory research.
