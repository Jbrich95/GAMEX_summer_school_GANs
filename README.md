# Generative Modelling for Extremes and Risk

**GAMEX - Edinburgh Summer School on Generative AI for Extremes**
**The University of Edinburgh · 8-11 September 2026** <br>
[GAMEX Summer School website](https://gamex-network.github.io/school/)

This repository contains materials for a 120-minute practical session on **Generative Modelling for Extremes and Risk** with PyTorch by [**Jordan Richards**](https://jbrich95.github.io/).
 
 The practical illustrates how to use torch to build and train a standard generative adversarial network (GAN), and compares the extrapolative properties of GANs with two extremal alternatives - EV-GAN and ExceedGAN. The original code for EV-GAN and ExceedGAN can be found at [https://github.com/michael-allouche/extreme-value-GAN](https://github.com/michael-allouche/extreme-value-GAN).
---

## Practical materials

| File | Topic | 
| --- | --- |
| [`01_standard_GAN.ipynb`](01_standard_GAN.ipynb) | Building standard GANs using torch in Python | 
| [`01_standard_GAN_R.ipynb`](01_standard_GAN_R.ipynb) | An R implementation of the first notebook |
| [`02_evGAN_vs_standard_GAN_1d.ipynb`](02_evGAN_vs_standard_GAN_1d.ipynb) | EV-GAN for univariate extremes |
| [`03_exceedgan_vs_evgan_vs_gan_bivariate.ipynb`](03_exceedgan_vs_evgan_vs_gan_bivariate.ipynb) | ExceedGAN for bivariate extremes |
| `handout.pdf` | Practical handout | 

---

## Requirements

Required software and packages:

- Python 3.11+
- PyTorch 2.10+
- NumPy
- Matplotlib
- JupyterLab
- statsmodels
- Git

Recommended softwares:

- Git
- VScode
- Anaconda or Miniforge

A **CPU is sufficient** for the practical. The current notebooks select CUDA when it is available and otherwise use CPU.

---

## Installation

Clone the repository and create a virtual environment:

```bash
git clone https://github.com/Jbrich95/GAMEX_summer_school_GANs.git
cd GAMEX_summer_school_GANs

python3 -m venv gan_ext_env
```

Activate it on macOS/Linux:

```bash
source gan_ext_env/bin/activate
```

or in Windows PowerShell:

```powershell
.\ gan_ext_env\Scripts\Activate.ps1
```

Install the required packages:

```bash
python -m pip install --upgrade pip
python -m pip install torch numpy matplotlib scipy statsmodels jupyter
```

Then launch JupyterLab:

```bash
jupyter lab
```

Open the notebooks in order:

```text
01_standard_GAN.ipynb
02_evGAN_vs_standard_GAN_1d.ipynb
03_exceedgan_vs_evgan_vs_gan_bivariate.ipynbd
```

Run the first code cell to confirm the installed PyTorch version and loaded compute device.

