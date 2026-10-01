# Tumor-aware Pix2Pix for gadolinium-free T1ce synthesis (BraTS 2021)

Code and final result tables for the paper "Mask-Guided Discriminator
Conditioning for Tumor-Aware Pix2Pix Synthesis of Gadolinium-Free
T1-Contrast-Enhanced MRI on BraTS 2021".

## Contents
- `pipeline_tumor_aware_pix2pix.ipynb`: full pipeline (preprocessing,
  Pix2Pix with U-Net generator, stabilization recipe, tumor-aware
  discriminator, evaluation).
- `resultados_test_final_4variantes.csv`, `resumen_test_final.csv`,
  `comparacion_peso_3.0_vs_1.5.csv`: final test-set results reported in
  the paper (per-seed values, summary, and kappa sensitivity).

## Data
BraTS 2021 is not redistributed here. Download it from the official
source (RSNA-ASNR-MICCAI) and set the data path in the notebook.

## Reproduce
Open the notebook in Google Colab (T4 GPU), set the data path, and run
all cells. Seeds used: 42, 123, 2024.

## Variants
Baseline, Stabilized, TA-Disc, TA-Disc+SSIM+Freq.

## License
MIT
