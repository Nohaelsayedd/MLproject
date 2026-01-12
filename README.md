# Fruit and Vegetable Classification using Hierarchical Machine Learning

## Project Overview
This project implements a **hierarchical machine learning system** designed to classify images of fruits and vegetables using a two-stage decision pipeline. Instead of a single "flat" classifier, this system separates feature extraction from classification to allow for a detailed comparison of different machine learning models.

The pipeline operates in two stages:
1. **Stage 1 (Binary):** Determines if the input is a "Fruit" or a "Vegetable."
2. **Stage 2 (Multi-class):** Classifies the image into its specific type (e.g., Apple, Mango, Carrot) based on the result of Stage 1.

**Key Goals:**
* Distinguish between fruits and vegetables accurately.
* Identify the specific type within the predicted category.
* Compare multiple ML models (Decision Trees, Random Forests, XGBoost,KNNs,SVM and ANNs) using the same high-level features.


## Dataset
The dataset consists of labeled images organized into training, validation, and test splits.

* **Main Categories:** Fruit and Vegetable.
* **Source:** [Kaggle: Fruit and Vegetable Image Recognition Dataset](https://www.kaggle.com/datasets/kritikseth/fruit-and-vegetable-image-recognition).

**Note:** The dataset is not included in this repository due to its large size. You must download it manually and place it in the root directory.

### Directory Structure
```text
Project Root
├── notebooks/          # Training and analysis notebooks
├── train/              # Training images
│   ├── fruit/
│   └── vegetable/
├── validation/         # Validation images
├── test/               # Test images
│   ├── fruit/
│   └── vegetable/
└── venv/               # Virtual environment (ignored)
