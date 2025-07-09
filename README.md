🧠 UMAP Clustering of Neuron Types
This repository contains a Jupyter notebook that performs clustering of primary visual cortex neurons using single-cell RNA-seq data from the Allen Institute. The goal is to visualize neuronal diversity and identify transcriptionally distinct neuron subtypes using unsupervised learning.

📊 Project Summary
This notebook walks through a complete pipeline to:

Load and filter neuron-level transcriptomic data from the Allen Mouse Whole Cortex + Hippocampus dataset

Preprocess expression data (log normalization, HVG selection)

Perform dimensionality reduction (PCA)

Generate UMAP embeddings

Cluster neurons using the Leiden algorithm

Identify and visualize marker genes for each cluster

🔬 Dataset
The dataset used is:

Mouse Whole Cortex + Hippocampus 10x Dataset from the Allen Brain Atlas

We subset the data to ~29,000 neurons specifically from the Primary Visual Cortex (VISp).

🧮 Analysis Workflow
Load Data: Expression matrix and cell metadata (filtered to neurons in VISp)

Preprocessing: Normalization, log transformation, highly variable gene (HVG) selection

PCA: Reduce high-dimensional data to 50 principal components

UMAP: Embed neurons in 2D space based on transcriptomic similarity

Leiden Clustering: Discover transcriptionally distinct subtypes

Marker Gene Analysis: Validate clusters against known subclass annotations


📁 Repository Structure
kotlin
Copy
Edit
📦UMAP_Clustering_NeuronTypes
 ┣ 📜UMAP_Clustering_NeuronTypes.ipynb
 ┣ 📜README.md
 ┗ 📂data/
     ┣ 📜X_hip.h5ad
     ┗ 📜metadata.csv
🧠 Author
Kiranmayi Vedantham
PhD in Computational Neuroscience | Patch-seq, scRNA-seq, and Machine Learning for Brain Cell Type Discovery
