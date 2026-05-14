# Brain-to-Language Neural Decoding

A machine learning pipeline for decoding semantic information from neuroimaging signals using BERT, CLIP embeddings, and Ridge Regression.

This project explores how brain activity patterns can be mapped to language representations by learning relationships between neuroimaging data and semantic embeddings.

---

# Overview

The project focuses on neural decoding — predicting semantic meaning from brain activity signals.

Using neuroimaging datasets and pretrained language/vision embeddings, the pipeline learns mappings between:

* Neuroimaging signals
* CLIP/BERT semantic embeddings
* Natural language representations

The system uses regression-based models to reconstruct semantic embeddings from brain activity and retrieve semantically similar captions.

---

# Features

* Neuroimaging-to-language decoding pipeline
* CLIP and BERT embedding integration
* Ridge Regression based semantic mapping
* Support for high-dimensional voxel-level brain signals
* Similarity-based semantic retrieval using cosine similarity
* ROI-based weight analysis and compression
* Train/test evaluation on neuroimaging datasets

---

# Tech Stack

* Python
* PyTorch
* NumPy
* Pandas
* Scikit-learn
* CLIP Embeddings
* BERT Embeddings
* Ridge Regression
* Neuroimaging Data Processing

---

# Dataset

The project was developed using:

* Algonauts NSD Dataset
* Neuroimaging (fMRI) recordings
* CLIP image/text embeddings
* Caption-based semantic representations

The datasets contain:

* Brain activity recordings
* Image-caption pairs
* Semantic text embeddings
* Voxel-level neural responses

---

# Pipeline

## 1. Data Loading

* Load neuroimaging data
* Load CLIP/BERT embeddings
* Perform train-test split

## 2. Preprocessing

* Normalization using MinMaxScaler
* Feature scaling
* Embedding preparation
* Voxel-level signal formatting

## 3. Model Training

Train Ridge Regression models to learn mappings between:

* Brain activity → semantic embeddings

Separate models are trained for:

* Left hemisphere
* Right hemisphere

---

# Semantic Retrieval

Predicted embeddings are compared against training embeddings using cosine similarity.

The closest semantic match is retrieved as the predicted sentence representation.

---

# ROI Analysis

The project also includes Region-of-Interest (ROI) based weight analysis:

* Visual ROI grouping
* Weight compression
* Brain-region contribution analysis
* Feature importance exploration

---

# Results

* Successfully reconstructed semantic representations from neuroimaging signals
* Achieved low reconstruction error using Ridge Regression
* Retrieved semantically meaningful captions from predicted embeddings
* Demonstrated brain-to-language semantic decoding using ML methods


