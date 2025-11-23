# PPG-Based Glucose Prediction using Machine Learning enhanced by EMD and IMF

## Overview

This repository contains thesis work on **Photoplethysmography (PPG) Signal Processing for Glucose Level Prediction** using advanced machine learning techniques combined with signal decomposition methods. The project explores the relationship between PPG signals and blood glucose levels using Empirical Mode Decomposition (EMD) and Intrinsic Mode Functions (IMF) for feature extraction.

## Project Objectives

- Extract meaningful features from PPG signals using EMD/IMF decomposition techniques
- Develop and compare multiple machine learning models for glucose prediction
- Analyze the relationship between PPG signal characteristics and glucose levels
- Implement robust signal processing pipelines for real-world applications

## Repository Structure

```
PPG-Glucose-ML-EMD-IMF/
├── Model/                           # Trained models directory
├── trials/                          # Experimental trials and variations
├── README.md                        # This file
├── LICENSE                          # MIT License
└── Visualization outputs/           # Generated plots and results
    ├── CB.png, CE_CB.png, CE_RF.png
    ├── LGB.png, RF.png, XGB.png
    ├── top30imf.png, top50imf.png, top30_imf+general.png
    ├── Red_imf.png, org+sumIMF.png
    └── output.png, output2.png, output3.png, output4.png, output5.png
```

## Dataset

The project utilizes PPG signal data along with corresponding glucose measurements. The dataset is stored in the `Data/` directory and includes:
- Raw PPG signal samples
- Preprocessed signal data
- Corresponding glucose level annotations

**Note:** Data is restricted and not included in the repository.

## Methodology

### 1. Signal Processing
- **Empirical Mode Decomposition (EMD)**: Decomposes PPG signals into Intrinsic Mode Functions (IMF)
- **Feature Extraction**: Top 30-50 IMF components are selected based on importance
- **Preprocessing**: Signal normalization and noise filtering

### 2. Machine Learning Models Implemented

The project evaluates and compares the following algorithms:

| Model | Abbreviation | Status |
|-------|--------------|--------|
| Gradient Boosting | GB/LGB | ✓ |
| Extreme Gradient Boosting | XGB | ✓ |
| Random Forest | RF | ✓ |
| CatBoost | CB | ✓ |
| Ensemble Methods | CE_CB, CE_RF | ✓ |

### 3. Performance Evaluation

Models are evaluated using:
- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- R² Score
- Cross-validation metrics

## Key Findings

Visualization outputs demonstrate:
- Comparison of model performances across different metrics
- IMF decomposition analysis and feature importance rankings
- Prediction accuracy results for various ensemble combinations
- Signal preprocessing and transformation visualizations

## Technologies & Libraries

- **Python 3.x**
- **Jupyter Notebook**: Interactive development and analysis
- **NumPy & Pandas**: Data manipulation and analysis
- **Scikit-learn**: Machine learning algorithms
- **LightGBM, XGBoost, CatBoost**: Gradient boosting frameworks
- **Matplotlib & Seaborn**: Data visualization
- **EMD (Empirical Mode Decomposition)**: Signal processing

## Installation & Setup

### Prerequisites
- Python 3.7 or higher
- Jupyter Notebook
- pip or conda package manager

### Required Packages

```bash
pip install numpy pandas scikit-learn lightgbm xgboost catboost matplotlib seaborn jupyter
```

### Running the Project

1. Clone or download the repository
2. Navigate to the repository directory
3. Open Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Open the main notebook file to view the complete analysis
5. Run the cells sequentially to reproduce results

## Experimental Trials

The `trials/` directory contains multiple experimental iterations including:
- Trial #1: Initial model implementations
- Trial #2: Variations with different feature sets (copies 1-2)
- Trial #3: Optimized ensemble methods and final implementations (copies 1-7)

Each trial represents an iterative refinement of the approach and hyperparameter tuning.

## Results & Visualizations

The repository includes comprehensive visualization outputs showing:

- **Model Comparisons**: CB.png, LGB.png, XGB.png, RF.png
- **Ensemble Performance**: CE_CB.png, CE_RF.png
- **Feature Analysis**: top30imf.png, top50imf.png, top30_imf+general.png
- **Signal Decomposition**: Red_imf.png, org+sumIMF.png
- **Prediction Results**: output.png, output2.png, output3.png, output4.png, output5.png

### Model Performance Comparisons

The repository includes comprehensive visualization outputs showing model performance, feature analysis, and signal decomposition:

#### CatBoost Performance
![CatBoost Results](CB.png)

#### LightGBM Performance
![LightGBM Results](LGB.png)

#### XGBoost Performance
![XGBoost Results](XGB.png)

#### Random Forest Performance
![Random Forest Results](RF.png)

### Ensemble Methods

#### CatBoost Ensemble
![CatBoost Ensemble](CE_CB.png)

#### Random Forest Ensemble
![Random Forest Ensemble](CE_RF.png)

### Feature Analysis & Importance

#### Top 30 IMF Features
![Top 30 IMF](top30imf.png)

#### Top 50 IMF Features
![Top 50 IMF](top50imf.png)

#### Top 30 IMF + General Features
![Top 30 IMF + General](top30_imf+general.png)

### Signal Decomposition Analysis

#### Red IMF Decomposition
![Red IMF](Red_imf.png)

#### Original + Sum IMF
![Original + Sum IMF](org+sumIMF.png)

### Prediction Results

#### Output Result 1
![Output 1](output.png)

#### Output Result 2
![Output 2](output2.png)

#### Output Result 3
![Output 3](output3.png)

#### Output Result 4
![Output 4](output4.png)

#### Output Result 5
![Output 5](output5.png)

## License

This project is licensed under the **MIT License**. See the `LICENSE` file for more details.

## Author

**Name:** Shama Satter  
**Email:** [shamasatter@gmail.com](mailto:shamasatter@gmail.com)  
**ORCID iD:** [0000-0002-9357-4286](https://orcid.org/0000-0002-9357-4286)  
**GitHub:** [https://github.com/shamasatter](https://github.com/shamasatter)  
**LinkedIn:** [https://www.linkedin.com/in/shamasatter](https://www.linkedin.com/in/shamasatter)

## Contact & Contributions

For questions, suggestions, or contributions related to this thesis work, please contact shamasatter@gmail.com or reach out through the repository's issue tracker.
