✅ SMILES_Generation_and_Prediction
📌 Project Title
Comparing VAE and GAN Models for Molecular SMILES Generation and Property Prediction with GNNs

🧠 Overview
This project compares two generative deep learning models—Variational Autoencoders (VAEs) and Generative Adversarial Networks (GANs)—for generating novel molecular SMILES strings. Generated molecules are further evaluated for chemical properties using Graph Neural Networks (GCNs & GINs).

🧪 Dataset
QM9: 134,000+ small organic molecules with computed properties

Format: SMILES strings + graph structure

🔍 Problem Statement
Can deep generative models produce novel, valid, and chemically diverse molecules?
How do different generators (VAE vs. GAN) influence downstream property prediction by GNNs?

🎯 Objectives
Train VAE and GAN on QM9 for SMILES generation

Train GCN and GIN for property prediction (e.g., dipole moment)

Compare generative quality (validity, novelty, diversity) and prediction accuracy

🧰 Tech Stack
Languages: Python

Frameworks: PyTorch, PyTorch Geometric

Libraries: RDKit, DeepChem, fcd-torch, NumPy, Pandas, Seaborn

🧱 Methodology
VAE/GAN Training:

Learn molecular structure distributions

Generate new SMILES strings

Post-processing:

Filter valid molecules using RDKit

GNN Training:

Predict properties from generated molecules

Evaluate with MSE, MAE, Tanimoto similarity, and FCD

📊 Results
VAE: High validity, novelty, and smoother latent space

GAN: Strong but less diverse molecules, minor mode collapse

GNNs: GIN outperformed GCN in predictive accuracy

Best Pipeline: VAE + GIN

🧬 Evaluation Metrics
Validity Rate

Uniqueness

Novelty

Fréchet ChemNet Distance (FCD)

Tanimoto Similarity

Internal Diversity
