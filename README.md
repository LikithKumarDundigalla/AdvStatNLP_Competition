# Author Identification Task

This repository contains code and instructions for solving the class competition task of identifying whether two spans of text are authored by the same person.

## Requirements

### Dependencies
Ensure you have the following Python libraries installed:
- `pandas`
- `scikit-learn`
- `numpy`
- `jupyter`
- `matplotlib`
- `tensorflow`
- `textstat`
- `re`

Install the required libraries using:
```bash
pip install pandas numpy scikit-learn re matplotlib tensorflow jupyter
```
# Repository Structure

```bash
.
├── train.csv                           # Training dataset
├── test.csv                            # Test dataset
├── submission.csv                      # Predicted output for test dataset
├── NLP_Competition_FinalCode.ipynb     # Jupyter notebook with the full code
└── README.md                           # Instructions for installation and running the code
```

## Running the Code

### Step 1: Open the Jupyter Notebook

Launch Jupyter Notebook using:

```bash
jupyter notebook
```

### Step 2: Open notebook.ipynb
Navigate to the directory containing this project and open notebook.ipynb.

### Step 3: Follow the Steps in the Notebook

#### 1. Load the Datasets
- Import **train.csv** and **test.csv** into your notebook.

#### 2. Execute the Notebook Step-by-Step
Follow the steps below to complete the task:
- Load the datasets: 
  - Import ```train.csv``` and ```test.csv```
- Perform Exploratory Data Analysis (EDA)
  - Analyze the dataset, including:
    - Document length and word count distributions.
    - Visualizations of data properties such as histograms for text length and word counts. 
- Feature Extraction
  - Use TF-IDF vectorization and stylometric features for text preprocessing and representation.
  - Combine features for model input.
- Model Training
  - Train a neural network with:
    - Input: Combined features from TF-IDF and stylometry.
    - Architecture: Dense layers with a ReLU activation function and dropout for regularization.
    - Optimizer: Adam optimizer with binary cross-entropy loss.
- Model Validation
  - Evaluate the model using an F1 score and accuracy on the validation set.
- Generate Predictions
  - Use the trained model to generate predictions for the test dataset.
  - Save predictions in `submission.csv`.
---
Make sure to run all the cells in the notebook sequentially and verify the outputs.

### Step 4: Check Output
The predictions for the test data will be saved in `submission.csv` in the required format for the competition
