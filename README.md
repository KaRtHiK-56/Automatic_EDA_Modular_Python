# Data Preprocessing library

## Introduction

Data preprocessing is a crucial step in any data analysis, machine learning, or data science project. It involves preparing raw data to improve the quality and reliability of results. This toolkit provides a comprehensive set of Python scripts to handle various preprocessing tasks such as handling missing values, detecting and managing outliers, scaling/standardizing data, encoding categorical data, and converting Colab notebooks to PDF. The toolkit is designed to be interactive, giving users the flexibility to choose specific actions for each column in their dataset.

## Problem Statement

Raw data often contains inconsistencies, missing values, outliers, and varying data types that can hinder analysis and modeling. These issues can lead to biased, incorrect, or incomplete results. Handling these challenges manually can be time-consuming and error-prone. Some of the common problems include:

- **Missing Values:** Missing or null values can disrupt analysis and lead to inaccuracies.
- **Outliers:** Outliers can skew the results and impact the performance of machine learning models.
- **Scaling/Standardizing Data:** Different scales of numeric features can affect model training and performance.
- **Encoding Categorical Data:** Categorical variables need to be transformed into numerical representations to be used in models.

## Solution Overview

This toolkit offers interactive Python scripts to automate preprocessing tasks, allowing users to select how each column should be processed, thus maintaining control and flexibility. Below is a summary of the key functionalities:

### 1. Handling Missing Values

**Problem:** Missing data can lead to inaccurate models and skewed analysis.

**Solution:** This script provides options to fill missing values using different strategies such as mean, median, mode, or leaving them unchanged. It helps ensure the dataset remains intact and consistent.

**Script Features:**
- Identifies columns with missing values.
- Provides user options to fill missing data or skip the column.

### 2. Handling Outliers

**Problem:** Outliers can distort the overall picture of the data, leading to misleading results.

**Solution:** This script detects outliers using the Z-score and IQR methods and allows the user to handle them by capping, removing, or leaving them unchanged.

**Script Features:**
- Detects outliers in numeric columns.
- Provides user options to handle detected outliers.

### 3. Scaling and Standardizing Data

**Problem:** Data with different scales can negatively impact model performance, particularly for algorithms sensitive to feature scaling.

**Solution:** This script offers multiple scaling options, including Min-Max, Standard, Robust, and Normalization, allowing users to scale data as per their needs while retaining the dataset’s structure.

**Script Features:**
- Supports various scaling methods (Min-Max, Standard, Robust, Normalization).
- Maintains the original shape of the DataFrame.

### 4. Encoding Categorical Data

**Problem:** Categorical data must be converted to numerical form for use in machine learning models, but expanding the DataFrame with one-hot encoding can alter its structure.

**Solution:** This script allows label encoding and one-hot encoding (without expanding the DataFrame) to transform categorical data while keeping the DataFrame’s original shape.

**Script Features:**
- Provides Label Encoding and One-Hot Encoding without expanding columns.
- Maintains the DataFrame's original shape.


## What This Overcomes

The toolkit overcomes key data preprocessing challenges, such as:
- **Efficiency:** Reduces time spent manually cleaning and preparing data.
- **Consistency:** Ensures data is consistently processed according to user specifications.
- **Flexibility:** Allows interactive selection of processing steps for each column, making it adaptable to various datasets.
- **Scalability:** Easily extendable for larger datasets and more complex preprocessing needs.

## Getting Started

### Prerequisites
- Python 3.x installed.
- Required libraries: `pandas`, `numpy`, `sklearn`, and `jupyter`.

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/KaRtHiK-56/data-preprocessing-toolkit.git
   ```
2. Install the required libraries:
   ```bash
   pip install pandas numpy scikit-learn jupyter
   ```

### Usage

1. **Handling Missing Values:**
   - Run the `handle_missing_values.py` script.
   - Follow the prompts to choose how to handle missing values for each column.

2. **Handling Outliers:**
   - Run the `handle_outliers.py` script.
   - Follow the prompts to detect and manage outliers.

3. **Scaling and Standardizing Data:**
   - Run the `scale_standardize_data.py` script.
   - Select the scaling or standardization method for each numeric column.

4. **Encoding Categorical Data:**
   - Run the `encode_categorical_data.py` script.
   - Choose Label or One-Hot Encoding for each categorical column.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue to discuss potential changes.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements

- [Pandas Documentation](https://pandas.pydata.org/)
- [Scikit-Learn Documentation](https://scikit-learn.org/)

