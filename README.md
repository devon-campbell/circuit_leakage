# Quantum Circuit/State Leakage Analysis

This repository contains two Jupyter notebooks for analyzing **quantum state leakage** and **syndrome correlations** in IBM Quantum experiments.

## Files
Navigate to `state_leakage`:
* **`circ_leakage.ipynb`** — Prepares and runs Qiskit-based circuits to probe state leakage across different programs and devices. It records shot-level measurement data (`syndrome_Z`, `syndrome_X`, etc.) for later analysis.
* **`analysis.ipynb`** — Loads the recorded CSV data and performs statistical analysis of leakage signatures, syndrome correlations, and phase dependence.

## Requirements

Install dependencies:

```bash
pip install qiskit qiskit-aer pandas polars matplotlib numpy tqdm
```

## Usage

1. Run `circ_leakage.ipynb` to generate or upload experimental results.
2. Run `analysis.ipynb` to process the output and visualize leakage trends.

## Output

Results are written under `out_program_leakage/`, including per-shot CSV logs and aggregated plots of leakage probabilities.
