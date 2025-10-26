# Session 3 — Inference and Causality

This repository contains the materials for **Session X** of *Course Y*.  
- Slides: see [`slides/`](./slides/) folder  
- Notebooks: see [`notebooks/`](./notebooks/) folder 
---

## 📑 Session Outline
---

## Overview
This week transitions from **discrete Bayesian reasoning** (cookies, dice, Monty Hall)  
to **continuous inference**, **Fisher Information**, and finally to **sampling-based inference** using **Markov Chain Monte Carlo (MCMC)**.

We ask:
> What happens when we can no longer count outcomes — or integrate analytically?

---

## Learning Goals

- Move from **discrete** to **continuous** Bayesian reasoning  
- Understand **conjugate priors** and when they simplify updating  
- Quantify **information** in data through Fisher Information  
- Grasp the motivation behind **Monte Carlo** and **MCMC** methods  
- Build intuition for sampling as an approximation to integration

---

## Notebooks

| # | Notebook | Topic | Description |
|---|-----------|--------|--------------|
| 1 | `1_InferenceAndCausality_Week2_ContinuousBayes.ipynb` | **Continuous Bayes** | From discrete Bayes to continuous updates. Introduces density-based posteriors, expectations, and credible intervals. |
| 2 | `2_InferenceAndCausality_Week2_FisherInformation.ipynb` | **Fisher Information** | Explores how the curvature of the log-likelihood reflects the precision of our estimates. Includes a Think Bayes–style interactive notebook. |
| 3 | `3_InferenceAndCausality_Week2_Distributions.ipynb` | **Conjugate Priors** | Review and glossary of common likelihood–prior pairs (Beta–Binomial, Gamma–Poisson, Normal–Normal). Includes a short “Conjugate Match Game.” |
| 4 | `4_InferenceAndCausality_Week2_MCMC_analogy.ipynb` | **MCMC Analogy** | Introduces Markov Chain Monte Carlo through an intuitive analogy (random walker). Students visualize how MCMC “samples” from a posterior. Ends with a reflection question. |

---

## Recommended Flow

1. **Notebook 1** — run through the “Guess the Coin” example  
2. **Notebook 2** — explore Fisher Information interactively  
3. **Notebook 3** — identify conjugate pairs and connect to Bayesian updating  
4. **Notebook 4** — play with the MCMC analogy and answer the reflection question

---

## Materials

Slides for this week:  
`/slides/Inference_and_Causality_W2_Statistical_Inference.pdf`

Additional readings:  
- Allen Downey, *Think Bayes 2*, Chapters 3–4  
- Wikipedia: [Conjugate prior](https://en.wikipedia.org/wiki/Conjugate_prior)  
- Stan & PyMC documentation on [MCMC basics](https://docs.pymc.io/en/latest/)

---

## Homework

- Complete the exercises in **Notebook 1**, **2**, and **4**  
- Commit your answers to GitHub before submission  
- Reflect: *What’s the main trade-off between analytical and sampling-based inference?*


---
## 🚀 Environment Setup

Before starting, please **fork this repository** and create a fresh Python virtual environment.  
All required libraries are listed in `requirements.txt`.

> ⚠️ If you encounter errors during `pip install`, try removing the version pinning for the failing package(s) in `requirements.txt`.  
> On Apple M1/M2 systems you may also need to install additional system packages (the “M1 shizzle”).

---

### macOS / Linux (bash/zsh)

```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate

# Upgrade pip and install dependencies
pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (PowerShell)
```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
.venv\Scripts\Activate.ps1

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (Git Bash)
```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/Scripts/activate

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

You’re now ready to run the session notebooks!

Deactivate the environment when you’re done:
```bash
deactivate
```
