# SAEB and Socioeconomic Data Analysis

This repository contains a Python script for analyzing and predicting SAEB (Sistema de Avaliação da Educação Básica) data in conjunction with socioeconomic data. The main objective is to explore the relationships between socioeconomic factors and student performance, as well as to apply a linear regression model to predict student performance based on socioeconomic features.

## Project Structure

The script performs the following tasks:

### 1. Data Collection and Integration
- Loads SAEB data (`dados_saeb.csv`) and socioeconomic data (`dados_socioeconomicos.csv`).
- Merges the two datasets using `codigo_municipio` as the key.

### 2. Exploratory Data Analysis (EDA)
- Displays descriptive statistics of the integrated data.
- Visualizes the distribution of mathematics scores.
- Plots the relationship between per capita income and mathematics scores.

### 3. Data Visualization
- Bar plot showing average mathematics scores by municipality.

### 4. Predictive Modeling (Optional)
- Prepares data by selecting relevant features (`renda_per_capita` and `taxa_analfabetismo`) for a linear regression model.
- Splits the data into training and test sets.
- Trains a linear regression model to predict mathematics scores based on selected features.
- Evaluates the model's performance using Mean Squared Error (MSE).

## Requirements

To run this script, you will need the following Python libraries:
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

You can install them using pip:

pip install pandas matplotlib seaborn scikit-learn

## Usage

1. Place your SAEB and socioeconomic data CSV files (`dados_saeb.csv` and `dados_socioeconomicos.csv`) in the project directory or update the file paths in the script.
2. Run the script to perform data analysis and prediction.

python saeb_analysis.py

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
