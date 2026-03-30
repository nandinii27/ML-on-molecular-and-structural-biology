# Computational Drug Discovery & Scientific ML — Notebooks

Hands-on notebooks covering the core methods at the intersection of cheminformatics, geometric deep learning, topological data analysis, physics-informed ML, and generative modelling for molecules.

## Notebooks

| # | Topic | Stack | What it does |
|---|-------|-------|-------------|
| 01 | **Cheminformatics** | RDKit, scikit-learn | Morgan fingerprints, Tanimoto similarity matrix, Murcko scaffold analysis, descriptor-based QSAR (Random Forest) with feature importance |
| 02 | **Topological Data Analysis** | GUDHI, RDKit | Persistent homology on 3D molecular conformers via Vietoris-Rips, persistence diagrams, Betti curves as topological fingerprints, bottleneck distance matrix |
| 03 | **Physics-Informed Neural Networks** | PyTorch | PINN solving the Fisher-KPP reaction-diffusion PDE (tumour invasion model), autograd-based PDE residual, travelling wave front recovery |
| 04 | **SE(3)-Invariant GNN** | PyTorch, RDKit | EGNN-style distance-based message passing from scratch, SO(3) rotation invariance verification, LogP prediction on drug molecules |
| 05 | **Diffusion Models** | PyTorch | DDPM for 2D molecular ring conformations, linear noise schedule, denoising score matching, reverse sampling with trajectory visualisation |

## Setup

```bash
pip install torch rdkit gudhi scikit-learn matplotlib numpy pandas jupyter
```

## Run

```bash
jupyter notebook
# or execute all:
for nb in *.ipynb; do jupyter nbconvert --to notebook --execute "$nb"; done
```

## Context

These notebooks are part of a broader research programme in geometric deep learning + topological data analysis + quantum ML for drug discovery. See the companion repo list for the full ecosystem of tools used.
