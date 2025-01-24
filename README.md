# Comparison of SEI Zero-dimensional Models (in PyBaMM)

This repository contains the analysis code and results for comparing common zero-dimensional solid electrolyte interphase (SEI) models (limited mechanisms) in [PyBaMM](https://github.com/pybamm-team/PyBaMM) in lithium-ion batteries, focusing on the formation cycle and early cycles.

## Overview

The project examines various SEI growth models including:
- Reaction limited
- Solvent-diffusion limited
- EC reaction limited 
- Electron-migration limited
- Interstitial-diffusion limited
- VonKolzenberg2020

Key aspects analysed:
- SEI growth behaviour during formation cycles
- Comparison between charging and discharging periods
- Impact of C-rate on SEI growth patterns
- Model validation against experimental data

## Requirements

This code requires PyBaMM version 25.1.0 or newer. The analysis was performed using this specific version to ensure the reproducibility of the results.

## Repository Structure

- `notebooks/`
  - `Initial_soc_VS_C-rate.ipynb`: Analysis of how initial state of charge affects SEI growth
  - `sei_ch-VS-dch.ipynb`: Comparison of SEI growth during charge vs discharge cycles

## Results

The analysis reveals several key findings:
1. Models show varying degrees of accuracy in matching experimental SEI formation data
2. C-rate has minimal impact on SEI growth in most models, with the EC reaction limited model being a notable exception
3. Higher initial SOC leads to more SEI growth across all models due to longer discharge times

## Citation

If you use this code or results in your research, please cite:

```
K. Manmi, M. Tuchel, E. Kendrick, F. Brosa Planella, "A Comparison of Standard SEI Growth Models in the Context of Battery Formation", ![J. Electrochem. Soc. 171 100530](https://iopscience.iop.org/article/10.1149/1945-7111/ad8548).
```

## License

This project is licensed under the BSD-3-Clause license.

## Acknowledgments

This work was supported by The Faraday Institution "Multi-Scale Modelling" project [EP/S003053/1 grant number FIRG059].
