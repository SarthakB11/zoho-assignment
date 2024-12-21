# Rotten Tomatoes Movie Rating Prediction

Dataset download link : https://docs.google.com/spreadsheets/d/1ehu9zIbmQPrW6DHJ8xQMVMBtAkM4mLSu/edit?usp=sharing&ouid=111881146371025480890&rtpof=true&sd=true


## Overview
This project focuses on predicting audience ratings for movies using various machine learning models. The dataset is preprocessed, and multiple models are trained and evaluated in parallel to find the best-performing one. The code includes downloading, preprocessing, training, and visualization steps.

---

## Features
- Downloads and extracts the dataset automatically.
- Preprocesses data with handling for both numerical and categorical features.
- Implements multiple regression models: Linear Regression, Random Forest, and Gradient Boosting.
- Utilizes parallel processing to train and evaluate models efficiently.
- Visualizes the performance of models and their predictions.

---

## Installation

### Prerequisites
Make sure you have the following installed:
- Python 3.7+
- Required Python libraries:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `joblib`
  - `scikit-learn`
  - `requests`

### Setup
1. Clone this repository:
   ```bash
   git clone https://github.com/SarthakB11/zoho-assignment.git
   cd zoho-assignment
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure internet connectivity for downloading the dataset.

---

## Usage

### Running the Code
Run the following command to start the process:
```bash
python main.ipynb
```

### Process Flow
1. **Download & Extraction**:
   - Downloads the dataset from the specified URL.
   - Extracts the data into a local directory.

2. **Data Loading**:
   - Loads the dataset from the extracted file or a fallback file.
   - Provides an overview of the dataset, missing values, and statistical summaries.

3. **Preprocessing**:
   - Handles missing values.
   - Encodes categorical features and scales numerical features.

4. **Model Training**:
   - Trains and evaluates Linear Regression, Random Forest, and Gradient Boosting models.
   - Uses 5-fold cross-validation for robust performance evaluation.

5. **Visualization**:
   - Plots actual vs. predicted audience ratings for each model.
   - Compares predictions of all models.

---

## Files
- **main.ipynb**: Main script to run the process.
- **data.zip**: Dataset downloaded and extracted during runtime.

---

## Constants
All literals, column names, and hyperparameters are defined at the beginning of the script for better configurability:

| Constant           | Description                                    |
|--------------------|------------------------------------------------|
| `ZIP_URL`          | URL to download the dataset                   |
| `EXTRACT_DIR`      | Directory to extract the dataset              |
| `FALLBACK_FILE`    | Fallback file path for dataset loading        |
| `COLUMN_NAMES`     | Object defining column names for features     |
| `TEST_SIZE`        | Proportion of the dataset for testing         |
| `CV_FOLDS`         | Number of cross-validation folds              |
| `RANDOM_STATE`     | Seed for random operations                    |
| `N_ESTIMATORS`     | Number of estimators for ensemble models      |

---

## Results
- Model performance is evaluated using R² Score, RMSE, and cross-validation metrics.
- Visualization provides insights into model accuracy and prediction trends.

---

## Contributions
Feel free to contribute to the project by:
- Improving data preprocessing.
- Adding new models or enhancing existing ones.
- Refining visualizations.

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---

## Contact
For questions or suggestions, please reach out to:
- **Name**: Sarthak Bhardwaj
- **Email**: sarthak.bhardwaj21b@iiitg.ac.in
- **GitHub**: github.com/SarthakB11

