# 🧪 SMILES Generation and Property Prediction using Deep Learning

## 📌 Project Title
**Comparing VAE and GAN Models for Molecular SMILES Generation and Property Prediction with GNNs**

## 🧠 Overview
This project explores the use of deep generative models—**Variational Autoencoders (VAEs)** and **Generative Adversarial Networks (GANs)**—to generate novel molecular structures represented as **SMILES strings**. These generated molecules are evaluated using **Graph Neural Networks (GCNs and GINs)** for chemical property prediction.

---

## 🧪 Dataset
- **QM9**: A widely used benchmark dataset with **134,000+** small organic molecules.
- **Format**: SMILES strings (for generation) + molecular graphs (for prediction).

---

## 🔍 Problem Statement
1. Can deep generative models produce **valid, novel, and chemically diverse** molecules?
2. How do different generators (VAE vs. GAN) influence downstream property prediction using GNNs?

---

## 🎯 Objectives
- Train **VAE** and **GAN** models on QM9 for molecular generation.
- Train **GCN** and **GIN** models to predict molecular properties (e.g., dipole moment).
- Compare:
  - Generative quality (validity, uniqueness, novelty, diversity).
  - Prediction accuracy (MAE, MSE, etc.).

---

## 🧰 Tech Stack
- **Languages**: Python
- **Frameworks**: PyTorch, PyTorch Geometric
- **Libraries**: RDKit, DeepChem, NumPy, Pandas, Seaborn, `fcd-torch`

---

## 🧱 Methodology

### 🔄 VAE / GAN Training
- Learn underlying distributions of molecular structures
- Generate SMILES strings from latent space or adversarial learning

### 🧹 Post-processing
- Use **RDKit** to validate generated molecules
- Remove syntactically or chemically invalid outputs

### 🔬 GNN Training
- Train **GCN** and **GIN** models to predict molecular properties
- Evaluate predictions using:
  - MSE (Mean Squared Error)
  - MAE (Mean Absolute Error)
  - Tanimoto similarity
  - FCD (Fréchet ChemNet Distance)

---

## 📊 Results Summary
| Model | Highlights |
|-------|------------|
| **VAE** | High validity, novelty, and a well-organized latent space |
| **GAN** | Good molecule quality but lower diversity (mode collapse observed) |
| **GIN** | Outperformed GCN in property prediction accuracy |
| **Best Pipeline** | **VAE + GIN** |

---

## 🧬 Evaluation Metrics
- ✅ Validity Rate
- 🎯 Uniqueness & Novelty
- 🔁 Internal Diversity
- 🧠 Tanimoto Similarity
- 📈 Fréchet ChemNet Distance (FCD)

---
