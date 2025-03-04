# Celestial Object Detection

Built a machine learning model to classify celestial objects as **stars**, **galaxies**, or **quasars** using astronomical survey data. The project combines exploratory analysis and supervised learning to assist astronomers in identifying object types based on photometric and spectroscopic measurements.

## Project Overview

This project applies machine learning techniques to classify celestial objects by analyzing their physical properties, such as redshift, magnitudes, and spectral data. Accurate classification of celestial objects supports research in astronomy and enables automated processing of large-scale sky surveys.

## Dataset

The dataset consists of spectroscopic and photometric measurements, with features including:
- Right Ascension (`ra`)
- Declination (`dec`)
- Magnitudes (`u`, `g`, `r`, `i`, `z`)
- Redshift (`redshift`)
- Instrument-related identifiers (e.g., `plate`, `mjd`, `fiberid`)

The target variable is:
- **Class** (Galaxy, Star, Quasar)

## Objectives

- Analyze and clean astronomical data to prepare for machine learning.
- Explore feature importance and class distributions.
- Build predictive models to classify celestial objects.
- Evaluate model performance and recommend the optimal algorithm.
- Provide insights into which features most significantly influence classification.

## Methods

- Data cleaning and preprocessing (removing redundant IDs, handling irrelevant features).
- Exploratory Data Analysis (EDA) to assess distributions, correlations, and feature relationships.
- Dimensionality reduction using **Principal Component Analysis (PCA)**.
- Classification using:
  - **k-Nearest Neighbors (kNN)**
  - **Decision Tree Classifier**
- Model evaluation with:
  - Confusion matrices
  - Classification reports (accuracy, precision, recall, F1-score)
  - **K-Fold Cross-Validation**

## Results

- Achieved **over 90% accuracy** using a **Decision Tree Classifier**.
- Identified **redshift** as the most important feature for distinguishing object classes.
- Decision Trees outperformed kNN in both efficiency and accuracy on this dataset.
- PCA improved computational efficiency while preserving essential variance.
- Visualized feature importance and decision boundaries, supporting explainability for astronomical applications.

## Business/Scientific Impact

- Automates the classification of celestial objects to assist astronomers in large-scale sky surveys.
- Provides an interpretable model (Decision Tree) suitable for integration into existing astronomical workflows.
- Demonstrates that machine learning can reinforce domain-specific knowledge, such as the significance of redshift in classifying galaxies and quasars.

## Technologies Used

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

## How to Run

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/celestial-object-detection.git
    ```

2. Install required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```

4. Open and run the notebook to reproduce the results.
